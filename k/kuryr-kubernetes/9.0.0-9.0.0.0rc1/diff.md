# Comparing `tmp/kuryr-kubernetes-9.0.0.tar.gz` & `tmp/kuryr-kubernetes-9.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuryr-kubernetes-9.0.0.tar", last modified: Wed Oct  4 11:08:46 2023, max compression
+gzip compressed data, was "kuryr-kubernetes-9.0.0.0rc1.tar", last modified: Fri Sep 15 14:26:20 2023, max compression
```

## Comparing `kuryr-kubernetes-9.0.0.tar` & `kuryr-kubernetes-9.0.0.0rc1.tar`

### file list

```diff
@@ -1,487 +1,487 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.732006 kuryr-kubernetes-9.0.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/.dockerignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/.pre-commit-config.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/.stestr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.639989 kuryr-kubernetes-9.0.0/.zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8802 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/.zuul.d/base.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5035 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/.zuul.d/k8s-np-e2e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/.zuul.d/nodesets.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1620 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/.zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8249 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/.zuul.d/tempest-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6291 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/.zuul.d/tempest-multinode-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5604 2023-10-04 11:08:46.000000 kuryr-kubernetes-9.0.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    60888 2023-10-04 11:08:46.000000 kuryr-kubernetes-9.0.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2365 2023-10-04 11:08:46.732006 kuryr-kubernetes-9.0.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1228 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/babel.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/cni.Dockerfile
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      581 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/cni_ds_init
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.639989 kuryr-kubernetes-9.0.0/contrib/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.643990 kuryr-kubernetes-9.0.0/contrib/devstack-heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/devstack-heat/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2930 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/devstack-heat/README.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8209 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/devstack-heat/devstack_heat.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.643990 kuryr-kubernetes-9.0.0/contrib/devstack-heat/hot/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3542 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/devstack-heat/hot/devstack_heat_template.yml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/devstack-heat/hot/distro_deps.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/devstack-heat/hot/networking_deployment.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6343 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/devstack-heat/hot/node.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/devstack-heat/hot/parameters.yml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.643990 kuryr-kubernetes-9.0.0/contrib/kubectl_plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/kubectl_plugins/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)  1865381 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/kubectl_plugins/kubectl_kuryr_plugin_1080.gif
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.647991 kuryr-kubernetes-9.0.0/contrib/kubectl_plugins/kuryr/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6378 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/kubectl_plugins/kuryr/kuryr
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/kubectl_plugins/kuryr/plugin.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.647991 kuryr-kubernetes-9.0.0/contrib/pools-management/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18565 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/pools-management/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6267 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/pools-management/subports.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      415 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/regenerate_controller_pod.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2694 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/regenerate_pod_resources_api.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/sctp_client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.627987 kuryr-kubernetes-9.0.0/contrib/testing/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.647991 kuryr-kubernetes-9.0.0/contrib/testing/container/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/testing/container/Dockerfile
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1104 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/testing/container/build.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/testing/container/hostname.c
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.647991 kuryr-kubernetes-9.0.0/contrib/vagrant/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3225 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/vagrant/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1553 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/vagrant/Vagrantfile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.647991 kuryr-kubernetes-9.0.0/contrib/vagrant/config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/vagrant/config/kuryr_rc
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1519 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/vagrant/devstack.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      512 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/contrib/vagrant/vagrant.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/controller.Dockerfile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.651991 kuryr-kubernetes-9.0.0/devstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.627987 kuryr-kubernetes-9.0.0/devstack/files/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.651991 kuryr-kubernetes-9.0.0/devstack/files/debs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/files/debs/kuryr-kubernetes
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.651991 kuryr-kubernetes-9.0.0/devstack/files/rpms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/files/rpms/kuryr-kubernetes
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.651991 kuryr-kubernetes-9.0.0/devstack/lib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6885 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/lib/kubernetes
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    59303 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/lib/kuryr_kubernetes
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8090 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/local.conf.ovs.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2314 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/local.conf.pod-in-vm.overcloud.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/local.conf.pod-in-vm.undercloud.ovn.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1604 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/local.conf.pod-in-vm.undercloud.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7686 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/local.conf.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1561 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/local.conf.worker.sample
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6260 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4364 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/devstack/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.651991 kuryr-kubernetes-9.0.0/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.655992 kuryr-kubernetes-9.0.0/doc/images/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   156783 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/controller_pipeline.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16165 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/create_network_policy_flow.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    74032 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/external_traffic_to_l7_router.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28274 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/fuxi_k8s_components.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64078 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/kuryr_k8s_components.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19764 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/kuryr_k8s_components.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   160802 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/kuryr_k8s_ingress_ctrl_flow_diagram.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   110459 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/kuryr_k8s_ingress_sw_components.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   123352 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/kuryr_k8s_ocp_route_ctrl_sw.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   117373 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/l7_routing_and_user_lb_neutron_entities.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   187600 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/lbaas_translation.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67092 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/net-policy.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   220449 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/pod_creation_flow_daemon.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    71366 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/pod_creation_flow_daemon.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    92990 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/service_creation_diagram.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   477823 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/service_creation_diagram.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11510 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/update_network_policy_on_pod_creation.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36189 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/images/vif_handler_drivers_design.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.659993 kuryr-kubernetes-9.0.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2678 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.659993 kuryr-kubernetes-9.0.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/contributor/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.659993 kuryr-kubernetes-9.0.0/doc/source/devref/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3847 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/annotation_project_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3392 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/health_manager.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5891 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/high_availability.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13015 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/kuryr_kubernetes_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2291 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/kuryr_kubernetes_versions.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16090 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/network_policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9513 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/port_manager.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6977 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/service_support.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4560 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/updating_pod_resources_api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5282 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/devref/vif_handler_drivers_design.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.663993 kuryr-kubernetes-9.0.0/doc/source/installation/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7155 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/containerized.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7749 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/default_configuration.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.663993 kuryr-kubernetes-9.0.0/doc/source/installation/devstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7051 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/devstack/basic.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2489 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/devstack/containerized.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/devstack/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5660 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/devstack/nested-dpdk.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/devstack/nested-macvlan.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3233 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/devstack/nested-vlan.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4149 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/devstack/ovn-octavia.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6646 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/devstack/ovn_support.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1300 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/devstack/ports-pool.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/https_kubernetes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16318 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/ipv6.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2081 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/listener_timeouts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10471 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/manual.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/multi_vif_with_npwg_spec.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4926 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/multiple_tenants.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5512 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/network_namespace.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10741 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/network_policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6028 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/ports-pool.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48019 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/services.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11539 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/testing_connectivity.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2911 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/testing_nested_connectivity.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11168 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/testing_sctp_services.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9112 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/testing_udp_services.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1844 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/trunk_ports.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3690 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/installation/upgrades.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1991 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/nested_vlan_mode.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/readme.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.631988 kuryr-kubernetes-9.0.0/doc/source/specs/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/doc/source/specs/pike/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3003 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/specs/pike/contrail_support.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8341 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/specs/pike/fuxi_kubernetes.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/doc/source/specs/queens/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22143 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/specs/queens/network_policy.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/doc/source/specs/rocky/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6200 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/specs/rocky/npwg_spec_support.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/doc/source/specs/stein/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7723 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/specs/stein/vhostuser.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/doc/source/usage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.631988 kuryr-kubernetes-9.0.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.631988 kuryr-kubernetes-9.0.0/etc/cni/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/etc/cni/net.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/etc/cni/net.d/10-kuryr.conflist
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/etc/cni/net.d/kuryr.conflist.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/etc/oslo-config-generator/kuryr.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/kubernetes_crds/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/kubernetes_crds/kuryr_crds/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7265 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kubernetes_crds/kuryr_crds/kuryrloadbalancer.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1489 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kubernetes_crds/kuryr_crds/kuryrnetwork.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4928 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kubernetes_crds/kuryr_crds/kuryrnetworkpolicy.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kubernetes_crds/kuryr_crds/kuryrport.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kubernetes_crds/network_attachment_definition_crd.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/kuryr_cni/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/README
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/go.mod
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8592 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/go.sum
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/kuryr_cni/hack/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      302 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/hack/build-go.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)       38 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/hack/update-deps.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.667994 kuryr-kubernetes-9.0.0/kuryr_cni/pkg/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6029 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/pkg/main.go
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/pkg/ovo.go
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.671995 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.631988 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.631988 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.671995 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/LICENSE
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.631988 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.671995 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/skel/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8254 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/skel/skel.go
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.671995 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.671995 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/020/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3106 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/020/types.go
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3343 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/args.go
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.671995 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/current/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6964 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/current/types.go
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5086 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/types.go
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.671995 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3070 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/utils/utils.go
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.671995 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1093 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/conf.go
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4285 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/plugin.go
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/reconcile.go
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2707 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/version.go
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_cni/vendor/modules.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.675996 kuryr-kubernetes-9.0.0/kuryr_kubernetes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3632 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/clients.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.679996 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/cni.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/daemon.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.679996 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/eventlet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/eventlet/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/eventlet/controller.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.683997 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/sanity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/sanity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3067 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/sanity/checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3562 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/sanity_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6653 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.683997 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5968 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.683997 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6107 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/bridge.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7838 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/dpdk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10170 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/nested.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4958 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/vhostuser.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.687998 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/daemon/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/daemon/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14888 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/daemon/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3300 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/daemon/watcher_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4714 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/handlers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5343 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2002 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/main.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.687998 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/plugins/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11356 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/plugins/k8s_cni_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2619 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/prometheus_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3515 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16461 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4204 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.687998 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.695999 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2501 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/annotation_project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27615 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2798 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/default_project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3231 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/default_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2154 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/default_subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4474 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/lb_public_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40512 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/lbaasv2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4660 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/multi_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9342 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/namespace_subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2974 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/nested_dpdk_vif.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7312 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/nested_macvlan_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2738 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/nested_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13230 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/nested_vlan_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    37116 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/network_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18358 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/network_policy_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6369 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/neutron_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7359 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/node_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6470 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/public_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26434 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    57382 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/vif_pool.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.700000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10478 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/kuryrnetwork.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4464 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/kuryrnetwork_population.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14639 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/kuryrnetworkpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20112 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/kuryrport.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18187 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/lbaas.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    40982 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/loadbalancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2673 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/machine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5545 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/namespace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3133 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/pipeline.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5123 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/pod_label.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2357 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9392 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/vif.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.700000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/managers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/managers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4385 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/managers/health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9232 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/managers/pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8039 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/managers/prometheus_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6939 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6757 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.700000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/__init__.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5373 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/asynchronous.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4405 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/dispatch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/health.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3720 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/k8s_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6126 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2514 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19459 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/k8s_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2056 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/linux_net_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.704001 kuryr-kubernetes-9.0.0/kuryr_kubernetes/objects/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/objects/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/objects/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/objects/fields.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5829 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/objects/lbaas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2459 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/objects/vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2521 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/opts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/os_vif_plug_noop.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15371 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/os_vif_util.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.704001 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6527 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/fake.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.708001 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.708001 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cmd/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.708001 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cmd/eventlet/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cmd/eventlet/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1247 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cmd/eventlet/test_controller.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cmd/test_daemon.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5125 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cmd/test_status.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.712002 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.712002 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12937 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/plugins/test_k8s_cni_registry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3673 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16787 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_binding.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2597 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_handlers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5394 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1671 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_main.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4499 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.712002 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.716003 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4960 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_annotation_project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4482 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3353 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_default_project.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_default_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3017 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_default_subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14674 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_lb_public_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    69826 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_lbaasv2.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7232 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_multi_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11367 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_namespace_subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8552 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_dpdk.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20672 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_macvlan_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5307 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29002 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_vlan_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29767 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_network_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25194 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_network_policy_security_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14332 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_neutron_vif.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19023 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_node_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6308 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_public_ip.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6189 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    73646 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_vif_pool.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.720004 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_fake_handler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17977 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetwork.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4702 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetwork_population.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3625 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetworkpolicy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33509 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrport.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15747 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_lbaas.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    29152 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_loadbalancer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3478 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_machine.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5501 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_namespace.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2816 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_pipeline.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5600 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_pod_label.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12980 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_vif.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.720004 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/managers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/managers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8029 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/managers/test_health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15312 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/managers/test_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6927 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/managers/test_prometheus_exporter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2372 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/test_service.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.720004 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6217 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_asynchronous.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4286 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_dispatch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_health.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_k8s_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_logging.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5345 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/kuryr_fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20696 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_k8s_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2850 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_linux_net_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2997 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_object.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3683 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_os_vif_plug_noop.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27709 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_os_vif_util.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21734 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12217 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_watcher.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28362 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9362 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes/watcher.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.679996 kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2365 2023-10-04 11:08:46.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17937 2023-10-04 11:08:46.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-04 11:08:46.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5658 2023-10-04 11:08:46.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-04 11:08:46.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-10-04 11:08:46.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2023-10-04 11:08:46.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-10-04 11:08:46.000000 kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.720004 kuryr-kubernetes-9.0.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/playbooks/copy-crio-logs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/playbooks/copy-k8s-logs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3242 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/playbooks/e2e-tests.patch
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/playbooks/get_amphora_tarball.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/playbooks/run_k8s_e2e_tests.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.635988 kuryr-kubernetes-9.0.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.728005 kuryr-kubernetes-9.0.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/active-passive-ha-cfbda8e6b527b48e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/add-tagging-ce56231f58bf7ad0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/bp-openshift-router-support-5f28108b39a2826f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/change-cni-daemon-default-port-e968a83fa1bf30b5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/changing-default-url-for-k8s-api-42c3b90183783291.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/cni-health-checks-d2b70f2f2551a9fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/containerization-2fba4dac5c097b19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/cri-o-support-ab7e810775754ea7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/deprecate-handlers-caching-9cdfd772aba9a7ce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/deprecate-non-daemonized-6dd2154238b1628c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/deprecate-sg-mode-option-96824c33335cd74b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/deprecate-worker-nodes-subnet-e452c84df5b5ed5c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/deprecate_lbaasv2-a524aedf5d3a36bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/drop-ingress-d78a7a9be8f20da1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/drop-py27-60f55b6bc1d082bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/fault-tolerable-watcher-24c51dbccabf5f17.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/golang-kuryr-cni-aab144831d4dc9dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/k8s-client-token-default-882ec49d1faffc29.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/kuryr-daemon-f09075b9eb60388f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/make-ext-subnet-optional-99e73bfcbde96c22.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/make-handlers-pluggable-844475484771ffd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/make-lbaas-timeout-configurable-8624ea32971c0cbe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/make-listener-timeouts-configurable-f563d85eg6c6fe6d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/multivif-pools-1cec757c77a8c4f8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/network-device-mtu-default-90faa7d685d4d0ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/network-namespace-2353f8013be398cd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/network-policy-support-on-services-without-selectors-fea06ab71a8a6f2a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/octavia-acls-7452d3406d75ea15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/oslo-caching-b11881cfb9dc306c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/remove-non-daemon-836e4825384b1b88.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/remove-physical-device-mapping-15d614b70c68fc73.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/remove-run-server-aca25a2d9d723dc7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/remove-sriov-5f44deb951264510.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/reusable-pool-drivers-00e7fdc1f4738441.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/started-using-reno-90dbe9da108ec5c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/stein-upgrade-226c8e7b735701ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/support-specify-project-by-namespace-annotation-18bc6eca729bff5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/svc-without-selectors-f36bab0883459b80.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/notes/zuul-v3-native-gates-4ed7698667a7b92e.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.732006 kuryr-kubernetes-9.0.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.732006 kuryr-kubernetes-9.0.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.732006 kuryr-kubernetes-9.0.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4743 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2023-10-04 11:08:17.000000 kuryr-kubernetes-9.0.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6885 2023-10-04 11:08:46.736007 kuryr-kubernetes-9.0.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.732006 kuryr-kubernetes-9.0.0/tools/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-04 11:08:46.732006 kuryr-kubernetes-9.0.0/tools/gate/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1183 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/tools/gate/copy_crio_logs.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3275 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/tools/gate/copy_k8s_logs.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1404 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/tools/generate_config_file_samples.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3345 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/tools/generate_k8s_resource_definitions.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2023-10-04 11:08:16.000000 kuryr-kubernetes-9.0.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.480026 kuryr-kubernetes-9.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       32 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/.dockerignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/.pre-commit-config.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/.stestr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.368025 kuryr-kubernetes-9.0.0.0rc1/.zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8802 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/.zuul.d/base.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5035 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/.zuul.d/k8s-np-e2e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/.zuul.d/nodesets.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1620 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/.zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8249 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/.zuul.d/tempest-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6291 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/.zuul.d/tempest-multinode-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5604 2023-09-15 14:26:19.000000 kuryr-kubernetes-9.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      639 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    60898 2023-09-15 14:26:19.000000 kuryr-kubernetes-9.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2370 2023-09-15 14:26:20.480026 kuryr-kubernetes-9.0.0.0rc1/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1228 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1522 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/cni.Dockerfile
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      581 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/cni_ds_init
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.368025 kuryr-kubernetes-9.0.0.0rc1/contrib/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.372025 kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2930 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/README.rst
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     8209 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/devstack_heat.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.372025 kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/hot/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3542 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/hot/devstack_heat_template.yml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/hot/distro_deps.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1954 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/hot/networking_deployment.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6343 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/hot/node.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/hot/parameters.yml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.372025 kuryr-kubernetes-9.0.0.0rc1/contrib/kubectl_plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      484 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/kubectl_plugins/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)  1865381 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/kubectl_plugins/kubectl_kuryr_plugin_1080.gif
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.376025 kuryr-kubernetes-9.0.0.0rc1/contrib/kubectl_plugins/kuryr/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     6378 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/kubectl_plugins/kuryr/kuryr
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      390 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/kubectl_plugins/kuryr/plugin.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.376025 kuryr-kubernetes-9.0.0.0rc1/contrib/pools-management/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18565 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/pools-management/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6267 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/pools-management/subports.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      415 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/regenerate_controller_pod.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2694 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/regenerate_pod_resources_api.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      978 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/sctp_client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.352024 kuryr-kubernetes-9.0.0.0rc1/contrib/testing/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.376025 kuryr-kubernetes-9.0.0.0rc1/contrib/testing/container/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/testing/container/Dockerfile
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1104 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/testing/container/build.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2735 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/testing/container/hostname.c
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.380025 kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3225 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1553 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/Vagrantfile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.380025 kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/config/kuryr_rc
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1519 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/devstack.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      512 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/vagrant.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/controller.Dockerfile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.380025 kuryr-kubernetes-9.0.0.0rc1/devstack/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.352024 kuryr-kubernetes-9.0.0.0rc1/devstack/files/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.380025 kuryr-kubernetes-9.0.0.0rc1/devstack/files/debs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/files/debs/kuryr-kubernetes
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.380025 kuryr-kubernetes-9.0.0.0rc1/devstack/files/rpms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/files/rpms/kuryr-kubernetes
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.384025 kuryr-kubernetes-9.0.0.0rc1/devstack/lib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6885 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/lib/kubernetes
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    59303 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/lib/kuryr_kubernetes
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8090 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.ovs.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2314 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.pod-in-vm.overcloud.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1368 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.pod-in-vm.undercloud.ovn.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1604 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.pod-in-vm.undercloud.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7686 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1561 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.worker.sample
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6260 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4364 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.384025 kuryr-kubernetes-9.0.0.0rc1/doc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.392025 kuryr-kubernetes-9.0.0.0rc1/doc/images/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   156783 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/controller_pipeline.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16165 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/create_network_policy_flow.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    74032 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/external_traffic_to_l7_router.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28274 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/fuxi_k8s_components.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64078 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/kuryr_k8s_components.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19764 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/kuryr_k8s_components.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   160802 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/kuryr_k8s_ingress_ctrl_flow_diagram.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   110459 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/kuryr_k8s_ingress_sw_components.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   123352 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/kuryr_k8s_ocp_route_ctrl_sw.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   117373 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/l7_routing_and_user_lb_neutron_entities.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   187600 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/lbaas_translation.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67092 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/net-policy.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   220449 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/pod_creation_flow_daemon.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    71366 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/pod_creation_flow_daemon.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    92990 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/service_creation_diagram.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   477823 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/service_creation_diagram.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11510 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/update_network_policy_on_pod_creation.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36189 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/images/vif_handler_drivers_design.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.392025 kuryr-kubernetes-9.0.0.0rc1/doc/source/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2678 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.392025 kuryr-kubernetes-9.0.0.0rc1/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/contributor/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.396025 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3847 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/annotation_project_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3392 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/health_manager.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5891 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/high_availability.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13015 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/kuryr_kubernetes_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2291 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/kuryr_kubernetes_versions.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16090 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/network_policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9513 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/port_manager.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6977 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/service_support.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4560 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/updating_pod_resources_api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5282 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/vif_handler_drivers_design.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      812 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.400025 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7155 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/containerized.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7749 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/default_configuration.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.404025 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7051 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/basic.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2489 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/containerized.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5660 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/nested-dpdk.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/nested-macvlan.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3233 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/nested-vlan.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4149 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/ovn-octavia.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6646 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/ovn_support.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1300 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/ports-pool.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      853 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/https_kubernetes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1359 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16318 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/ipv6.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2081 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/listener_timeouts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10471 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/manual.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2675 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/multi_vif_with_npwg_spec.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4926 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/multiple_tenants.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5512 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/network_namespace.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10741 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/network_policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6028 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/ports-pool.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48019 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/services.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11539 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/testing_connectivity.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2911 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/testing_nested_connectivity.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11168 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/testing_sctp_services.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9112 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/testing_udp_services.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1844 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/trunk_ports.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3690 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/upgrades.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1991 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/nested_vlan_mode.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       30 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/readme.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.356025 kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.404025 kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/pike/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3003 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/pike/contrail_support.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8341 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/pike/fuxi_kubernetes.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.404025 kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/queens/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22143 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/queens/network_policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.404025 kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/rocky/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6200 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/rocky/npwg_spec_support.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.404025 kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/stein/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7723 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/stein/vhostuser.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/doc/source/usage.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.356025 kuryr-kubernetes-9.0.0.0rc1/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.356025 kuryr-kubernetes-9.0.0.0rc1/etc/cni/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.404025 kuryr-kubernetes-9.0.0.0rc1/etc/cni/net.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/etc/cni/net.d/10-kuryr.conflist
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/etc/cni/net.d/kuryr.conflist.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.404025 kuryr-kubernetes-9.0.0.0rc1/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/etc/oslo-config-generator/kuryr.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.404025 kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.408025 kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/kuryr_crds/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7265 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/kuryr_crds/kuryrloadbalancer.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1489 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/kuryr_crds/kuryrnetwork.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4928 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/kuryr_crds/kuryrnetworkpolicy.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1400 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/kuryr_crds/kuryrport.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      606 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/network_attachment_definition_crd.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.408025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/README
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/go.mod
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8592 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/go.sum
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.408025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/hack/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      302 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/hack/build-go.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)       38 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/hack/update-deps.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.408025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/pkg/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6029 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/pkg/main.go
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2846 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/pkg/ovo.go
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.408025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.356025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.356025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.408025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/LICENSE
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.360025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.408025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/skel/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8254 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/skel/skel.go
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.408025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.408025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/020/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3106 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/020/types.go
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3343 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/args.go
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.408025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/current/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6964 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/current/types.go
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5086 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/types.go
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.412025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3070 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/utils/utils.go
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.412025 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1093 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/conf.go
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4285 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/plugin.go
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/reconcile.go
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2707 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/version.go
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/modules.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.416025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3632 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/clients.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.420025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1104 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      727 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/cni.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/daemon.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.420025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/eventlet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      675 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/eventlet/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      746 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/eventlet/controller.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.420025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/sanity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/sanity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3067 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/sanity/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3562 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/sanity_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6653 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.420025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5968 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.424025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6107 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/bridge.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7838 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/dpdk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10170 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/nested.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4958 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/vhostuser.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.424025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/daemon/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/daemon/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14888 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/daemon/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3300 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/daemon/watcher_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4714 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/handlers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5343 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2002 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/main.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.424025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      875 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/plugins/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11356 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/plugins/k8s_cni_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2619 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/prometheus_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3515 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16461 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4204 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.424025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.432025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2501 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/annotation_project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27615 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2798 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/default_project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3231 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/default_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2154 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/default_subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4474 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/lb_public_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40512 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/lbaasv2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4660 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/multi_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9342 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/namespace_subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2974 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/nested_dpdk_vif.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7312 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/nested_macvlan_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2738 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/nested_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13230 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/nested_vlan_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    37116 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/network_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18358 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/network_policy_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6369 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/neutron_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7359 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/node_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6470 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/public_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26434 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    57382 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/vif_pool.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.436025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10478 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/kuryrnetwork.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4464 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/kuryrnetwork_population.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14639 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/kuryrnetworkpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20112 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/kuryrport.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18187 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/lbaas.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    40982 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/loadbalancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2673 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/machine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5545 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/namespace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3133 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/pipeline.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5123 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/pod_label.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2357 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9392 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/vif.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.436025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/managers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/managers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4385 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/managers/health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9232 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/managers/pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8039 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/managers/prometheus_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6939 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6757 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.440025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/__init__.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5373 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/asynchronous.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      943 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4405 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/dispatch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1622 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/health.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3720 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/k8s_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1861 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6126 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2514 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19459 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/k8s_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2056 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/linux_net_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.440025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/objects/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/objects/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/objects/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1015 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/objects/fields.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5829 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/objects/lbaas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2459 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/objects/vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2521 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/opts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1626 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/os_vif_plug_noop.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15371 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/os_vif_util.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.440025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      846 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6527 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/fake.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.444025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.444025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cmd/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.444025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cmd/eventlet/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cmd/eventlet/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1247 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cmd/eventlet/test_controller.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cmd/test_daemon.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5125 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cmd/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.448026 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.448026 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12937 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/plugins/test_k8s_cni_registry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3673 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16787 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_binding.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2597 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_handlers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5394 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1671 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_main.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4499 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1389 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.448026 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.456025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4960 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_annotation_project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4482 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3353 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_default_project.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2595 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_default_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3017 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_default_subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14674 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_lb_public_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    69826 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_lbaasv2.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7232 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_multi_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11367 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_namespace_subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8552 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_dpdk.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20672 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_macvlan_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5307 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29002 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_vlan_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29767 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_network_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25194 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_network_policy_security_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14332 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_neutron_vif.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19023 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_node_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6308 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_public_ip.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6189 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    73646 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_vif_pool.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.460026 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      863 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_fake_handler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17977 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetwork.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4702 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetwork_population.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3625 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetworkpolicy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33509 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrport.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15747 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_lbaas.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    29152 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_loadbalancer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3478 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_machine.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5501 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_namespace.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2816 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_pipeline.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5600 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_pod_label.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12980 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_vif.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.460026 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/managers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/managers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8029 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/managers/test_health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15312 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/managers/test_pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6927 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/managers/test_prometheus_exporter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2372 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/test_service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.464026 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6217 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_asynchronous.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4286 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_dispatch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1678 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_health.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_k8s_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2323 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_logging.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5345 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/kuryr_fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1882 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20696 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_k8s_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2850 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_linux_net_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2997 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_object.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3683 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_os_vif_plug_noop.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27709 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_os_vif_util.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21734 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12217 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_watcher.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28362 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      625 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/version.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9362 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/watcher.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.416025 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2370 2023-09-15 14:26:19.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17937 2023-09-15 14:26:20.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-09-15 14:26:19.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5658 2023-09-15 14:26:19.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-09-15 14:26:19.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-09-15 14:26:19.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2023-09-15 14:26:19.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2023-09-15 14:26:19.000000 kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.464026 kuryr-kubernetes-9.0.0.0rc1/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      413 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/playbooks/copy-crio-logs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/playbooks/copy-k8s-logs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3242 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/playbooks/e2e-tests.patch
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/playbooks/get_amphora_tarball.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3688 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/playbooks/run_k8s_e2e_tests.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.364024 kuryr-kubernetes-9.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.472026 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/active-passive-ha-cfbda8e6b527b48e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      580 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/add-tagging-ce56231f58bf7ad0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      559 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/bp-openshift-router-support-5f28108b39a2826f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/change-cni-daemon-default-port-e968a83fa1bf30b5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/changing-default-url-for-k8s-api-42c3b90183783291.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/cni-health-checks-d2b70f2f2551a9fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      247 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/containerization-2fba4dac5c097b19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/cri-o-support-ab7e810775754ea7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      458 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/deprecate-handlers-caching-9cdfd772aba9a7ce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      770 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/deprecate-non-daemonized-6dd2154238b1628c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      446 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/deprecate-sg-mode-option-96824c33335cd74b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      440 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/deprecate-worker-nodes-subnet-e452c84df5b5ed5c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      609 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/deprecate_lbaasv2-a524aedf5d3a36bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      345 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/drop-ingress-d78a7a9be8f20da1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/drop-py27-60f55b6bc1d082bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/fault-tolerable-watcher-24c51dbccabf5f17.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      647 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/golang-kuryr-cni-aab144831d4dc9dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      595 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/k8s-client-token-default-882ec49d1faffc29.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      507 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/kuryr-daemon-f09075b9eb60388f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      876 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/make-ext-subnet-optional-99e73bfcbde96c22.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      837 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/make-handlers-pluggable-844475484771ffd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      284 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/make-lbaas-timeout-configurable-8624ea32971c0cbe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/make-listener-timeouts-configurable-f563d85eg6c6fe6d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1542 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/multivif-pools-1cec757c77a8c4f8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/network-device-mtu-default-90faa7d685d4d0ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      438 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/network-namespace-2353f8013be398cd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/network-policy-support-on-services-without-selectors-fea06ab71a8a6f2a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/octavia-acls-7452d3406d75ea15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      772 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/oslo-caching-b11881cfb9dc306c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/remove-non-daemon-836e4825384b1b88.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/remove-physical-device-mapping-15d614b70c68fc73.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/remove-run-server-aca25a2d9d723dc7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/remove-sriov-5f44deb951264510.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1220 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/reusable-pool-drivers-00e7fdc1f4738441.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       49 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/started-using-reno-90dbe9da108ec5c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/stein-upgrade-226c8e7b735701ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/support-specify-project-by-namespace-annotation-18bc6eca729bff5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/svc-without-selectors-f36bab0883459b80.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/zuul-v3-native-gates-4ed7698667a7b92e.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.476026 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      598 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.476026 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.476026 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4743 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      352 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1144 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6885 2023-09-15 14:26:20.484026 kuryr-kubernetes-9.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.476026 kuryr-kubernetes-9.0.0.0rc1/tools/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-09-15 14:26:20.480026 kuryr-kubernetes-9.0.0.0rc1/tools/gate/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1183 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/tools/gate/copy_crio_logs.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3275 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/tools/gate/copy_k8s_logs.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1404 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/tools/generate_config_file_samples.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3345 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/tools/generate_k8s_resource_definitions.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2023-09-15 14:25:51.000000 kuryr-kubernetes-9.0.0.0rc1/tox.ini
```

### Comparing `kuryr-kubernetes-9.0.0/.zuul.d/base.yaml` & `kuryr-kubernetes-9.0.0.0rc1/.zuul.d/base.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/.zuul.d/k8s-np-e2e.yaml` & `kuryr-kubernetes-9.0.0.0rc1/.zuul.d/k8s-np-e2e.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/.zuul.d/nodesets.yaml` & `kuryr-kubernetes-9.0.0.0rc1/.zuul.d/nodesets.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/.zuul.d/project.yaml` & `kuryr-kubernetes-9.0.0.0rc1/.zuul.d/project.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/.zuul.d/tempest-jobs.yaml` & `kuryr-kubernetes-9.0.0.0rc1/.zuul.d/tempest-jobs.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/.zuul.d/tempest-multinode-jobs.yaml` & `kuryr-kubernetes-9.0.0.0rc1/.zuul.d/tempest-multinode-jobs.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/AUTHORS` & `kuryr-kubernetes-9.0.0.0rc1/AUTHORS`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/CONTRIBUTING.rst` & `kuryr-kubernetes-9.0.0.0rc1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/ChangeLog` & `kuryr-kubernetes-9.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 CHANGES
 =======
 
-9.0.0
------
+9.0.0.0rc1
+----------
 
 * Cleanup hyperkube leftovers
 * Bump kubernetes to version 1.27
 * Bump Kubernetes and cri-o version to 1.26
 * Update CNI to v0.8.1
 * Skip retry of Network Policy event
 * KuryrPort cleanup: Fix issue of subport not found
```

### Comparing `kuryr-kubernetes-9.0.0/LICENSE` & `kuryr-kubernetes-9.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/PKG-INFO` & `kuryr-kubernetes-9.0.0.0rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kuryr-kubernetes
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Kubernetes integration with OpenStack networking
 Home-page: https://docs.openstack.org/kuryr-kubernetes/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `kuryr-kubernetes-9.0.0/README.rst` & `kuryr-kubernetes-9.0.0.0rc1/README.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/cni.Dockerfile` & `kuryr-kubernetes-9.0.0.0rc1/cni.Dockerfile`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/cni_ds_init` & `kuryr-kubernetes-9.0.0.0rc1/cni_ds_init`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/devstack-heat/README.rst` & `kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/README.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/devstack-heat/devstack_heat.py` & `kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/devstack_heat.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/devstack-heat/hot/devstack_heat_template.yml` & `kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/hot/devstack_heat_template.yml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/devstack-heat/hot/distro_deps.sh` & `kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/hot/distro_deps.sh`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/devstack-heat/hot/networking_deployment.yaml` & `kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/hot/networking_deployment.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/devstack-heat/hot/node.yaml` & `kuryr-kubernetes-9.0.0.0rc1/contrib/devstack-heat/hot/node.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/kubectl_plugins/kubectl_kuryr_plugin_1080.gif` & `kuryr-kubernetes-9.0.0.0rc1/contrib/kubectl_plugins/kubectl_kuryr_plugin_1080.gif`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/kubectl_plugins/kuryr/kuryr` & `kuryr-kubernetes-9.0.0.0rc1/contrib/kubectl_plugins/kuryr/kuryr`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/pools-management/README.rst` & `kuryr-kubernetes-9.0.0.0rc1/contrib/pools-management/README.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/pools-management/subports.py` & `kuryr-kubernetes-9.0.0.0rc1/contrib/pools-management/subports.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/regenerate_pod_resources_api.sh` & `kuryr-kubernetes-9.0.0.0rc1/contrib/regenerate_pod_resources_api.sh`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/sctp_client.py` & `kuryr-kubernetes-9.0.0.0rc1/contrib/sctp_client.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/testing/container/build.sh` & `kuryr-kubernetes-9.0.0.0rc1/contrib/testing/container/build.sh`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/testing/container/hostname.c` & `kuryr-kubernetes-9.0.0.0rc1/contrib/testing/container/hostname.c`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/vagrant/README.rst` & `kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/README.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/vagrant/Vagrantfile` & `kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/Vagrantfile`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/vagrant/devstack.sh` & `kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/devstack.sh`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/contrib/vagrant/vagrant.sh` & `kuryr-kubernetes-9.0.0.0rc1/contrib/vagrant/vagrant.sh`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/controller.Dockerfile` & `kuryr-kubernetes-9.0.0.0rc1/controller.Dockerfile`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/devstack/lib/kubernetes` & `kuryr-kubernetes-9.0.0.0rc1/devstack/lib/kubernetes`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/devstack/lib/kuryr_kubernetes` & `kuryr-kubernetes-9.0.0.0rc1/devstack/lib/kuryr_kubernetes`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/devstack/local.conf.ovs.sample` & `kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.ovs.sample`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/devstack/local.conf.pod-in-vm.overcloud.sample` & `kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.pod-in-vm.overcloud.sample`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/devstack/local.conf.pod-in-vm.undercloud.ovn.sample` & `kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.pod-in-vm.undercloud.ovn.sample`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/devstack/local.conf.pod-in-vm.undercloud.sample` & `kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.pod-in-vm.undercloud.sample`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/devstack/local.conf.sample` & `kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.sample`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/devstack/local.conf.worker.sample` & `kuryr-kubernetes-9.0.0.0rc1/devstack/local.conf.worker.sample`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/devstack/plugin.sh` & `kuryr-kubernetes-9.0.0.0rc1/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/devstack/settings` & `kuryr-kubernetes-9.0.0.0rc1/devstack/settings`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/controller_pipeline.png` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/controller_pipeline.png`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/create_network_policy_flow.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/create_network_policy_flow.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/external_traffic_to_l7_router.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/external_traffic_to_l7_router.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/fuxi_k8s_components.png` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/fuxi_k8s_components.png`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/kuryr_k8s_components.png` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/kuryr_k8s_components.png`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/kuryr_k8s_components.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/kuryr_k8s_components.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/kuryr_k8s_ingress_ctrl_flow_diagram.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/kuryr_k8s_ingress_ctrl_flow_diagram.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/kuryr_k8s_ingress_sw_components.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/kuryr_k8s_ingress_sw_components.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/kuryr_k8s_ocp_route_ctrl_sw.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/kuryr_k8s_ocp_route_ctrl_sw.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/l7_routing_and_user_lb_neutron_entities.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/l7_routing_and_user_lb_neutron_entities.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/lbaas_translation.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/lbaas_translation.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/net-policy.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/net-policy.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/pod_creation_flow_daemon.png` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/pod_creation_flow_daemon.png`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/pod_creation_flow_daemon.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/pod_creation_flow_daemon.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/service_creation_diagram.png` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/service_creation_diagram.png`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/service_creation_diagram.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/service_creation_diagram.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/update_network_policy_on_pod_creation.svg` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/update_network_policy_on_pod_creation.svg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/images/vif_handler_drivers_design.png` & `kuryr-kubernetes-9.0.0.0rc1/doc/images/vif_handler_drivers_design.png`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/conf.py` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/contributor/contributing.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/annotation_project_driver.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/annotation_project_driver.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/health_manager.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/health_manager.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/high_availability.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/high_availability.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/index.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/index.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/kuryr_kubernetes_design.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/kuryr_kubernetes_design.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/kuryr_kubernetes_versions.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/kuryr_kubernetes_versions.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/network_policy.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/network_policy.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/port_manager.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/port_manager.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/service_support.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/service_support.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/updating_pod_resources_api.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/updating_pod_resources_api.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/devref/vif_handler_drivers_design.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/devref/vif_handler_drivers_design.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/index.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/containerized.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/containerized.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/default_configuration.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/default_configuration.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/devstack/basic.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/basic.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/devstack/containerized.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/containerized.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/devstack/index.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/index.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/devstack/nested-dpdk.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/nested-dpdk.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/devstack/nested-macvlan.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/nested-macvlan.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/devstack/nested-vlan.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/nested-vlan.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/devstack/ovn-octavia.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/ovn-octavia.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/devstack/ovn_support.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/ovn_support.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/devstack/ports-pool.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/devstack/ports-pool.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/https_kubernetes.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/https_kubernetes.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/index.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/index.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/ipv6.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/ipv6.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/listener_timeouts.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/listener_timeouts.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/manual.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/manual.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/multi_vif_with_npwg_spec.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/multi_vif_with_npwg_spec.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/multiple_tenants.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/multiple_tenants.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/network_namespace.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/network_namespace.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/network_policy.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/network_policy.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/ports-pool.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/ports-pool.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/services.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/services.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/testing_connectivity.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/testing_connectivity.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/testing_nested_connectivity.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/testing_nested_connectivity.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/testing_sctp_services.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/testing_sctp_services.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/testing_udp_services.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/testing_udp_services.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/trunk_ports.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/trunk_ports.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/installation/upgrades.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/installation/upgrades.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/nested_vlan_mode.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/nested_vlan_mode.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/specs/pike/contrail_support.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/pike/contrail_support.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/specs/pike/fuxi_kubernetes.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/pike/fuxi_kubernetes.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/specs/queens/network_policy.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/queens/network_policy.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/specs/rocky/npwg_spec_support.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/rocky/npwg_spec_support.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/doc/source/specs/stein/vhostuser.rst` & `kuryr-kubernetes-9.0.0.0rc1/doc/source/specs/stein/vhostuser.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kubernetes_crds/kuryr_crds/kuryrloadbalancer.yaml` & `kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/kuryr_crds/kuryrloadbalancer.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kubernetes_crds/kuryr_crds/kuryrnetwork.yaml` & `kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/kuryr_crds/kuryrnetwork.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kubernetes_crds/kuryr_crds/kuryrnetworkpolicy.yaml` & `kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/kuryr_crds/kuryrnetworkpolicy.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kubernetes_crds/kuryr_crds/kuryrport.yaml` & `kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/kuryr_crds/kuryrport.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kubernetes_crds/network_attachment_definition_crd.yaml` & `kuryr-kubernetes-9.0.0.0rc1/kubernetes_crds/network_attachment_definition_crd.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/go.sum` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/go.sum`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/pkg/main.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/pkg/main.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/pkg/ovo.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/pkg/ovo.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/LICENSE` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/LICENSE`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/skel/skel.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/skel/skel.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/020/types.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/020/types.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/args.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/args.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/current/types.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/current/types.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/types.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/types/types.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/utils/utils.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/utils/utils.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/conf.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/conf.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/plugin.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/plugin.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/reconcile.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/reconcile.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/version.go` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_cni/vendor/github.com/containernetworking/cni/pkg/version/version.go`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/clients.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/clients.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/__init__.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/__init__.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/cni.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/cni.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/daemon.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/daemon.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/eventlet/__init__.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/eventlet/__init__.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/eventlet/controller.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/eventlet/controller.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/sanity/checks.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/sanity/checks.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/sanity_checks.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cmd/status.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cmd/status.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/api.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/api.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/base.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/base.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/bridge.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/bridge.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/dpdk.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/dpdk.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/nested.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/nested.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/binding/vhostuser.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/binding/vhostuser.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/daemon/service.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/daemon/service.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/daemon/watcher_service.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/daemon/watcher_service.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/handlers.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/handlers.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/health.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/health.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/main.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/main.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/plugins/base.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/plugins/base.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/plugins/k8s_cni_registry.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/plugins/k8s_cni_registry.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/prometheus_exporter.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/cni/utils.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/cni/utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/config.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/constants.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/constants.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/annotation_project.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/annotation_project.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/base.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/base.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/default_project.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/default_project.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/default_security_groups.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/default_security_groups.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/default_subnet.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/default_subnet.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/lb_public_ip.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/lb_public_ip.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/lbaasv2.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/lbaasv2.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/multi_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/multi_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/namespace_subnet.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/namespace_subnet.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/nested_dpdk_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/nested_dpdk_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/nested_macvlan_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/nested_macvlan_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/nested_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/nested_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/nested_vlan_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/nested_vlan_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/network_policy.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/network_policy.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/network_policy_security_groups.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/network_policy_security_groups.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/neutron_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/neutron_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/node_subnets.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/node_subnets.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/public_ip.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/public_ip.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/utils.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/drivers/vif_pool.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/drivers/vif_pool.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/kuryrnetwork.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/kuryrnetwork.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/kuryrnetwork_population.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/kuryrnetwork_population.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/kuryrnetworkpolicy.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/kuryrnetworkpolicy.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/kuryrport.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/kuryrport.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/lbaas.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/lbaas.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/loadbalancer.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/loadbalancer.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/machine.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/machine.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/namespace.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/namespace.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/pipeline.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/pipeline.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/pod_label.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/pod_label.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/policy.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/policy.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/handlers/vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/handlers/vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/managers/health.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/managers/health.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/managers/pool.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/managers/pool.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/managers/prometheus_exporter.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/managers/prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/controller/service.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/controller/service.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/exceptions.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/exceptions.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/asynchronous.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/asynchronous.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/base.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/base.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/dispatch.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/dispatch.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/health.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/health.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/k8s_base.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/k8s_base.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/logging.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/logging.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/handlers/retry.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/handlers/retry.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/health.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/health.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/k8s_client.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/k8s_client.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/linux_net_utils.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/linux_net_utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/objects/base.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/objects/base.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/objects/fields.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/objects/fields.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/objects/lbaas.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/objects/lbaas.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/objects/vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/objects/vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/opts.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/opts.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/os_vif_plug_noop.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/os_vif_plug_noop.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/os_vif_util.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/os_vif_util.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/base.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/base.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/fake.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/fake.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cmd/eventlet/test_controller.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cmd/eventlet/test_controller.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cmd/test_daemon.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cmd/test_daemon.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cmd/test_status.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/plugins/test_k8s_cni_registry.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/plugins/test_k8s_cni_registry.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_api.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_api.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_binding.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_binding.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_handlers.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_handlers.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_health.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_health.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_main.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_main.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_service.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_service.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/cni/test_utils.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/cni/test_utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_annotation_project.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_annotation_project.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_base.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_base.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_default_project.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_default_project.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_default_security_groups.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_default_security_groups.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_default_subnet.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_default_subnet.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_lb_public_ip.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_lb_public_ip.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_lbaasv2.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_lbaasv2.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_multi_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_multi_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_namespace_subnet.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_namespace_subnet.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_dpdk.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_dpdk.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_macvlan_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_macvlan_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_vlan_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_nested_vlan_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_network_policy.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_network_policy.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_network_policy_security_groups.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_network_policy_security_groups.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_neutron_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_neutron_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_node_subnets.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_node_subnets.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_public_ip.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_public_ip.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_utils.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/drivers/test_vif_pool.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/drivers/test_vif_pool.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_fake_handler.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_fake_handler.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetwork.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetwork.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetwork_population.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetwork_population.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetworkpolicy.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrnetworkpolicy.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrport.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_kuryrport.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_lbaas.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_lbaas.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_loadbalancer.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_machine.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_machine.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_namespace.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_namespace.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_pipeline.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_pod_label.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_pod_label.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_policy.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_policy.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/handlers/test_vif.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/handlers/test_vif.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/managers/test_health.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/managers/test_health.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/managers/test_pool.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/managers/test_pool.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/managers/test_prometheus_exporter.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/managers/test_prometheus_exporter.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/controller/test_service.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/controller/test_service.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_asynchronous.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_asynchronous.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_dispatch.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_dispatch.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_health.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_health.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_k8s_base.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_k8s_base.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_logging.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_logging.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/handlers/test_retry.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/handlers/test_retry.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/kuryr_fixtures.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/kuryr_fixtures.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_clients.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_clients.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_k8s_client.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_k8s_client.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_linux_net_utils.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_linux_net_utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_object.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_object.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_os_vif_plug_noop.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_os_vif_plug_noop.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_os_vif_util.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_os_vif_util.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_utils.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/tests/unit/test_watcher.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/tests/unit/test_watcher.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/utils.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/version.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/version.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes/watcher.py` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes/watcher.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/PKG-INFO` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: kuryr-kubernetes
-Version: 9.0.0
+Version: 9.0.0.0rc1
 Summary: Kubernetes integration with OpenStack networking
 Home-page: https://docs.openstack.org/kuryr-kubernetes/latest
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/SOURCES.txt` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/kuryr_kubernetes.egg-info/entry_points.txt` & `kuryr-kubernetes-9.0.0.0rc1/kuryr_kubernetes.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/playbooks/e2e-tests.patch` & `kuryr-kubernetes-9.0.0.0rc1/playbooks/e2e-tests.patch`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/playbooks/run_k8s_e2e_tests.yaml` & `kuryr-kubernetes-9.0.0.0rc1/playbooks/run_k8s_e2e_tests.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/add-tagging-ce56231f58bf7ad0.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/add-tagging-ce56231f58bf7ad0.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/bp-openshift-router-support-5f28108b39a2826f.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/bp-openshift-router-support-5f28108b39a2826f.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/cni-health-checks-d2b70f2f2551a9fc.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/cni-health-checks-d2b70f2f2551a9fc.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/deprecate-non-daemonized-6dd2154238b1628c.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/deprecate-non-daemonized-6dd2154238b1628c.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/deprecate_lbaasv2-a524aedf5d3a36bc.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/deprecate_lbaasv2-a524aedf5d3a36bc.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/fault-tolerable-watcher-24c51dbccabf5f17.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/fault-tolerable-watcher-24c51dbccabf5f17.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/golang-kuryr-cni-aab144831d4dc9dd.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/golang-kuryr-cni-aab144831d4dc9dd.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/k8s-client-token-default-882ec49d1faffc29.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/k8s-client-token-default-882ec49d1faffc29.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/make-ext-subnet-optional-99e73bfcbde96c22.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/make-ext-subnet-optional-99e73bfcbde96c22.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/make-handlers-pluggable-844475484771ffd6.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/make-handlers-pluggable-844475484771ffd6.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/make-listener-timeouts-configurable-f563d85eg6c6fe6d.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/make-listener-timeouts-configurable-f563d85eg6c6fe6d.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/multivif-pools-1cec757c77a8c4f8.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/multivif-pools-1cec757c77a8c4f8.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/oslo-caching-b11881cfb9dc306c.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/oslo-caching-b11881cfb9dc306c.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/notes/reusable-pool-drivers-00e7fdc1f4738441.yaml` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/notes/reusable-pool-drivers-00e7fdc1f4738441.yaml`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/source/README.rst` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/README.rst`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/releasenotes/source/conf.py` & `kuryr-kubernetes-9.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/requirements.txt` & `kuryr-kubernetes-9.0.0.0rc1/requirements.txt`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/setup.cfg` & `kuryr-kubernetes-9.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/setup.py` & `kuryr-kubernetes-9.0.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/test-requirements.txt` & `kuryr-kubernetes-9.0.0.0rc1/test-requirements.txt`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/tools/gate/copy_crio_logs.sh` & `kuryr-kubernetes-9.0.0.0rc1/tools/gate/copy_crio_logs.sh`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/tools/gate/copy_k8s_logs.sh` & `kuryr-kubernetes-9.0.0.0rc1/tools/gate/copy_k8s_logs.sh`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/tools/generate_config_file_samples.sh` & `kuryr-kubernetes-9.0.0.0rc1/tools/generate_config_file_samples.sh`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/tools/generate_k8s_resource_definitions.sh` & `kuryr-kubernetes-9.0.0.0rc1/tools/generate_k8s_resource_definitions.sh`

 * *Files identical despite different names*

### Comparing `kuryr-kubernetes-9.0.0/tox.ini` & `kuryr-kubernetes-9.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

