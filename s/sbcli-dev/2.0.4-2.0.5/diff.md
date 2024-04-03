# Comparing `tmp/sbcli-dev-2.0.4.zip` & `tmp/sbcli-dev-2.0.5.zip`

## zipinfo {}

```diff
@@ -1,135 +1,146 @@
-Zip file size: 161347 bytes, number of entries: 133
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/simplyblock_core/
--rw-r--r--  2.0 unx      149 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/env_var
--rw-r--r--  2.0 unx     2159 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-03 15:34 sbcli-dev-2.0.4/setup.cfg
--rw-r--r--  2.0 unx      730 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/README.md
--rw-r--r--  2.0 unx       84 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/pyproject.toml
--rw-r--r--  2.0 unx     1129 b- defN 24-Apr-03 15:34 sbcli-dev-2.0.4/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/app.py
--rw-r--r--  2.0 unx     5078 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      703 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx      463 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      827 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx     1302 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx      434 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      322 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx     1890 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     4795 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx    12198 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx      975 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     5274 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     5547 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx     8654 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8169 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx      357 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_cli/main.py
--rw-r--r--  2.0 unx    76335 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-03 15:34 sbcli-dev-2.0.4/sbcli_dev.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 15:34 sbcli-dev-2.0.4/sbcli_dev.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-03 15:34 sbcli-dev-2.0.4/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-03 15:34 sbcli-dev-2.0.4/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx     4651 b- defN 24-Apr-03 15:34 sbcli-dev-2.0.4/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx     1129 b- defN 24-Apr-03 15:34 sbcli-dev-2.0.4/sbcli_dev.egg-info/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 15:34 sbcli-dev-2.0.4/simplyblock_core/controllers/
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     1426 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/constants.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7626 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    63042 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx    23197 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx     6262 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx    21452 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx      648 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1493 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     6716 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx     5305 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     3203 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx      173 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     4637 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     3003 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2410 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     7218 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2612 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6245 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx      837 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     5462 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     2490 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     5443 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/capacity_collector.py
--rw-r--r--  2.0 unx     4817 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     2193 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx      736 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx      806 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     3222 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    46637 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    22847 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx    10787 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx    13535 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx     1122 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    11300 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Apr-03 15:33 sbcli-dev-2.0.4/simplyblock_core/controllers/pool_controller.py
-133 files, 579399 bytes uncompressed, 137365 bytes compressed:  76.3%
+Zip file size: 177737 bytes, number of entries: 144
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_core/
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-03 16:00 sbcli-dev-2.0.5/setup.cfg
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/pyproject.toml
+-rw-r--r--  2.0 unx      730 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/README.md
+-rw-r--r--  2.0 unx     2251 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/setup.py
+-rw-r--r--  2.0 unx      149 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/env_var
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-03 16:00 sbcli-dev-2.0.5/PKG-INFO
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-03 16:00 sbcli-dev-2.0.5/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     5073 b- defN 24-Apr-03 16:00 sbcli-dev-2.0.5/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-03 16:00 sbcli-dev-2.0.5/sbcli_dev.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-03 16:00 sbcli-dev-2.0.5/sbcli_dev.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-03 16:00 sbcli-dev-2.0.5/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-03 16:00 sbcli-dev-2.0.5/sbcli_dev.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx    76335 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_web/static/
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     5078 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     1890 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     8169 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     8654 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_web/static/tst.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_core/models/
+-rw-r--r--  2.0 unx     6262 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx    21452 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     1426 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx    63042 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    23335 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7626 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/snode_client.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-03 16:00 sbcli-dev-2.0.5/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1694 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      360 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/db_config_single.sh
+-rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx     8081 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     5860 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1853 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    98143 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    98031 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    98198 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    98086 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    22847 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx    13535 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    10787 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     1961 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    46637 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    11300 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5443 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/capacity_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4817 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2490 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     6245 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     4637 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     7218 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2193 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     3222 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-03 15:59 sbcli-dev-2.0.5/simplyblock_core/models/lvol_model.py
+144 files, 983035 bytes uncompressed, 151601 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -1,400 +1,433 @@
-Filename: sbcli-dev-2.0.4/
+Filename: sbcli-dev-2.0.5/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/
+Filename: sbcli-dev-2.0.5/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_cli/
+Filename: sbcli-dev-2.0.5/simplyblock_cli/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/sbcli_dev.egg-info/
+Filename: sbcli-dev-2.0.5/simplyblock_web/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/
+Filename: sbcli-dev-2.0.5/simplyblock_core/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/env_var
+Filename: sbcli-dev-2.0.5/setup.cfg
 Comment: 
 
-Filename: sbcli-dev-2.0.4/setup.py
+Filename: sbcli-dev-2.0.5/pyproject.toml
 Comment: 
 
-Filename: sbcli-dev-2.0.4/setup.cfg
+Filename: sbcli-dev-2.0.5/README.md
 Comment: 
 
-Filename: sbcli-dev-2.0.4/README.md
+Filename: sbcli-dev-2.0.5/setup.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/pyproject.toml
+Filename: sbcli-dev-2.0.5/env_var
 Comment: 
 
-Filename: sbcli-dev-2.0.4/PKG-INFO
+Filename: sbcli-dev-2.0.5/PKG-INFO
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/static/
+Filename: sbcli-dev-2.0.5/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/templates/
+Filename: sbcli-dev-2.0.5/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/
+Filename: sbcli-dev-2.0.5/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/__init__.py
+Filename: sbcli-dev-2.0.5/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/caching_node_app.py
+Filename: sbcli-dev-2.0.5/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/utils.py
+Filename: sbcli-dev-2.0.5/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/auth_middleware.py
+Filename: sbcli-dev-2.0.5/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli-dev-2.0.5/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/app.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/node_utils.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/node_webapp.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/snode_app.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli-dev-2.0.5/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/static/list_deps.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/static/rpac.yaml
+Filename: sbcli-dev-2.0.5/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/static/delete.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli-dev-2.0.5/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/static/deploy.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/static/is_up.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/static/tst.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli-dev-2.0.5/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/__init__.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/csi.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_cli/main.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_cli/cli.py
+Filename: sbcli-dev-2.0.5/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli-dev-2.0.4/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli-dev-2.0.5/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli-dev-2.0.5/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli-dev-2.0.4/sbcli_dev.egg-info/requires.txt
+Filename: sbcli-dev-2.0.5/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli-dev-2.0.5/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli-dev-2.0.5/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli-dev-2.0.5/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/snode_client.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/constants.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/__init__.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/cnode_client.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/utils.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/storage_node_ops.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/shell_utils.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/cluster_ops.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/pci_utils.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/distr_controller.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/rpc_client.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/kv_store.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/compute_node_ops.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/__init__.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/__init__.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/remove_service.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/log_agg_service.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/service_template.service
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/cap_monitor.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/install_service.sh
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/health_check_service.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/device_monitor.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/capacity_collector.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/events.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/__init__.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/nvme_device.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/global_settings.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/caching_node.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/port_stat.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/snapshot.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/iface.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/stats.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/storage_node.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/compute_node.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/mgmt_node.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/capacity_collector.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/pool.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/cluster.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/base_model.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/models/lvol_model.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/__init__.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/storage_events.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/events_controller.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/pool_events.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/device_controller.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/device_events.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/health_controller.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli-dev-2.0.4/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/events.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/iface.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/base_model.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/__init__.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/stats.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/nvme_device.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/storage_node.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/port_stat.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/mgmt_node.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/snapshot.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/compute_node.py
+Comment: 
+
+Filename: sbcli-dev-2.0.5/simplyblock_core/models/lvol_model.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli-dev-2.0.4/setup.py` & `sbcli-dev-2.0.5/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,16 @@
 COMMAND_NAME = get_env_var("SIMPLY_BLOCK_COMMAND_NAME", "sbcli")
 VERSION = get_env_var("SIMPLY_BLOCK_VERSION", "1")
 
 data_files = gen_data_files(
         "simplyblock_core/controllers",
         "simplyblock_core/models",
         "simplyblock_core/scripts",
+        "simplyblock_core/scripts/alerting",
+        "simplyblock_core/scripts/dashboards",
         "simplyblock_core/services",
         "simplyblock_web/blueprints",
         "simplyblock_web/static",
         "simplyblock_web/templates")
 
 data_files.append(('', ['env_var']))
```

## Comparing `sbcli-dev-2.0.4/README.md` & `sbcli-dev-2.0.5/README.md`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/PKG-INFO` & `sbcli-dev-2.0.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.0.4
+Version: 2.0.5
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli-dev-2.0.4/simplyblock_web/caching_node_app.py` & `sbcli-dev-2.0.5/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/utils.py` & `sbcli-dev-2.0.5/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/auth_middleware.py` & `sbcli-dev-2.0.5/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/caching_node_app_k8s.py` & `sbcli-dev-2.0.5/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/app.py` & `sbcli-dev-2.0.5/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/node_utils.py` & `sbcli-dev-2.0.5/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/node_webapp.py` & `sbcli-dev-2.0.5/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/snode_app.py` & `sbcli-dev-2.0.5/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/static/deploy_spdk.yaml` & `sbcli-dev-2.0.5/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/static/delete.py` & `sbcli-dev-2.0.5/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/static/deploy.py` & `sbcli-dev-2.0.5/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli-dev-2.0.5/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_pool.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/node_api_basic.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_device.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/csi.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/snode_ops.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli-dev-2.0.5/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_cli/cli.py` & `sbcli-dev-2.0.5/simplyblock_cli/cli.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/sbcli_dev.egg-info/SOURCES.txt` & `sbcli-dev-2.0.5/sbcli_dev.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -52,25 +52,34 @@
 simplyblock_core/models/nvme_device.py
 simplyblock_core/models/pool.py
 simplyblock_core/models/port_stat.py
 simplyblock_core/models/snapshot.py
 simplyblock_core/models/stats.py
 simplyblock_core/models/storage_node.py
 simplyblock_core/scripts/__init__.py
+simplyblock_core/scripts/apply_dashboard.sh
 simplyblock_core/scripts/clean_local_storage_deploy.sh
 simplyblock_core/scripts/config_docker.sh
+simplyblock_core/scripts/datasource.yml
 simplyblock_core/scripts/db_config_double.sh
 simplyblock_core/scripts/db_config_single.sh
 simplyblock_core/scripts/deploy_stack.sh
 simplyblock_core/scripts/docker-compose-swarm.yml
 simplyblock_core/scripts/haproxy.cfg
 simplyblock_core/scripts/install_deps.sh
+simplyblock_core/scripts/prometheus.yml
 simplyblock_core/scripts/run_ssh.sh
 simplyblock_core/scripts/set_db_config.sh
 simplyblock_core/scripts/stack_deploy_wait.sh
+simplyblock_core/scripts/alerting/alert_resources.yaml
+simplyblock_core/scripts/alerting/alert_rules.yaml
+simplyblock_core/scripts/dashboards/cluster.json
+simplyblock_core/scripts/dashboards/devices.json
+simplyblock_core/scripts/dashboards/lvols.json
+simplyblock_core/scripts/dashboards/nodes.json
 simplyblock_core/services/__init__.py
 simplyblock_core/services/caching_node_monitor.py
 simplyblock_core/services/cap_monitor.py
 simplyblock_core/services/capacity_and_stats_collector.py
 simplyblock_core/services/capacity_collector.py
 simplyblock_core/services/device_monitor.py
 simplyblock_core/services/distr_event_collector.py
```

## Comparing `sbcli-dev-2.0.4/sbcli_dev.egg-info/PKG-INFO` & `sbcli-dev-2.0.5/sbcli_dev.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.0.4
+Version: 2.0.5
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli-dev-2.0.4/simplyblock_core/snode_client.py` & `sbcli-dev-2.0.5/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/constants.py` & `sbcli-dev-2.0.5/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/cnode_client.py` & `sbcli-dev-2.0.5/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/mgmt_node_ops.py` & `sbcli-dev-2.0.5/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/utils.py` & `sbcli-dev-2.0.5/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/storage_node_ops.py` & `sbcli-dev-2.0.5/simplyblock_core/storage_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/cluster_ops.py` & `sbcli-dev-2.0.5/simplyblock_core/cluster_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     }
     session = requests.session()
     session.auth = ("admin", password)
     response = session.request("POST", url, headers=headers, data=payload)
     logger.debug(response.text)
     return response.status_code == 201
 
-
 def create_cluster(blk_size, page_size_in_blocks, ha_type, tls,
                    auth_hosts_only, cli_pass, model_ids,
                    cap_warn, cap_crit, prov_cap_warn, prov_cap_crit, ifname):
     logger.info("Installing dependencies...")
     ret = scripts.install_deps()
     logger.info("Installing dependencies > Done")
 
@@ -104,15 +103,15 @@
         c.cap_crit = cap_crit
     if prov_cap_warn and prov_cap_warn > 0:
         c.prov_cap_warn = prov_cap_warn
     if prov_cap_crit and prov_cap_crit > 0:
         c.prov_cap_crit = prov_cap_crit
 
     logger.info("Deploying swarm stack ...")
-    ret = scripts.deploy_stack(cli_pass, DEV_IP, constants.SIMPLY_BLOCK_DOCKER_IMAGE, c.secret)
+    ret = scripts.deploy_stack(cli_pass, DEV_IP, constants.SIMPLY_BLOCK_DOCKER_IMAGE, c.secret, c.uuid)
     logger.info("Deploying swarm stack > Done")
 
     logger.info("Configuring DB...")
     out = scripts.set_db_config_single()
     logger.info("Configuring DB > Done")
 
     _add_graylog_input(DEV_IP, c.secret)
@@ -123,14 +122,18 @@
     c.updated_at = int(time.time())
     c.write_to_db(db_controller.kv_store)
 
     cluster_events.cluster_create(c)
 
     mgmt_node_ops.add_mgmt_node(DEV_IP, c.uuid)
 
+    logger.info("Applying dashboard...")
+    ret = scripts.apply_dashboard(c.secret)
+    logger.info("Applying dashboard > Done")
+
     logger.info("New Cluster has been created")
     logger.info(c.uuid)
     return c.uuid
 
 
 # Deprecated
 def deploy_spdk(node_docker, spdk_cpu_mask, spdk_mem):
```

## Comparing `sbcli-dev-2.0.4/simplyblock_core/pci_utils.py` & `sbcli-dev-2.0.5/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/distr_controller.py` & `sbcli-dev-2.0.5/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/rpc_client.py` & `sbcli-dev-2.0.5/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/kv_store.py` & `sbcli-dev-2.0.5/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/compute_node_ops.py` & `sbcli-dev-2.0.5/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/scripts/haproxy.cfg` & `sbcli-dev-2.0.5/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/scripts/__init__.py` & `sbcli-dev-2.0.5/simplyblock_core/scripts/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,18 +26,22 @@
     return __run_script(['bash', '-x', os.path.join(DIR_PATH, 'install_deps.sh')])
 
 
 def configure_docker(docker_ip):
     return __run_script(['bash', '-x', os.path.join(DIR_PATH, 'config_docker.sh'), docker_ip])
 
 
-def deploy_stack(cli_pass, dev_ip, image_name, graylog_password):
+def deploy_stack(cli_pass, dev_ip, image_name, graylog_password, cluster_id):
     pass_hash = hashlib.sha256(graylog_password.encode('utf-8')).hexdigest()
     return __run_script(
-        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), cli_pass, dev_ip, image_name, pass_hash])
+        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'deploy_stack.sh'), cli_pass, dev_ip, image_name, pass_hash, graylog_password, cluster_id])
+
+def apply_dashboard(grafanaPassword):
+    return __run_script(
+        ['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'apply_dashboard.sh'), grafanaPassword])
 
 
 def deploy_cleaner():
     return __run_script(['sudo', 'bash', '-x', os.path.join(DIR_PATH, 'clean_local_storage_deploy.sh')])
 
 
 def set_db_config(DEV_IP):
```

## Comparing `sbcli-dev-2.0.4/simplyblock_core/scripts/install_deps.sh` & `sbcli-dev-2.0.5/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli-dev-2.0.5/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files 18% similar despite different names*

```diff
@@ -15,15 +15,14 @@
       - "/etc/foundationdb/logs:/var/fdb/logs"
 
     deploy:
       mode: global
       placement:
         constraints: [ node.role == manager ]
 
-
   WebAppAPI:
     image: $SIMPLYBLOCK_DOCKER_IMAGE
     command: "python simplyblock_web/app.py"
     deploy:
       endpoint_mode: dnsrr
       mode: global
       placement:
@@ -118,38 +117,35 @@
       - 8081:8080
     volumes:
       - "/var/run/docker.sock:/var/run/docker.sock"
     deploy:
       placement:
         constraints: [node.role == manager]
 
-
   HAProxy:
     image: haproxytech/haproxy-debian:latest
     deploy:
       mode: global
       placement:
         constraints: [node.role == manager]
     ports:
       - 80:80
       - 8404:8404
     volumes:
       - "$DIR/haproxy.cfg:/usr/local/etc/haproxy/haproxy.cfg"
 
-
   CapacityAndStatsCollector:
     image: $SIMPLYBLOCK_DOCKER_IMAGE
     command: "python simplyblock_core/services/capacity_and_stats_collector.py"
     deploy:
       placement:
         constraints: [node.role == manager]
     volumes:
       - "/etc/foundationdb:/etc/foundationdb"
 
-
   CapacityMonitor:
     image: $SIMPLYBLOCK_DOCKER_IMAGE
     command: "python simplyblock_core/services/cap_monitor.py"
     deploy:
       placement:
         constraints: [node.role == manager]
     volumes:
@@ -178,15 +174,15 @@
     command: "python simplyblock_core/services/lvol_monitor.py"
     deploy:
       placement:
         constraints: [node.role == manager]
     volumes:
       - "/etc/foundationdb:/etc/foundationdb"
 
-
+  ### monitoring ###
   mongodb:
     image: "mongo:5.0"
     volumes:
       - "mongodb_data:/data/db"
     deploy:
       placement:
         constraints: [node.role == manager]
@@ -196,17 +192,14 @@
     environment:
       - "OPENSEARCH_JAVA_OPTS=-Xms1g -Xmx1g"
       - "bootstrap.memory_lock=true"
       - "discovery.type=single-node"
       - "action.auto_create_index=false"
       - "plugins.security.ssl.http.enabled=false"
       - "plugins.security.disabled=true"
-    ports:
-      - "9200:9200"
-      - "9600:9600"  # required for Performance Analyzer
     volumes:
       - "os_data:/usr/share/opensearch/data"
     deploy:
       placement:
         constraints: [node.role == manager]
 
   graylog:
@@ -235,17 +228,73 @@
     volumes:
       - "graylog_data:/usr/share/graylog/data/data"
       - "graylog_journal:/usr/share/graylog/data/journal"
     deploy:
       placement:
         constraints: [node.role == manager]
 
+  promagent:
+    image: simplyblock/promagent
+    environment:
+      ClusterID: "${CLUSTER_ID}"
+      ClusterIP: "${CLUSTER_IP}"
+      ClusterSecret: "${CLUSTER_SECRET}"
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+
+  pushgateway:
+    image: prom/pushgateway
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+
+  prometheus:
+    image: prom/prometheus:v2.44.0
+    user: root
+    volumes:
+      - ./prometheus.yml:/etc/prometheus/prometheus.yml
+      - prometheus_data:/prometheus
+    command:
+      - "--config.file=/etc/prometheus/prometheus.yml"
+      - "--storage.tsdb.path=/prometheus"
+    restart: "always"
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+
+  grafana:
+    image: grafana/grafana:10.0.12
+    environment:
+      GF_SECURITY_ADMIN_USER: "admin"
+      GF_SECURITY_ADMIN_PASSWORD: "${CLUSTER_SECRET}"
+      GF_ALERTING_ENABLED: "true"
+      GF_PATHS_PROVISIONING: "/etc/grafana/provisioning"
+    volumes:
+      - ./datasource.yml:/etc/grafana/provisioning/datasources/datasource.yaml
+      - grafana_data:/var/lib/grafana
+      - ./alerting:/etc/grafana/provisioning/alerting
+    restart: "always"
+    ports:
+      - target: 3000
+        published: 3000
+        protocol: tcp
+        mode: host
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+
+  ### monitoring ###
+
 volumes:
   mongodb_data:
   os_data:
   graylog_data:
   graylog_journal:
+  grafana_data:
+  prometheus_data:
+  alertmanager_data:
 
 networks:
   hostnet:
     external: true
     name: host
```

## Comparing `sbcli-dev-2.0.4/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli-dev-2.0.5/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/caching_node_monitor.py` & `sbcli-dev-2.0.5/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/__init__.py` & `sbcli-dev-2.0.5/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/port_stat_collector.py` & `sbcli-dev-2.0.5/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/lvol_monitor.py` & `sbcli-dev-2.0.5/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/distr_event_collector.py` & `sbcli-dev-2.0.5/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli-dev-2.0.5/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/log_agg_service.py` & `sbcli-dev-2.0.5/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli-dev-2.0.5/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/cap_monitor.py` & `sbcli-dev-2.0.5/simplyblock_core/services/cap_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
 gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
+### script to test connection once connection is ascertain
 # get DB controller
 db_controller = kv_store.DBController()
 
 logger.info("Starting capacity monitoring service...")
 while True:
     clusters = db_controller.get_clusters()
     for cl in clusters:
```

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/storage_node_monitor.py` & `sbcli-dev-2.0.5/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/install_service.sh` & `sbcli-dev-2.0.5/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/health_check_service.py` & `sbcli-dev-2.0.5/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/device_monitor.py` & `sbcli-dev-2.0.5/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/capacity_collector.py` & `sbcli-dev-2.0.5/simplyblock_core/services/capacity_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/services/lvol_stat_collector.py` & `sbcli-dev-2.0.5/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/events.py` & `sbcli-dev-2.0.5/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/nvme_device.py` & `sbcli-dev-2.0.5/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/global_settings.py` & `sbcli-dev-2.0.5/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/caching_node.py` & `sbcli-dev-2.0.5/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/port_stat.py` & `sbcli-dev-2.0.5/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/snapshot.py` & `sbcli-dev-2.0.5/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/iface.py` & `sbcli-dev-2.0.5/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/stats.py` & `sbcli-dev-2.0.5/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/storage_node.py` & `sbcli-dev-2.0.5/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/compute_node.py` & `sbcli-dev-2.0.5/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/mgmt_node.py` & `sbcli-dev-2.0.5/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/pool.py` & `sbcli-dev-2.0.5/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/cluster.py` & `sbcli-dev-2.0.5/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/base_model.py` & `sbcli-dev-2.0.5/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/models/lvol_model.py` & `sbcli-dev-2.0.5/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/storage_events.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/cluster_events.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/events_controller.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/lvol_controller.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/pool_events.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/caching_node_controller.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/snapshot_controller.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/mgmt_events.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/device_controller.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/lvol_events.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/device_events.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/snapshot_events.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/health_controller.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-2.0.4/simplyblock_core/controllers/pool_controller.py` & `sbcli-dev-2.0.5/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

