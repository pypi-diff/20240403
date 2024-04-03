# Comparing `tmp/ceilometer-9.0.6.tar.gz` & `tmp/ceilometer-9.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ceilometer-9.0.6.tar", last modified: Thu Jun 14 14:55:51 2018, max compression
+gzip compressed data, was "dist/ceilometer-9.0.7.tar", last modified: Fri Apr 26 14:51:53 2019, max compression
```

## Comparing `ceilometer-9.0.6.tar` & `ceilometer-9.0.7.tar`

### file list

```diff
@@ -1,866 +1,864 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       17 2018-06-14 14:51:59.000000 ceilometer-9.0.6/babel.cfg
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      920 2018-06-14 14:52:09.000000 ceilometer-9.0.6/README.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3627 2018-06-14 14:52:09.000000 ceilometer-9.0.6/.zuul.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      425 2018-06-14 14:52:09.000000 ceilometer-9.0.6/MAINTAINERS
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       98 2018-06-14 14:51:59.000000 ceilometer-9.0.6/.coveragerc
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)      744 2018-06-14 14:52:09.000000 ceilometer-9.0.6/run-tests.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1990 2018-06-14 14:51:59.000000 ceilometer-9.0.6/.mailmap
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/playbooks/legacy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mysql/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2409 2018-06-14 14:52:09.000000 ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mysql/post.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1979 2018-06-14 14:52:09.000000 ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mysql/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2409 2018-06-14 14:52:09.000000 ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb/post.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1931 2018-06-14 14:52:09.000000 ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2409 2018-06-14 14:52:09.000000 ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only/post.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1982 2018-06-14 14:52:09.000000 ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/playbooks/legacy/grenade-dsvm-ceilometer/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2018-06-14 14:51:59.000000 ceilometer-9.0.6/playbooks/legacy/grenade-dsvm-ceilometer/post.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1645 2018-06-14 14:52:09.000000 ceilometer-9.0.6/playbooks/legacy/grenade-dsvm-ceilometer/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       33 2018-06-14 14:55:51.000000 ceilometer-9.0.6/RELEASENOTES.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32940 2018-06-14 14:55:44.000000 ceilometer-9.0.6/ceilometer.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16651 2018-06-14 14:55:41.000000 ceilometer-9.0.6/ceilometer.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2018-06-14 14:55:41.000000 ceilometer-9.0.6/ceilometer.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2018-06-14 14:55:41.000000 ceilometer-9.0.6/ceilometer.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1603 2018-06-14 14:55:41.000000 ceilometer-9.0.6/ceilometer.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2018-06-14 14:55:41.000000 ceilometer-9.0.6/ceilometer.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2018-06-14 14:55:41.000000 ceilometer-9.0.6/ceilometer.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2018-06-14 14:55:23.000000 ceilometer-9.0.6/ceilometer.egg-info/not-zip-safe
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/rally-jobs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/rally-jobs/plugins/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      390 2018-06-14 14:52:09.000000 ceilometer-9.0.6/rally-jobs/plugins/README.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      974 2018-06-14 14:52:09.000000 ceilometer-9.0.6/rally-jobs/plugins/plugin_sample.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      888 2018-06-14 14:52:09.000000 ceilometer-9.0.6/rally-jobs/README.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1438 2018-06-14 14:52:09.000000 ceilometer-9.0.6/rally-jobs/ceilometer.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/rally-jobs/extra/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      173 2018-06-14 14:52:09.000000 ceilometer-9.0.6/rally-jobs/extra/README.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/rally-jobs/extra/fake.img
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1023 2018-06-14 14:52:09.000000 ceilometer-9.0.6/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16106 2018-06-14 14:55:40.000000 ceilometer-9.0.6/AUTHORS
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      319 2018-06-14 14:52:09.000000 ceilometer-9.0.6/bindep.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   150817 2018-06-14 14:55:40.000000 ceilometer-9.0.6/ChangeLog
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      483 2018-06-14 14:51:59.000000 ceilometer-9.0.6/.testr.conf
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3229 2018-06-14 14:52:09.000000 ceilometer-9.0.6/tox.ini
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      565 2018-06-14 14:51:59.000000 ceilometer-9.0.6/CONTRIBUTING.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1028 2018-06-14 14:51:59.000000 ceilometer-9.0.6/setup.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/webapi/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1527 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/webapi/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25428 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/webapi/v2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/install/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1972 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/install-base-rdo.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4725 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/verify.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1589 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/install/get_started.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6121 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/install/install-base-prereq-common.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/install/neutron/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      710 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/install/neutron/install-neutron-ubuntu.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      778 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/install/neutron/install-neutron-rdo.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      776 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/install/neutron/install-neutron-obs.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/install/swift/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1294 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/swift/install-swift-config-common.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      709 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/swift/install-swift-obs.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/swift/install-swift-prereq-common.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      708 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/swift/install-swift-rdo.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      634 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/swift/install-swift-ubuntu.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      439 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/install-compute.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1062 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/install-compute-rdo.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1540 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/install-base-ubuntu.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2216 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/install/install-gnocchi.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1429 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/install/install-base-config-common.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1102 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/install-compute-obs.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/install/glance/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1099 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/glance/install-glance-obs.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1028 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/glance/install-glance-ubuntu.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1101 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/glance/install-glance-rdo.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/install/heat/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      859 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/heat/install-heat-obs.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      861 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/heat/install-heat-rdo.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      784 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/heat/install-heat-ubuntu.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10422 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/install/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      782 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/install-compute-ubuntu.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      692 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/install/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1963 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/install/install-compute-common.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1657 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/install-controller.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/install/cinder/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      994 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/cinder/install-cinder-ubuntu.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1086 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/cinder/install-cinder-rdo.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      620 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/cinder/install-cinder-config-common.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1084 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/cinder/install-cinder-obs.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2001 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/install-base-obs.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      234 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/install/next-steps.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/contributor/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    42751 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/5-multi-publish.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    42222 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/contributor/4-Transformer.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    46678 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/contributor/3-Pipeline.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    44022 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/2-accessmodel.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   115795 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/ceilo-gnocchi-arch.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3082 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/contributor/new_resource_types.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1528 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/overview.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    52865 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/6-storagemodel.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8061 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/contributor/plugins.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    50041 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/1-agents.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7326 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/contributor/architecture.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    87960 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/ceilo-arch.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11887 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/contributor/events.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    32911 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/2-2-collection-poll.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3113 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/gmr.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1212 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/contributor/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1739 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/testing.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1123 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/contributor/devstack.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4060 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/contributor/measurements.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    33278 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/contributor/2-1-collection-notification.png
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4799 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/glossary.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/configuration/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      873 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/configuration/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9850 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1595 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/admin/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   101269 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/admin/telemetry-measurements.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20628 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/admin/telemetry-data-pipelines.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3981 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/admin/telemetry-system-architecture.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4678 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/admin/telemetry-best-practices.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      519 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/admin/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30708 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/admin/telemetry-data-retrieval.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6520 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/admin/telemetry-events.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15493 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/admin/telemetry-data-collection.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      868 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/admin/telemetry-troubleshooting-guide.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/doc/source/releasenotes/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2594 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/source/releasenotes/folsom.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1505 2018-06-14 14:51:59.000000 ceilometer-9.0.6/doc/source/releasenotes/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6027 2018-06-14 14:52:09.000000 ceilometer-9.0.6/doc/Makefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/devstack/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      869 2018-06-14 14:51:59.000000 ceilometer-9.0.6/devstack/README.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3781 2018-06-14 14:52:09.000000 ceilometer-9.0.6/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/devstack/upgrade/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)      649 2018-06-14 14:52:09.000000 ceilometer-9.0.6/devstack/upgrade/shutdown.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      556 2018-06-14 14:52:09.000000 ceilometer-9.0.6/devstack/upgrade/settings
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     3180 2018-06-14 14:52:09.000000 ceilometer-9.0.6/devstack/upgrade/upgrade.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21517 2018-06-14 14:52:09.000000 ceilometer-9.0.6/devstack/plugin.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/devstack/files/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/devstack/files/rpms/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       24 2018-06-14 14:51:59.000000 ceilometer-9.0.6/devstack/files/rpms/ceilometer
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      498 2018-06-14 14:52:09.000000 ceilometer-9.0.6/devstack/apache-ceilometer.template
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18425 2018-06-14 14:55:51.000000 ceilometer-9.0.6/setup.cfg
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1886 2018-06-14 14:52:09.000000 ceilometer-9.0.6/requirements.txt
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10143 2018-06-14 14:51:59.000000 ceilometer-9.0.6/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2018-06-14 14:55:51.000000 ceilometer-9.0.6/PKG-INFO
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1071 2018-06-14 14:51:59.000000 ceilometer-9.0.6/HACKING.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/etc/apache2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1442 2018-06-14 14:52:09.000000 ceilometer-9.0.6/etc/apache2/ceilometer
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/etc/ceilometer/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/etc/ceilometer/rootwrap.d/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      240 2018-06-14 14:51:59.000000 ceilometer-9.0.6/etc/ceilometer/rootwrap.d/ipmi.filters
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      937 2018-06-14 14:52:09.000000 ceilometer-9.0.6/etc/ceilometer/api_paste.ini
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      983 2018-06-14 14:51:59.000000 ceilometer-9.0.6/etc/ceilometer/rootwrap.conf
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       87 2018-06-14 14:51:59.000000 ceilometer-9.0.6/etc/ceilometer/polling_all.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      398 2018-06-14 14:52:09.000000 ceilometer-9.0.6/etc/ceilometer/ceilometer-config-generator.conf
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      365 2018-06-14 14:52:09.000000 ceilometer-9.0.6/etc/ceilometer/policy.json
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/etc/ceilometer/examples/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8957 2018-06-14 14:51:59.000000 ceilometer-9.0.6/etc/ceilometer/examples/loadbalancer_v2_meter_definitions.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      706 2018-06-14 14:51:59.000000 ceilometer-9.0.6/etc/ceilometer/examples/osprofiler_event_definitions.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      813 2018-06-14 14:52:09.000000 ceilometer-9.0.6/etc/ceilometer/polling.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/releasenotes/source/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      110 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/source/unreleased.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/releasenotes/source/_static/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/source/_static/.placeholder
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      136 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/source/ocata.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9461 2018-06-14 14:52:09.000000 ceilometer-9.0.6/releasenotes/source/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      163 2018-06-14 14:52:09.000000 ceilometer-9.0.6/releasenotes/source/index.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      140 2018-06-14 14:52:09.000000 ceilometer-9.0.6/releasenotes/source/newton.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      144 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/source/liberty.rst
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      140 2018-06-14 14:52:09.000000 ceilometer-9.0.6/releasenotes/source/mitaka.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/releasenotes/notes/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      384 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/improve-events-rbac-support-f216bd7f34b02032.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      151 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/polling-deprecation-4d5b83180893c053.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      428 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/refresh-legacy-cache-e4dbbd3e2eeca70b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      218 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/index-events-mongodb-63cb04200b03a093.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      135 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/remove-alarms-4df3cdb4f1fb5faa.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      245 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/ship-yaml-files-33aa5852bedba7f0.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      165 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/use-notification-transport-url-489f3d31dc66c4d2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      170 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/memory-bandwidth-meter-f86cf01178573671.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      246 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/parallel_requests_option-a3f901b6001e26e4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      584 2018-06-14 14:52:09.000000 ceilometer-9.0.6/releasenotes/notes/always-requeue-7a2df9243987ab67.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       80 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/drop-kwapi-b687bc476186d01b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      279 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/support-meter-batch-recording-mongo-6c2bdf4fbb9764eb.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      202 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/gnocchi-cache-b9ad4d85a1da8d3f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      340 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/cors-support-70c33ba1f6825a7b.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      518 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/batch-messaging-d126cc525879d58e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      450 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/deprecate-ceilometer-collector-b793b91cd28b9e7f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      357 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/handle-malformed-resource-definitions-ad4f69f898ced34d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      425 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/remove-refresh-pipeline-618af089c5435db7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      436 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/fix-agent-coordination-a7103a78fecaec24.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      274 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/network-statistics-from-opendaylight-787df77484d8d751.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      328 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/remove-rpc-collector-d0d0a354140fd107.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      394 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/fix-floatingip-pollster-f5172060c626b19e.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      357 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/configurable-data-collector-e247aadbffb85243.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      254 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/unify-timestamp-of-polled-data-fbfcff43cd2d04bc.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      122 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/kwapi_deprecated-c92b9e72c78365f0.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      225 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/thread-safe-matching-4a635fc4965c5d4c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      592 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/polling-definition-efffb92e3810e571.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      568 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/single-thread-pipelines-f9e6ac4b062747fe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2018-06-14 14:55:51.000000 ceilometer-9.0.6/releasenotes/notes/reno.cache
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      210 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/gnocchi-host-metrics-829bcb965d8f2533.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      251 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/remove-cadf-http-f8449ced3d2a29d4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      183 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/gnocchi-client-42cd992075ee53ab.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       62 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/pecan-debug-removed-dc737efbf911bde7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      373 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/deprecate-http-control-exchanges-026a8de6819841f8.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1200 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/less-nova-polling-ac56687da3f8b1a3.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      233 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/cache-json-parsers-888307f3b6b498a2.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      170 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/deprecated_database_event_dispatcher_panko-607d558c86a90f17.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      240 2018-06-14 14:52:09.000000 ceilometer-9.0.6/releasenotes/notes/use-glance-v2-in-image-pollsters-137a315577d5dc4c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      104 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/add-memory-swap-metric-f1633962ab2cf0f6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      277 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/perf-events-meter-b06c2a915c33bfaf.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      158 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/gnocchi-orchestration-3497c689268df0d1.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      102 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/remove-ceilometer-dbsync-53aa1b529f194f15.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       87 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/remove-eventlet-6738321434b60c78.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      201 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/ceilometer-event-api-removed-49c57835e307b997.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      231 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/tooz-coordination-system-d1054b9d1a5ddf32.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      266 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/support-unique-meter-query-221c6e0c1dc1b726.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      727 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/http_proxy_to_wsgi_enabled-616fa123809e1600.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      204 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/fix-network-lb-bytes-sample-5dec2c6f3a8ae174.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      170 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/aggregator-transformer-timeout-e0f42b6c96aa7ada.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/support-snmp-cpu-util-5c1c7afb713c1acd.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      244 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/http-dispatcher-batching-4e17fce46a196b07.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/support-cinder-volume-snapshot-backup-metering-d0a93b86bd53e803.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      364 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/skip-duplicate-meter-def-0420164f6a95c50c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      167 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/deprecate-pollster-list-ccf22b0dea44f043.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      439 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/drop-instance-meter-1b657717b21a0f55.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      251 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/deprecate-file-dispatcher-2aff376db7609136.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      332 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/instance-discovery-new-default-7f9b451a515dddf4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      100 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/add-magnum-event-4c75ed0bb268d19c.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      143 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/gnocchi-udp-collector-00415e6674b5cc0f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      225 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/add-tool-for-migrating-data-to-gnocchi-cea8d4db68ce03d0.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       67 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/keystone-v3-fab1e257c5672965.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      221 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/sql-query-optimisation-ebb2233f7a9b5d06.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      593 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/http-dispatcher-verify-ssl-551d639f37849c6f.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      484 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/drop-image-meter-9c9b6cebd546dae7.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      252 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/fix-aggregation-transformer-9472aea189fa8f65.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/.placeholder
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      326 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/mongodb-handle-large-numbers-7c235598ca700f2d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      127 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/scan-domains-for-tenants-8f8c9edcb74cc173.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      606 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/deprecate-http-dispatcher-dbbaacee8182b550.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      178 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/add-db-legacy-clean-tool-7b3e3714f414c448.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      148 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/add-full-snmpv3-usm-support-ab540c902fa89b9d.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      636 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/support-lbaasv2-polling-c830dd49bcf25f64.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      566 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/rename-ceilometer-dbsync-eb7a1fa503085528.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      132 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/ceilometer-api-deprecate-862bfaa54e80fa01.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      159 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/support-None-query-45abaae45f08eda4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      353 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/lookup-meter-def-vol-correctly-0122ae429275f2a6.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      165 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/event-type-race-c295baf7f1661eab.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      354 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/gnocchi-cache-1d8025dfc954f281.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)       86 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/zaqar-publisher-f7efa030b71731f4.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      469 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/deprecate-kafka-publisher-17b4f221758e15da.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      413 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/compute-discovery-interval-d19f7c9036a8c186.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      242 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/support-multiple-meter-definition-files-e3ce1fa73ef2e1de.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      775 2018-06-14 14:51:59.000000 ceilometer-9.0.6/releasenotes/notes/http-publisher-authentication-6371c5a9aa8d4c03.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/api-ref/source/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1379 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/resources.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7741 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/meters.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5383 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/alarms.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/api-ref/source/samples/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      703 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/resources-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      513 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/sample-show-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      924 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/resources-list-response.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      972 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/alarms-list-response.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      741 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/alarms-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3306 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/capabilities-list-response.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      395 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/meters-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      585 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/samples-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      659 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/sample-create-request.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      503 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/events-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      483 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/meters-list-response.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      641 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/alarm-show-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      731 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/sample-show-response.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      515 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/sample-create-request.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      827 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/resource-show-response.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      819 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/samples-list-response.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      857 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/alarm-show-response.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      468 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/statistics-list-response.xml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      371 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/statistics-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      427 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/event-show-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1459 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/capabilities-list-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      619 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples/resource-show-response.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1744 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/samples.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17275 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/parameters.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1215 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/events.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3170 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/capabilities.inc
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9002 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/conf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      111 2018-06-14 14:52:09.000000 ceilometer-9.0.6/api-ref/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/tools/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     7148 2018-06-14 14:52:09.000000 ceilometer-9.0.6/tools/make_test_data.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     7336 2018-06-14 14:52:09.000000 ceilometer-9.0.6/tools/migrate_data_to_gnocchi.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)      426 2018-06-14 14:51:59.000000 ceilometer-9.0.6/tools/pretty_tox.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/tools/__init__.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1485 2018-06-14 14:52:09.000000 ceilometer-9.0.6/tools/make_test_data.sh
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     4677 2018-06-14 14:51:59.000000 ceilometer-9.0.6/tools/send_test_data.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/meter/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/meter/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9539 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/meter/notifications.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14149 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/notification.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3748 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/keystone_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/dispatcher/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1467 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/dispatcher/gnocchi_opts.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6720 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/dispatcher/http.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/dispatcher/data/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8977 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/dispatcher/data/gnocchi_resources.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2939 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/dispatcher/file.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2527 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/dispatcher/database.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3323 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/dispatcher/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21513 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/dispatcher/gnocchi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/objectstore/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7334 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/objectstore/swift.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7635 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/objectstore/rgw.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/objectstore/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2593 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/objectstore/rgw_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/compute/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11955 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/compute/discovery.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/compute/pollsters/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7123 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/compute/pollsters/disk.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3491 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/pollsters/net.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2952 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/pollsters/instance_stats.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6836 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/compute/pollsters/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3524 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/pollsters/util.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/compute/virt/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/compute/virt/hyperv/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/virt/hyperv/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5867 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/compute/virt/hyperv/inspector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/compute/virt/vmware/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/virt/vmware/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10338 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/virt/vmware/vsphere_operations.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     8473 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/compute/virt/vmware/inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/virt/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/compute/virt/xenapi/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/virt/xenapi/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7592 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/compute/virt/xenapi/inspector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/compute/virt/libvirt/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/virt/libvirt/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4180 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/virt/libvirt/utils.py
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     9073 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/compute/virt/libvirt/inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9933 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/compute/virt/inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/compute/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6632 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/ipmi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/ipmi/platform/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4490 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/ipmi/platform/ipmitool.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13194 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/ipmi/platform/intel_node_manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/ipmi/platform/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4014 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/ipmi/platform/ipmi_sensor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      726 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/ipmi/platform/exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/ipmi/notifications/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5898 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/ipmi/notifications/ironic.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/ipmi/notifications/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/ipmi/pollsters/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5045 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/ipmi/pollsters/node.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      956 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/ipmi/pollsters/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3851 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/ipmi/pollsters/sensor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/ipmi/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7811 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/collector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/conf/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/conf/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1404 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/conf/defaults.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1063 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/pipeline/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/pipeline/data/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      195 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/pipeline/data/event_pipeline.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16763 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/pipeline/data/event_definitions.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2507 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/pipeline/data/pipeline.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/telemetry/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/telemetry/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2076 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/telemetry/notifications.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/data/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/data/meters.d/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11102 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/data/meters.d/meters.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/publisher/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7438 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/publisher/http.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4146 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/publisher/kafka_broker.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3680 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/publisher/file.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2803 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/publisher/zaqar.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1394 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/publisher/test.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2972 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/publisher/udp.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2359 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/publisher/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3911 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/publisher/direct.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3877 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/publisher/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9446 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/publisher/messaging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/volume/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1981 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/volume/discovery.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/volume/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3389 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/volume/cinder.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9401 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/gnocchi_client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6707 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/declarative.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/hardware/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5151 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/hardware/discovery.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/hardware/pollsters/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8538 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/hardware/pollsters/generic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/hardware/pollsters/data/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5109 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/hardware/pollsters/data/snmp.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/hardware/pollsters/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1948 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/hardware/pollsters/util.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/hardware/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/hardware/inspector/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1590 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/hardware/inspector/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13475 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/hardware/inspector/snmp.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      969 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/hardware/inspector/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1332 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/middleware.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/cmd/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      968 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/cmd/collector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      981 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/cmd/agent_notification.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1087 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/cmd/api.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3382 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/cmd/polling.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5959 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/cmd/storage.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/cmd/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3183 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/cmd/sample.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5424 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/nova_client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2395 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/storage/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30861 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/impl_mongodb.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4856 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/impl_log.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/storage/mongo/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/mongo/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21688 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/mongo/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8985 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6732 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/pymongo_base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18962 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/impl_hbase.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      979 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1230 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/migrate.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      913 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/009_event_strings.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      864 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/004_add_counter_unit.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3122 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/023_add_trait_types.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3309 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/001_add_meter_table.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      888 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/006_counter_volume_is_float.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      786 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/023_sqlite_upgrade.sql
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2479 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/015_add_alarm_history_table.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1206 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/034_drop_dump_tables.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      846 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/010_add_index_to_meter.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2098 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/025_alarm_use_floatingprecision.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      949 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/005_remove_resource_timestamp.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1721 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/014_add_event_message_id.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1141 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/003_set_utf8_charset.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2967 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/021_add_event_types.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      896 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/019_alarm_history_detail_is_text.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5041 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/028_alembic_migrations.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4206 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/030_rename_meter_table.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2206 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/024_event_use_floatingprecision.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      864 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/045_add_resource_metadatahash_index.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1569 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/027_remove_alarm_fk_constraints.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2549 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/020_add_metadata_tables.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2111 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/016_simpler_alarm.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2202 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/041_expand_event_traits.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1319 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/011_indexes_cleanup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      906 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/022_metadata_int_is_bigint.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2229 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/039_event_floatingprecision_pgsql.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1630 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/044_restore_long_uuid_data_types.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1980 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/017_convert_timestamp_as_datetime_to_decimal.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1695 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/037_sample_index_cleanup.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      763 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/042_add_raw_column.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5498 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/038_normalise_tables.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      885 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/032_add_alarm_time_constraints.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1821 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/007_add_alarm_table.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      871 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/002_remove_duration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      937 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/029_sample_recorded_at.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2781 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/036_drop_sourceassoc_resource_tables.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      869 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/040_add_alarm_severity.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2342 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/012_add_missing_foreign_keys.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      837 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/043_reduce_uuid_data_types.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      627 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/021_sqlite_upgrade.sql
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2100 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/008_add_events.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      902 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/018_resource_resource_metadata_is_text.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      915 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/026_float_size.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      767 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/033_alarm_id_rename.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3209 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/031_add_new_meter_table.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      822 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/013_rename_counter_to_meter_alarm.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3384 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/035_drop_user_project_tables.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      143 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/README
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      116 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/manage.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4833 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8052 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/sqlalchemy/models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    37120 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/impl_sqlalchemy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5432 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/storage/hbase/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9553 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/hbase/inmemory.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3323 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/hbase/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2735 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/hbase/migration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/hbase/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16240 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/hbase/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6509 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/storage/models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      817 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/image/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1981 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/image/glance.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1377 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/image/discovery.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/image/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/network/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/network/services/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3206 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/services/vpnaas.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3825 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/network/services/discovery.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1142 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/network/services/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15021 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/services/lbaas.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/services/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2919 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/services/fwaas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/network/statistics/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      981 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/driver.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1897 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/port_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/network/statistics/opencontrail/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6956 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/opencontrail/driver.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3581 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/opencontrail/client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/opencontrail/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1436 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/flow.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      945 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/switch.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/network/statistics/opendaylight/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17521 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/network/statistics/opendaylight/driver.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6284 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/opendaylight/client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/opendaylight/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3424 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/network/statistics/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2969 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/port.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1303 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/statistics/table.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1893 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/network/floatingip.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/api/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2871 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/hooks.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3339 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/app.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      943 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/app.wsgi
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5293 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/middleware.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2947 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/rbac.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/api/controllers/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/api/controllers/v2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7668 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/v2/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8952 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/v2/root.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18887 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/v2/meters.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3648 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/v2/capabilities.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6214 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/v2/resources.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/v2/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12716 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/v2/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13783 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/v2/query.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4648 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/v2/samples.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1897 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/root.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/api/controllers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/event/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2238 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/event/endpoint.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/event/storage/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/event/storage/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4206 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/event/storage/models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11815 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/event/converter.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/event/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8534 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/event/trait_plugins.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16188 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/neutron_client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7925 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      649 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/version.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4026 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/exchange_control.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/transformer/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1322 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/transformer/accumulator.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2359 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/transformer/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13387 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/transformer/conversions.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6190 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/transformer/arithmetic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/ko_KR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/ko_KR/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4908 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-error.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5596 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-warning.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16497 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4283 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-info.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/ru/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/ru/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19452 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/ru/LC_MESSAGES/ceilometer.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/zh_CN/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/zh_CN/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14977 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/zh_CN/LC_MESSAGES/ceilometer.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/fr/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17087 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/fr/LC_MESSAGES/ceilometer.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/es/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4515 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/es/LC_MESSAGES/ceilometer-log-error.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16105 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/es/LC_MESSAGES/ceilometer.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4444 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/es/LC_MESSAGES/ceilometer-log-info.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/pt_BR/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/pt_BR/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15631 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/pt_BR/LC_MESSAGES/ceilometer.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/zh_TW/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/zh_TW/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14792 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/zh_TW/LC_MESSAGES/ceilometer.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/it/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/it/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15920 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/it/LC_MESSAGES/ceilometer.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/ja/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/ja/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19081 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/ja/LC_MESSAGES/ceilometer.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/de/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/locale/de/LC_MESSAGES/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4577 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-error.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4235 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-warning.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16528 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/de/LC_MESSAGES/ceilometer.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4488 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-info.po
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3373 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/messaging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/hacking/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1732 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/hacking/checks.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/hacking/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    32697 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/pipeline.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/agent/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/agent/discovery/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1526 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/agent/discovery/endpoint.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/agent/discovery/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      787 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/agent/discovery/localnode.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1691 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/agent/discovery/tenant.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9549 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/agent/plugin_base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/agent/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21371 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/agent/manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5694 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/sample.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/integration/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/integration/gabbi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/integration/gabbi/gabbits-live/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3155 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/integration/gabbi/gabbits-live/create_stack.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5053 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/integration/gabbi/gabbits-live/autoscaling.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11274 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/integration/gabbi/gabbits-live/aodh-gnocchi-threshold-alarm.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3124 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/integration/gabbi/gabbits-live/update_stack.json
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/integration/gabbi/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1400 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/integration/gabbi/test_gabbi_live.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/integration/hooks/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     3104 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/integration/hooks/post_test_hook.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/integration/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3904 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/meter/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    41007 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/meter/test_notifications.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3195 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/meter/test_meter_plugins.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/meter/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14621 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_neutronclient_lbaas_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3625 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/test_file.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27462 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/test_gnocchi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1673 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/test_dispatcher.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3130 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/test_db.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8705 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/test_http.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/objectstore/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10179 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/objectstore/test_swift.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7779 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/objectstore/test_rgw.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/objectstore/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6205 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/objectstore/test_rgw_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2687 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3856 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_perf.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6715 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_cpu.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8362 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_memory.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12986 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_net.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14261 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_diskio.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5213 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_location_metadata.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/hyperv/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7632 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/hyperv/test_inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/hyperv/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/vmware/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7921 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/vmware/test_inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7369 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/vmware/test_vsphere_operations.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/vmware/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/xenapi/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6809 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/xenapi/test_inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/xenapi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/libvirt/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)    22696 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/libvirt/test_inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/libvirt/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11611 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/compute/test_discovery.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1631 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_declarative.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2694 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_messaging.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/platform/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3898 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/platform/fake_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13467 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/platform/ipmitool_test_data.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4585 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/platform/test_ipmi_sensor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/platform/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7016 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/platform/test_intel_node_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/notifications/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30749 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/notifications/ipmi_test_data.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/notifications/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8503 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/notifications/test_ironic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/pollsters/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2722 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/pollsters/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4921 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/pollsters/test_node.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/pollsters/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4149 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/pollsters/test_sensor.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/ipmi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/telemetry/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3969 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/telemetry/test_notifications.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/telemetry/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/publisher/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14855 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_messaging_publisher.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8730 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_kafka_broker_publisher.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4460 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_file.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4776 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_utils.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4521 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_zaqar.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/publisher/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6540 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_udp.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10485 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_http.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2489 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_collector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7651 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/volume/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6943 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/volume/test_cinder.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/volume/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7870 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_neutronclient.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/hardware/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/hardware/pollsters/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2428 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/hardware/pollsters/test_util.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7354 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/hardware/pollsters/test_generic.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/hardware/pollsters/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/hardware/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/hardware/inspector/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1102 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/hardware/inspector/test_inspector.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10605 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/hardware/inspector/test_snmp.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/hardware/inspector/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17018 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_event_pipeline.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    88909 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/pipeline_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/storage/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3064 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/storage/test_get_connection.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/storage/sqlalchemy/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3788 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/storage/sqlalchemy/test_models.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/storage/sqlalchemy/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/storage/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2199 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/storage/test_base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/image/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4177 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/image/test_glance.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/image/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/services/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7561 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/services/test_vpnaas.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21669 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/services/test_lbaas.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/services/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13430 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/services/test_lbaas_v2.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7224 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/services/test_fwaas.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4431 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/test_floating_ip.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1812 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_flow.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3879 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_port.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1641 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_table.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1160 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_switch.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opencontrail/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opencontrail/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11977 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opencontrail/test_driver.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2746 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opencontrail/test_client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6738 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_statistics.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2472 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_port_v2.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opendaylight/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opendaylight/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    66706 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opendaylight/test_driver.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6227 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opendaylight/test_client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1157 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/network/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/api/v2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16485 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/api/v2/test_query.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4240 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/api/v2/test_statistics.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14623 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/api/v2/test_complex_query.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/api/v2/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1196 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/api/test_hooks.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/api/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1239 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/api/test_app.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/event/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    33054 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/event/test_converter.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7492 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/event/test_endpoint.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/event/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4328 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/event/test_trait_plugins.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4017 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_sample.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4340 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_middleware.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/transformer/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4529 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/transformer/test_conversions.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/unit/transformer/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11466 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_decoupled_pipeline.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9623 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_novaclient.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/unit/agent/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19317 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/agent/test_manager.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27306 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/agent/agentbase.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/agent/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8522 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/agent/test_discovery.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3993 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/unit/test_polling.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7065 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/db.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/functional/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/functional/publisher/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/publisher/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2595 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/publisher/test_direct.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9940 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/test_collector.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits_prefix/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      515 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits_prefix/basic.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      612 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits_prefix/resources-fixtured.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1464 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits_prefix/clean-samples.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1214 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/test_gabbi_prefix.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      440 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbi_pipeline.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4428 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/samples.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1426 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/resources-empty.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1093 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/middleware.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      452 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/fixture-samples.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      688 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/basic.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      247 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/capabilities.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11538 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/meters.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2556 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/resources-fixtured.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3149 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/clean-samples.yaml
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1186 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/test_gabbi.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6190 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/fixtures.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      793 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbi_paste.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/functional/hooks/
--rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1827 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/hooks/post_test_hook.sh
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7122 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/test_bin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/functional/storage/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)   127917 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/storage/test_storage_scenarios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4697 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/storage/test_impl_mongodb.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3575 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/storage/test_impl_hbase.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/storage/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5963 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/storage/test_impl_sqlalchemy.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5609 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/storage/test_pymongo_base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1068 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/storage/test_impl_log.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1601 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_versions.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    81197 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_statistics_scenarios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12964 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_complex_query_scenarios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7782 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_compute_duration_by_resource_scenarios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20613 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_list_resources_scenarios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7970 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_api_upgrade.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1142 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_capabilities.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16363 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_post_samples_scenarios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)      714 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7587 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_acl_scenarios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4479 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_app.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5614 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_list_samples_scenarios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    34350 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_list_meters_scenarios.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7320 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/api/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23177 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/functional/test_notification.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:51:59.000000 ceilometer-9.0.6/ceilometer/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/tempest/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/tempest/scenario/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5752 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/scenario/test_telemetry_integration.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/scenario/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5744 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/scenario/test_object_storage_telemetry_middleware.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2238 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/config.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1543 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/tempest/service/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3969 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/service/client.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/service/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:55:51.000000 ceilometer-9.0.6/ceilometer/tests/tempest/api/
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4995 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/api/base.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3075 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/api/test_telemetry_notification_api.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/api/__init__.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5320 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/tempest/exceptions.py
--rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3516 2018-06-14 14:52:09.000000 ceilometer-9.0.6/ceilometer/tests/mocks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      565 2019-04-26 14:49:21.000000 ceilometer-9.0.7/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   150966 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ChangeLog
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       17 2019-04-26 14:49:21.000000 ceilometer-9.0.7/babel.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/etc/apache2/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1442 2019-04-26 14:49:27.000000 ceilometer-9.0.7/etc/apache2/ceilometer
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/etc/ceilometer/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/etc/ceilometer/rootwrap.d/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      240 2019-04-26 14:49:27.000000 ceilometer-9.0.7/etc/ceilometer/rootwrap.d/ipmi.filters
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      398 2019-04-26 14:49:27.000000 ceilometer-9.0.7/etc/ceilometer/ceilometer-config-generator.conf
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       87 2019-04-26 14:49:21.000000 ceilometer-9.0.7/etc/ceilometer/polling_all.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      937 2019-04-26 14:49:27.000000 ceilometer-9.0.7/etc/ceilometer/api_paste.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/etc/ceilometer/examples/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      706 2019-04-26 14:49:21.000000 ceilometer-9.0.7/etc/ceilometer/examples/osprofiler_event_definitions.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8957 2019-04-26 14:49:21.000000 ceilometer-9.0.7/etc/ceilometer/examples/loadbalancer_v2_meter_definitions.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      813 2019-04-26 14:49:27.000000 ceilometer-9.0.7/etc/ceilometer/polling.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      983 2019-04-26 14:49:21.000000 ceilometer-9.0.7/etc/ceilometer/rootwrap.conf
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      365 2019-04-26 14:49:27.000000 ceilometer-9.0.7/etc/ceilometer/policy.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       98 2019-04-26 14:49:21.000000 ceilometer-9.0.7/.coveragerc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      425 2019-04-26 14:49:27.000000 ceilometer-9.0.7/MAINTAINERS
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1071 2019-04-26 14:49:21.000000 ceilometer-9.0.7/HACKING.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      920 2019-04-26 14:49:27.000000 ceilometer-9.0.7/README.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1990 2019-04-26 14:49:21.000000 ceilometer-9.0.7/.mailmap
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/contributor/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8061 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/contributor/plugins.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1212 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/contributor/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    44022 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/2-accessmodel.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7326 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/contributor/architecture.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)   115795 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/ceilo-gnocchi-arch.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1123 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/contributor/devstack.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3113 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/gmr.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    50041 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/1-agents.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11887 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/contributor/events.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    42222 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/contributor/4-Transformer.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    32911 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/2-2-collection-poll.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    87960 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/ceilo-arch.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    52865 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/6-storagemodel.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    33278 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/2-1-collection-notification.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1528 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/overview.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    46678 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/contributor/3-Pipeline.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3082 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/contributor/new_resource_types.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    42751 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/5-multi-publish.png
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4060 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/contributor/measurements.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1739 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/contributor/testing.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1595 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4799 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/glossary.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/webapi/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1527 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/webapi/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    25428 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/webapi/v2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/admin/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15493 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/admin/telemetry-data-collection.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      868 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/admin/telemetry-troubleshooting-guide.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)   101269 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/admin/telemetry-measurements.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      519 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/admin/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4678 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/admin/telemetry-best-practices.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3981 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/admin/telemetry-system-architecture.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20628 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/admin/telemetry-data-pipelines.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6520 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/admin/telemetry-events.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30708 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/admin/telemetry-data-retrieval.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/releasenotes/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1505 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/releasenotes/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2594 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/releasenotes/folsom.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9850 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/configuration/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      873 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/install/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1972 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/install-base-rdo.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1540 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/install-base-ubuntu.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4725 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/verify.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      692 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/install/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2001 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/install-base-obs.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6121 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/install/install-base-prereq-common.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1657 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/install-controller.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1589 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/install/get_started.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/install/swift/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      709 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/swift/install-swift-obs.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1294 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/swift/install-swift-config-common.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      708 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/swift/install-swift-rdo.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1030 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/swift/install-swift-prereq-common.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      634 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/swift/install-swift-ubuntu.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1429 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/install/install-base-config-common.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      234 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/next-steps.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/install/cinder/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      620 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/cinder/install-cinder-config-common.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      994 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/cinder/install-cinder-ubuntu.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1086 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/cinder/install-cinder-rdo.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1084 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/cinder/install-cinder-obs.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1102 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/install-compute-obs.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      439 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/install-compute.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/install/heat/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      859 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/heat/install-heat-obs.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      861 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/heat/install-heat-rdo.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      784 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/heat/install-heat-ubuntu.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/install/glance/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1099 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/glance/install-glance-obs.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1028 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/glance/install-glance-ubuntu.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1101 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/glance/install-glance-rdo.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10422 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/install/conf.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2216 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/install/install-gnocchi.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1062 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/install-compute-rdo.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1963 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/install/install-compute-common.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/doc/source/install/neutron/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      776 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/install/neutron/install-neutron-obs.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      778 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/install/neutron/install-neutron-rdo.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      710 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/source/install/neutron/install-neutron-ubuntu.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      782 2019-04-26 14:49:21.000000 ceilometer-9.0.7/doc/source/install/install-compute-ubuntu.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6027 2019-04-26 14:49:27.000000 ceilometer-9.0.7/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2019-04-26 14:51:53.000000 ceilometer-9.0.7/PKG-INFO
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1066 2019-04-26 14:49:27.000000 ceilometer-9.0.7/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/rally-jobs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/rally-jobs/plugins/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      390 2019-04-26 14:49:27.000000 ceilometer-9.0.7/rally-jobs/plugins/README.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      974 2019-04-26 14:49:27.000000 ceilometer-9.0.7/rally-jobs/plugins/plugin_sample.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      888 2019-04-26 14:49:27.000000 ceilometer-9.0.7/rally-jobs/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/rally-jobs/extra/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      173 2019-04-26 14:49:27.000000 ceilometer-9.0.7/rally-jobs/extra/README.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/rally-jobs/extra/fake.img
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1438 2019-04-26 14:49:27.000000 ceilometer-9.0.7/rally-jobs/ceilometer.yaml
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)      744 2019-04-26 14:49:27.000000 ceilometer-9.0.7/run-tests.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/tools/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/tools/__init__.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     7148 2019-04-26 14:49:27.000000 ceilometer-9.0.7/tools/make_test_data.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     4677 2019-04-26 14:49:21.000000 ceilometer-9.0.7/tools/send_test_data.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)      426 2019-04-26 14:49:27.000000 ceilometer-9.0.7/tools/pretty_tox.sh
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     7336 2019-04-26 14:49:27.000000 ceilometer-9.0.7/tools/migrate_data_to_gnocchi.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1485 2019-04-26 14:49:27.000000 ceilometer-9.0.7/tools/make_test_data.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/playbooks/legacy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1986 2019-04-26 14:49:27.000000 ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2409 2019-04-26 14:49:27.000000 ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/playbooks/legacy/grenade-dsvm-ceilometer/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1647 2019-04-26 14:49:27.000000 ceilometer-9.0.7/playbooks/legacy/grenade-dsvm-ceilometer/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      411 2019-04-26 14:49:21.000000 ceilometer-9.0.7/playbooks/legacy/grenade-dsvm-ceilometer/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1935 2019-04-26 14:49:27.000000 ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2409 2019-04-26 14:49:27.000000 ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mysql/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1983 2019-04-26 14:49:27.000000 ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mysql/run.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2409 2019-04-26 14:49:27.000000 ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mysql/post.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      483 2019-04-26 14:49:27.000000 ceilometer-9.0.7/.testr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/api-ref/source/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      111 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1379 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/resources.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5383 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/alarms.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1215 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/events.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1744 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/api-ref/source/samples/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      827 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/resource-show-response.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      819 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/samples-list-response.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      483 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/meters-list-response.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      972 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/alarms-list-response.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      857 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/alarm-show-response.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      513 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/sample-show-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      703 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/resources-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      515 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/sample-create-request.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      585 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/samples-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      619 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/resource-show-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3306 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/capabilities-list-response.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      731 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/sample-show-response.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      371 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/statistics-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      641 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/alarm-show-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      659 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/sample-create-request.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      924 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/resources-list-response.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      395 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/meters-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      741 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/alarms-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      503 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/events-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      468 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/statistics-list-response.xml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1459 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/capabilities-list-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      427 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/samples/event-show-response.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17275 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/parameters.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3170 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/capabilities.inc
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9002 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/conf.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7741 2019-04-26 14:49:27.000000 ceilometer-9.0.7/api-ref/source/meters.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16144 2019-04-26 14:51:52.000000 ceilometer-9.0.7/AUTHORS
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/releasenotes/source/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      163 2019-04-26 14:49:27.000000 ceilometer-9.0.7/releasenotes/source/index.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      144 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/source/liberty.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      110 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/source/unreleased.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      136 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/source/ocata.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      140 2019-04-26 14:49:27.000000 ceilometer-9.0.7/releasenotes/source/newton.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      140 2019-04-26 14:49:27.000000 ceilometer-9.0.7/releasenotes/source/mitaka.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/releasenotes/source/_static/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/source/_static/.placeholder
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9461 2019-04-26 14:49:27.000000 ceilometer-9.0.7/releasenotes/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/releasenotes/notes/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/support-snmp-cpu-util-5c1c7afb713c1acd.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      210 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/gnocchi-host-metrics-829bcb965d8f2533.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      100 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/add-magnum-event-4c75ed0bb268d19c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      170 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/memory-bandwidth-meter-f86cf01178573671.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       86 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/zaqar-publisher-f7efa030b71731f4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      225 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/add-tool-for-migrating-data-to-gnocchi-cea8d4db68ce03d0.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      242 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/support-multiple-meter-definition-files-e3ce1fa73ef2e1de.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      135 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/remove-alarms-4df3cdb4f1fb5faa.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      251 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/deprecate-file-dispatcher-2aff376db7609136.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      274 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/network-statistics-from-opendaylight-787df77484d8d751.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      104 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/add-memory-swap-metric-f1633962ab2cf0f6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      122 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/kwapi_deprecated-c92b9e72c78365f0.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      775 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/http-publisher-authentication-6371c5a9aa8d4c03.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      332 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/instance-discovery-new-default-7f9b451a515dddf4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       80 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/drop-kwapi-b687bc476186d01b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      127 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/scan-domains-for-tenants-8f8c9edcb74cc173.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      254 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/unify-timestamp-of-polled-data-fbfcff43cd2d04bc.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      566 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/rename-ceilometer-dbsync-eb7a1fa503085528.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       62 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/pecan-debug-removed-dc737efbf911bde7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      221 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/sql-query-optimisation-ebb2233f7a9b5d06.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      251 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/remove-cadf-http-f8449ced3d2a29d4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      436 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/fix-agent-coordination-a7103a78fecaec24.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      727 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/http_proxy_to_wsgi_enabled-616fa123809e1600.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      233 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/cache-json-parsers-888307f3b6b498a2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      132 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/ceilometer-api-deprecate-862bfaa54e80fa01.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      246 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/parallel_requests_option-a3f901b6001e26e4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      151 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/polling-deprecation-4d5b83180893c053.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      425 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/remove-refresh-pipeline-618af089c5435db7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      439 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/drop-instance-meter-1b657717b21a0f55.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      244 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/http-dispatcher-batching-4e17fce46a196b07.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      158 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/gnocchi-orchestration-3497c689268df0d1.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      218 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/index-events-mongodb-63cb04200b03a093.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      394 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/fix-floatingip-pollster-f5172060c626b19e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/.placeholder
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      225 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/thread-safe-matching-4a635fc4965c5d4c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      165 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/event-type-race-c295baf7f1661eab.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      159 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/support-None-query-45abaae45f08eda4.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1200 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/less-nova-polling-ac56687da3f8b1a3.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      568 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/single-thread-pipelines-f9e6ac4b062747fe.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      170 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/deprecated_database_event_dispatcher_panko-607d558c86a90f17.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      357 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/configurable-data-collector-e247aadbffb85243.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      636 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/support-lbaasv2-polling-c830dd49bcf25f64.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      364 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/skip-duplicate-meter-def-0420164f6a95c50c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      428 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/refresh-legacy-cache-e4dbbd3e2eeca70b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      357 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/handle-malformed-resource-definitions-ad4f69f898ced34d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      469 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/deprecate-kafka-publisher-17b4f221758e15da.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      279 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/support-meter-batch-recording-mongo-6c2bdf4fbb9764eb.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      584 2019-04-26 14:49:27.000000 ceilometer-9.0.7/releasenotes/notes/always-requeue-7a2df9243987ab67.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      165 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/use-notification-transport-url-489f3d31dc66c4d2.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      148 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/add-full-snmpv3-usm-support-ab540c902fa89b9d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       67 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/keystone-v3-fab1e257c5672965.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      592 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/polling-definition-efffb92e3810e571.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      231 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/tooz-coordination-system-d1054b9d1a5ddf32.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      252 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/fix-aggregation-transformer-9472aea189fa8f65.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      450 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/deprecate-ceilometer-collector-b793b91cd28b9e7f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      201 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/ceilometer-event-api-removed-49c57835e307b997.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      606 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/deprecate-http-dispatcher-dbbaacee8182b550.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      340 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/cors-support-70c33ba1f6825a7b.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      102 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/remove-ceilometer-dbsync-53aa1b529f194f15.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      143 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/gnocchi-udp-collector-00415e6674b5cc0f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      384 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/improve-events-rbac-support-f216bd7f34b02032.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      145 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/support-cinder-volume-snapshot-backup-metering-d0a93b86bd53e803.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      170 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/aggregator-transformer-timeout-e0f42b6c96aa7ada.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      484 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/drop-image-meter-9c9b6cebd546dae7.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      326 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/mongodb-handle-large-numbers-7c235598ca700f2d.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      178 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/add-db-legacy-clean-tool-7b3e3714f414c448.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      167 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/deprecate-pollster-list-ccf22b0dea44f043.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      354 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/gnocchi-cache-1d8025dfc954f281.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      183 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/gnocchi-client-42cd992075ee53ab.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      277 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/perf-events-meter-b06c2a915c33bfaf.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      518 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/batch-messaging-d126cc525879d58e.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      204 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/fix-network-lb-bytes-sample-5dec2c6f3a8ae174.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      373 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/deprecate-http-control-exchanges-026a8de6819841f8.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      353 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/lookup-meter-def-vol-correctly-0122ae429275f2a6.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      413 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/compute-discovery-interval-d19f7c9036a8c186.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      266 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/support-unique-meter-query-221c6e0c1dc1b726.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      245 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/ship-yaml-files-33aa5852bedba7f0.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      202 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/gnocchi-cache-b9ad4d85a1da8d3f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      593 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/http-dispatcher-verify-ssl-551d639f37849c6f.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      328 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/remove-rpc-collector-d0d0a354140fd107.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       87 2019-04-26 14:49:21.000000 ceilometer-9.0.7/releasenotes/notes/remove-eventlet-6738321434b60c78.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      240 2019-04-26 14:49:27.000000 ceilometer-9.0.7/releasenotes/notes/use-glance-v2-in-image-pollsters-137a315577d5dc4c.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3821 2019-04-26 14:49:27.000000 ceilometer-9.0.7/.zuul.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1886 2019-04-26 14:49:27.000000 ceilometer-9.0.7/requirements.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      319 2019-04-26 14:49:27.000000 ceilometer-9.0.7/bindep.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1028 2019-04-26 14:49:21.000000 ceilometer-9.0.7/setup.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/devstack/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21519 2019-04-26 14:49:27.000000 ceilometer-9.0.7/devstack/plugin.sh
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      869 2019-04-26 14:49:27.000000 ceilometer-9.0.7/devstack/README.rst
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3781 2019-04-26 14:49:27.000000 ceilometer-9.0.7/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/devstack/files/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/devstack/files/rpms/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)       24 2019-04-26 14:49:21.000000 ceilometer-9.0.7/devstack/files/rpms/ceilometer
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      498 2019-04-26 14:49:27.000000 ceilometer-9.0.7/devstack/apache-ceilometer.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/devstack/upgrade/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      560 2019-04-26 14:49:27.000000 ceilometer-9.0.7/devstack/upgrade/settings
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)      649 2019-04-26 14:49:27.000000 ceilometer-9.0.7/devstack/upgrade/shutdown.sh
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     3180 2019-04-26 14:49:27.000000 ceilometer-9.0.7/devstack/upgrade/upgrade.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2085 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1718 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32940 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       11 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer.egg-info/top_level.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16651 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer.egg-info/entry_points.txt
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3229 2019-04-26 14:49:27.000000 ceilometer-9.0.7/tox.ini
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18425 2019-04-26 14:51:53.000000 ceilometer-9.0.7/setup.cfg
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/cmd/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/cmd/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3183 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/cmd/sample.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1087 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/cmd/api.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3382 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/cmd/polling.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      968 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/cmd/collector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      981 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/cmd/agent_notification.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5959 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/cmd/storage.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5424 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/nova_client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      817 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/pipeline/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/pipeline/data/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      195 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/pipeline/data/event_pipeline.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2507 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/pipeline/data/pipeline.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16763 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/pipeline/data/event_definitions.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3748 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/keystone_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/data/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/data/meters.d/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11102 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/data/meters.d/meters.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5694 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/sample.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/de/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/locale/de/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4235 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-warning.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4488 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-info.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4577 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-error.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16528 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/de/LC_MESSAGES/ceilometer.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/ru/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/locale/ru/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19452 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/ru/LC_MESSAGES/ceilometer.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/zh_TW/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/locale/zh_TW/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14792 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/zh_TW/LC_MESSAGES/ceilometer.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/locale/es/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4444 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/es/LC_MESSAGES/ceilometer-log-info.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4515 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/es/LC_MESSAGES/ceilometer-log-error.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16105 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/es/LC_MESSAGES/ceilometer.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/ja/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/locale/ja/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19081 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/ja/LC_MESSAGES/ceilometer.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/pt_BR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/locale/pt_BR/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15631 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/pt_BR/LC_MESSAGES/ceilometer.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/zh_CN/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/locale/zh_CN/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14977 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/zh_CN/LC_MESSAGES/ceilometer.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/ko_KR/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/locale/ko_KR/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5596 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-warning.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4283 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-info.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4908 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-error.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16497 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/it/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/locale/it/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15920 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/it/LC_MESSAGES/ceilometer.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:52.000000 ceilometer-9.0.7/ceilometer/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/locale/fr/LC_MESSAGES/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17087 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/locale/fr/LC_MESSAGES/ceilometer.po
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16188 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/neutron_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/hacking/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/hacking/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1732 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/hacking/checks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/image/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/image/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1377 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/image/discovery.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1981 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/image/glance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/network/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/network/statistics/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3424 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/network/statistics/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1436 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/flow.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1303 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/table.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/network/statistics/opendaylight/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/opendaylight/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17521 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/network/statistics/opendaylight/driver.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6284 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/opendaylight/client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2969 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/port.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/network/statistics/opencontrail/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/opencontrail/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6956 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/opencontrail/driver.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3581 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/opencontrail/client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      945 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/switch.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      981 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/driver.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1897 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/statistics/port_v2.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/network/services/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/services/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3206 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/services/vpnaas.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3825 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/network/services/discovery.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2919 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/services/fwaas.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1142 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/network/services/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    15021 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/services/lbaas.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1893 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/network/floatingip.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/objectstore/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/objectstore/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2593 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/objectstore/rgw_client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7334 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/objectstore/swift.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7635 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/objectstore/rgw.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/hardware/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/hardware/inspector/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      969 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/hardware/inspector/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13475 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/hardware/inspector/snmp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1590 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/hardware/inspector/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/hardware/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5151 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/hardware/discovery.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/hardware/pollsters/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/hardware/pollsters/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/hardware/pollsters/data/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5109 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/hardware/pollsters/data/snmp.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8538 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/hardware/pollsters/generic.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1948 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/hardware/pollsters/util.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7925 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/meter/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/meter/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9539 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/meter/notifications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/api/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/api/controllers/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1897 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/root.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/api/controllers/v2/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/v2/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8952 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/v2/root.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12716 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/v2/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4648 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/v2/samples.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3648 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/v2/capabilities.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6214 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/v2/resources.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18887 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/v2/meters.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13783 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/v2/query.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7668 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/controllers/v2/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3339 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/app.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2947 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/rbac.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2871 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/hooks.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5293 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/middleware.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      943 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/api/app.wsgi
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7811 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/collector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/storage/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30861 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/impl_mongodb.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6509 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/models.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5432 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    18962 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/impl_hbase.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    37120 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/impl_sqlalchemy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      116 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/manage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1569 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/027_remove_alarm_fk_constraints.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      871 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/002_remove_duration.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1141 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/003_set_utf8_charset.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      864 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/004_add_counter_unit.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1821 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/007_add_alarm_table.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      786 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/023_sqlite_upgrade.sql
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1319 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/011_indexes_cleanup.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5041 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/028_alembic_migrations.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      906 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/022_metadata_int_is_bigint.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2781 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/036_drop_sourceassoc_resource_tables.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3209 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/031_add_new_meter_table.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2206 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/024_event_use_floatingprecision.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2549 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/020_add_metadata_tables.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1980 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/017_convert_timestamp_as_datetime_to_decimal.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3122 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/023_add_trait_types.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      888 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/006_counter_volume_is_float.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2100 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/008_add_events.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      885 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/032_add_alarm_time_constraints.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2479 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/015_add_alarm_history_table.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      937 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/029_sample_recorded_at.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2098 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/025_alarm_use_floatingprecision.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4206 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/030_rename_meter_table.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5498 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/038_normalise_tables.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      822 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/013_rename_counter_to_meter_alarm.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2202 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/041_expand_event_traits.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      902 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/018_resource_resource_metadata_is_text.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      837 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/043_reduce_uuid_data_types.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1206 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/034_drop_dump_tables.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      949 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/005_remove_resource_timestamp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      763 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/042_add_raw_column.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      896 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/019_alarm_history_detail_is_text.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2342 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/012_add_missing_foreign_keys.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      846 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/010_add_index_to_meter.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2967 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/021_add_event_types.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2229 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/039_event_floatingprecision_pgsql.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      864 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/045_add_resource_metadatahash_index.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1630 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/044_restore_long_uuid_data_types.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      869 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/040_add_alarm_severity.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      913 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/009_event_strings.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3309 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/001_add_meter_table.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1721 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/014_add_event_message_id.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      767 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/033_alarm_id_rename.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3384 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/035_drop_user_project_tables.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      915 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/026_float_size.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2111 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/016_simpler_alarm.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1695 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/037_sample_index_cleanup.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      627 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/021_sqlite_upgrade.sql
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1230 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/migrate.cfg
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      143 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/README
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8052 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/models.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      979 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migration.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4833 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/sqlalchemy/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4856 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/impl_log.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/storage/mongo/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/mongo/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21688 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/mongo/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/storage/hbase/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/hbase/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2735 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/hbase/migration.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16240 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/hbase/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9553 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/hbase/inmemory.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3323 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/hbase/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8985 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6732 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/storage/pymongo_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/tempest/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/tempest/api/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/api/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3075 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/api/test_telemetry_notification_api.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4995 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/api/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/tempest/scenario/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/scenario/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5744 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/scenario/test_object_storage_telemetry_middleware.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5752 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/scenario/test_telemetry_integration.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1543 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/plugin.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5320 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/exceptions.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2238 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/tempest/service/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/service/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3969 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/tempest/service/client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7065 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/integration/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/integration/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/integration/gabbi/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/integration/gabbi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/integration/gabbi/gabbits-live/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11274 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/integration/gabbi/gabbits-live/aodh-gnocchi-threshold-alarm.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5053 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/integration/gabbi/gabbits-live/autoscaling.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3155 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/integration/gabbi/gabbits-live/create_stack.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3124 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/integration/gabbi/gabbits-live/update_stack.json
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1400 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/integration/gabbi/test_gabbi_live.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/integration/hooks/
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     3104 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/integration/hooks/post_test_hook.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/functional/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3149 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/clean-samples.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1426 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/resources-empty.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2556 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/resources-fixtured.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      452 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/fixture-samples.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1093 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/middleware.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      247 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/capabilities.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      688 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/basic.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11538 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/meters.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4428 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/samples.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1214 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/test_gabbi_prefix.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      793 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbi_paste.ini
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1186 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/test_gabbi.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      440 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbi_pipeline.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits_prefix/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1464 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits_prefix/clean-samples.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      612 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits_prefix/resources-fixtured.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      515 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits_prefix/basic.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6190 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/gabbi/fixtures.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    23177 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/test_notification.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7320 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      714 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7782 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_compute_duration_by_resource_scenarios.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1142 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_capabilities.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4479 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_app.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16363 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_post_samples_scenarios.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1601 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_versions.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    81197 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_statistics_scenarios.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7970 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_api_upgrade.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5614 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_list_samples_scenarios.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    20613 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_list_resources_scenarios.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12964 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_complex_query_scenarios.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7587 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_acl_scenarios.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    34350 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_list_meters_scenarios.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/functional/storage/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/storage/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5963 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/storage/test_impl_sqlalchemy.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1068 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/storage/test_impl_log.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)   127917 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/storage/test_storage_scenarios.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3575 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/storage/test_impl_hbase.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5609 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/storage/test_pymongo_base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4697 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/storage/test_impl_mongodb.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/functional/publisher/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/publisher/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2595 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/publisher/test_direct.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/functional/hooks/
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     1827 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/hooks/post_test_hook.sh
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9940 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/test_collector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7122 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/functional/test_bin.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7870 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_neutronclient.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2694 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_messaging.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    17018 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_event_pipeline.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    88909 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/pipeline_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/image/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/image/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4177 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/image/test_glance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1157 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3879 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_port.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opendaylight/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opendaylight/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    66706 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opendaylight/test_driver.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6227 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opendaylight/test_client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1160 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_switch.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opencontrail/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opencontrail/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11977 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opencontrail/test_driver.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2746 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opencontrail/test_client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1641 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_table.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1812 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_flow.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2472 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_port_v2.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6738 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_statistics.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/services/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7224 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/services/test_fwaas.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/services/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13430 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/services/test_lbaas_v2.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7561 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/services/test_vpnaas.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21669 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/services/test_lbaas.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4431 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/network/test_floating_ip.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/objectstore/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/objectstore/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7779 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/objectstore/test_rgw.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10179 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/objectstore/test_swift.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6205 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/objectstore/test_rgw_client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7651 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/hardware/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/hardware/inspector/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/hardware/inspector/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10605 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/hardware/inspector/test_snmp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1102 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/hardware/inspector/test_inspector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/hardware/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/hardware/pollsters/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/hardware/pollsters/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2428 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/hardware/pollsters/test_util.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7354 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/hardware/pollsters/test_generic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/meter/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/meter/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3195 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/meter/test_meter_plugins.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    41007 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/meter/test_notifications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/api/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/api/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1239 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/api/test_app.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1196 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/api/test_hooks.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/api/v2/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/api/v2/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14623 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/api/v2/test_complex_query.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4240 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/api/v2/test_statistics.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    16485 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/api/v2/test_query.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/storage/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/storage/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3064 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/storage/test_get_connection.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/storage/sqlalchemy/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/storage/sqlalchemy/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3788 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/storage/sqlalchemy/test_models.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2199 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/storage/test_base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4017 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_sample.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/agent/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/agent/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    19317 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/agent/test_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8522 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/agent/test_discovery.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27306 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/agent/agentbase.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/telemetry/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/telemetry/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3969 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/telemetry/test_notifications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/volume/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/volume/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6943 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/volume/test_cinder.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4340 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_middleware.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/publisher/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/publisher/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4776 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4460 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_file.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6540 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_udp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14855 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_messaging_publisher.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8730 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_kafka_broker_publisher.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4521 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_zaqar.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10485 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_http.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11611 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/test_discovery.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/hyperv/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/hyperv/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7632 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/hyperv/test_inspector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/xenapi/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/xenapi/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6809 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/xenapi/test_inspector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/vmware/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/vmware/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7369 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/vmware/test_vsphere_operations.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7921 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/vmware/test_inspector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/libvirt/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/libvirt/__init__.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)    22696 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/libvirt/test_inspector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    12986 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_net.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6715 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_cpu.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3856 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_perf.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8362 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_memory.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5213 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_location_metadata.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2687 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14261 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_diskio.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3625 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/test_file.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    27462 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/test_gnocchi.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1673 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/test_dispatcher.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8705 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/test_http.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3130 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/test_db.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/transformer/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/transformer/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4529 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/transformer/test_conversions.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14621 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_neutronclient_lbaas_v2.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11466 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_decoupled_pipeline.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/event/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/event/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    33054 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/event/test_converter.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7492 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/event/test_endpoint.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4328 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/event/test_trait_plugins.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/platform/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/platform/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3898 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/platform/fake_utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13467 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/platform/ipmitool_test_data.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7016 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/platform/test_intel_node_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4585 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/platform/test_ipmi_sensor.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/notifications/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/notifications/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8503 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/notifications/test_ironic.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    30749 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/notifications/ipmi_test_data.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/pollsters/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/pollsters/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4149 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/pollsters/test_sensor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2722 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/pollsters/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4921 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/ipmi/pollsters/test_node.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9623 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_novaclient.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1631 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_declarative.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2489 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_collector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3993 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/unit/test_polling.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3516 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/mocks.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3904 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/tests/base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4026 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/exchange_control.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      649 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/agent/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/agent/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9549 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/agent/plugin_base.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21371 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/agent/manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/agent/discovery/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1691 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/agent/discovery/tenant.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/agent/discovery/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1526 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/agent/discovery/endpoint.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      787 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/agent/discovery/localnode.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1063 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/telemetry/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/telemetry/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2076 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/telemetry/notifications.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/conf/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1404 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/conf/defaults.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/conf/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/volume/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/volume/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1981 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/volume/discovery.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3389 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/volume/cinder.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/publisher/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2359 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/publisher/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7438 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/publisher/http.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3911 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/publisher/direct.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2803 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/publisher/zaqar.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3877 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/publisher/utils.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3680 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/publisher/file.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2972 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/publisher/udp.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9446 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/publisher/messaging.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4146 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/publisher/kafka_broker.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1394 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/publisher/test.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3373 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/messaging.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/compute/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11955 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/compute/discovery.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/compute/virt/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/virt/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/compute/virt/hyperv/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/virt/hyperv/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5867 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/compute/virt/hyperv/inspector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9933 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/compute/virt/inspector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/compute/virt/xenapi/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/virt/xenapi/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7592 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/compute/virt/xenapi/inspector.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/compute/virt/vmware/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/virt/vmware/__init__.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     8473 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/compute/virt/vmware/inspector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10338 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/virt/vmware/vsphere_operations.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/compute/virt/libvirt/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/virt/libvirt/__init__.py
+-rwxrwxrwx   0 zuul      (1000) zuul      (1000)     9073 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/compute/virt/libvirt/inspector.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4180 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/virt/libvirt/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/compute/pollsters/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6836 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/compute/pollsters/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     7123 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/compute/pollsters/disk.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3491 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/pollsters/net.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2952 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/pollsters/instance_stats.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3524 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/compute/pollsters/util.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2395 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/dispatcher/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3323 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/dispatcher/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6720 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/dispatcher/http.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/dispatcher/data/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8977 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/dispatcher/data/gnocchi_resources.yaml
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    21513 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/dispatcher/gnocchi.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2939 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/dispatcher/file.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1467 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/dispatcher/gnocchi_opts.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2527 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/dispatcher/database.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    32697 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/pipeline.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/transformer/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2359 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/transformer/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1322 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/transformer/accumulator.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6190 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/transformer/arithmetic.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13387 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/transformer/conversions.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     9401 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/gnocchi_client.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6632 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/event/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/event/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/event/storage/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4206 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/event/storage/models.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/event/storage/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     8534 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/event/trait_plugins.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     2238 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/event/endpoint.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    11815 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/event/converter.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     6707 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/declarative.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/ipmi/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/ipmi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/ipmi/platform/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/ipmi/platform/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    13194 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/ipmi/platform/intel_node_manager.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      726 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/ipmi/platform/exception.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4014 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/ipmi/platform/ipmi_sensor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     4490 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/ipmi/platform/ipmitool.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/ipmi/notifications/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/ipmi/notifications/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5898 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/ipmi/notifications/ironic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2019-04-26 14:51:53.000000 ceilometer-9.0.7/ceilometer/ipmi/pollsters/
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)      956 2019-04-26 14:49:21.000000 ceilometer-9.0.7/ceilometer/ipmi/pollsters/__init__.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     3851 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/ipmi/pollsters/sensor.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     5045 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/ipmi/pollsters/node.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)     1332 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/middleware.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    14149 2019-04-26 14:49:27.000000 ceilometer-9.0.7/ceilometer/notification.py
+-rw-rw-rw-   0 zuul      (1000) zuul      (1000)    10143 2019-04-26 14:49:21.000000 ceilometer-9.0.7/LICENSE
```

### Comparing `ceilometer-9.0.6/README.rst` & `ceilometer-9.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/.zuul.yaml` & `ceilometer-9.0.7/.zuul.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,20 @@
     timeout: 10800
     required-projects:
       - openstack-dev/grenade
       - openstack-infra/devstack-gate
       - openstack/ceilometer
 
 - project:
+    templates:
+      - openstack-python-jobs
+      - openstack-python35-jobs
+      - publish-openstack-sphinx-docs
+      - periodic-stable-jobs
+      - release-notes-jobs
     check:
       jobs:
         - ceilometer-dsvm-tempest-plugin-mongodb
         - ceilometer-dsvm-tempest-plugin-mysql
         - ceilometer-tox-py27-mongodb
         - ceilometer-tox-py27-mysql
         - ceilometer-tox-py27-postgresql
@@ -87,14 +93,15 @@
         - tripleo-ci-centos-7-scenario001-multinode-oooq-container:
             voting: false
         - tripleo-ci-centos-7-scenario002-multinode-oooq:
             voting: false
         - tripleo-ci-centos-7-scenario002-multinode-oooq-container:
             voting: false
     gate:
+      queue: telemetry
       jobs:
         - ceilometer-dsvm-tempest-plugin-mongodb
         - ceilometer-dsvm-tempest-plugin-mysql
         - ceilometer-tox-py27-mongodb
         - ceilometer-tox-py27-mysql
         - ceilometer-tox-py27-postgresql
         - grenade-dsvm-ceilometer:
```

### Comparing `ceilometer-9.0.6/run-tests.sh` & `ceilometer-9.0.7/run-tests.sh`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/.mailmap` & `ceilometer-9.0.7/.mailmap`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mysql/post.yaml` & `ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only/post.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mysql/run.yaml` & `ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mysql/run.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -14,30 +14,30 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
           set -e
           set -x
           export PYTHONUNBUFFERED=true
           export DEVSTACK_GATE_TEMPEST=1
           export DEVSTACK_GATE_TEMPEST_REGEX="^ceilometer\."
           export DEVSTACK_GATE_TEMPEST_ALL_PLUGINS=1
           export DEVSTACK_GATE_CEILOMETER_BACKEND=mysql
-          export DEVSTACK_LOCAL_CONFIG="enable_plugin ceilometer git://git.openstack.org/openstack/ceilometer"
+          export DEVSTACK_LOCAL_CONFIG="enable_plugin ceilometer https://git.openstack.org/openstack/ceilometer"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"CEILOMETER_BACKEND=mysql"
 
           export BRANCH_OVERRIDE=default
           if [ "$BRANCH_OVERRIDE" != "default" ] ; then
               export OVERRIDE_ZUUL_BRANCH=$BRANCH_OVERRIDE
           fi
           if [ "mysql" = "postgresql" ] ; then
```

### Comparing `ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb/post.yaml` & `ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb/post.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb/run.yaml` & `ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only/run.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 - hosts: all
-  name: Autoconverted job legacy-ceilometer-dsvm-tempest-plugin-mongodb from old job
-    gate-ceilometer-dsvm-tempest-plugin-mongodb-ubuntu-xenial
+  name: Autoconverted job legacy-ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only
+    from old job gate-ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only-ubuntu-xenial
   tasks:
 
     - name: Ensure legacy workspace directory
       file:
         path: '{{ ansible_user_dir }}/workspace'
         state: directory
 
@@ -14,39 +14,39 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
           set -e
           set -x
           export PYTHONUNBUFFERED=true
           export DEVSTACK_GATE_TEMPEST=1
           export DEVSTACK_GATE_TEMPEST_REGEX="^ceilometer\."
           export DEVSTACK_GATE_TEMPEST_ALL_PLUGINS=1
-          export DEVSTACK_LOCAL_CONFIG="enable_plugin ceilometer git://git.openstack.org/openstack/ceilometer"
+          export DEVSTACK_LOCAL_CONFIG="enable_plugin ceilometer https://git.openstack.org/openstack/ceilometer"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"CEILOMETER_BACKEND=mongodb"
 
           export BRANCH_OVERRIDE=default
           if [ "$BRANCH_OVERRIDE" != "default" ] ; then
               export OVERRIDE_ZUUL_BRANCH=$BRANCH_OVERRIDE
           fi
           if [ "mongodb" = "postgresql" ] ; then
               export DEVSTACK_GATE_POSTGRES=1
           fi
-          if [ "" == "-identity-v3-only" ] ; then
+          if [ "-identity-v3-only" == "-identity-v3-only" ] ; then
               export DEVSTACK_LOCAL_CONFIG+=$'\n'"ENABLE_IDENTITY_V2=False"
           fi
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
           ./safe-devstack-vm-gate-wrap.sh
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
```

### Comparing `ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only/post.yaml` & `ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mysql/post.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only/run.yaml` & `ceilometer-9.0.7/playbooks/legacy/ceilometer-dsvm-tempest-plugin-mongodb/run.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 - hosts: all
-  name: Autoconverted job legacy-ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only
-    from old job gate-ceilometer-dsvm-tempest-plugin-mongodb-identity-v3-only-ubuntu-xenial
+  name: Autoconverted job legacy-ceilometer-dsvm-tempest-plugin-mongodb from old job
+    gate-ceilometer-dsvm-tempest-plugin-mongodb-ubuntu-xenial
   tasks:
 
     - name: Ensure legacy workspace directory
       file:
         path: '{{ ansible_user_dir }}/workspace'
         state: directory
 
@@ -14,39 +14,39 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
           set -e
           set -x
           export PYTHONUNBUFFERED=true
           export DEVSTACK_GATE_TEMPEST=1
           export DEVSTACK_GATE_TEMPEST_REGEX="^ceilometer\."
           export DEVSTACK_GATE_TEMPEST_ALL_PLUGINS=1
-          export DEVSTACK_LOCAL_CONFIG="enable_plugin ceilometer git://git.openstack.org/openstack/ceilometer"
+          export DEVSTACK_LOCAL_CONFIG="enable_plugin ceilometer https://git.openstack.org/openstack/ceilometer"
           export DEVSTACK_LOCAL_CONFIG+=$'\n'"CEILOMETER_BACKEND=mongodb"
 
           export BRANCH_OVERRIDE=default
           if [ "$BRANCH_OVERRIDE" != "default" ] ; then
               export OVERRIDE_ZUUL_BRANCH=$BRANCH_OVERRIDE
           fi
           if [ "mongodb" = "postgresql" ] ; then
               export DEVSTACK_GATE_POSTGRES=1
           fi
-          if [ "-identity-v3-only" == "-identity-v3-only" ] ; then
+          if [ "" == "-identity-v3-only" ] ; then
               export DEVSTACK_LOCAL_CONFIG+=$'\n'"ENABLE_IDENTITY_V2=False"
           fi
           cp devstack-gate/devstack-vm-gate-wrap.sh ./safe-devstack-vm-gate-wrap.sh
           ./safe-devstack-vm-gate-wrap.sh
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
```

### Comparing `ceilometer-9.0.6/playbooks/legacy/grenade-dsvm-ceilometer/run.yaml` & `ceilometer-9.0.7/playbooks/legacy/grenade-dsvm-ceilometer/run.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
           set -x
           cat > clonemap.yaml << EOF
           clonemap:
             - name: openstack-infra/devstack-gate
               dest: devstack-gate
           EOF
           /usr/zuul-env/bin/zuul-cloner -m clonemap.yaml --cache-dir /opt/git \
-              git://git.openstack.org \
+              https://git.openstack.org \
               openstack-infra/devstack-gate
         executable: /bin/bash
         chdir: '{{ ansible_user_dir }}/workspace'
       environment: '{{ zuul | zuul_legacy_vars }}'
 
     - shell:
         cmd: |
```

### Comparing `ceilometer-9.0.6/ceilometer.egg-info/SOURCES.txt` & `ceilometer-9.0.7/ceilometer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer.egg-info/entry_points.txt` & `ceilometer-9.0.7/ceilometer.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer.egg-info/requires.txt` & `ceilometer-9.0.7/ceilometer.egg-info/requires.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 cachetools>=1.1.0
 cotyledon>=1.3.0
-futures>=3.0
 futurist>=0.11.0
 debtcollector>=1.2.0
 jsonpath-rw-ext>=0.1.9
 jsonschema!=2.5.0,<3.0.0,>=2.0.0
 kafka-python>=1.3.2
 keystonemiddleware!=4.1.0,!=4.19.0,>=4.0.0
 lxml>=2.3
@@ -42,14 +41,17 @@
 tenacity>=3.2.1
 tooz[zake]>=1.47.0
 WebOb>=1.5.0
 WSME>=0.8
 python-dateutil>=2.4.2
 os-xenapi>=0.1.1
 
+[:(python_version=='2.7' or python_version=='2.6')]
+futures>=3.0
+
 [gnocchi]
 gnocchiclient>=3.1.0
 
 [mongo]
 pymongo!=3.1,>=3.0.2
 
 [mysql]
@@ -57,19 +59,19 @@
 
 [postgresql]
 psycopg2>=2.5
 
 [test]
 coverage>=3.6
 fixtures<2.0,>=1.3.1
-happybase!=0.7,<1.0.0,>=0.5
 mock>=1.2
 os-win>=0.2.3
 oslo.cache>=1.5.0
 openstackdocstheme>=1.11.0
+oslo.messaging[kafka]>=5.12.0
 reno>=1.6.2
 oslotest>=2.15.0
 oslo.vmware>=1.16.0
 python-subunit>=0.0.18
 pyOpenSSL>=0.14
 sphinx>=1.6.2
 sphinxcontrib-httpdomain
@@ -81,9 +83,12 @@
 requests-aws>=0.1.4
 os-testr>=0.4.1
 tempest>=14.0.0
 WebTest>=2.0
 pifpaf>=0.0.11
 os-api-ref>=0.1.0
 
+[test:(python_version=='2.7')]
+happybase!=0.7,<1.0.0,>=0.5
+
 [zaqar]
 python-zaqarclient>=1.0.0
```

### Comparing `ceilometer-9.0.6/ceilometer.egg-info/PKG-INFO` & `ceilometer-9.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ceilometer
-Version: 9.0.6
+Version: 9.0.7
 Summary: OpenStack Telemetry
 Home-page: https://docs.openstack.org/ceilometer/latest/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ==========
         Ceilometer
@@ -44,13 +44,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: System :: Monitoring
+Provides-Extra: test
 Provides-Extra: postgresql
-Provides-Extra: mongo
 Provides-Extra: zaqar
-Provides-Extra: mysql
-Provides-Extra: test
 Provides-Extra: gnocchi
+Provides-Extra: mysql
+Provides-Extra: mongo
```

### Comparing `ceilometer-9.0.6/rally-jobs/plugins/plugin_sample.py` & `ceilometer-9.0.7/rally-jobs/plugins/plugin_sample.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/rally-jobs/README.rst` & `ceilometer-9.0.7/rally-jobs/README.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/rally-jobs/ceilometer.yaml` & `ceilometer-9.0.7/rally-jobs/ceilometer.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/test-requirements.txt` & `ceilometer-9.0.7/test-requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 fixtures<2.0,>=1.3.1 # Apache-2.0/BSD
 happybase!=0.7,>=0.5,<1.0.0;python_version=='2.7' # MIT
 mock>=1.2 # BSD
 os-win>=0.2.3 # Apache-2.0
 oslo.cache>=1.5.0 # Apache-2.0
 # Docs Requirements
 openstackdocstheme>=1.11.0 # Apache-2.0
+oslo.messaging[kafka]>=5.12.0 # Apache-2.0
 reno>=1.6.2 # Apache2
 oslotest>=2.15.0 # Apache-2.0
 oslo.vmware>=1.16.0 # Apache-2.0
 python-subunit>=0.0.18 # Apache-2.0/BSD
 pyOpenSSL>=0.14  # Apache-2.0
 sphinx>=1.6.2  # BSD
 sphinxcontrib-httpdomain # BSD
```

### Comparing `ceilometer-9.0.6/AUTHORS` & `ceilometer-9.0.7/AUTHORS`

 * *Files 0% similar despite different names*

```diff
@@ -74,14 +74,15 @@
 Dina Belova <dbelova@mirantis.com>
 Dirk Mueller <dirk@dmllr.de>
 Divya <dikonoor@in.ibm.com>
 Dong Ma <winterma.dong@gmail.com>
 Doug Hellmann <doug@doughellmann.com>
 Drew Thorstensen <thorst@us.ibm.com>
 Edwin Zhai <edwin.zhai@intel.com>
+Elod Illes <elod.illes@ericsson.com>
 Emilien Macchi <emilien@redhat.com>
 Emma Foley <emma.l.foley@intel.com>
 Endre Karlson <endre.karlson@gmail.com>
 Eoghan Glynn <eglynn@redhat.com>
 Eoghan Glynn <elynn@redhat.com>
 Eric Berglund <esberglu@us.ibm.com>
 Eric Brown <browne@vmware.com>
@@ -111,14 +112,15 @@
 Haomeng, Wang <whaom@cn.ibm.com>
 Harri Hämäläinen <hhamalai@iki.fi>
 Hisashi Osanai <osanai.hisashi@jp.fujitsu.com>
 Hongbin Lu <hongbin.lu@huawei.com>
 Huachao Mao <huachaomao@gmail.com>
 Huan Xie <huan.xie@citrix.com>
 Huang Rui <bjhuangr@cn.ibm.com>
+Ian Wienand <iwienand@redhat.com>
 Ianeta Hutchinson <ianeta.hutchinson@intel.com>
 Igor Degtiarov <idegtiarov@mirantis.com>
 Ihar Hrachyshka <ihrachys@redhat.com>
 Ildar Svetlov <isvetlov@mirantis.com>
 Ildiko Vancsa <ildiko.vancsa@ericsson.com>
 Ilya Sviridov <isviridov@mirantis.com>
 Ilya Tyaptin <ityaptin@mirantis.com>
@@ -327,15 +329,14 @@
 ZhaoBo <zhaobo6@huawei.com>
 Zhengwei Gao <gaozhengwei1@letv.com>
 Zhi Kun Liu <zhikunli@cn.ibm.com>
 Zhi Yan Liu <zhiyanl@cn.ibm.com>
 ZhiQiang Fan <zhiqiang.fan@huawei.com>
 Zhongyue Luo <zhongyue.nah@intel.com>
 Zi Lian Ji <jizilian@cn.ibm.com>
-Zuul <zuul@review.openstack.org>
 aggaatul <atula@hp.com>
 alextricity25 <miguel.cantu@rackspace.com>
 ananya23d <ananya.chatterjee@nectechnologies.in>
 annegentle <anne@openstack.org>
 ansaba <ahmed.nooras.saba@gmail.com>
 blue55 <yllan@fiberhome.com>
 caoyuan <cao.yuan@99cloud.net>
```

### Comparing `ceilometer-9.0.6/ChangeLog` & `ceilometer-9.0.7/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 CHANGES
 =======
 
+9.0.7
+-----
+
+* Replace openstack.org git:// URLs with https://
+* Use kafka extras for oslo.messaging
+* import zuul job settings from project-config
+
 9.0.6
 -----
 
 * snmp: ignore rfc1905.NoSuchInstance result
 * snmp: make oid value retrieval more solid
 * ignore compute.instance.create.start for metrics
 * Modify Ceilometer API specification
```

### Comparing `ceilometer-9.0.6/tox.ini` & `ceilometer-9.0.7/tox.ini`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/CONTRIBUTING.rst` & `ceilometer-9.0.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/setup.py` & `ceilometer-9.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/webapi/index.rst` & `ceilometer-9.0.7/doc/source/webapi/index.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/webapi/v2.rst` & `ceilometer-9.0.7/doc/source/webapi/v2.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-base-rdo.rst` & `ceilometer-9.0.7/doc/source/install/install-base-rdo.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/verify.rst` & `ceilometer-9.0.7/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/get_started.rst` & `ceilometer-9.0.7/doc/source/install/get_started.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-base-prereq-common.inc` & `ceilometer-9.0.7/doc/source/install/install-base-prereq-common.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/neutron/install-neutron-ubuntu.rst` & `ceilometer-9.0.7/doc/source/install/neutron/install-neutron-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/neutron/install-neutron-rdo.rst` & `ceilometer-9.0.7/doc/source/install/neutron/install-neutron-rdo.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/neutron/install-neutron-obs.rst` & `ceilometer-9.0.7/doc/source/install/neutron/install-neutron-obs.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/swift/install-swift-config-common.inc` & `ceilometer-9.0.7/doc/source/install/swift/install-swift-config-common.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/swift/install-swift-obs.rst` & `ceilometer-9.0.7/doc/source/install/swift/install-swift-obs.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/swift/install-swift-prereq-common.inc` & `ceilometer-9.0.7/doc/source/install/swift/install-swift-prereq-common.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/swift/install-swift-rdo.rst` & `ceilometer-9.0.7/doc/source/install/swift/install-swift-rdo.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/swift/install-swift-ubuntu.rst` & `ceilometer-9.0.7/doc/source/install/swift/install-swift-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-compute-rdo.rst` & `ceilometer-9.0.7/doc/source/install/install-compute-rdo.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-base-ubuntu.rst` & `ceilometer-9.0.7/doc/source/install/install-base-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-gnocchi.inc` & `ceilometer-9.0.7/doc/source/install/install-gnocchi.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-base-config-common.inc` & `ceilometer-9.0.7/doc/source/install/install-base-config-common.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-compute-obs.rst` & `ceilometer-9.0.7/doc/source/install/install-compute-obs.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/glance/install-glance-obs.rst` & `ceilometer-9.0.7/doc/source/install/glance/install-glance-obs.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/glance/install-glance-ubuntu.rst` & `ceilometer-9.0.7/doc/source/install/glance/install-glance-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/glance/install-glance-rdo.rst` & `ceilometer-9.0.7/doc/source/install/glance/install-glance-rdo.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/heat/install-heat-obs.rst` & `ceilometer-9.0.7/doc/source/install/heat/install-heat-obs.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/heat/install-heat-rdo.rst` & `ceilometer-9.0.7/doc/source/install/heat/install-heat-rdo.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/heat/install-heat-ubuntu.rst` & `ceilometer-9.0.7/doc/source/install/heat/install-heat-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/conf.py` & `ceilometer-9.0.7/doc/source/install/conf.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-compute-ubuntu.rst` & `ceilometer-9.0.7/doc/source/install/install-compute-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/index.rst` & `ceilometer-9.0.7/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-compute-common.inc` & `ceilometer-9.0.7/doc/source/install/install-compute-common.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-controller.rst` & `ceilometer-9.0.7/doc/source/install/install-controller.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/cinder/install-cinder-ubuntu.rst` & `ceilometer-9.0.7/doc/source/install/cinder/install-cinder-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/cinder/install-cinder-rdo.rst` & `ceilometer-9.0.7/doc/source/install/cinder/install-cinder-rdo.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/cinder/install-cinder-config-common.inc` & `ceilometer-9.0.7/doc/source/install/cinder/install-cinder-config-common.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/cinder/install-cinder-obs.rst` & `ceilometer-9.0.7/doc/source/install/cinder/install-cinder-obs.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/install/install-base-obs.rst` & `ceilometer-9.0.7/doc/source/install/install-base-obs.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/5-multi-publish.png` & `ceilometer-9.0.7/doc/source/contributor/5-multi-publish.png`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/4-Transformer.png` & `ceilometer-9.0.7/doc/source/contributor/4-Transformer.png`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/3-Pipeline.png` & `ceilometer-9.0.7/doc/source/contributor/3-Pipeline.png`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/2-accessmodel.png` & `ceilometer-9.0.7/doc/source/contributor/2-accessmodel.png`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/ceilo-gnocchi-arch.png` & `ceilometer-9.0.7/doc/source/contributor/ceilo-gnocchi-arch.png`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/new_resource_types.rst` & `ceilometer-9.0.7/doc/source/contributor/new_resource_types.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/overview.rst` & `ceilometer-9.0.7/doc/source/contributor/overview.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/6-storagemodel.png` & `ceilometer-9.0.7/doc/source/contributor/6-storagemodel.png`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/plugins.rst` & `ceilometer-9.0.7/doc/source/contributor/plugins.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/1-agents.png` & `ceilometer-9.0.7/doc/source/contributor/1-agents.png`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/architecture.rst` & `ceilometer-9.0.7/doc/source/contributor/architecture.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/ceilo-arch.png` & `ceilometer-9.0.7/doc/source/contributor/ceilo-arch.png`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/events.rst` & `ceilometer-9.0.7/doc/source/contributor/events.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/2-2-collection-poll.png` & `ceilometer-9.0.7/doc/source/contributor/2-2-collection-poll.png`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/gmr.rst` & `ceilometer-9.0.7/doc/source/contributor/gmr.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/index.rst` & `ceilometer-9.0.7/doc/source/contributor/index.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/testing.rst` & `ceilometer-9.0.7/doc/source/contributor/testing.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/devstack.rst` & `ceilometer-9.0.7/doc/source/contributor/devstack.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/measurements.rst` & `ceilometer-9.0.7/doc/source/contributor/measurements.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/contributor/2-1-collection-notification.png` & `ceilometer-9.0.7/doc/source/contributor/2-1-collection-notification.png`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/glossary.rst` & `ceilometer-9.0.7/doc/source/glossary.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/configuration/index.rst` & `ceilometer-9.0.7/doc/source/configuration/index.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/conf.py` & `ceilometer-9.0.7/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/index.rst` & `ceilometer-9.0.7/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/admin/telemetry-measurements.rst` & `ceilometer-9.0.7/doc/source/admin/telemetry-measurements.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/admin/telemetry-data-pipelines.rst` & `ceilometer-9.0.7/doc/source/admin/telemetry-data-pipelines.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/admin/telemetry-system-architecture.rst` & `ceilometer-9.0.7/doc/source/admin/telemetry-system-architecture.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/admin/telemetry-best-practices.rst` & `ceilometer-9.0.7/doc/source/admin/telemetry-best-practices.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/admin/index.rst` & `ceilometer-9.0.7/doc/source/admin/index.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/admin/telemetry-data-retrieval.rst` & `ceilometer-9.0.7/doc/source/admin/telemetry-data-retrieval.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/admin/telemetry-events.rst` & `ceilometer-9.0.7/doc/source/admin/telemetry-events.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/admin/telemetry-data-collection.rst` & `ceilometer-9.0.7/doc/source/admin/telemetry-data-collection.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/admin/telemetry-troubleshooting-guide.rst` & `ceilometer-9.0.7/doc/source/admin/telemetry-troubleshooting-guide.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/releasenotes/folsom.rst` & `ceilometer-9.0.7/doc/source/releasenotes/folsom.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/source/releasenotes/index.rst` & `ceilometer-9.0.7/doc/source/releasenotes/index.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/doc/Makefile` & `ceilometer-9.0.7/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/devstack/README.rst` & `ceilometer-9.0.7/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/devstack/settings` & `ceilometer-9.0.7/devstack/settings`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/devstack/upgrade/shutdown.sh` & `ceilometer-9.0.7/devstack/upgrade/shutdown.sh`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/devstack/upgrade/settings` & `ceilometer-9.0.7/devstack/upgrade/settings`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 register_project_for_upgrade ceilometer
 
-devstack_localrc base enable_plugin ceilometer git://git.openstack.org/openstack/ceilometer
+devstack_localrc base enable_plugin ceilometer https://git.openstack.org/openstack/ceilometer
 devstack_localrc base enable_service ceilometer-acompute ceilometer-acentral ceilometer-aipmi ceilometer-anotification ceilometer-collector ceilometer-api tempest
 
-devstack_localrc target enable_plugin ceilometer git://git.openstack.org/openstack/ceilometer
+devstack_localrc target enable_plugin ceilometer https://git.openstack.org/openstack/ceilometer
 devstack_localrc target enable_service ceilometer-acompute ceilometer-acentral ceilometer-aipmi ceilometer-anotification ceilometer-collector ceilometer-api tempest
```

### Comparing `ceilometer-9.0.6/devstack/upgrade/upgrade.sh` & `ceilometer-9.0.7/devstack/upgrade/upgrade.sh`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/devstack/plugin.sh` & `ceilometer-9.0.7/devstack/plugin.sh`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Install and start **Ceilometer** service in devstack
 #
 # To enable Ceilometer in devstack add an entry to local.conf that
 # looks like
 #
 # [[local|localrc]]
-# enable_plugin ceilometer git://git.openstack.org/openstack/ceilometer
+# enable_plugin ceilometer https://git.openstack.org/openstack/ceilometer
 #
 # By default all ceilometer services are started (see devstack/settings)
 # except for the ceilometer-aipmi service. To disable a specific service
 # use the disable_service function.
 #
 # NOTE: Currently, there are two ways to get the IPMI based meters in
 # OpenStack. One way is to configure Ironic conductor to report those meters
```

### Comparing `ceilometer-9.0.6/setup.cfg` & `ceilometer-9.0.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/requirements.txt` & `ceilometer-9.0.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/LICENSE` & `ceilometer-9.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/PKG-INFO` & `ceilometer-9.0.7/ceilometer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ceilometer
-Version: 9.0.6
+Version: 9.0.7
 Summary: OpenStack Telemetry
 Home-page: https://docs.openstack.org/ceilometer/latest/
 Author: OpenStack
 Author-email: openstack-dev@lists.openstack.org
 License: UNKNOWN
 Description: ==========
         Ceilometer
@@ -44,13 +44,13 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Topic :: System :: Monitoring
+Provides-Extra: test
 Provides-Extra: postgresql
-Provides-Extra: mongo
 Provides-Extra: zaqar
-Provides-Extra: mysql
-Provides-Extra: test
 Provides-Extra: gnocchi
+Provides-Extra: mysql
+Provides-Extra: mongo
```

### Comparing `ceilometer-9.0.6/HACKING.rst` & `ceilometer-9.0.7/HACKING.rst`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/etc/apache2/ceilometer` & `ceilometer-9.0.7/etc/apache2/ceilometer`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/etc/ceilometer/api_paste.ini` & `ceilometer-9.0.7/etc/ceilometer/api_paste.ini`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/etc/ceilometer/rootwrap.conf` & `ceilometer-9.0.7/etc/ceilometer/rootwrap.conf`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/etc/ceilometer/examples/loadbalancer_v2_meter_definitions.yaml` & `ceilometer-9.0.7/etc/ceilometer/examples/loadbalancer_v2_meter_definitions.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/etc/ceilometer/examples/osprofiler_event_definitions.yaml` & `ceilometer-9.0.7/etc/ceilometer/examples/osprofiler_event_definitions.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/etc/ceilometer/polling.yaml` & `ceilometer-9.0.7/etc/ceilometer/polling.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/source/conf.py` & `ceilometer-9.0.7/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/always-requeue-7a2df9243987ab67.yaml` & `ceilometer-9.0.7/releasenotes/notes/always-requeue-7a2df9243987ab67.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/batch-messaging-d126cc525879d58e.yaml` & `ceilometer-9.0.7/releasenotes/notes/batch-messaging-d126cc525879d58e.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/polling-definition-efffb92e3810e571.yaml` & `ceilometer-9.0.7/releasenotes/notes/polling-definition-efffb92e3810e571.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/single-thread-pipelines-f9e6ac4b062747fe.yaml` & `ceilometer-9.0.7/releasenotes/notes/single-thread-pipelines-f9e6ac4b062747fe.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/less-nova-polling-ac56687da3f8b1a3.yaml` & `ceilometer-9.0.7/releasenotes/notes/less-nova-polling-ac56687da3f8b1a3.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/http_proxy_to_wsgi_enabled-616fa123809e1600.yaml` & `ceilometer-9.0.7/releasenotes/notes/http_proxy_to_wsgi_enabled-616fa123809e1600.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/http-dispatcher-verify-ssl-551d639f37849c6f.yaml` & `ceilometer-9.0.7/releasenotes/notes/http-dispatcher-verify-ssl-551d639f37849c6f.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/deprecate-http-dispatcher-dbbaacee8182b550.yaml` & `ceilometer-9.0.7/releasenotes/notes/deprecate-http-dispatcher-dbbaacee8182b550.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/support-lbaasv2-polling-c830dd49bcf25f64.yaml` & `ceilometer-9.0.7/releasenotes/notes/support-lbaasv2-polling-c830dd49bcf25f64.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/rename-ceilometer-dbsync-eb7a1fa503085528.yaml` & `ceilometer-9.0.7/releasenotes/notes/rename-ceilometer-dbsync-eb7a1fa503085528.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/releasenotes/notes/http-publisher-authentication-6371c5a9aa8d4c03.yaml` & `ceilometer-9.0.7/releasenotes/notes/http-publisher-authentication-6371c5a9aa8d4c03.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/resources.inc` & `ceilometer-9.0.7/api-ref/source/resources.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/meters.inc` & `ceilometer-9.0.7/api-ref/source/meters.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/alarms.inc` & `ceilometer-9.0.7/api-ref/source/alarms.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/resources-list-response.json` & `ceilometer-9.0.7/api-ref/source/samples/resources-list-response.json`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/sample-show-response.json` & `ceilometer-9.0.7/api-ref/source/samples/sample-show-response.json`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/resources-list-response.xml` & `ceilometer-9.0.7/api-ref/source/samples/resources-list-response.xml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/alarms-list-response.xml` & `ceilometer-9.0.7/api-ref/source/samples/alarms-list-response.xml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/alarms-list-response.json` & `ceilometer-9.0.7/api-ref/source/samples/alarms-list-response.json`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/capabilities-list-response.xml` & `ceilometer-9.0.7/api-ref/source/samples/capabilities-list-response.xml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/samples-list-response.json` & `ceilometer-9.0.7/api-ref/source/samples/samples-list-response.json`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/sample-create-request.xml` & `ceilometer-9.0.7/api-ref/source/samples/sample-create-request.xml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/alarm-show-response.json` & `ceilometer-9.0.7/api-ref/source/samples/alarm-show-response.json`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/sample-show-response.xml` & `ceilometer-9.0.7/api-ref/source/samples/sample-show-response.xml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/sample-create-request.json` & `ceilometer-9.0.7/api-ref/source/samples/sample-create-request.json`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/resource-show-response.xml` & `ceilometer-9.0.7/api-ref/source/samples/resource-show-response.xml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/samples-list-response.xml` & `ceilometer-9.0.7/api-ref/source/samples/samples-list-response.xml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/alarm-show-response.xml` & `ceilometer-9.0.7/api-ref/source/samples/alarm-show-response.xml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/capabilities-list-response.json` & `ceilometer-9.0.7/api-ref/source/samples/capabilities-list-response.json`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples/resource-show-response.json` & `ceilometer-9.0.7/api-ref/source/samples/resource-show-response.json`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/samples.inc` & `ceilometer-9.0.7/api-ref/source/samples.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/parameters.yaml` & `ceilometer-9.0.7/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/events.inc` & `ceilometer-9.0.7/api-ref/source/events.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/capabilities.inc` & `ceilometer-9.0.7/api-ref/source/capabilities.inc`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/api-ref/source/conf.py` & `ceilometer-9.0.7/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/tools/make_test_data.py` & `ceilometer-9.0.7/tools/make_test_data.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/tools/migrate_data_to_gnocchi.py` & `ceilometer-9.0.7/tools/migrate_data_to_gnocchi.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/tools/make_test_data.sh` & `ceilometer-9.0.7/tools/make_test_data.sh`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/tools/send_test_data.py` & `ceilometer-9.0.7/tools/send_test_data.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/meter/notifications.py` & `ceilometer-9.0.7/ceilometer/meter/notifications.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/notification.py` & `ceilometer-9.0.7/ceilometer/notification.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/keystone_client.py` & `ceilometer-9.0.7/ceilometer/keystone_client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/dispatcher/gnocchi_opts.py` & `ceilometer-9.0.7/ceilometer/dispatcher/gnocchi_opts.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/dispatcher/http.py` & `ceilometer-9.0.7/ceilometer/dispatcher/http.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/dispatcher/data/gnocchi_resources.yaml` & `ceilometer-9.0.7/ceilometer/dispatcher/data/gnocchi_resources.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/dispatcher/file.py` & `ceilometer-9.0.7/ceilometer/dispatcher/file.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/dispatcher/database.py` & `ceilometer-9.0.7/ceilometer/dispatcher/database.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/dispatcher/__init__.py` & `ceilometer-9.0.7/ceilometer/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/dispatcher/gnocchi.py` & `ceilometer-9.0.7/ceilometer/dispatcher/gnocchi.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/objectstore/swift.py` & `ceilometer-9.0.7/ceilometer/objectstore/swift.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/objectstore/rgw.py` & `ceilometer-9.0.7/ceilometer/objectstore/rgw.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/objectstore/rgw_client.py` & `ceilometer-9.0.7/ceilometer/objectstore/rgw_client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/discovery.py` & `ceilometer-9.0.7/ceilometer/compute/discovery.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/pollsters/disk.py` & `ceilometer-9.0.7/ceilometer/compute/pollsters/disk.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/pollsters/net.py` & `ceilometer-9.0.7/ceilometer/compute/pollsters/net.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/pollsters/instance_stats.py` & `ceilometer-9.0.7/ceilometer/compute/pollsters/instance_stats.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/pollsters/__init__.py` & `ceilometer-9.0.7/ceilometer/compute/pollsters/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/pollsters/util.py` & `ceilometer-9.0.7/ceilometer/compute/pollsters/util.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/virt/hyperv/inspector.py` & `ceilometer-9.0.7/ceilometer/compute/virt/hyperv/inspector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/virt/vmware/vsphere_operations.py` & `ceilometer-9.0.7/ceilometer/compute/virt/vmware/vsphere_operations.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/virt/vmware/inspector.py` & `ceilometer-9.0.7/ceilometer/compute/virt/vmware/inspector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/virt/xenapi/inspector.py` & `ceilometer-9.0.7/ceilometer/compute/virt/xenapi/inspector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/virt/libvirt/utils.py` & `ceilometer-9.0.7/ceilometer/compute/virt/libvirt/utils.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/virt/libvirt/inspector.py` & `ceilometer-9.0.7/ceilometer/compute/virt/libvirt/inspector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/compute/virt/inspector.py` & `ceilometer-9.0.7/ceilometer/compute/virt/inspector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/opts.py` & `ceilometer-9.0.7/ceilometer/opts.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/ipmi/platform/ipmitool.py` & `ceilometer-9.0.7/ceilometer/ipmi/platform/ipmitool.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/ipmi/platform/intel_node_manager.py` & `ceilometer-9.0.7/ceilometer/ipmi/platform/intel_node_manager.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/ipmi/platform/ipmi_sensor.py` & `ceilometer-9.0.7/ceilometer/ipmi/platform/ipmi_sensor.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/ipmi/platform/exception.py` & `ceilometer-9.0.7/ceilometer/ipmi/platform/exception.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/ipmi/notifications/ironic.py` & `ceilometer-9.0.7/ceilometer/ipmi/notifications/ironic.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/ipmi/pollsters/node.py` & `ceilometer-9.0.7/ceilometer/ipmi/pollsters/node.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/ipmi/pollsters/__init__.py` & `ceilometer-9.0.7/ceilometer/ipmi/pollsters/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/ipmi/pollsters/sensor.py` & `ceilometer-9.0.7/ceilometer/ipmi/pollsters/sensor.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/collector.py` & `ceilometer-9.0.7/ceilometer/collector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/conf/defaults.py` & `ceilometer-9.0.7/ceilometer/conf/defaults.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/i18n.py` & `ceilometer-9.0.7/ceilometer/i18n.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/pipeline/data/event_definitions.yaml` & `ceilometer-9.0.7/ceilometer/pipeline/data/event_definitions.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/pipeline/data/pipeline.yaml` & `ceilometer-9.0.7/ceilometer/pipeline/data/pipeline.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/telemetry/notifications.py` & `ceilometer-9.0.7/ceilometer/telemetry/notifications.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/data/meters.d/meters.yaml` & `ceilometer-9.0.7/ceilometer/data/meters.d/meters.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/publisher/http.py` & `ceilometer-9.0.7/ceilometer/publisher/http.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/publisher/kafka_broker.py` & `ceilometer-9.0.7/ceilometer/publisher/kafka_broker.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/publisher/file.py` & `ceilometer-9.0.7/ceilometer/publisher/file.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/publisher/zaqar.py` & `ceilometer-9.0.7/ceilometer/publisher/zaqar.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/publisher/test.py` & `ceilometer-9.0.7/ceilometer/publisher/test.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/publisher/udp.py` & `ceilometer-9.0.7/ceilometer/publisher/udp.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/publisher/__init__.py` & `ceilometer-9.0.7/ceilometer/publisher/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/publisher/direct.py` & `ceilometer-9.0.7/ceilometer/publisher/direct.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/publisher/utils.py` & `ceilometer-9.0.7/ceilometer/publisher/utils.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/publisher/messaging.py` & `ceilometer-9.0.7/ceilometer/publisher/messaging.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/volume/discovery.py` & `ceilometer-9.0.7/ceilometer/volume/discovery.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/volume/cinder.py` & `ceilometer-9.0.7/ceilometer/volume/cinder.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/gnocchi_client.py` & `ceilometer-9.0.7/ceilometer/gnocchi_client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/declarative.py` & `ceilometer-9.0.7/ceilometer/declarative.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/hardware/discovery.py` & `ceilometer-9.0.7/ceilometer/hardware/discovery.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/hardware/pollsters/generic.py` & `ceilometer-9.0.7/ceilometer/hardware/pollsters/generic.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/hardware/pollsters/data/snmp.yaml` & `ceilometer-9.0.7/ceilometer/hardware/pollsters/data/snmp.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/hardware/pollsters/util.py` & `ceilometer-9.0.7/ceilometer/hardware/pollsters/util.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/hardware/inspector/base.py` & `ceilometer-9.0.7/ceilometer/hardware/inspector/base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/hardware/inspector/snmp.py` & `ceilometer-9.0.7/ceilometer/hardware/inspector/snmp.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/hardware/inspector/__init__.py` & `ceilometer-9.0.7/ceilometer/hardware/inspector/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/middleware.py` & `ceilometer-9.0.7/ceilometer/middleware.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/cmd/collector.py` & `ceilometer-9.0.7/ceilometer/cmd/collector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/cmd/agent_notification.py` & `ceilometer-9.0.7/ceilometer/cmd/agent_notification.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/cmd/api.py` & `ceilometer-9.0.7/ceilometer/cmd/api.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/cmd/polling.py` & `ceilometer-9.0.7/ceilometer/cmd/polling.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/cmd/storage.py` & `ceilometer-9.0.7/ceilometer/cmd/storage.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/cmd/sample.py` & `ceilometer-9.0.7/ceilometer/cmd/sample.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/nova_client.py` & `ceilometer-9.0.7/ceilometer/nova_client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/service.py` & `ceilometer-9.0.7/ceilometer/service.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/impl_mongodb.py` & `ceilometer-9.0.7/ceilometer/storage/impl_mongodb.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/impl_log.py` & `ceilometer-9.0.7/ceilometer/storage/impl_log.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/mongo/utils.py` & `ceilometer-9.0.7/ceilometer/storage/mongo/utils.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/base.py` & `ceilometer-9.0.7/ceilometer/storage/base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/pymongo_base.py` & `ceilometer-9.0.7/ceilometer/storage/pymongo_base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/impl_hbase.py` & `ceilometer-9.0.7/ceilometer/storage/impl_hbase.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migration.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migration.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/migrate.cfg` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/migrate.cfg`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/009_event_strings.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/009_event_strings.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/004_add_counter_unit.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/004_add_counter_unit.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/023_add_trait_types.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/023_add_trait_types.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/001_add_meter_table.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/001_add_meter_table.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/006_counter_volume_is_float.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/006_counter_volume_is_float.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/023_sqlite_upgrade.sql` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/023_sqlite_upgrade.sql`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/015_add_alarm_history_table.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/015_add_alarm_history_table.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/034_drop_dump_tables.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/034_drop_dump_tables.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/010_add_index_to_meter.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/010_add_index_to_meter.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/025_alarm_use_floatingprecision.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/025_alarm_use_floatingprecision.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/005_remove_resource_timestamp.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/005_remove_resource_timestamp.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/014_add_event_message_id.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/014_add_event_message_id.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/003_set_utf8_charset.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/003_set_utf8_charset.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/021_add_event_types.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/021_add_event_types.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/019_alarm_history_detail_is_text.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/019_alarm_history_detail_is_text.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/028_alembic_migrations.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/028_alembic_migrations.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/030_rename_meter_table.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/030_rename_meter_table.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/024_event_use_floatingprecision.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/024_event_use_floatingprecision.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/045_add_resource_metadatahash_index.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/045_add_resource_metadatahash_index.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/027_remove_alarm_fk_constraints.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/027_remove_alarm_fk_constraints.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/020_add_metadata_tables.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/020_add_metadata_tables.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/016_simpler_alarm.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/016_simpler_alarm.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/041_expand_event_traits.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/041_expand_event_traits.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/011_indexes_cleanup.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/011_indexes_cleanup.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/022_metadata_int_is_bigint.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/022_metadata_int_is_bigint.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/039_event_floatingprecision_pgsql.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/039_event_floatingprecision_pgsql.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/044_restore_long_uuid_data_types.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/044_restore_long_uuid_data_types.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/017_convert_timestamp_as_datetime_to_decimal.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/017_convert_timestamp_as_datetime_to_decimal.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/037_sample_index_cleanup.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/037_sample_index_cleanup.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/042_add_raw_column.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/042_add_raw_column.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/038_normalise_tables.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/038_normalise_tables.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/032_add_alarm_time_constraints.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/032_add_alarm_time_constraints.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/007_add_alarm_table.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/007_add_alarm_table.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/002_remove_duration.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/002_remove_duration.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/029_sample_recorded_at.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/029_sample_recorded_at.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/036_drop_sourceassoc_resource_tables.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/036_drop_sourceassoc_resource_tables.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/040_add_alarm_severity.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/040_add_alarm_severity.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/012_add_missing_foreign_keys.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/012_add_missing_foreign_keys.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/043_reduce_uuid_data_types.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/043_reduce_uuid_data_types.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/021_sqlite_upgrade.sql` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/021_sqlite_upgrade.sql`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/008_add_events.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/008_add_events.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/018_resource_resource_metadata_is_text.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/018_resource_resource_metadata_is_text.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/026_float_size.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/026_float_size.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/033_alarm_id_rename.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/033_alarm_id_rename.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/031_add_new_meter_table.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/031_add_new_meter_table.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/013_rename_counter_to_meter_alarm.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/013_rename_counter_to_meter_alarm.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/migrate_repo/versions/035_drop_user_project_tables.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/migrate_repo/versions/035_drop_user_project_tables.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/utils.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/utils.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/sqlalchemy/models.py` & `ceilometer-9.0.7/ceilometer/storage/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/impl_sqlalchemy.py` & `ceilometer-9.0.7/ceilometer/storage/impl_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/__init__.py` & `ceilometer-9.0.7/ceilometer/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/hbase/inmemory.py` & `ceilometer-9.0.7/ceilometer/storage/hbase/inmemory.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/hbase/base.py` & `ceilometer-9.0.7/ceilometer/storage/hbase/base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/hbase/migration.py` & `ceilometer-9.0.7/ceilometer/storage/hbase/migration.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/hbase/utils.py` & `ceilometer-9.0.7/ceilometer/storage/hbase/utils.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/storage/models.py` & `ceilometer-9.0.7/ceilometer/storage/models.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/__init__.py` & `ceilometer-9.0.7/ceilometer/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/image/glance.py` & `ceilometer-9.0.7/ceilometer/image/glance.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/image/discovery.py` & `ceilometer-9.0.7/ceilometer/image/discovery.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/services/vpnaas.py` & `ceilometer-9.0.7/ceilometer/network/services/vpnaas.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/services/discovery.py` & `ceilometer-9.0.7/ceilometer/network/services/discovery.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/services/base.py` & `ceilometer-9.0.7/ceilometer/network/services/base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/services/lbaas.py` & `ceilometer-9.0.7/ceilometer/network/services/lbaas.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/services/fwaas.py` & `ceilometer-9.0.7/ceilometer/network/services/fwaas.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/driver.py` & `ceilometer-9.0.7/ceilometer/network/statistics/driver.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/port_v2.py` & `ceilometer-9.0.7/ceilometer/network/statistics/port_v2.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/opencontrail/driver.py` & `ceilometer-9.0.7/ceilometer/network/statistics/opencontrail/driver.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/opencontrail/client.py` & `ceilometer-9.0.7/ceilometer/network/statistics/opencontrail/client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/flow.py` & `ceilometer-9.0.7/ceilometer/network/statistics/flow.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/switch.py` & `ceilometer-9.0.7/ceilometer/network/statistics/switch.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/opendaylight/driver.py` & `ceilometer-9.0.7/ceilometer/network/statistics/opendaylight/driver.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/opendaylight/client.py` & `ceilometer-9.0.7/ceilometer/network/statistics/opendaylight/client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/__init__.py` & `ceilometer-9.0.7/ceilometer/network/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/port.py` & `ceilometer-9.0.7/ceilometer/network/statistics/port.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/statistics/table.py` & `ceilometer-9.0.7/ceilometer/network/statistics/table.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/network/floatingip.py` & `ceilometer-9.0.7/ceilometer/network/floatingip.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/hooks.py` & `ceilometer-9.0.7/ceilometer/api/hooks.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/app.py` & `ceilometer-9.0.7/ceilometer/api/app.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/app.wsgi` & `ceilometer-9.0.7/ceilometer/api/app.wsgi`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/middleware.py` & `ceilometer-9.0.7/ceilometer/api/middleware.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/rbac.py` & `ceilometer-9.0.7/ceilometer/api/rbac.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/controllers/v2/base.py` & `ceilometer-9.0.7/ceilometer/api/controllers/v2/base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/controllers/v2/root.py` & `ceilometer-9.0.7/ceilometer/api/controllers/v2/root.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/controllers/v2/meters.py` & `ceilometer-9.0.7/ceilometer/api/controllers/v2/meters.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/controllers/v2/capabilities.py` & `ceilometer-9.0.7/ceilometer/api/controllers/v2/capabilities.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/controllers/v2/resources.py` & `ceilometer-9.0.7/ceilometer/api/controllers/v2/resources.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/controllers/v2/utils.py` & `ceilometer-9.0.7/ceilometer/api/controllers/v2/utils.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/controllers/v2/query.py` & `ceilometer-9.0.7/ceilometer/api/controllers/v2/query.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/controllers/v2/samples.py` & `ceilometer-9.0.7/ceilometer/api/controllers/v2/samples.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/api/controllers/root.py` & `ceilometer-9.0.7/ceilometer/api/controllers/root.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/event/endpoint.py` & `ceilometer-9.0.7/ceilometer/event/endpoint.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/event/storage/models.py` & `ceilometer-9.0.7/ceilometer/event/storage/models.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/event/converter.py` & `ceilometer-9.0.7/ceilometer/event/converter.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/event/trait_plugins.py` & `ceilometer-9.0.7/ceilometer/event/trait_plugins.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/neutron_client.py` & `ceilometer-9.0.7/ceilometer/neutron_client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/utils.py` & `ceilometer-9.0.7/ceilometer/utils.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/version.py` & `ceilometer-9.0.7/ceilometer/version.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/exchange_control.py` & `ceilometer-9.0.7/ceilometer/exchange_control.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/transformer/accumulator.py` & `ceilometer-9.0.7/ceilometer/transformer/accumulator.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/transformer/__init__.py` & `ceilometer-9.0.7/ceilometer/transformer/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/transformer/conversions.py` & `ceilometer-9.0.7/ceilometer/transformer/conversions.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/transformer/arithmetic.py` & `ceilometer-9.0.7/ceilometer/transformer/arithmetic.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-error.po` & `ceilometer-9.0.7/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-error.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-warning.po` & `ceilometer-9.0.7/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-warning.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer.po` & `ceilometer-9.0.7/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-info.po` & `ceilometer-9.0.7/ceilometer/locale/ko_KR/LC_MESSAGES/ceilometer-log-info.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/ru/LC_MESSAGES/ceilometer.po` & `ceilometer-9.0.7/ceilometer/locale/ru/LC_MESSAGES/ceilometer.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/zh_CN/LC_MESSAGES/ceilometer.po` & `ceilometer-9.0.7/ceilometer/locale/zh_CN/LC_MESSAGES/ceilometer.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/fr/LC_MESSAGES/ceilometer.po` & `ceilometer-9.0.7/ceilometer/locale/fr/LC_MESSAGES/ceilometer.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/es/LC_MESSAGES/ceilometer-log-error.po` & `ceilometer-9.0.7/ceilometer/locale/es/LC_MESSAGES/ceilometer-log-error.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/es/LC_MESSAGES/ceilometer.po` & `ceilometer-9.0.7/ceilometer/locale/es/LC_MESSAGES/ceilometer.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/es/LC_MESSAGES/ceilometer-log-info.po` & `ceilometer-9.0.7/ceilometer/locale/es/LC_MESSAGES/ceilometer-log-info.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/pt_BR/LC_MESSAGES/ceilometer.po` & `ceilometer-9.0.7/ceilometer/locale/pt_BR/LC_MESSAGES/ceilometer.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/zh_TW/LC_MESSAGES/ceilometer.po` & `ceilometer-9.0.7/ceilometer/locale/zh_TW/LC_MESSAGES/ceilometer.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/it/LC_MESSAGES/ceilometer.po` & `ceilometer-9.0.7/ceilometer/locale/it/LC_MESSAGES/ceilometer.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/ja/LC_MESSAGES/ceilometer.po` & `ceilometer-9.0.7/ceilometer/locale/ja/LC_MESSAGES/ceilometer.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-error.po` & `ceilometer-9.0.7/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-error.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-warning.po` & `ceilometer-9.0.7/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-warning.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/de/LC_MESSAGES/ceilometer.po` & `ceilometer-9.0.7/ceilometer/locale/de/LC_MESSAGES/ceilometer.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-info.po` & `ceilometer-9.0.7/ceilometer/locale/de/LC_MESSAGES/ceilometer-log-info.po`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/messaging.py` & `ceilometer-9.0.7/ceilometer/messaging.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/hacking/checks.py` & `ceilometer-9.0.7/ceilometer/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/pipeline.py` & `ceilometer-9.0.7/ceilometer/pipeline.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/agent/discovery/endpoint.py` & `ceilometer-9.0.7/ceilometer/agent/discovery/endpoint.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/agent/discovery/localnode.py` & `ceilometer-9.0.7/ceilometer/agent/discovery/localnode.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/agent/discovery/tenant.py` & `ceilometer-9.0.7/ceilometer/agent/discovery/tenant.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/agent/plugin_base.py` & `ceilometer-9.0.7/ceilometer/agent/plugin_base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/agent/manager.py` & `ceilometer-9.0.7/ceilometer/agent/manager.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/sample.py` & `ceilometer-9.0.7/ceilometer/sample.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/integration/gabbi/gabbits-live/create_stack.json` & `ceilometer-9.0.7/ceilometer/tests/integration/gabbi/gabbits-live/create_stack.json`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/integration/gabbi/gabbits-live/autoscaling.yaml` & `ceilometer-9.0.7/ceilometer/tests/integration/gabbi/gabbits-live/autoscaling.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/integration/gabbi/gabbits-live/aodh-gnocchi-threshold-alarm.yaml` & `ceilometer-9.0.7/ceilometer/tests/integration/gabbi/gabbits-live/aodh-gnocchi-threshold-alarm.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/integration/gabbi/gabbits-live/update_stack.json` & `ceilometer-9.0.7/ceilometer/tests/integration/gabbi/gabbits-live/update_stack.json`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/integration/gabbi/test_gabbi_live.py` & `ceilometer-9.0.7/ceilometer/tests/integration/gabbi/test_gabbi_live.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/integration/hooks/post_test_hook.sh` & `ceilometer-9.0.7/ceilometer/tests/integration/hooks/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/base.py` & `ceilometer-9.0.7/ceilometer/tests/base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/meter/test_notifications.py` & `ceilometer-9.0.7/ceilometer/tests/unit/meter/test_notifications.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/meter/test_meter_plugins.py` & `ceilometer-9.0.7/ceilometer/tests/unit/meter/test_meter_plugins.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_neutronclient_lbaas_v2.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_neutronclient_lbaas_v2.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/test_file.py` & `ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/test_file.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/test_gnocchi.py` & `ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/test_gnocchi.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/test_dispatcher.py` & `ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/test_db.py` & `ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/test_db.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/dispatcher/test_http.py` & `ceilometer-9.0.7/ceilometer/tests/unit/dispatcher/test_http.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/objectstore/test_swift.py` & `ceilometer-9.0.7/ceilometer/tests/unit/objectstore/test_swift.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/objectstore/test_rgw.py` & `ceilometer-9.0.7/ceilometer/tests/unit/objectstore/test_rgw.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/objectstore/test_rgw_client.py` & `ceilometer-9.0.7/ceilometer/tests/unit/objectstore/test_rgw_client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/base.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_perf.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_perf.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_cpu.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_cpu.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_memory.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_memory.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_net.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_net.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_diskio.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_diskio.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/pollsters/test_location_metadata.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/pollsters/test_location_metadata.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/hyperv/test_inspector.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/hyperv/test_inspector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/vmware/test_inspector.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/vmware/test_inspector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/vmware/test_vsphere_operations.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/vmware/test_vsphere_operations.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/xenapi/test_inspector.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/xenapi/test_inspector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/virt/libvirt/test_inspector.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/virt/libvirt/test_inspector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/compute/test_discovery.py` & `ceilometer-9.0.7/ceilometer/tests/unit/compute/test_discovery.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_declarative.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_declarative.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_messaging.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_messaging.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/ipmi/platform/fake_utils.py` & `ceilometer-9.0.7/ceilometer/tests/unit/ipmi/platform/fake_utils.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/ipmi/platform/ipmitool_test_data.py` & `ceilometer-9.0.7/ceilometer/tests/unit/ipmi/platform/ipmitool_test_data.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/ipmi/platform/test_ipmi_sensor.py` & `ceilometer-9.0.7/ceilometer/tests/unit/ipmi/platform/test_ipmi_sensor.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/ipmi/platform/test_intel_node_manager.py` & `ceilometer-9.0.7/ceilometer/tests/unit/ipmi/platform/test_intel_node_manager.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/ipmi/notifications/ipmi_test_data.py` & `ceilometer-9.0.7/ceilometer/tests/unit/ipmi/notifications/ipmi_test_data.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/ipmi/notifications/test_ironic.py` & `ceilometer-9.0.7/ceilometer/tests/unit/ipmi/notifications/test_ironic.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/ipmi/pollsters/base.py` & `ceilometer-9.0.7/ceilometer/tests/unit/ipmi/pollsters/base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/ipmi/pollsters/test_node.py` & `ceilometer-9.0.7/ceilometer/tests/unit/ipmi/pollsters/test_node.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/ipmi/pollsters/test_sensor.py` & `ceilometer-9.0.7/ceilometer/tests/unit/ipmi/pollsters/test_sensor.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/telemetry/test_notifications.py` & `ceilometer-9.0.7/ceilometer/tests/unit/telemetry/test_notifications.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_messaging_publisher.py` & `ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_messaging_publisher.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_kafka_broker_publisher.py` & `ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_kafka_broker_publisher.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_file.py` & `ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_file.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_utils.py` & `ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_utils.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_zaqar.py` & `ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_zaqar.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_udp.py` & `ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_udp.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/publisher/test_http.py` & `ceilometer-9.0.7/ceilometer/tests/unit/publisher/test_http.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_collector.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_collector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_utils.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/volume/test_cinder.py` & `ceilometer-9.0.7/ceilometer/tests/unit/volume/test_cinder.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_neutronclient.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_neutronclient.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/hardware/pollsters/test_util.py` & `ceilometer-9.0.7/ceilometer/tests/unit/hardware/pollsters/test_util.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/hardware/pollsters/test_generic.py` & `ceilometer-9.0.7/ceilometer/tests/unit/hardware/pollsters/test_generic.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/hardware/inspector/test_inspector.py` & `ceilometer-9.0.7/ceilometer/tests/unit/hardware/inspector/test_inspector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/hardware/inspector/test_snmp.py` & `ceilometer-9.0.7/ceilometer/tests/unit/hardware/inspector/test_snmp.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_event_pipeline.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_event_pipeline.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/pipeline_base.py` & `ceilometer-9.0.7/ceilometer/tests/unit/pipeline_base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/storage/test_get_connection.py` & `ceilometer-9.0.7/ceilometer/tests/unit/storage/test_get_connection.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/storage/sqlalchemy/test_models.py` & `ceilometer-9.0.7/ceilometer/tests/unit/storage/sqlalchemy/test_models.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/storage/test_base.py` & `ceilometer-9.0.7/ceilometer/tests/unit/storage/test_base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/image/test_glance.py` & `ceilometer-9.0.7/ceilometer/tests/unit/image/test_glance.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/services/test_vpnaas.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/services/test_vpnaas.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/services/test_lbaas.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/services/test_lbaas.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/services/test_lbaas_v2.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/services/test_lbaas_v2.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/services/test_fwaas.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/services/test_fwaas.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/test_floating_ip.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/test_floating_ip.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_flow.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_flow.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_port.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_port.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_table.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_table.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_switch.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_switch.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opencontrail/test_driver.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opencontrail/test_driver.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opencontrail/test_client.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opencontrail/test_client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_statistics.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_statistics.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/test_port_v2.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/test_port_v2.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opendaylight/test_driver.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opendaylight/test_driver.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/opendaylight/test_client.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/opendaylight/test_client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/network/statistics/__init__.py` & `ceilometer-9.0.7/ceilometer/tests/unit/network/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/api/v2/test_query.py` & `ceilometer-9.0.7/ceilometer/tests/unit/api/v2/test_query.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/api/v2/test_statistics.py` & `ceilometer-9.0.7/ceilometer/tests/unit/api/v2/test_statistics.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/api/v2/test_complex_query.py` & `ceilometer-9.0.7/ceilometer/tests/unit/api/v2/test_complex_query.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/api/test_hooks.py` & `ceilometer-9.0.7/ceilometer/tests/unit/api/test_hooks.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/api/test_app.py` & `ceilometer-9.0.7/ceilometer/tests/unit/api/test_app.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/event/test_converter.py` & `ceilometer-9.0.7/ceilometer/tests/unit/event/test_converter.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/event/test_endpoint.py` & `ceilometer-9.0.7/ceilometer/tests/unit/event/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/event/test_trait_plugins.py` & `ceilometer-9.0.7/ceilometer/tests/unit/event/test_trait_plugins.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_sample.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_sample.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_middleware.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_middleware.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/transformer/test_conversions.py` & `ceilometer-9.0.7/ceilometer/tests/unit/transformer/test_conversions.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_decoupled_pipeline.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_decoupled_pipeline.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_novaclient.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_novaclient.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/agent/test_manager.py` & `ceilometer-9.0.7/ceilometer/tests/unit/agent/test_manager.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/agent/agentbase.py` & `ceilometer-9.0.7/ceilometer/tests/unit/agent/agentbase.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/agent/test_discovery.py` & `ceilometer-9.0.7/ceilometer/tests/unit/agent/test_discovery.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/unit/test_polling.py` & `ceilometer-9.0.7/ceilometer/tests/unit/test_polling.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/db.py` & `ceilometer-9.0.7/ceilometer/tests/db.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/publisher/test_direct.py` & `ceilometer-9.0.7/ceilometer/tests/functional/publisher/test_direct.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/test_collector.py` & `ceilometer-9.0.7/ceilometer/tests/functional/test_collector.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits_prefix/basic.yaml` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits_prefix/basic.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits_prefix/resources-fixtured.yaml` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits_prefix/resources-fixtured.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits_prefix/clean-samples.yaml` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits_prefix/clean-samples.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/test_gabbi_prefix.py` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/test_gabbi_prefix.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/samples.yaml` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/samples.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/resources-empty.yaml` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/resources-empty.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/middleware.yaml` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/middleware.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/basic.yaml` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/basic.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/meters.yaml` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/meters.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/resources-fixtured.yaml` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/resources-fixtured.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbits/clean-samples.yaml` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbits/clean-samples.yaml`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/test_gabbi.py` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/test_gabbi.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/fixtures.py` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/fixtures.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/gabbi/gabbi_paste.ini` & `ceilometer-9.0.7/ceilometer/tests/functional/gabbi/gabbi_paste.ini`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/hooks/post_test_hook.sh` & `ceilometer-9.0.7/ceilometer/tests/functional/hooks/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/test_bin.py` & `ceilometer-9.0.7/ceilometer/tests/functional/test_bin.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/storage/test_storage_scenarios.py` & `ceilometer-9.0.7/ceilometer/tests/functional/storage/test_storage_scenarios.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/storage/test_impl_mongodb.py` & `ceilometer-9.0.7/ceilometer/tests/functional/storage/test_impl_mongodb.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/storage/test_impl_hbase.py` & `ceilometer-9.0.7/ceilometer/tests/functional/storage/test_impl_hbase.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/storage/test_impl_sqlalchemy.py` & `ceilometer-9.0.7/ceilometer/tests/functional/storage/test_impl_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/storage/test_pymongo_base.py` & `ceilometer-9.0.7/ceilometer/tests/functional/storage/test_pymongo_base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/storage/test_impl_log.py` & `ceilometer-9.0.7/ceilometer/tests/functional/storage/test_impl_log.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_versions.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_versions.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_statistics_scenarios.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_statistics_scenarios.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_complex_query_scenarios.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_complex_query_scenarios.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_compute_duration_by_resource_scenarios.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_compute_duration_by_resource_scenarios.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_list_resources_scenarios.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_list_resources_scenarios.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_api_upgrade.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_api_upgrade.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_capabilities.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_post_samples_scenarios.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_post_samples_scenarios.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/__init__.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_acl_scenarios.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_acl_scenarios.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_app.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_app.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_list_samples_scenarios.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_list_samples_scenarios.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/v2/test_list_meters_scenarios.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/v2/test_list_meters_scenarios.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/api/__init__.py` & `ceilometer-9.0.7/ceilometer/tests/functional/api/__init__.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/functional/test_notification.py` & `ceilometer-9.0.7/ceilometer/tests/functional/test_notification.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/tempest/scenario/test_telemetry_integration.py` & `ceilometer-9.0.7/ceilometer/tests/tempest/scenario/test_telemetry_integration.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/tempest/scenario/test_object_storage_telemetry_middleware.py` & `ceilometer-9.0.7/ceilometer/tests/tempest/scenario/test_object_storage_telemetry_middleware.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/tempest/config.py` & `ceilometer-9.0.7/ceilometer/tests/tempest/config.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/tempest/plugin.py` & `ceilometer-9.0.7/ceilometer/tests/tempest/plugin.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/tempest/service/client.py` & `ceilometer-9.0.7/ceilometer/tests/tempest/service/client.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/tempest/api/base.py` & `ceilometer-9.0.7/ceilometer/tests/tempest/api/base.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/tempest/api/test_telemetry_notification_api.py` & `ceilometer-9.0.7/ceilometer/tests/tempest/api/test_telemetry_notification_api.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/tempest/exceptions.py` & `ceilometer-9.0.7/ceilometer/tests/tempest/exceptions.py`

 * *Files identical despite different names*

### Comparing `ceilometer-9.0.6/ceilometer/tests/mocks.py` & `ceilometer-9.0.7/ceilometer/tests/mocks.py`

 * *Files identical despite different names*

