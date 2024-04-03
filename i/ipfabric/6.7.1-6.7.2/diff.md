# Comparing `tmp/ipfabric-6.7.1.tar.gz` & `tmp/ipfabric-6.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric-6.7.1.tar", max compression
+gzip compressed data, was "ipfabric-6.7.2.tar", max compression
```

## Comparing `ipfabric-6.7.1.tar` & `ipfabric-6.7.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
--rw-r--r--   0        0        0     1294 2024-02-21 17:21:14.240240 ipfabric-6.7.1/ipfabric/__init__.py
--rw-r--r--   0        0        0    12055 2024-03-20 16:35:10.764022 ipfabric-6.7.1/ipfabric/api.py
--rw-r--r--   0        0        0    10156 2024-03-20 16:35:10.766172 ipfabric-6.7.1/ipfabric/auth.py
--rw-r--r--   0        0        0    23368 2024-03-20 16:35:10.767248 ipfabric-6.7.1/ipfabric/client.py
--rw-r--r--   0        0        0      693 2024-02-29 12:11:26.623633 ipfabric-6.7.1/ipfabric/diagrams/__init__.py
--rw-r--r--   0        0        0    18216 2024-03-29 13:49:06.793074 ipfabric-6.7.1/ipfabric/diagrams/graphs.py
--rw-r--r--   0        0        0     3625 2024-02-22 21:24:28.609926 ipfabric-6.7.1/ipfabric/diagrams/icmp.py
--rw-r--r--   0        0        0      867 2024-02-29 12:11:26.625974 ipfabric-6.7.1/ipfabric/diagrams/input_models/__init__.py
--rw-r--r--   0        0        0     3808 2024-02-29 12:11:26.627304 ipfabric-6.7.1/ipfabric/diagrams/input_models/constants.py
--rw-r--r--   0        0        0        0 2023-12-13 15:03:30.792953 ipfabric-6.7.1/ipfabric/diagrams/input_models/factory_defaults/__init__.py
--rw-r--r--   0        0        0     5792 2023-12-13 15:03:30.792953 ipfabric-6.7.1/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
--rw-r--r--   0        0        0     2173 2023-12-13 15:03:30.794172 ipfabric-6.7.1/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
--rw-r--r--   0        0        0    12911 2024-02-29 12:11:26.628310 ipfabric-6.7.1/ipfabric/diagrams/input_models/graph_parameters.py
--rw-r--r--   0        0        0    13870 2024-02-29 12:11:26.629771 ipfabric-6.7.1/ipfabric/diagrams/input_models/graph_settings.py
--rw-r--r--   0        0        0     5026 2024-02-29 12:11:26.630778 ipfabric-6.7.1/ipfabric/diagrams/input_models/shared_view.py
--rw-r--r--   0        0        0       90 2024-02-29 12:11:26.632075 ipfabric-6.7.1/ipfabric/diagrams/output_models/__init__.py
--rw-r--r--   0        0        0     5241 2024-02-29 12:11:26.633080 ipfabric-6.7.1/ipfabric/diagrams/output_models/graph_result.py
--rw-r--r--   0        0        0     2278 2024-01-25 18:33:47.040766 ipfabric-6.7.1/ipfabric/diagrams/output_models/protocols.py
--rw-r--r--   0        0        0     4556 2024-02-29 12:11:26.634080 ipfabric-6.7.1/ipfabric/diagrams/output_models/trace.py
--rw-r--r--   0        0        0     2283 2024-03-20 16:35:10.768244 ipfabric-6.7.1/ipfabric/exceptions.py
--rw-r--r--   0        0        0      670 2024-03-20 16:35:10.769326 ipfabric-6.7.1/ipfabric/models/__init__.py
--rw-r--r--   0        0        0    22013 2024-03-20 16:35:10.770406 ipfabric-6.7.1/ipfabric/models/device.py
--rw-r--r--   0        0        0     7677 2024-03-20 16:35:10.771408 ipfabric-6.7.1/ipfabric/models/intent.py
--rw-r--r--   0        0        0     2796 2023-07-31 14:49:28.275721 ipfabric-6.7.1/ipfabric/models/intent_check.py
--rw-r--r--   0        0        0    10641 2024-03-20 16:35:10.772481 ipfabric-6.7.1/ipfabric/models/inventory.py
--rw-r--r--   0        0        0     5787 2024-03-20 16:35:10.773517 ipfabric-6.7.1/ipfabric/models/jobs.py
--rw-r--r--   0        0        0     4128 2024-03-20 16:35:10.774564 ipfabric-6.7.1/ipfabric/models/oas.py
--rw-r--r--   0        0        0     1888 2024-03-20 16:35:10.774564 ipfabric-6.7.1/ipfabric/models/rbac.py
--rw-r--r--   0        0        0    27927 2024-03-20 16:35:10.775608 ipfabric-6.7.1/ipfabric/models/snapshot.py
--rw-r--r--   0        0        0     5759 2024-03-20 16:35:10.775608 ipfabric-6.7.1/ipfabric/models/snapshots.py
--rw-r--r--   0        0        0    23837 2024-03-20 16:35:10.776646 ipfabric-6.7.1/ipfabric/models/table.py
--rw-r--r--   0        0        0     4145 2024-03-20 16:35:10.777686 ipfabric-6.7.1/ipfabric/models/technology/__init__.py
--rw-r--r--   0        0        0     1504 2024-03-20 16:35:10.778718 ipfabric-6.7.1/ipfabric/models/technology/addressing.py
--rw-r--r--   0        0        0      661 2024-03-20 16:35:10.778718 ipfabric-6.7.1/ipfabric/models/technology/cloud.py
--rw-r--r--   0        0        0     2731 2024-03-20 16:35:10.779749 ipfabric-6.7.1/ipfabric/models/technology/dhcp.py
--rw-r--r--   0        0        0     1315 2024-03-20 16:35:10.780776 ipfabric-6.7.1/ipfabric/models/technology/fhrp.py
--rw-r--r--   0        0        0     8591 2024-03-20 16:35:10.781802 ipfabric-6.7.1/ipfabric/models/technology/interfaces.py
--rw-r--r--   0        0        0      462 2024-03-20 16:35:10.781802 ipfabric-6.7.1/ipfabric/models/technology/ip_telephony.py
--rw-r--r--   0        0        0     1086 2024-03-20 16:35:10.783360 ipfabric-6.7.1/ipfabric/models/technology/load_balancing.py
--rw-r--r--   0        0        0      643 2024-03-20 16:35:10.784362 ipfabric-6.7.1/ipfabric/models/technology/managed_networks.py
--rw-r--r--   0        0        0     7447 2024-03-20 16:35:10.785416 ipfabric-6.7.1/ipfabric/models/technology/management.py
--rw-r--r--   0        0        0     2604 2024-03-20 16:35:10.785466 ipfabric-6.7.1/ipfabric/models/technology/mpls.py
--rw-r--r--   0        0        0     3516 2024-03-20 16:35:10.786534 ipfabric-6.7.1/ipfabric/models/technology/multicast.py
--rw-r--r--   0        0        0     1002 2024-03-20 16:35:10.787589 ipfabric-6.7.1/ipfabric/models/technology/neighbors.py
--rw-r--r--   0        0        0      806 2024-03-20 16:35:10.787589 ipfabric-6.7.1/ipfabric/models/technology/oam.py
--rw-r--r--   0        0        0     4436 2024-03-20 16:35:10.788591 ipfabric-6.7.1/ipfabric/models/technology/platforms.py
--rw-r--r--   0        0        0     1579 2024-03-20 16:35:10.789626 ipfabric-6.7.1/ipfabric/models/technology/port_channels.py
--rw-r--r--   0        0        0     1424 2024-03-20 16:35:10.790651 ipfabric-6.7.1/ipfabric/models/technology/qos.py
--rw-r--r--   0        0        0     6912 2024-03-20 16:35:10.791753 ipfabric-6.7.1/ipfabric/models/technology/routing.py
--rw-r--r--   0        0        0     2962 2024-03-20 16:35:10.791753 ipfabric-6.7.1/ipfabric/models/technology/sdn.py
--rw-r--r--   0        0        0      604 2024-03-20 16:35:10.792841 ipfabric-6.7.1/ipfabric/models/technology/sdwan.py
--rw-r--r--   0        0        0     2620 2024-03-20 16:35:10.793894 ipfabric-6.7.1/ipfabric/models/technology/security.py
--rw-r--r--   0        0        0     2641 2024-03-20 16:35:10.793894 ipfabric-6.7.1/ipfabric/models/technology/stp.py
--rw-r--r--   0        0        0     1134 2024-03-20 16:35:10.794896 ipfabric-6.7.1/ipfabric/models/technology/vlans.py
--rw-r--r--   0        0        0     1145 2024-03-20 16:35:10.795936 ipfabric-6.7.1/ipfabric/models/technology/wireless.py
--rw-r--r--   0        0        0     2409 2024-03-20 16:35:10.795936 ipfabric-6.7.1/ipfabric/models/users.py
--rw-r--r--   0        0        0        0 2024-01-25 18:33:47.048277 ipfabric-6.7.1/ipfabric/oas/__init__.py
--rw-r--r--   0        0        0   326420 2024-03-20 16:35:10.799023 ipfabric-6.7.1/ipfabric/oas/v6.6.json
--rw-r--r--   0        0        0   327148 2024-03-20 16:35:10.801329 ipfabric-6.7.1/ipfabric/oas/v6.7.json
--rw-r--r--   0        0        0     1172 2024-03-20 16:35:10.803997 ipfabric-6.7.1/ipfabric/settings/__init__.py
--rw-r--r--   0        0        0     3641 2024-03-20 16:35:10.805129 ipfabric-6.7.1/ipfabric/settings/api_tokens.py
--rw-r--r--   0        0        0     6751 2024-03-20 16:35:10.806145 ipfabric-6.7.1/ipfabric/settings/attributes.py
--rw-r--r--   0        0        0     9119 2024-03-20 16:35:10.808322 ipfabric-6.7.1/ipfabric/settings/authentication.py
--rw-r--r--   0        0        0     1394 2024-03-20 16:35:10.809455 ipfabric-6.7.1/ipfabric/settings/discovery.py
--rw-r--r--   0        0        0     3266 2024-03-20 16:35:10.810505 ipfabric-6.7.1/ipfabric/settings/local_users.py
--rw-r--r--   0        0        0    14522 2024-03-29 13:49:06.795074 ipfabric-6.7.1/ipfabric/settings/rbac.py
--rw-r--r--   0        0        0     2284 2024-03-20 16:35:10.811555 ipfabric-6.7.1/ipfabric/settings/seeds.py
--rw-r--r--   0        0        0     3137 2024-03-20 16:35:10.812643 ipfabric-6.7.1/ipfabric/settings/settings.py
--rw-r--r--   0        0        0     2102 2024-03-20 16:35:10.813841 ipfabric-6.7.1/ipfabric/settings/site_separation.py
--rw-r--r--   0        0        0     4487 2024-03-20 16:35:10.814866 ipfabric-6.7.1/ipfabric/settings/vendor_api.py
--rw-r--r--   0        0        0     9120 2024-03-20 16:35:10.815971 ipfabric-6.7.1/ipfabric/settings/vendor_api_models.py
--rw-r--r--   0        0        0      644 2024-03-20 16:35:10.817051 ipfabric-6.7.1/ipfabric/tools/__init__.py
--rw-r--r--   0        0        0     8583 2024-03-20 16:35:10.818051 ipfabric-6.7.1/ipfabric/tools/configuration.py
--rw-r--r--   0        0        0     5656 2024-03-20 16:35:10.819099 ipfabric-6.7.1/ipfabric/tools/discovery_history.py
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.819099 ipfabric-6.7.1/ipfabric/tools/managed_rbac/__init__.py
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.820129 ipfabric-6.7.1/ipfabric/tools/managed_rbac/v6/7/__init__.py
--rw-r--r--   0        0        0    37895 2024-03-29 13:49:06.797076 ipfabric-6.7.1/ipfabric/tools/managed_rbac/v6/7/policies.json
--rw-r--r--   0        0        0     3383 2024-03-29 13:49:06.798242 ipfabric-6.7.1/ipfabric/tools/managed_rbac/v6/7/roles.json
--rw-r--r--   0        0        0        0 2024-03-20 16:35:10.821154 ipfabric-6.7.1/ipfabric/tools/managed_rbac/v6/__init__.py
--rw-r--r--   0        0        0     4730 2024-01-25 18:33:47.054282 ipfabric-6.7.1/ipfabric/tools/nist.py
--rw-r--r--   0        0        0     6782 2024-03-29 13:49:06.800107 ipfabric-6.7.1/ipfabric/tools/rbac.py
--rw-r--r--   0        0        0     4260 2024-03-20 16:35:10.822260 ipfabric-6.7.1/ipfabric/tools/restore_intents.py
--rw-r--r--   0        0        0    22669 2024-03-20 16:35:10.823261 ipfabric-6.7.1/ipfabric/tools/shared.py
--rw-r--r--   0        0        0     2644 2024-02-07 13:28:55.569790 ipfabric-6.7.1/ipfabric/tools/site_seperation_report.py
--rw-r--r--   0        0        0     2690 2023-12-13 15:03:30.822909 ipfabric-6.7.1/ipfabric/tools/vulnerabilities.py
--rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.7.1/LICENSE
--rw-r--r--   0        0        0     2787 2024-01-25 18:33:47.021681 ipfabric-6.7.1/NOTICES.md
--rw-r--r--   0        0        0     3300 2024-03-29 13:49:06.804122 ipfabric-6.7.1/pyproject.toml
--rw-r--r--   0        0        0     6226 2024-03-20 16:35:10.732833 ipfabric-6.7.1/README.md
--rw-r--r--   0        0        0     8376 1970-01-01 00:00:00.000000 ipfabric-6.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1294 2024-02-21 17:21:14.240240 ipfabric-6.7.2/ipfabric/__init__.py
+-rw-r--r--   0        0        0    12155 2024-04-03 16:20:13.646541 ipfabric-6.7.2/ipfabric/api.py
+-rw-r--r--   0        0        0    10196 2024-04-03 16:20:13.647975 ipfabric-6.7.2/ipfabric/auth.py
+-rw-r--r--   0        0        0    23368 2024-03-20 16:35:10.767248 ipfabric-6.7.2/ipfabric/client.py
+-rw-r--r--   0        0        0      693 2024-02-29 12:11:26.623633 ipfabric-6.7.2/ipfabric/diagrams/__init__.py
+-rw-r--r--   0        0        0    18216 2024-03-29 13:49:06.793074 ipfabric-6.7.2/ipfabric/diagrams/graphs.py
+-rw-r--r--   0        0        0     3625 2024-02-22 21:24:28.609926 ipfabric-6.7.2/ipfabric/diagrams/icmp.py
+-rw-r--r--   0        0        0      867 2024-02-29 12:11:26.625974 ipfabric-6.7.2/ipfabric/diagrams/input_models/__init__.py
+-rw-r--r--   0        0        0     3808 2024-02-29 12:11:26.627304 ipfabric-6.7.2/ipfabric/diagrams/input_models/constants.py
+-rw-r--r--   0        0        0        0 2023-12-13 15:03:30.792953 ipfabric-6.7.2/ipfabric/diagrams/input_models/factory_defaults/__init__.py
+-rw-r--r--   0        0        0     5792 2023-12-13 15:03:30.792953 ipfabric-6.7.2/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
+-rw-r--r--   0        0        0     2173 2023-12-13 15:03:30.794172 ipfabric-6.7.2/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
+-rw-r--r--   0        0        0    12911 2024-02-29 12:11:26.628310 ipfabric-6.7.2/ipfabric/diagrams/input_models/graph_parameters.py
+-rw-r--r--   0        0        0    13870 2024-02-29 12:11:26.629771 ipfabric-6.7.2/ipfabric/diagrams/input_models/graph_settings.py
+-rw-r--r--   0        0        0     5026 2024-02-29 12:11:26.630778 ipfabric-6.7.2/ipfabric/diagrams/input_models/shared_view.py
+-rw-r--r--   0        0        0       90 2024-02-29 12:11:26.632075 ipfabric-6.7.2/ipfabric/diagrams/output_models/__init__.py
+-rw-r--r--   0        0        0     5241 2024-02-29 12:11:26.633080 ipfabric-6.7.2/ipfabric/diagrams/output_models/graph_result.py
+-rw-r--r--   0        0        0     2278 2024-01-25 18:33:47.040766 ipfabric-6.7.2/ipfabric/diagrams/output_models/protocols.py
+-rw-r--r--   0        0        0     4556 2024-02-29 12:11:26.634080 ipfabric-6.7.2/ipfabric/diagrams/output_models/trace.py
+-rw-r--r--   0        0        0     2283 2024-03-20 16:35:10.768244 ipfabric-6.7.2/ipfabric/exceptions.py
+-rw-r--r--   0        0        0      670 2024-03-20 16:35:10.769326 ipfabric-6.7.2/ipfabric/models/__init__.py
+-rw-r--r--   0        0        0    22013 2024-03-20 16:35:10.770406 ipfabric-6.7.2/ipfabric/models/device.py
+-rw-r--r--   0        0        0     7677 2024-03-20 16:35:10.771408 ipfabric-6.7.2/ipfabric/models/intent.py
+-rw-r--r--   0        0        0     2796 2023-07-31 14:49:28.275721 ipfabric-6.7.2/ipfabric/models/intent_check.py
+-rw-r--r--   0        0        0    10641 2024-03-20 16:35:10.772481 ipfabric-6.7.2/ipfabric/models/inventory.py
+-rw-r--r--   0        0        0     5787 2024-03-20 16:35:10.773517 ipfabric-6.7.2/ipfabric/models/jobs.py
+-rw-r--r--   0        0        0     4128 2024-03-20 16:35:10.774564 ipfabric-6.7.2/ipfabric/models/oas.py
+-rw-r--r--   0        0        0     1888 2024-03-20 16:35:10.774564 ipfabric-6.7.2/ipfabric/models/rbac.py
+-rw-r--r--   0        0        0    27927 2024-03-20 16:35:10.775608 ipfabric-6.7.2/ipfabric/models/snapshot.py
+-rw-r--r--   0        0        0     5759 2024-03-20 16:35:10.775608 ipfabric-6.7.2/ipfabric/models/snapshots.py
+-rw-r--r--   0        0        0    23837 2024-03-20 16:35:10.776646 ipfabric-6.7.2/ipfabric/models/table.py
+-rw-r--r--   0        0        0     4145 2024-03-20 16:35:10.777686 ipfabric-6.7.2/ipfabric/models/technology/__init__.py
+-rw-r--r--   0        0        0     1504 2024-03-20 16:35:10.778718 ipfabric-6.7.2/ipfabric/models/technology/addressing.py
+-rw-r--r--   0        0        0      661 2024-03-20 16:35:10.778718 ipfabric-6.7.2/ipfabric/models/technology/cloud.py
+-rw-r--r--   0        0        0     2731 2024-03-20 16:35:10.779749 ipfabric-6.7.2/ipfabric/models/technology/dhcp.py
+-rw-r--r--   0        0        0     1315 2024-03-20 16:35:10.780776 ipfabric-6.7.2/ipfabric/models/technology/fhrp.py
+-rw-r--r--   0        0        0     8591 2024-03-20 16:35:10.781802 ipfabric-6.7.2/ipfabric/models/technology/interfaces.py
+-rw-r--r--   0        0        0      462 2024-03-20 16:35:10.781802 ipfabric-6.7.2/ipfabric/models/technology/ip_telephony.py
+-rw-r--r--   0        0        0     1086 2024-03-20 16:35:10.783360 ipfabric-6.7.2/ipfabric/models/technology/load_balancing.py
+-rw-r--r--   0        0        0      643 2024-03-20 16:35:10.784362 ipfabric-6.7.2/ipfabric/models/technology/managed_networks.py
+-rw-r--r--   0        0        0     7447 2024-03-20 16:35:10.785416 ipfabric-6.7.2/ipfabric/models/technology/management.py
+-rw-r--r--   0        0        0     2604 2024-03-20 16:35:10.785466 ipfabric-6.7.2/ipfabric/models/technology/mpls.py
+-rw-r--r--   0        0        0     3516 2024-03-20 16:35:10.786534 ipfabric-6.7.2/ipfabric/models/technology/multicast.py
+-rw-r--r--   0        0        0     1002 2024-03-20 16:35:10.787589 ipfabric-6.7.2/ipfabric/models/technology/neighbors.py
+-rw-r--r--   0        0        0      806 2024-03-20 16:35:10.787589 ipfabric-6.7.2/ipfabric/models/technology/oam.py
+-rw-r--r--   0        0        0     4436 2024-03-20 16:35:10.788591 ipfabric-6.7.2/ipfabric/models/technology/platforms.py
+-rw-r--r--   0        0        0     1579 2024-03-20 16:35:10.789626 ipfabric-6.7.2/ipfabric/models/technology/port_channels.py
+-rw-r--r--   0        0        0     1424 2024-03-20 16:35:10.790651 ipfabric-6.7.2/ipfabric/models/technology/qos.py
+-rw-r--r--   0        0        0     6912 2024-03-20 16:35:10.791753 ipfabric-6.7.2/ipfabric/models/technology/routing.py
+-rw-r--r--   0        0        0     2962 2024-03-20 16:35:10.791753 ipfabric-6.7.2/ipfabric/models/technology/sdn.py
+-rw-r--r--   0        0        0      604 2024-03-20 16:35:10.792841 ipfabric-6.7.2/ipfabric/models/technology/sdwan.py
+-rw-r--r--   0        0        0     2620 2024-03-20 16:35:10.793894 ipfabric-6.7.2/ipfabric/models/technology/security.py
+-rw-r--r--   0        0        0     2641 2024-03-20 16:35:10.793894 ipfabric-6.7.2/ipfabric/models/technology/stp.py
+-rw-r--r--   0        0        0     1134 2024-03-20 16:35:10.794896 ipfabric-6.7.2/ipfabric/models/technology/vlans.py
+-rw-r--r--   0        0        0     1145 2024-03-20 16:35:10.795936 ipfabric-6.7.2/ipfabric/models/technology/wireless.py
+-rw-r--r--   0        0        0     2409 2024-03-20 16:35:10.795936 ipfabric-6.7.2/ipfabric/models/users.py
+-rw-r--r--   0        0        0        0 2024-01-25 18:33:47.048277 ipfabric-6.7.2/ipfabric/oas/__init__.py
+-rw-r--r--   0        0        0   326420 2024-03-20 16:35:10.799023 ipfabric-6.7.2/ipfabric/oas/v6.6.json
+-rw-r--r--   0        0        0   327148 2024-03-20 16:35:10.801329 ipfabric-6.7.2/ipfabric/oas/v6.7.json
+-rw-r--r--   0        0        0     1172 2024-03-20 16:35:10.803997 ipfabric-6.7.2/ipfabric/settings/__init__.py
+-rw-r--r--   0        0        0     3641 2024-03-20 16:35:10.805129 ipfabric-6.7.2/ipfabric/settings/api_tokens.py
+-rw-r--r--   0        0        0     6751 2024-03-20 16:35:10.806145 ipfabric-6.7.2/ipfabric/settings/attributes.py
+-rw-r--r--   0        0        0     9119 2024-03-20 16:35:10.808322 ipfabric-6.7.2/ipfabric/settings/authentication.py
+-rw-r--r--   0        0        0     1394 2024-03-20 16:35:10.809455 ipfabric-6.7.2/ipfabric/settings/discovery.py
+-rw-r--r--   0        0        0     3266 2024-03-20 16:35:10.810505 ipfabric-6.7.2/ipfabric/settings/local_users.py
+-rw-r--r--   0        0        0    14522 2024-03-29 13:49:06.795074 ipfabric-6.7.2/ipfabric/settings/rbac.py
+-rw-r--r--   0        0        0     2284 2024-03-20 16:35:10.811555 ipfabric-6.7.2/ipfabric/settings/seeds.py
+-rw-r--r--   0        0        0     3137 2024-03-20 16:35:10.812643 ipfabric-6.7.2/ipfabric/settings/settings.py
+-rw-r--r--   0        0        0     2102 2024-03-20 16:35:10.813841 ipfabric-6.7.2/ipfabric/settings/site_separation.py
+-rw-r--r--   0        0        0     4487 2024-03-20 16:35:10.814866 ipfabric-6.7.2/ipfabric/settings/vendor_api.py
+-rw-r--r--   0        0        0     9120 2024-03-20 16:35:10.815971 ipfabric-6.7.2/ipfabric/settings/vendor_api_models.py
+-rw-r--r--   0        0        0      644 2024-03-20 16:35:10.817051 ipfabric-6.7.2/ipfabric/tools/__init__.py
+-rw-r--r--   0        0        0     8583 2024-03-20 16:35:10.818051 ipfabric-6.7.2/ipfabric/tools/configuration.py
+-rw-r--r--   0        0        0     5656 2024-03-20 16:35:10.819099 ipfabric-6.7.2/ipfabric/tools/discovery_history.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.819099 ipfabric-6.7.2/ipfabric/tools/managed_rbac/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.820129 ipfabric-6.7.2/ipfabric/tools/managed_rbac/v6/7/__init__.py
+-rw-r--r--   0        0        0    37895 2024-03-29 13:49:06.797076 ipfabric-6.7.2/ipfabric/tools/managed_rbac/v6/7/policies.json
+-rw-r--r--   0        0        0     3383 2024-03-29 13:49:06.798242 ipfabric-6.7.2/ipfabric/tools/managed_rbac/v6/7/roles.json
+-rw-r--r--   0        0        0        0 2024-03-20 16:35:10.821154 ipfabric-6.7.2/ipfabric/tools/managed_rbac/v6/__init__.py
+-rw-r--r--   0        0        0     4730 2024-01-25 18:33:47.054282 ipfabric-6.7.2/ipfabric/tools/nist.py
+-rw-r--r--   0        0        0     6782 2024-03-29 13:49:06.800107 ipfabric-6.7.2/ipfabric/tools/rbac.py
+-rw-r--r--   0        0        0     4260 2024-03-20 16:35:10.822260 ipfabric-6.7.2/ipfabric/tools/restore_intents.py
+-rw-r--r--   0        0        0    22669 2024-03-20 16:35:10.823261 ipfabric-6.7.2/ipfabric/tools/shared.py
+-rw-r--r--   0        0        0     2644 2024-02-07 13:28:55.569790 ipfabric-6.7.2/ipfabric/tools/site_seperation_report.py
+-rw-r--r--   0        0        0     2690 2023-12-13 15:03:30.822909 ipfabric-6.7.2/ipfabric/tools/vulnerabilities.py
+-rw-r--r--   0        0        0     1094 2021-11-18 17:57:34.710047 ipfabric-6.7.2/LICENSE
+-rw-r--r--   0        0        0     2787 2024-01-25 18:33:47.021681 ipfabric-6.7.2/NOTICES.md
+-rw-r--r--   0        0        0     3300 2024-04-03 16:20:13.648982 ipfabric-6.7.2/pyproject.toml
+-rw-r--r--   0        0        0     6226 2024-03-20 16:35:10.732833 ipfabric-6.7.2/README.md
+-rw-r--r--   0        0        0     8376 1970-01-01 00:00:00.000000 ipfabric-6.7.2/PKG-INFO
```

### Comparing `ipfabric-6.7.1/ipfabric/__init__.py` & `ipfabric-6.7.2/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/api.py` & `ipfabric-6.7.2/ipfabric/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     proxy: InitVar[Optional[ProxyTypes]] = field(default=None)
     proxies: InitVar[Optional[ProxiesTypes]] = field(default=None)
     mounts: InitVar[Optional[Mapping[str, Optional[BaseTransport]]]] = field(default=None)
     cert: InitVar[Optional[CertTypes]] = field(default=None)
     event_hooks: InitVar[Optional[Mapping[str, List[EventHook]]]] = field(default=None)
     local_oas: bool = Field(True, description="Default True, use local minified OAS file instead of servers.")
     debug: Optional[bool] = None
+    http2: InitVar[Optional[bool]] = field(default=True)
     _os_version: Optional[str] = None
     _client: Client = None
     _prev_snapshot_id: Optional[str] = None
     _attribute_filters: Optional[dict] = None
     _no_loaded_snapshots: bool = False
     _oas: Optional[OAS] = None
     _user: Optional[User] = None
@@ -85,14 +86,15 @@
         verify,
         timeout,
         proxy,
         proxies,
         mounts,
         cert,
         event_hooks,
+        http2,
     ):
         if token or (username and password):  # TODO: Remove v6.8
             warn(
                 "`token=''` or `username='', password=''` authentication will be deprecated in v6.8.0.",
                 DeprecationWarning,
                 stacklevel=2,
             )
@@ -115,14 +117,15 @@
             timeout=timeout,
             proxy=proxy,
             proxies=proxies,
             mounts=mounts,
             cert=cert,
             event_hooks=event_hooks,
             debug=self.debug,
+            http2=http2,
         )
         [setattr(self, k, v) for k, v in setup.update_attrs.items()]
 
         self._oas = OAS(client=self, local_oas=self.local_oas)
         self._user = self.get_user()
         self._snapshots = Snapshots(client=self)
         self.snapshot_id = setup.snapshot_id
```

### Comparing `ipfabric-6.7.1/ipfabric/auth.py` & `ipfabric-6.7.2/ipfabric/auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,15 @@
     snapshot_id: Optional[Union[str, None]] = Field(
         "$last", validation_alias=AliasChoices("snapshot_id", "ipf_snapshot")
     )
     verify: Optional[VerifyTypes] = True
     timeout: Union[TimeoutTypes, Literal["DEFAULT"]] = Timeout(timeout=5.0)
     nvd_api_key: Optional[str] = Field(None, alias="nvd_api_key")
     debug: Optional[bool] = False
+    http2: Optional[bool] = True
     proxy: Optional[Union[ProxyTypes, None]] = None
     proxies: Optional[Union[ProxiesTypes, None]] = None
     mounts: Optional[Mapping[str, Optional[BaseTransport]]] = None
     cert: Optional[Union[CertTypes, None]] = None
     event_hooks: Optional[Mapping[str, List[EventHook]]] = None
     _cookie_jar: CookieJar = PrivateAttr(default_factory=CookieJar)
     client: Optional[Client] = Field(None, exclude=True)
@@ -119,15 +120,15 @@
         )
 
     def model_post_init(self, __context):
         event_hooks = {"request": [log_request], "response": [log_response]} if self.debug else self.event_hooks
         self.client = Client(
             base_url=self.base_url,
             cookies=self._cookie_jar,
-            http2=True,
+            http2=self.http2,
             verify=self.verify,
             timeout=self.timeout,
             headers={"User-Agent": f'python-ipfabric-sdk/{metadata.version("ipfabric")}'},
             event_hooks=event_hooks,
             proxy=self.proxy,
             proxies=self.proxies,
             mounts=self.mounts,
```

### Comparing `ipfabric-6.7.1/ipfabric/client.py` & `ipfabric-6.7.2/ipfabric/client.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/__init__.py` & `ipfabric-6.7.2/ipfabric/diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/graphs.py` & `ipfabric-6.7.2/ipfabric/diagrams/graphs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/icmp.py` & `ipfabric-6.7.2/ipfabric/diagrams/icmp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/input_models/__init__.py` & `ipfabric-6.7.2/ipfabric/diagrams/input_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/input_models/constants.py` & `ipfabric-6.7.2/ipfabric/diagrams/input_models/constants.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json` & `ipfabric-6.7.2/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json` & `ipfabric-6.7.2/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/input_models/graph_parameters.py` & `ipfabric-6.7.2/ipfabric/diagrams/input_models/graph_parameters.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/input_models/graph_settings.py` & `ipfabric-6.7.2/ipfabric/diagrams/input_models/graph_settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/input_models/shared_view.py` & `ipfabric-6.7.2/ipfabric/diagrams/input_models/shared_view.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/output_models/graph_result.py` & `ipfabric-6.7.2/ipfabric/diagrams/output_models/graph_result.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/output_models/protocols.py` & `ipfabric-6.7.2/ipfabric/diagrams/output_models/protocols.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/diagrams/output_models/trace.py` & `ipfabric-6.7.2/ipfabric/diagrams/output_models/trace.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/exceptions.py` & `ipfabric-6.7.2/ipfabric/exceptions.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/__init__.py` & `ipfabric-6.7.2/ipfabric/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/device.py` & `ipfabric-6.7.2/ipfabric/models/device.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/intent.py` & `ipfabric-6.7.2/ipfabric/models/intent.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/intent_check.py` & `ipfabric-6.7.2/ipfabric/models/intent_check.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/inventory.py` & `ipfabric-6.7.2/ipfabric/models/inventory.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/jobs.py` & `ipfabric-6.7.2/ipfabric/models/jobs.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/oas.py` & `ipfabric-6.7.2/ipfabric/models/oas.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/rbac.py` & `ipfabric-6.7.2/ipfabric/models/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/snapshot.py` & `ipfabric-6.7.2/ipfabric/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/snapshots.py` & `ipfabric-6.7.2/ipfabric/models/snapshots.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/table.py` & `ipfabric-6.7.2/ipfabric/models/table.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/__init__.py` & `ipfabric-6.7.2/ipfabric/models/technology/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/addressing.py` & `ipfabric-6.7.2/ipfabric/models/technology/addressing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/cloud.py` & `ipfabric-6.7.2/ipfabric/models/technology/cloud.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/dhcp.py` & `ipfabric-6.7.2/ipfabric/models/technology/dhcp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/fhrp.py` & `ipfabric-6.7.2/ipfabric/models/technology/fhrp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/interfaces.py` & `ipfabric-6.7.2/ipfabric/models/technology/interfaces.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/load_balancing.py` & `ipfabric-6.7.2/ipfabric/models/technology/load_balancing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/managed_networks.py` & `ipfabric-6.7.2/ipfabric/models/technology/managed_networks.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/management.py` & `ipfabric-6.7.2/ipfabric/models/technology/management.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/mpls.py` & `ipfabric-6.7.2/ipfabric/models/technology/mpls.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/multicast.py` & `ipfabric-6.7.2/ipfabric/models/technology/multicast.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/neighbors.py` & `ipfabric-6.7.2/ipfabric/models/technology/neighbors.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/oam.py` & `ipfabric-6.7.2/ipfabric/models/technology/oam.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/platforms.py` & `ipfabric-6.7.2/ipfabric/models/technology/platforms.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/port_channels.py` & `ipfabric-6.7.2/ipfabric/models/technology/port_channels.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/qos.py` & `ipfabric-6.7.2/ipfabric/models/technology/qos.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/routing.py` & `ipfabric-6.7.2/ipfabric/models/technology/routing.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/sdn.py` & `ipfabric-6.7.2/ipfabric/models/technology/sdn.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/sdwan.py` & `ipfabric-6.7.2/ipfabric/models/technology/sdwan.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/security.py` & `ipfabric-6.7.2/ipfabric/models/technology/security.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/stp.py` & `ipfabric-6.7.2/ipfabric/models/technology/stp.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/vlans.py` & `ipfabric-6.7.2/ipfabric/models/technology/vlans.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/technology/wireless.py` & `ipfabric-6.7.2/ipfabric/models/technology/wireless.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/models/users.py` & `ipfabric-6.7.2/ipfabric/models/users.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/oas/v6.6.json` & `ipfabric-6.7.2/ipfabric/oas/v6.6.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/oas/v6.7.json` & `ipfabric-6.7.2/ipfabric/oas/v6.7.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/__init__.py` & `ipfabric-6.7.2/ipfabric/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/api_tokens.py` & `ipfabric-6.7.2/ipfabric/settings/api_tokens.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/attributes.py` & `ipfabric-6.7.2/ipfabric/settings/attributes.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/authentication.py` & `ipfabric-6.7.2/ipfabric/settings/authentication.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/discovery.py` & `ipfabric-6.7.2/ipfabric/settings/discovery.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/local_users.py` & `ipfabric-6.7.2/ipfabric/settings/local_users.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/rbac.py` & `ipfabric-6.7.2/ipfabric/settings/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/seeds.py` & `ipfabric-6.7.2/ipfabric/settings/seeds.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/settings.py` & `ipfabric-6.7.2/ipfabric/settings/settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/site_separation.py` & `ipfabric-6.7.2/ipfabric/settings/site_separation.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/vendor_api.py` & `ipfabric-6.7.2/ipfabric/settings/vendor_api.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/settings/vendor_api_models.py` & `ipfabric-6.7.2/ipfabric/settings/vendor_api_models.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/__init__.py` & `ipfabric-6.7.2/ipfabric/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/configuration.py` & `ipfabric-6.7.2/ipfabric/tools/configuration.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/discovery_history.py` & `ipfabric-6.7.2/ipfabric/tools/discovery_history.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/managed_rbac/v6/7/policies.json` & `ipfabric-6.7.2/ipfabric/tools/managed_rbac/v6/7/policies.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/managed_rbac/v6/7/roles.json` & `ipfabric-6.7.2/ipfabric/tools/managed_rbac/v6/7/roles.json`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/nist.py` & `ipfabric-6.7.2/ipfabric/tools/nist.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/rbac.py` & `ipfabric-6.7.2/ipfabric/tools/rbac.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/restore_intents.py` & `ipfabric-6.7.2/ipfabric/tools/restore_intents.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/shared.py` & `ipfabric-6.7.2/ipfabric/tools/shared.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/site_seperation_report.py` & `ipfabric-6.7.2/ipfabric/tools/site_seperation_report.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/ipfabric/tools/vulnerabilities.py` & `ipfabric-6.7.2/ipfabric/tools/vulnerabilities.py`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/LICENSE` & `ipfabric-6.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/NOTICES.md` & `ipfabric-6.7.2/NOTICES.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/pyproject.toml` & `ipfabric-6.7.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric"
-version = "v6.7.1"
+version = "v6.7.2"
 description = "Python package for interacting with IP Fabric"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Cristian Cordero <cristian.cordero@ipfabric.io>",
     "Solution Architecture <solution.architecture@ipfabric.io>"
 ]
 license = "MIT"
```

### Comparing `ipfabric-6.7.1/README.md` & `ipfabric-6.7.2/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric-6.7.1/PKG-INFO` & `ipfabric-6.7.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric
-Version: 6.7.1
+Version: 6.7.2
 Summary: Python package for interacting with IP Fabric
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.8,<4.0
```

