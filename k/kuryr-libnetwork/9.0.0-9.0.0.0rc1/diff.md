# Comparing `tmp/kuryr-libnetwork-9.0.0.tar.gz` & `tmp/kuryr-libnetwork-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuryr-libnetwork-9.0.0.tar", last modified: Wed Mar 30 11:48:16 2022, max compression
+gzip compressed data, was "kuryr-libnetwork-9.0.0.0rc1.tar", last modified: Thu Mar 10 08:43:26 2022, max compression
```

## Comparing `kuryr-libnetwork-9.0.0.tar` & `kuryr-libnetwork-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.103978 kuryr-libnetwork-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4066 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4141 2022-03-30 11:48:15.000000 kuryr-libnetwork-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26957 2022-03-30 11:48:15.000000 kuryr-libnetwork-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/Dockerfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20864 2022-03-30 11:48:16.103978 kuryr-libnetwork-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16019 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.075976 kuryr-libnetwork-9.0.0/contrib/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.083976 kuryr-libnetwork-9.0.0/contrib/busybox/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/busybox/Dockerfile
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      105 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/busybox/build_image.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   596520 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/busybox/busybox.tar.xz
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.083976 kuryr-libnetwork-9.0.0/contrib/docker/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      633 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/docker/run_kuryr.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.083976 kuryr-libnetwork-9.0.0/contrib/docker/v2plugin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3121 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/docker/v2plugin/config.json
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      614 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/docker/v2plugin/v2plugin_rootfs.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.083976 kuryr-libnetwork-9.0.0/contrib/tls/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/tls/kuryr.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.083976 kuryr-libnetwork-9.0.0/contrib/vagrant/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2609 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/vagrant/README.md
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1543 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/vagrant/Vagrantfile
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      727 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/vagrant/add_vagrant_user.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.083976 kuryr-libnetwork-9.0.0/contrib/vagrant/config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/vagrant/config/kuryr_rc
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1493 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/vagrant/devstack.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      219 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/contrib/vagrant/vagrant.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.083976 kuryr-libnetwork-9.0.0/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/devstack/local.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6261 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.083976 kuryr-libnetwork-9.0.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6811 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.087976 kuryr-libnetwork-9.0.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2660 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4347 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/config-sriov.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.087976 kuryr-libnetwork-9.0.0/doc/source/devref/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/devref/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16000 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/devref/libnetwork_remote_driver_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1512 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/fullstack-test.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.087976 kuryr-libnetwork-9.0.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3034 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/install/compute-install-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/install/compute-install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/install/controller-install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/install/get_started.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/install/next-steps.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/install/verify.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.087976 kuryr-libnetwork-9.0.0/etc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/etc/README-config.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/etc/kuryr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/etc/kuryr.spec
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.087976 kuryr-libnetwork-9.0.0/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/etc/oslo-config-generator/kuryr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.087976 kuryr-libnetwork-9.0.0/init/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/init/kuryr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.087976 kuryr-libnetwork-9.0.0/kuryr_libnetwork/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3446 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    76653 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/controllers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1836 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.091977 kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9670 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.091977 kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6531 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/drivers/nested.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5977 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/drivers/sriov.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3609 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/drivers/veth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/drivers/vlan.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.091977 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11369 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/commons.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/endpoint_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/endpoint_delete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/endpoint_info.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1671 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/join.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/leave.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1903 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/network_create.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1273 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/network_delete.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/release_address.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1267 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/release_pool.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1656 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/request_address.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2126 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/request_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/server.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.091977 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.091977 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/contrib/gate_hook.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1708 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/contrib/post_test_hook.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.095977 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/fullstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/fullstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3882 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/fullstack/kuryr_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4348 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/fullstack/test_container.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28746 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/fullstack/test_ipam.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8038 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/fullstack/test_network.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.095977 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14255 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.095977 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.095977 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9577 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/drivers/test_nested.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8072 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/drivers/test_sriov.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10318 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/drivers/test_veth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15388 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/drivers/test_vlan.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6268 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4744 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14140 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_external_connectivity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4260 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_ipam_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2169 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_join.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   108065 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_kuryr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14653 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_kuryr_endpoint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23999 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_kuryr_existing_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    76224 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_kuryr_ipam.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15018 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_kuryr_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1942 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_leave.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3498 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_schema.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1453 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5193 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.091977 kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20864 2022-03-30 11:48:15.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5689 2022-03-30 11:48:16.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-30 11:48:15.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-03-30 11:48:15.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-30 11:48:15.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-30 11:48:15.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2022-03-30 11:48:15.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2022-03-30 11:48:15.000000 kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2156 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/lower-constraints.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.095977 kuryr-libnetwork-9.0.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/playbooks/post_fullstack_job.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/playbooks/run_fullstack_job.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.095977 kuryr-libnetwork-9.0.0/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.095977 kuryr-libnetwork-9.0.0/rally-jobs/extra/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/extra/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/kuryr-libnetwork.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.099977 kuryr-libnetwork-9.0.0/rally-jobs/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/plugins/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.099977 kuryr-libnetwork-9.0.0/rally-jobs/plugins/context/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/plugins/context/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/plugins/context/docker_networks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.099977 kuryr-libnetwork-9.0.0/rally-jobs/plugins/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/plugins/scenarios/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3431 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/plugins/scenarios/kuryr.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3653 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/plugins/scenarios/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.079976 kuryr-libnetwork-9.0.0/rally-jobs/tasks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.099977 kuryr-libnetwork-9.0.0/rally-jobs/tasks/scenarios/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/tasks/scenarios/create_and_delete_networks_with_kuryr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/tasks/scenarios/create_and_delete_networks_without_kuryr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/rally-jobs/tasks/scenarios/list_networks.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.079976 kuryr-libnetwork-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.099977 kuryr-libnetwork-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/notes/add_support_ipv6_subnet-a024ffd6f7acc883.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      608 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/notes/bp-existing-subnetpool-aa454cf843cba47c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/notes/bug-1668803-c39f746e38878239.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/notes/bug-1671222-9ea0cf3ab39f0abc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/notes/drop-py-2-7-033606554411d7c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/notes/started-using-reno-8411d91eb3fe9e6c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/notes/use-uwsgi-to-run-server-4f43e615fd277c73.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.103978 kuryr-libnetwork-9.0.0/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.103978 kuryr-libnetwork-9.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.103978 kuryr-libnetwork-9.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4987 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.103978 kuryr-libnetwork-9.0.0/scripts/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4028 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/scripts/run_kuryr.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      622 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/scripts/run_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1103 2022-03-30 11:48:16.103978 kuryr-libnetwork-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-30 11:48:16.103978 kuryr-libnetwork-9.0.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1405 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/tools/generate_config_file_samples.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2294 2022-03-30 11:47:38.000000 kuryr-libnetwork-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.975084 kuryr-libnetwork-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4066 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4141 2022-03-10 08:43:26.000000 kuryr-libnetwork-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      793 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26967 2022-03-10 08:43:26.000000 kuryr-libnetwork-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      882 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/Dockerfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20869 2022-03-10 08:43:26.975084 kuryr-libnetwork-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16019 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      656 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.931086 kuryr-libnetwork-9.0.0.0rc1/contrib/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.943086 kuryr-libnetwork-9.0.0.0rc1/contrib/busybox/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       45 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/busybox/Dockerfile
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      105 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/busybox/build_image.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   596520 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/busybox/busybox.tar.xz
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.943086 kuryr-libnetwork-9.0.0.0rc1/contrib/docker/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      633 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/docker/run_kuryr.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.943086 kuryr-libnetwork-9.0.0.0rc1/contrib/docker/v2plugin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3121 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/docker/v2plugin/config.json
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      614 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/docker/v2plugin/v2plugin_rootfs.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.943086 kuryr-libnetwork-9.0.0.0rc1/contrib/tls/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      254 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/tls/kuryr.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.947085 kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2609 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/README.md
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1543 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/Vagrantfile
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      727 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/add_vagrant_user.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.947085 kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/config/kuryr_rc
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1493 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/devstack.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      219 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/vagrant.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.947085 kuryr-libnetwork-9.0.0.0rc1/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      826 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/devstack/local.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6261 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1548 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.947085 kuryr-libnetwork-9.0.0.0rc1/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6811 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.947085 kuryr-libnetwork-9.0.0.0rc1/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2660 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4347 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/config-sriov.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.947085 kuryr-libnetwork-9.0.0.0rc1/doc/source/devref/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1338 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/devref/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16000 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/devref/libnetwork_remote_driver_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1512 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/fullstack-test.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      652 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.951085 kuryr-libnetwork-9.0.0.0rc1/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3034 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/install/compute-install-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/install/compute-install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1308 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/install/controller-install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/install/get_started.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      368 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      350 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/install/next-steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1404 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/install/verify.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.951085 kuryr-libnetwork-9.0.0.0rc1/etc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/etc/README-config.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/etc/kuryr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       23 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/etc/kuryr.spec
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.951085 kuryr-libnetwork-9.0.0.0rc1/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/etc/oslo-config-generator/kuryr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.951085 kuryr-libnetwork-9.0.0.0rc1/init/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      347 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/init/kuryr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.955085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      720 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3446 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2403 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    76653 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/controllers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1836 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.955085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9670 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.955085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6531 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/drivers/nested.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5977 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/drivers/sriov.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3609 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/drivers/veth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/drivers/vlan.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.959085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1760 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11369 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/commons.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1733 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/endpoint_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1411 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/endpoint_delete.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1437 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/endpoint_info.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1671 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/join.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      901 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/leave.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1903 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/network_create.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1273 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/network_delete.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1454 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/release_address.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1267 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/release_pool.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1656 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/request_address.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2126 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/request_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/server.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.959085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.959085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      362 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/contrib/gate_hook.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1708 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/contrib/post_test_hook.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.963085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/fullstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/fullstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3882 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/fullstack/kuryr_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4348 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/fullstack/test_container.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28746 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/fullstack/test_ipam.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8038 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/fullstack/test_network.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.963085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14255 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.967085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.967085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9577 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/drivers/test_nested.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8072 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/drivers/test_sriov.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10318 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/drivers/test_veth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15388 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/drivers/test_vlan.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2757 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6268 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4744 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14140 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_external_connectivity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4260 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_ipam_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2169 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_join.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   108065 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_kuryr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14653 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_kuryr_endpoint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23999 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_kuryr_existing_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    76224 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_kuryr_ipam.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15018 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_kuryr_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1942 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_leave.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3498 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_schema.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1453 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5193 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      695 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.955085 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20869 2022-03-10 08:43:26.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5689 2022-03-10 08:43:26.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-10 08:43:26.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2022-03-10 08:43:26.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2022-03-10 08:43:26.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2022-03-10 08:43:26.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2022-03-10 08:43:26.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2022-03-10 08:43:26.000000 kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2156 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.967085 kuryr-libnetwork-9.0.0.0rc1/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/playbooks/post_fullstack_job.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/playbooks/run_fullstack_job.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.967085 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.967085 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/extra/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/extra/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1156 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/kuryr-libnetwork.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.967085 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.967085 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/context/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/context/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/context/docker_networks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.971084 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/scenarios/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3431 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/scenarios/kuryr.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3653 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/scenarios/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.935086 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/tasks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.971084 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/tasks/scenarios/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      555 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/tasks/scenarios/create_and_delete_networks_with_kuryr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/tasks/scenarios/create_and_delete_networks_without_kuryr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/rally-jobs/tasks/scenarios/list_networks.json
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.935086 kuryr-libnetwork-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.971084 kuryr-libnetwork-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      346 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/notes/add_support_ipv6_subnet-a024ffd6f7acc883.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      608 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/notes/bp-existing-subnetpool-aa454cf843cba47c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/notes/bug-1668803-c39f746e38878239.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/notes/bug-1671222-9ea0cf3ab39f0abc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/notes/drop-py-2-7-033606554411d7c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/notes/started-using-reno-8411d91eb3fe9e6c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      256 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/notes/use-uwsgi-to-run-server-4f43e615fd277c73.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.975084 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.975084 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.975084 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4987 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      593 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.975084 kuryr-libnetwork-9.0.0.0rc1/scripts/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4028 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/scripts/run_kuryr.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      622 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/scripts/run_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1103 2022-03-10 08:43:26.975084 kuryr-libnetwork-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      527 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2022-03-10 08:43:26.975084 kuryr-libnetwork-9.0.0.0rc1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1405 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/tools/generate_config_file_samples.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2294 2022-03-10 08:42:36.000000 kuryr-libnetwork-9.0.0.0rc1/tox.ini
```

### Comparing `kuryr-libnetwork-9.0.0/.zuul.yaml` & `kuryr-libnetwork-9.0.0.0rc1/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/AUTHORS` & `kuryr-libnetwork-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/CONTRIBUTING.rst` & `kuryr-libnetwork-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/ChangeLog` & `kuryr-libnetwork-9.0.0.0rc1/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Add Python3 yoga unit tests
 * Update master for stable/xena
 
 8.0.0
 -----
```

### Comparing `kuryr-libnetwork-9.0.0/Dockerfile` & `kuryr-libnetwork-9.0.0.0rc1/Dockerfile`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/LICENSE` & `kuryr-libnetwork-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/PKG-INFO` & `kuryr-libnetwork-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kuryr-libnetwork
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Docker libnetwork driver for OpenStack Neutron
 Home-page: https://docs.openstack.org/kuryr-libnetwork/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `kuryr-libnetwork-9.0.0/README.rst` & `kuryr-libnetwork-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/__init__.py` & `kuryr-libnetwork-9.0.0.0rc1/__init__.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/contrib/busybox/busybox.tar.xz` & `kuryr-libnetwork-9.0.0.0rc1/contrib/busybox/busybox.tar.xz`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/contrib/docker/run_kuryr.sh` & `kuryr-libnetwork-9.0.0.0rc1/contrib/docker/run_kuryr.sh`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/contrib/docker/v2plugin/config.json` & `kuryr-libnetwork-9.0.0.0rc1/contrib/docker/v2plugin/config.json`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/contrib/docker/v2plugin/v2plugin_rootfs.sh` & `kuryr-libnetwork-9.0.0.0rc1/contrib/docker/v2plugin/v2plugin_rootfs.sh`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/contrib/vagrant/README.md` & `kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/README.md`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/contrib/vagrant/Vagrantfile` & `kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/Vagrantfile`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/contrib/vagrant/add_vagrant_user.sh` & `kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/add_vagrant_user.sh`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/contrib/vagrant/devstack.sh` & `kuryr-libnetwork-9.0.0.0rc1/contrib/vagrant/devstack.sh`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/devstack/local.conf.sample` & `kuryr-libnetwork-9.0.0.0rc1/devstack/local.conf.sample`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/devstack/plugin.sh` & `kuryr-libnetwork-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/devstack/settings` & `kuryr-libnetwork-9.0.0.0rc1/devstack/settings`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/Makefile` & `kuryr-libnetwork-9.0.0.0rc1/doc/Makefile`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/conf.py` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/config-sriov.rst` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/config-sriov.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/devref/index.rst` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/devref/index.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/devref/libnetwork_remote_driver_design.rst` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/devref/libnetwork_remote_driver_design.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/fullstack-test.rst` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/fullstack-test.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/index.rst` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/install/compute-install-ubuntu.rst` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/install/compute-install-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/install/compute-install.rst` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/install/compute-install.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/install/controller-install.rst` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/install/controller-install.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/install/get_started.rst` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/install/get_started.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/doc/source/install/verify.rst` & `kuryr-libnetwork-9.0.0.0rc1/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/__init__.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/__init__.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/config.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/config.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/constants.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/constants.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/controllers.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/controllers.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/opts.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/opts.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/base.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/base.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/driver.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/driver.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/drivers/nested.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/drivers/nested.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/drivers/sriov.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/drivers/sriov.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/drivers/veth.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/drivers/veth.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/port_driver/drivers/vlan.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/port_driver/drivers/vlan.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/__init__.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/__init__.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/commons.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/commons.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/endpoint_create.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/endpoint_create.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/endpoint_delete.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/endpoint_delete.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/endpoint_info.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/endpoint_info.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/join.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/join.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/leave.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/leave.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/network_create.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/network_create.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/network_delete.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/network_delete.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/release_address.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/release_address.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/release_pool.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/release_pool.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/request_address.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/request_address.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/schemata/request_pool.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/schemata/request_pool.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/server.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/server.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/contrib/post_test_hook.sh` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/contrib/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/fullstack/kuryr_base.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/fullstack/kuryr_base.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/fullstack/test_container.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/fullstack/test_container.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/fullstack/test_ipam.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/fullstack/test_ipam.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/fullstack/test_network.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/fullstack/test_network.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/base.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/base.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/drivers/test_nested.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/drivers/test_nested.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/drivers/test_sriov.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/drivers/test_sriov.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/drivers/test_veth.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/drivers/test_veth.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/drivers/test_vlan.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/drivers/test_vlan.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/test_base.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/test_base.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/port_driver/test_driver.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/port_driver/test_driver.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_config.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_external_connectivity.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_external_connectivity.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_ipam_pool.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_ipam_pool.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_join.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_join.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_kuryr.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_kuryr.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_kuryr_endpoint.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_kuryr_endpoint.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_kuryr_existing_network.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_kuryr_existing_network.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_kuryr_ipam.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_kuryr_ipam.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_kuryr_network.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_kuryr_network.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_leave.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_leave.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_schema.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_schema.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/tests/unit/test_utils.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/utils.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork/version.py` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork/version.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/PKG-INFO` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: kuryr-libnetwork
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Docker libnetwork driver for OpenStack Neutron
 Home-page: https://docs.openstack.org/kuryr-libnetwork/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `kuryr-libnetwork-9.0.0/kuryr_libnetwork.egg-info/SOURCES.txt` & `kuryr-libnetwork-9.0.0.0rc1/kuryr_libnetwork.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/lower-constraints.txt` & `kuryr-libnetwork-9.0.0.0rc1/lower-constraints.txt`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/rally-jobs/README.rst` & `kuryr-libnetwork-9.0.0.0rc1/rally-jobs/README.rst`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/rally-jobs/kuryr-libnetwork.yaml` & `kuryr-libnetwork-9.0.0.0rc1/rally-jobs/kuryr-libnetwork.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/rally-jobs/plugins/context/docker_networks.py` & `kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/context/docker_networks.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/rally-jobs/plugins/scenarios/kuryr.py` & `kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/scenarios/kuryr.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/rally-jobs/plugins/scenarios/utils.py` & `kuryr-libnetwork-9.0.0.0rc1/rally-jobs/plugins/scenarios/utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/rally-jobs/tasks/scenarios/create_and_delete_networks_with_kuryr.json` & `kuryr-libnetwork-9.0.0.0rc1/rally-jobs/tasks/scenarios/create_and_delete_networks_with_kuryr.json`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/rally-jobs/tasks/scenarios/create_and_delete_networks_without_kuryr.json` & `kuryr-libnetwork-9.0.0.0rc1/rally-jobs/tasks/scenarios/create_and_delete_networks_without_kuryr.json`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/rally-jobs/tasks/scenarios/list_networks.json` & `kuryr-libnetwork-9.0.0.0rc1/rally-jobs/tasks/scenarios/list_networks.json`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/releasenotes/notes/bp-existing-subnetpool-aa454cf843cba47c.yaml` & `kuryr-libnetwork-9.0.0.0rc1/releasenotes/notes/bp-existing-subnetpool-aa454cf843cba47c.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/releasenotes/source/conf.py` & `kuryr-libnetwork-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/requirements.txt` & `kuryr-libnetwork-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/scripts/run_kuryr.sh` & `kuryr-libnetwork-9.0.0.0rc1/scripts/run_kuryr.sh`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/scripts/run_server.py` & `kuryr-libnetwork-9.0.0.0rc1/scripts/run_server.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/setup.cfg` & `kuryr-libnetwork-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/setup.py` & `kuryr-libnetwork-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/test-requirements.txt` & `kuryr-libnetwork-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/tools/generate_config_file_samples.sh` & `kuryr-libnetwork-9.0.0.0rc1/tools/generate_config_file_samples.sh`

 * *Files identical despite different names*

### Comparing `kuryr-libnetwork-9.0.0/tox.ini` & `kuryr-libnetwork-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

