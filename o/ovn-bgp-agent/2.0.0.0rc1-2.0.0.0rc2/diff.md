# Comparing `tmp/ovn-bgp-agent-2.0.0.0rc1.tar.gz` & `tmp/ovn-bgp-agent-2.0.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovn-bgp-agent-2.0.0.0rc1.tar", last modified: Thu Mar 14 07:29:12 2024, max compression
+gzip compressed data, was "ovn-bgp-agent-2.0.0.0rc2.tar", last modified: Thu Mar 28 14:36:00 2024, max compression
```

## Comparing `ovn-bgp-agent-2.0.0.0rc1.tar` & `ovn-bgp-agent-2.0.0.0rc2.tar`

### file list

```diff
@@ -1,173 +1,173 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.474175 ovn-bgp-agent-2.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/.mailmap
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2024-03-14 07:29:12.000000 ovn-bgp-agent-2.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2024-03-14 07:29:12.000000 ovn-bgp-agent-2.0.0.0rc1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2024-03-14 07:29:12.474175 ovn-bgp-agent-2.0.0.0rc1/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.446167 ovn-bgp-agent-2.0.0.0rc1/devstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.446167 ovn-bgp-agent-2.0.0.0rc1/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5528 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/devstack/lib/ovn-bgp-agent
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2748 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/devstack/local.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1375 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.446167 ovn-bgp-agent-2.0.0.0rc1/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.450168 ovn-bgp-agent-2.0.0.0rc1/doc/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   105821 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/images/evpn_traffic_flow.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    97580 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/images/networking-bgpvpn_integration.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    45390 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/images/ovn-cluster-overview.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.450168 ovn-bgp-agent-2.0.0.0rc1/doc/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10718 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/bgp_supportability_matrix.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2652 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.450168 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6102 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/agent_deployment.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2428 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/bgp_advertising.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2999 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/bgp_traffic_redirection.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.450168 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14010 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/bgp_mode_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11439 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/bgp_mode_stretched_l2_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21095 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/evpn_mode_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18755 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/nb_bgp_mode_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10814 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/ovn_bgp_mode_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.442166 ovn-bgp-agent-2.0.0.0rc1/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.450168 ovn-bgp-agent-2.0.0.0rc1/etc/frr/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/etc/frr/daemons
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1401 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/etc/frr/frr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.450168 ovn-bgp-agent-2.0.0.0rc1/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/etc/oslo-config-generator/bgp-agent.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.450168 ovn-bgp-agent-2.0.0.0rc1/etc/ovn-bgp-agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/etc/ovn-bgp-agent/rootwrap.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.454169 ovn-bgp-agent-2.0.0.0rc1/etc/ovn-bgp-agent/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/etc/ovn-bgp-agent/rootwrap.d/rootwrap.filters
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.454169 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2677 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.454169 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/cmd/agent.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12808 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3717 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.454169 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/driver_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.458170 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44797 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/nb_ovn_bgp_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52277 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/ovn_bgp_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36112 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/ovn_evpn_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19868 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/ovn_stretched_l2_bgp_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.458170 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1795 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/bgp.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2259 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/driver_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4474 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/frr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32082 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/ovn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11879 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/ovs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29185 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/wire.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.458170 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/watchers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/watchers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6409 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/watchers/base_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20017 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/watchers/bgp_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9060 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/watchers/evpn_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31541 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/watchers/nb_bgp_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4243 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.462171 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20685 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/privileged/linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/privileged/ovs_vsctl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/privileged/vtysh.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.462171 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.462171 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4301 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.462171 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27568 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/privileged/test_linux_net.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.462171 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5952 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/utils/test_linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/test_ovn_bgp_agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.462171 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.462171 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/cmd/test_agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.462171 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.466173 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    75315 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/test_nb_ovn_bgp_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   105260 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_bgp_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34238 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_evpn_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42246 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_stretched_l2_bgp_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.466173 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4009 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_driver_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3789 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_frr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35947 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovn.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21336 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25295 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_wire.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.466173 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8538 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_base_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    49088 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_bgp_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22830 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_evpn_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    68241 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_nb_bgp_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.470173 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/privileged/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/privileged/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4149 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/privileged/test_linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3234 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/privileged/test_ovs_vsctl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2233 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/privileged/test_vtysh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/test_agent.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.470173 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2999 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/utils/test_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36468 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/utils/test_linux_net.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1751 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.470173 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/utils/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1386 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/utils/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27640 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/utils/linux_net.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.454169 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2024-03-14 07:29:12.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5254 2024-03-14 07:29:12.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 07:29:12.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2024-03-14 07:29:12.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-14 07:29:12.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-14 07:29:12.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-03-14 07:29:12.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2024-03-14 07:29:12.000000 ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.442166 ovn-bgp-agent-2.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.470173 ovn-bgp-agent-2.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/releasenotes/notes/nb_driver-cc7098183fcedb0a.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.474175 ovn-bgp-agent-2.0.0.0rc1/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.474175 ovn-bgp-agent-2.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.474175 ovn-bgp-agent-2.0.0.0rc1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2024-03-14 07:29:12.474175 ovn-bgp-agent-2.0.0.0rc1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1650 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-14 07:29:12.474175 ovn-bgp-agent-2.0.0.0rc1/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-03-14 07:28:45.000000 ovn-bgp-agent-2.0.0.0rc1/zuul.d/tempest-singlenode.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.919339 ovn-bgp-agent-2.0.0.0rc2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/.mailmap
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      775 2024-03-28 14:36:00.000000 ovn-bgp-agent-2.0.0.0rc2/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12076 2024-03-28 14:36:00.000000 ovn-bgp-agent-2.0.0.0rc2/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2024-03-28 14:36:00.919339 ovn-bgp-agent-2.0.0.0rc2/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      474 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.891338 ovn-bgp-agent-2.0.0.0rc2/devstack/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.891338 ovn-bgp-agent-2.0.0.0rc2/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5528 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/devstack/lib/ovn-bgp-agent
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2748 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/devstack/local.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1375 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1099 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.891338 ovn-bgp-agent-2.0.0.0rc2/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.891338 ovn-bgp-agent-2.0.0.0rc2/doc/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   105821 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/images/evpn_traffic_flow.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    97580 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/images/networking-bgpvpn_integration.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    45390 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/images/ovn-cluster-overview.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.891338 ovn-bgp-agent-2.0.0.0rc2/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10718 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/bgp_supportability_matrix.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2652 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.891338 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6102 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/agent_deployment.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2428 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/bgp_advertising.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2999 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/bgp_traffic_redirection.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.895338 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14010 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/bgp_mode_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11439 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/bgp_mode_stretched_l2_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21095 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/evpn_mode_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18755 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/nb_bgp_mode_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10814 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/ovn_bgp_mode_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      203 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      556 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.883338 ovn-bgp-agent-2.0.0.0rc2/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.895338 ovn-bgp-agent-2.0.0.0rc2/etc/frr/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/etc/frr/daemons
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1401 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/etc/frr/frr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.895338 ovn-bgp-agent-2.0.0.0rc2/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/etc/oslo-config-generator/bgp-agent.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.895338 ovn-bgp-agent-2.0.0.0rc2/etc/ovn-bgp-agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      994 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/etc/ovn-bgp-agent/rootwrap.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.895338 ovn-bgp-agent-2.0.0.0rc2/etc/ovn-bgp-agent/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      637 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/etc/ovn-bgp-agent/rootwrap.d/rootwrap.filters
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.895338 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2677 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.895338 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      669 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/cmd/agent.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12808 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3717 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.899339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/driver_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.899339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44797 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/nb_ovn_bgp_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52277 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/ovn_bgp_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36112 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/ovn_evpn_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19868 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/ovn_stretched_l2_bgp_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.899339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1795 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/bgp.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3593 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/driver_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4474 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/frr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31935 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/ovn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11879 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/ovs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29185 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/wire.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.903339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/watchers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/watchers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5274 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/watchers/base_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20017 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/watchers/bgp_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9060 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/watchers/evpn_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31541 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/watchers/nb_bgp_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4243 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.903339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20685 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/privileged/linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1478 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/privileged/ovs_vsctl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1576 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/privileged/vtysh.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.903339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1388 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.907339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4301 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.907339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27568 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/privileged/test_linux_net.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.907339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5952 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/utils/test_linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      792 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/test_ovn_bgp_agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.907339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.907339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      904 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/cmd/test_agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.907339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.911339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    75315 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/test_nb_ovn_bgp_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   105260 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_bgp_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34238 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_evpn_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42246 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_stretched_l2_bgp_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.911339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5591 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_driver_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3789 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_frr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35947 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovn.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21336 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25295 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_wire.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.915339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8538 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_base_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    49088 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_bgp_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22830 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_evpn_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    68241 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_nb_bgp_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.915339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/privileged/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/privileged/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4149 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/privileged/test_linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3234 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/privileged/test_ovs_vsctl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2233 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/privileged/test_vtysh.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1424 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/test_agent.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.915339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2999 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/utils/test_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36468 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/utils/test_linux_net.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1751 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.915339 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      683 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/utils/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1386 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/utils/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27640 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/utils/linux_net.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.895338 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1525 2024-03-28 14:36:00.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5254 2024-03-28 14:36:00.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-28 14:36:00.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      616 2024-03-28 14:36:00.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-28 14:36:00.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-28 14:36:00.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-03-28 14:36:00.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       14 2024-03-28 14:36:00.000000 ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.887338 ovn-bgp-agent-2.0.0.0rc2/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.919339 ovn-bgp-agent-2.0.0.0rc2/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/releasenotes/notes/nb_driver-cc7098183fcedb0a.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.919339 ovn-bgp-agent-2.0.0.0rc2/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.919339 ovn-bgp-agent-2.0.0.0rc2/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.919339 ovn-bgp-agent-2.0.0.0rc2/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2024-03-28 14:36:00.923339 ovn-bgp-agent-2.0.0.0rc2/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      493 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/test-requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1648 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-28 14:36:00.919339 ovn-bgp-agent-2.0.0.0rc2/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      432 2024-03-28 14:35:37.000000 ovn-bgp-agent-2.0.0.0rc2/zuul.d/tempest-singlenode.yaml
```

### Comparing `ovn-bgp-agent-2.0.0.0rc1/AUTHORS` & `ovn-bgp-agent-2.0.0.0rc2/AUTHORS`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/CONTRIBUTING.rst` & `ovn-bgp-agent-2.0.0.0rc2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ChangeLog` & `ovn-bgp-agent-2.0.0.0rc2/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+2.0.0.0rc2
+----------
+
+* Fix placement of lsp when external\_ids not in sync
+* Update TOX\_CONSTRAINTS\_FILE for stable/2024.1
+* Update .gitreview for stable/2024.1
+
 2.0.0.0rc1
 ----------
 
 * [NB watcher] Prevent lsp events for remote tenant events
 * Change default to NB DB Driver
 * Fix typo for linux util function used at evpn driver
 * Bump OVS version (branch 3.3) for devstack local.conf sample
```

### Comparing `ovn-bgp-agent-2.0.0.0rc1/LICENSE` & `ovn-bgp-agent-2.0.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/PKG-INFO` & `ovn-bgp-agent-2.0.0.0rc2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovn-bgp-agent
-Version: 2.0.0.0rc1
+Version: 2.0.0.0rc2
 Summary: The OVN BGP Agent allows to expose VMs/Containers/Networks through BGP on OVN
 Home-page: https://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =============
         OVN BGP Agent
```

### Comparing `ovn-bgp-agent-2.0.0.0rc1/devstack/lib/ovn-bgp-agent` & `ovn-bgp-agent-2.0.0.0rc2/devstack/lib/ovn-bgp-agent`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/devstack/local.conf.sample` & `ovn-bgp-agent-2.0.0.0rc2/devstack/local.conf.sample`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/devstack/plugin.sh` & `ovn-bgp-agent-2.0.0.0rc2/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/devstack/settings` & `ovn-bgp-agent-2.0.0.0rc2/devstack/settings`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/images/evpn_traffic_flow.png` & `ovn-bgp-agent-2.0.0.0rc2/doc/images/evpn_traffic_flow.png`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/images/networking-bgpvpn_integration.png` & `ovn-bgp-agent-2.0.0.0rc2/doc/images/networking-bgpvpn_integration.png`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/images/ovn-cluster-overview.png` & `ovn-bgp-agent-2.0.0.0rc2/doc/images/ovn-cluster-overview.png`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/bgp_supportability_matrix.rst` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/bgp_supportability_matrix.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/conf.py` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/agent_deployment.rst` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/agent_deployment.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/bgp_advertising.rst` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/bgp_advertising.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/bgp_traffic_redirection.rst` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/bgp_traffic_redirection.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/bgp_mode_design.rst` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/bgp_mode_design.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/bgp_mode_stretched_l2_design.rst` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/bgp_mode_stretched_l2_design.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/evpn_mode_design.rst` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/evpn_mode_design.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/nb_bgp_mode_design.rst` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/nb_bgp_mode_design.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/contributor/drivers/ovn_bgp_mode_design.rst` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/contributor/drivers/ovn_bgp_mode_design.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/doc/source/index.rst` & `ovn-bgp-agent-2.0.0.0rc2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/etc/frr/daemons` & `ovn-bgp-agent-2.0.0.0rc2/etc/frr/daemons`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/etc/frr/frr.conf` & `ovn-bgp-agent-2.0.0.0rc2/etc/frr/frr.conf`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/etc/ovn-bgp-agent/rootwrap.conf` & `ovn-bgp-agent-2.0.0.0rc2/etc/ovn-bgp-agent/rootwrap.conf`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/etc/ovn-bgp-agent/rootwrap.d/rootwrap.filters` & `ovn-bgp-agent-2.0.0.0rc2/etc/ovn-bgp-agent/rootwrap.d/rootwrap.filters`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/__init__.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/agent.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/agent.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/cmd/agent.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/cmd/agent.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/config.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/config.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/constants.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/constants.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/driver_api.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/driver_api.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/nb_ovn_bgp_driver.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/nb_ovn_bgp_driver.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/ovn_bgp_driver.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/ovn_bgp_driver.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/ovn_evpn_driver.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/ovn_evpn_driver.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/ovn_stretched_l2_bgp_driver.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/ovn_stretched_l2_bgp_driver.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/bgp.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/bgp.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/frr.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/frr.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/ovn.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/ovn.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 from ovsdbapp.backend.ovs_idl import idlutils
 from ovsdbapp.backend.ovs_idl import rowview
 from ovsdbapp import event
 from ovsdbapp.schema.ovn_northbound import impl_idl as nb_impl_idl
 from ovsdbapp.schema.ovn_southbound import impl_idl as sb_impl_idl
 
 from ovn_bgp_agent import constants
+from ovn_bgp_agent.drivers.openstack.utils import driver_utils
 from ovn_bgp_agent import exceptions
 from ovn_bgp_agent.utils import helpers
 
 CONF = cfg.CONF
 LOG = logging.getLogger(__name__)
 
 
@@ -410,22 +411,18 @@
         nat_info = cmd.execute(check_error=True)
         return nat_info[0] if nat_info else []
 
     def get_active_lsp_on_chassis(self, chassis):
         ports = []
         cmd = self.db_find_rows('Logical_Switch_Port', ('up', '=', True))
         for row in cmd.execute(check_error=True):
-            if (row.external_ids and
-                    row.external_ids.get(
-                        constants.OVN_HOST_ID_EXT_ID_KEY) == chassis):
-                ports.append(row)
-            elif (row.options and
-                    row.options.get(
-                        constants.OVN_REQUESTED_CHASSIS) == chassis):
+            port_chassis, _ = driver_utils.get_port_chassis(row, chassis)
+            if port_chassis == chassis:
                 ports.append(row)
+
         return ports
 
     def get_active_cr_lrp_on_chassis(self, chassis):
         ports = []
         rows = self.db_list_rows('Logical_Router_Port').execute(
             check_error=True)
```

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/ovs.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/ovs.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/utils/wire.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/utils/wire.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/watchers/base_watcher.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/watchers/base_watcher.py`

 * *Files 14% similar despite different names*

```diff
@@ -93,38 +93,16 @@
             events, table, None)
         self.event_name = self.__class__.__name__
 
     def _check_ip_associated(self, mac):
         return len(mac.strip().split(' ')) > 1
 
     def _get_chassis(self, row, default_type=constants.OVN_VM_VIF_PORT_TYPE):
-        # row.options['requested-chassis'] superseeds the id in external_ids.
-        # Since it is not used for virtual ports by ovn, this option will be
-        # ignored for virtual ports.
-
-        # since 'old' rows could be used, it will not hold the type information
-        # if that is the case, please supply a default in the arguments.
-        row_type = getattr(row, 'type', default_type)
-        if (row_type not in [constants.OVN_VIRTUAL_VIF_PORT_TYPE] and
-                hasattr(row, 'options') and
-                row.options.get(constants.OVN_REQUESTED_CHASSIS)):
-
-            # requested-chassis can be a comma separated list,
-            # so lets only return our chassis if it is a list, to be able to
-            # do a == equal comparison
-            req_chassis = row.options[constants.OVN_REQUESTED_CHASSIS]
-            if self.agent.chassis in req_chassis.split(','):
-                req_chassis = self.agent.chassis
-
-            return (req_chassis, constants.OVN_CHASSIS_AT_OPTIONS)
-        elif (hasattr(row, 'external_ids') and
-                row.external_ids.get(constants.OVN_HOST_ID_EXT_ID_KEY)):
-            return (row.external_ids[constants.OVN_HOST_ID_EXT_ID_KEY],
-                    constants.OVN_CHASSIS_AT_EXT_IDS)
-        return None, None
+        return driver_utils.get_port_chassis(row, self.agent.chassis,
+                                             default_port_type=default_type)
 
     def _has_additional_binding(self, row):
         if (hasattr(row, 'options') and
                 row.options.get(constants.OVN_REQUESTED_CHASSIS)):
 
             # requested-chassis can be a comma separated list, so if there
             # is a comma in the string, there is an additional binding.
```

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/watchers/bgp_watcher.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/watchers/bgp_watcher.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/watchers/evpn_watcher.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/watchers/evpn_watcher.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/drivers/openstack/watchers/nb_bgp_watcher.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/drivers/openstack/watchers/nb_bgp_watcher.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/exceptions.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/exceptions.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/privileged/__init__.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/privileged/__init__.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/privileged/linux_net.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/privileged/linux_net.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/privileged/ovs_vsctl.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/privileged/ovs_vsctl.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/privileged/vtysh.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/privileged/vtysh.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/base.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/base.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/base.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/privileged/test_linux_net.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/privileged/test_linux_net.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/functional/utils/test_linux_net.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/functional/utils/test_linux_net.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/test_ovn_bgp_agent.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/test_ovn_bgp_agent.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/cmd/test_agent.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/cmd/test_agent.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/test_nb_ovn_bgp_driver.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/test_nb_ovn_bgp_driver.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_bgp_driver.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_bgp_driver.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_evpn_driver.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_evpn_driver.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_stretched_l2_bgp_driver.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/test_ovn_stretched_l2_bgp_driver.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_driver_utils.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_driver_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -64,14 +64,52 @@
         # No Address pools
         port = utils.create_row(external_ids={})
         self.assertDictEqual(driver_utils.get_addr_scopes(port), {
             constants.IP_VERSION_4: None,
             constants.IP_VERSION_6: None,
         })
 
+    def test_get_port_chassis_from_options(self):
+        my_host = 'foo-host'
+
+        # it is a VM port type, should use options field.
+        row = utils.create_row(
+            external_ids={constants.OVN_HOST_ID_EXT_ID_KEY: 'bar-host'},
+            options={constants.OVN_REQUESTED_CHASSIS: my_host})
+
+        self.assertEqual(driver_utils.get_port_chassis(row, chassis=my_host),
+                         (my_host, constants.OVN_CHASSIS_AT_OPTIONS))
+
+    def test_get_port_chassis_from_external_ids(self):
+        my_host = 'foo-host'
+
+        # it is a VM port type, should use options field.
+        row = utils.create_row(
+            external_ids={constants.OVN_HOST_ID_EXT_ID_KEY: my_host})
+
+        self.assertEqual(driver_utils.get_port_chassis(row, chassis=my_host),
+                         (my_host, constants.OVN_CHASSIS_AT_EXT_IDS))
+
+    def test_get_port_chassis_from_external_ids_virtual_port(self):
+        my_host = 'foo-host'
+
+        # it is a VM port type, should use options field.
+        row = utils.create_row(
+            external_ids={constants.OVN_HOST_ID_EXT_ID_KEY: my_host},
+            options={constants.OVN_REQUESTED_CHASSIS: 'bar-host'},
+            type=constants.OVN_VIRTUAL_VIF_PORT_TYPE)
+
+        self.assertEqual(driver_utils.get_port_chassis(row, chassis=my_host),
+                         (my_host, constants.OVN_CHASSIS_AT_EXT_IDS))
+
+    def test_get_port_chassis_no_information(self):
+        row = utils.create_row()
+        self.assertEqual(driver_utils.get_port_chassis(row, chassis='foo'),
+                         (None, None))
+
     def test_check_name_prefix(self):
         lb = utils.create_row(name='some-name')
         self.assertTrue(driver_utils.check_name_prefix(lb, 'some'))
         self.assertFalse(driver_utils.check_name_prefix(lb, 'other'))
 
         lb = utils.create_row(no_name='aa')
         self.assertFalse(driver_utils.check_name_prefix(lb, ''))
```

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_frr.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_frr.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovn.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovn.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovs.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_ovs.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_wire.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/utils/test_wire.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_base_watcher.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_base_watcher.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_bgp_watcher.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_bgp_watcher.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_evpn_watcher.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_evpn_watcher.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_nb_bgp_watcher.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/drivers/openstack/watchers/test_nb_bgp_watcher.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/fakes.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/fakes.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/privileged/test_linux_net.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/privileged/test_linux_net.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/privileged/test_ovs_vsctl.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/privileged/test_ovs_vsctl.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/privileged/test_vtysh.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/privileged/test_vtysh.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/test_agent.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/test_agent.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/utils/test_helpers.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/unit/utils/test_linux_net.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/unit/utils/test_linux_net.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/tests/utils.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/utils/common.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/utils/common.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/utils/helpers.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent/utils/linux_net.py` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent/utils/linux_net.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/PKG-INFO` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovn-bgp-agent
-Version: 2.0.0.0rc1
+Version: 2.0.0.0rc2
 Summary: The OVN BGP Agent allows to expose VMs/Containers/Networks through BGP on OVN
 Home-page: https://www.openstack.org/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: =============
         OVN BGP Agent
```

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/SOURCES.txt` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/ovn_bgp_agent.egg-info/entry_points.txt` & `ovn-bgp-agent-2.0.0.0rc2/ovn_bgp_agent.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/releasenotes/source/conf.py` & `ovn-bgp-agent-2.0.0.0rc2/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/requirements.txt` & `ovn-bgp-agent-2.0.0.0rc2/requirements.txt`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/setup.cfg` & `ovn-bgp-agent-2.0.0.0rc2/setup.cfg`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/setup.py` & `ovn-bgp-agent-2.0.0.0rc2/setup.py`

 * *Files identical despite different names*

### Comparing `ovn-bgp-agent-2.0.0.0rc1/tox.ini` & `ovn-bgp-agent-2.0.0.0rc2/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 usedevelop = True
 setenv =
    VIRTUAL_ENV={envdir}
    PYTHONWARNINGS=default::DeprecationWarning
    OS_STDOUT_CAPTURE=1
    OS_STDERR_CAPTURE=1
    OS_TEST_TIMEOUT=60
-deps = -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/master}
+deps = -c{env:TOX_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/2024.1}
        -r{toxinidir}/test-requirements.txt
 commands = stestr run --exclude-regex ".tests.functional" {posargs}
 
 [testenv:pep8]
 commands = flake8 {posargs}
 
 [testenv:venv]
```

### Comparing `ovn-bgp-agent-2.0.0.0rc1/zuul.d/project.yaml` & `ovn-bgp-agent-2.0.0.0rc2/zuul.d/project.yaml`

 * *Files identical despite different names*

