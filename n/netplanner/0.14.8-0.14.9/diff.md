# Comparing `tmp/netplanner-0.14.8.tar.gz` & `tmp/netplanner-0.14.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netplanner-0.14.8.tar", max compression
+gzip compressed data, was "netplanner-0.14.9.tar", max compression
```

## Comparing `netplanner-0.14.8.tar` & `netplanner-0.14.9.tar`

### file list

```diff
@@ -1,63 +1,64 @@
--rw-r--r--   0        0        0    35148 2024-01-11 14:16:49.906413 netplanner-0.14.8/LICENSE
--rw-r--r--   0        0        0     2977 2024-01-11 14:16:49.906413 netplanner-0.14.8/README.md
--rw-r--r--   0        0        0      878 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/__init__.py
--rw-r--r--   0        0        0     6091 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/__main__.py
--rw-r--r--   0        0        0     3115 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/config.py
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/__init__.py
--rw-r--r--   0        0        0     6327 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/base.py
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l2/__init__.py
--rw-r--r--   0        0        0     3333 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l2/bond.py
--rw-r--r--   0        0        0     2661 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l2/bridge.py
--rw-r--r--   0        0        0     1702 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l2/dummy.py
--rw-r--r--   0        0        0     3341 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l2/ethernet.py
--rw-r--r--   0        0        0     1574 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l2/veth.py
--rw-r--r--   0        0        0     3178 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l2/vlan.py
--rw-r--r--   0        0        0     1653 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l2/vrf.py
--rw-r--r--   0        0        0     3609 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l2/vxlan.py
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l3/__init__.py
--rw-r--r--   0        0        0      975 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l3/nameserver.py
--rw-r--r--   0        0        0     1530 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l3/route.py
--rw-r--r--   0        0        0     1256 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/l3/routing_policy.py
--rw-r--r--   0        0        0      993 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/match_object.py
--rw-r--r--   0        0        0     5023 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/interfaces/typing.py
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/loader/__init__.py
--rw-r--r--   0        0        0     2987 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/loader/config.py
--rw-r--r--   0        0        0     3304 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/loader/templates.py
--rw-r--r--   0        0        0     1574 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/loader/util.py
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/__init__.py
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/__init__.py
--rw-r--r--   0        0        0      241 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/files/10-vxlan-default.link
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/files/__init__.py
--rw-r--r--   0        0        0    11210 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/provider.py
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/__init__.py
--rw-r--r--   0        0        0      398 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/additionals.j2
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/__init__.py
--rw-r--r--   0        0        0      537 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/bond.j2
--rw-r--r--   0        0        0     1150 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/bridge.j2
--rw-r--r--   0        0        0      166 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/veth.j2
--rw-r--r--   0        0        0      860 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/vlan.j2
--rw-r--r--   0        0        0       27 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/vrf.j2
--rw-r--r--   0        0        0     2793 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/vxlan.j2
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/__init__.py
--rw-r--r--   0        0        0      342 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/bridge_port.j2
--rw-r--r--   0        0        0     1030 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/link.j2
--rw-r--r--   0        0        0     1038 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/match.j2
--rw-r--r--   0        0        0      338 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/nameserver.j2
--rw-r--r--   0        0        0     2055 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/network.j2
--rw-r--r--   0        0        0     1125 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/route.j2
--rw-r--r--   0        0        0      744 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/route_policy.j2
--rw-r--r--   0        0        0      156 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/sriov.j2
--rw-r--r--   0        0        0     1406 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/unused.j2
--rw-r--r--   0        0        0      915 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/systemd.link.j2
--rwxr-xr-x   0        0        0     1502 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/systemd.netdev.j2
--rwxr-xr-x   0        0        0      629 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/providers/networkd/templates/systemd.network.j2
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/sriov/__init__.py
--rw-r--r--   0        0        0     4542 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/sriov/__main__.py
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/sriov/files/__init__.py
--rw-r--r--   0        0        0      363 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/sriov/files/sriov-setup.service
--rw-r--r--   0        0        0      118 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/sriov/files/sriov-udev.rules
--rw-r--r--   0        0        0    14269 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/sriov/pci.py
--rw-r--r--   0        0        0        0 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/sriov/templates/__init__.py
--rw-r--r--   0        0        0      320 2024-01-11 14:16:49.906413 netplanner-0.14.8/netplanner/sriov/templates/netplanner-delayed-rebind.j2
--rw-r--r--   0        0        0      683 2024-01-11 14:16:49.906413 netplanner-0.14.8/pyproject.toml
--rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 netplanner-0.14.8/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-03 13:44:41.287334 netplanner-0.14.9/LICENSE
+-rw-r--r--   0        0        0      301 2024-04-03 13:44:41.287334 netplanner-0.14.9/NOTICE
+-rw-r--r--   0        0        0     2977 2024-04-03 13:44:41.287334 netplanner-0.14.9/README.md
+-rw-r--r--   0        0        0      878 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/__init__.py
+-rw-r--r--   0        0        0     6091 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/__main__.py
+-rw-r--r--   0        0        0     3115 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/config.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/__init__.py
+-rw-r--r--   0        0        0     6327 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/base.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l2/__init__.py
+-rw-r--r--   0        0        0     3333 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l2/bond.py
+-rw-r--r--   0        0        0     2661 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l2/bridge.py
+-rw-r--r--   0        0        0     1702 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l2/dummy.py
+-rw-r--r--   0        0        0     3341 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l2/ethernet.py
+-rw-r--r--   0        0        0     1574 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l2/veth.py
+-rw-r--r--   0        0        0     3178 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l2/vlan.py
+-rw-r--r--   0        0        0     1653 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l2/vrf.py
+-rw-r--r--   0        0        0     3609 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l2/vxlan.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l3/__init__.py
+-rw-r--r--   0        0        0      975 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l3/nameserver.py
+-rw-r--r--   0        0        0     1530 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l3/route.py
+-rw-r--r--   0        0        0     1256 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/l3/routing_policy.py
+-rw-r--r--   0        0        0      993 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/match_object.py
+-rw-r--r--   0        0        0     5023 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/interfaces/typing.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/loader/__init__.py
+-rw-r--r--   0        0        0     2987 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/loader/config.py
+-rw-r--r--   0        0        0     3304 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/loader/templates.py
+-rw-r--r--   0        0        0     1574 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/loader/util.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/__init__.py
+-rw-r--r--   0        0        0      241 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/files/10-vxlan-default.link
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/files/__init__.py
+-rw-r--r--   0        0        0    11210 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/provider.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/__init__.py
+-rw-r--r--   0        0        0      398 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/additionals.j2
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/__init__.py
+-rw-r--r--   0        0        0      537 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/bond.j2
+-rw-r--r--   0        0        0     1150 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/bridge.j2
+-rw-r--r--   0        0        0      166 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/veth.j2
+-rw-r--r--   0        0        0      860 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/vlan.j2
+-rw-r--r--   0        0        0       27 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/vrf.j2
+-rw-r--r--   0        0        0     2793 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/vxlan.j2
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/__init__.py
+-rw-r--r--   0        0        0      342 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/bridge_port.j2
+-rw-r--r--   0        0        0     1030 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/link.j2
+-rw-r--r--   0        0        0     1038 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/match.j2
+-rw-r--r--   0        0        0      338 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/nameserver.j2
+-rw-r--r--   0        0        0     2055 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/network.j2
+-rw-r--r--   0        0        0     1125 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/route.j2
+-rw-r--r--   0        0        0      744 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/route_policy.j2
+-rw-r--r--   0        0        0      156 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/sriov.j2
+-rw-r--r--   0        0        0     1406 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/unused.j2
+-rw-r--r--   0        0        0      915 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/systemd.link.j2
+-rwxr-xr-x   0        0        0     1502 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/systemd.netdev.j2
+-rwxr-xr-x   0        0        0      629 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/providers/networkd/templates/systemd.network.j2
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/sriov/__init__.py
+-rw-r--r--   0        0        0     4588 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/sriov/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/sriov/files/__init__.py
+-rw-r--r--   0        0        0      363 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/sriov/files/sriov-setup.service
+-rw-r--r--   0        0        0      118 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/sriov/files/sriov-udev.rules
+-rw-r--r--   0        0        0    14871 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/sriov/pci.py
+-rw-r--r--   0        0        0        0 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/sriov/templates/__init__.py
+-rw-r--r--   0        0        0      320 2024-04-03 13:44:41.287334 netplanner-0.14.9/netplanner/sriov/templates/netplanner-delayed-rebind.j2
+-rw-r--r--   0        0        0      683 2024-04-03 13:44:41.291334 netplanner-0.14.9/pyproject.toml
+-rw-r--r--   0        0        0     3675 1970-01-01 00:00:00.000000 netplanner-0.14.9/PKG-INFO
```

### Comparing `netplanner-0.14.8/LICENSE` & `netplanner-0.14.9/LICENSE`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/README.md` & `netplanner-0.14.9/README.md`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/__init__.py` & `netplanner-0.14.9/netplanner/__init__.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/__main__.py` & `netplanner-0.14.9/netplanner/__main__.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/config.py` & `netplanner-0.14.9/netplanner/config.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/base.py` & `netplanner-0.14.9/netplanner/interfaces/base.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l2/bond.py` & `netplanner-0.14.9/netplanner/interfaces/l2/bond.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l2/bridge.py` & `netplanner-0.14.9/netplanner/interfaces/l2/bridge.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l2/dummy.py` & `netplanner-0.14.9/netplanner/interfaces/l2/dummy.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l2/ethernet.py` & `netplanner-0.14.9/netplanner/interfaces/l2/ethernet.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l2/veth.py` & `netplanner-0.14.9/netplanner/interfaces/l2/veth.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l2/vlan.py` & `netplanner-0.14.9/netplanner/interfaces/l2/vlan.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l2/vrf.py` & `netplanner-0.14.9/netplanner/interfaces/l2/vrf.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l2/vxlan.py` & `netplanner-0.14.9/netplanner/interfaces/l2/vxlan.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l3/nameserver.py` & `netplanner-0.14.9/netplanner/interfaces/l3/nameserver.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l3/route.py` & `netplanner-0.14.9/netplanner/interfaces/l3/route.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/l3/routing_policy.py` & `netplanner-0.14.9/netplanner/interfaces/l3/routing_policy.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/match_object.py` & `netplanner-0.14.9/netplanner/interfaces/match_object.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/interfaces/typing.py` & `netplanner-0.14.9/netplanner/interfaces/typing.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/loader/config.py` & `netplanner-0.14.9/netplanner/loader/config.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/loader/templates.py` & `netplanner-0.14.9/netplanner/loader/templates.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/loader/util.py` & `netplanner-0.14.9/netplanner/loader/util.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/provider.py` & `netplanner-0.14.9/netplanner/providers/networkd/provider.py`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/bond.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/bond.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/bridge.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/bridge.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/vlan.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/vlan.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/netdev_includes/vxlan.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/netdev_includes/vxlan.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/link.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/link.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/match.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/match.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/network.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/network.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/route.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/route.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/route_policy.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/route_policy.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/network_includes/unused.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/network_includes/unused.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/systemd.link.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/systemd.link.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/systemd.netdev.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/systemd.netdev.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/providers/networkd/templates/systemd.network.j2` & `netplanner-0.14.9/netplanner/providers/networkd/templates/systemd.network.j2`

 * *Files identical despite different names*

### Comparing `netplanner-0.14.8/netplanner/sriov/__main__.py` & `netplanner-0.14.9/netplanner/sriov/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,8 +111,9 @@
                     ]
                 )
 
 
 def rebind(pci_addresses: list[str]):
     for pci_address in pci_addresses:
         device = pci.PCIDevice(pci_address)
+        device.sriov_drivers_autoprobe = True
         pci.bind_vfs(device.vfs)
```

### Comparing `netplanner-0.14.8/netplanner/sriov/pci.py` & `netplanner-0.14.9/netplanner/sriov/pci.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,14 +168,27 @@
                 "set",
                 "pci/{}".format(self.pci_addr),
                 prop,
                 value,
             ]
         )
 
+    @property
+    def sriov_drivers_autoprobe(self) -> bool:
+        sriov_drivers_autoprobe_file = self.subpath("sriov_drivers_autoprobe")
+        with open(sriov_drivers_autoprobe_file, "r") as f:
+            read_data = f.read()
+        return bool(int(read_data.strip()))
+
+    @sriov_drivers_autoprobe.setter
+    def sriov_drivers_autoprobe(self, value: bool):
+        sriov_drivers_autoprobe_file = self.subpath("sriov_drivers_autoprobe")
+        with open(sriov_drivers_autoprobe_file, "w") as f:
+            f.write("1" if value else "0")
+
     def __str__(self) -> str:
         """String represenation of object
 
         :return: PCI address of string
         :rtype: str
         """
         return self.pci_addr
@@ -420,14 +433,15 @@
                 unbind_vfs(self.pci_device.vfs)
                 self.pci_device.devlink_set("eswitch", "mode", switch_mode)
             finally:
                 pass
             self.update_attributes()
 
     def bind_vfs(self):
+        self.pci_device.sriov_drivers_autoprobe = True
         bind_vfs(self.pci_device.vfs)
 
 
 class PCINetDevices(object):
     def __init__(self):
         self.pci_devices = [PCINetDevice(dev) for dev in get_pci_ethernet_addresses()]
```

### Comparing `netplanner-0.14.8/pyproject.toml` & `netplanner-0.14.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "netplanner"
-version = "0.14.8"
+version = "0.14.9"
 description = "Mimir the Netplanner is the ground of all network wisdöm"
 authors = ["Marcel Fest <marcel.fest@telekom.de>", "Christopher Dziomba <christopher.dziomba@telekom.de>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4"
```

### Comparing `netplanner-0.14.8/PKG-INFO` & `netplanner-0.14.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netplanner
-Version: 0.14.8
+Version: 0.14.9
 Summary: Mimir the Netplanner is the ground of all network wisdöm
 License: GPL-3.0-only
 Author: Marcel Fest
 Author-email: marcel.fest@telekom.de
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
```

