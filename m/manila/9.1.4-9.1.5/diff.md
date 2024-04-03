# Comparing `tmp/manila-9.1.4.tar.gz` & `tmp/manila-9.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/manila-9.1.4.tar", last modified: Fri Jul 31 09:56:47 2020, max compression
+gzip compressed data, was "dist/manila-9.1.5.tar", last modified: Mon Feb  1 17:28:24 2021, max compression
```

## Comparing `manila-9.1.4.tar` & `manila-9.1.5.tar`

### file list

```diff
@@ -1,1881 +1,1894 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/devstack/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/devstack/upgrade/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/upgrade/settings
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/devstack/upgrade/from-mitaka/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/upgrade/from-mitaka/upgrade-manila
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2189 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/upgrade/upgrade.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18064 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/upgrade/resources.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/devstack/upgrade/from-newton/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/upgrade/from-newton/upgrade-manila
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      464 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/upgrade/shutdown.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/devstack/files/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/devstack/files/debs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/files/debs/manila
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/devstack/files/rpms/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/files/rpms/manila
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/devstack/files/rpms-suse/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/files/rpms-suse/manila
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12058 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/settings
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/README.rst
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    57308 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/plugin.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2020-07-31 09:55:01.000000 manila-9.1.4/devstack/apache-manila.template
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2020-07-31 09:55:01.000000 manila-9.1.4/etc/oslo-config-generator/manila.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/etc/manila/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1271 2020-07-31 09:55:01.000000 manila-9.1.4/etc/manila/logging_sample.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2020-07-31 09:55:01.000000 manila-9.1.4/etc/manila/manila-policy-generator.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2020-07-31 09:55:01.000000 manila-9.1.4/etc/manila/README.manila.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1886 2020-07-31 09:55:01.000000 manila-9.1.4/etc/manila/api-paste.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2020-07-31 09:55:01.000000 manila-9.1.4/etc/manila/rootwrap.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/etc/manila/rootwrap.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8112 2020-07-31 09:55:01.000000 manila-9.1.4/etc/manila/rootwrap.d/share.filters
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2020-07-31 09:55:01.000000 manila-9.1.4/rally-jobs/rally-manila-no-ss.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2020-07-31 09:55:01.000000 manila-9.1.4/rally-jobs/rally-manila.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14035 2020-07-31 09:56:46.000000 manila-9.1.4/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-07-31 09:55:01.000000 manila-9.1.4/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2020-07-31 09:55:01.000000 manila-9.1.4/test-requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-07-31 09:55:01.000000 manila-9.1.4/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5283 2020-07-31 09:55:01.000000 manila-9.1.4/tox.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1072 2020-07-31 09:55:01.000000 manila-9.1.4/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2020-07-31 09:55:01.000000 manila-9.1.4/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5470 2020-07-31 09:55:01.000000 manila-9.1.4/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2020-07-31 09:55:01.000000 manila-9.1.4/.coveragerc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2020-07-31 09:55:01.000000 manila-9.1.4/LICENSE
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/migration-access-fix-71a0f52ea7a152a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/introduce-tooz-library-5fed75b8caffcf42.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1275 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/nexentastor5-v1.1-1ad6c8f7b5cc11b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1745436-remove-data-node-access-ip-config-opt-709f330c57cdb0d5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-667744-fix-c64071e6e5a098f7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/veritas-access-manila-driver-d75558c01ce6d428.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1822099-fix-multisegment-mtu.yaml-ac2e31c084d8bbb6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/qnap-enhance-support-53848fda525b7ea4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/lv-mounting-inside-containers-af8f84d1fab256d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1707946-nfs-helper-0-netmask-224da94b82056f93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/ibm-gpfs-manage-support-c110120c350728e3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-managing-twice-hnas-4956a7653d27e320.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-volume-efficiency-status-2102ad630c5407a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bp-admin-network-hnas-9b714736e521101e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/reset_tap_device_after_node_restart-0690a6beca077b95.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-share-instance-list-with-limit-db7b5b99138e22ee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/manage-share-snapshot-in-huawei-driver-007b2c763fbdf480.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/container-driver-5d972cc40e314663.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1667450-migration-stale-source-9c092fee267a7a0f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-standalone-network-plugin-ip-version-440ebcf27ffd22f8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-nova-network-support-f5bcb8b2fcd38581.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1804656-netapp-cdot-add-port-ids-to-share-server-backend-424ca11a1eb44826.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-hds-hnas-unconfined-09b79f3bdb24a83c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1811680-destroy-quotas-usages-reservations-when-deleting-share-type-a18f2e00a65fe922.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1660686-snapshot-export-locations-mount-not-supported-cdc2f5a3b57a9319.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bp-share-type-supported-azs-2e12ed406f181b3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/unexpected-data-of-share-from-snap-134189fc0f3eeedf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1658133-fix-lvm-revert-34a90e70c9aa7354.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/snapshot-force-delete-4432bebfb5a0bbc9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1639188-fix-extend-operation-of-shrinked-share-in-generic-driver-5c7f82faefaf26ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1657033-fix-share-metadata-error-when-deleting-share.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1745436-78c46f8a0c96cbca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/api-versions-mark-v1-deprecated-3540d39279fbd60e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1602525-port_binding_mandatory-2aaba0fa72b82676.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1660319-1660336-migration-share-groups-e66a1478634947ad.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1804651-netapp-cdot-add-peferred-dc-to-cifs-ad-99072ce663762e83.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-cdot-clone-split-control-a68b5fc80f1fc368.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1696669-add-ou-to-security-service-06b69615bd417d40.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/drop-support-for-lvm-share-export-ip-e031ef4c5f95b534.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1815038-extend-remove_version_from_href-support-ea479daaaf5c5700.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/dedupe-support-hnas-driver-017d2f2a93a8b487.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1651578-gpfs-prepend-beb99f408cf20bb5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1885956-enforce-policy-check-getting-share-type-by-name-5eca17b02bea5261.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1717135-ganesha-cleanup-of-tmp-config-files-66082b2384ace0a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1747695-fixed-ip-version-in-neutron-bind-network-plugin-526958e2d83df072.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1705533-manage-api-error-message-fix-967b0d44c09b914a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1638994-drop-fake-cg-support-from-generic-driver-16efce98f94b1b6b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/infinidat-balance-network-spaces-ips-25a9f1e587b87156.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1690785-fix-gpfs-path-91a354bc69bf6a47.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1845452-unity--fix-fail-to-delete-cifs-share-c502a10ae306e506.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1785129-fix-sighup-behavior-with-scheduler-8ee803ad0e543cce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-create_share_from_snapshot_support-extra-spec-9b1c3ad6796dd07d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1654598-enforce-policy-checks-for-share-export-locations-a5cea1ec123b1469.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1646603-netapp-broadcast-domains-411a626d38835177.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1660726-migration-export-locations-5670734670435015.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1872872-fix-quota-checking-b06fd372be143101.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1665072-migration-success-fix-3da1e80fbab666de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/unity-shrink-share-support-cc748daebfe8f562.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug_1582931-1437eae20fa544d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1707066-deny-ipv6-access-in-error-bce379ee310060f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1698258-netapp-fix-tenant-network-gateways-85935582e89a72a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1688620-netapp-migration-cancelation-fb913131eb8eb82a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1703660-fix-netapp-driver-preferred-state-0ce1a62961cded35.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-hnas-mount-on-manage-snapshot-91e094c579ddf1a3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1597940-fix-hpe3par-delete-share-0daf75193f318c41.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/neutron-binding-driver-43f01565051b031b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/huawei-driver-sectorsize-config-da776132ba6da2a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-snapshot-instances-admin-api-959a1121aa407629.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-perodic-task-7454sd45deopb13e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/use-oslo-logging-for-config-options-388da64bb4ce45db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-cdot-apply-mtu-from-network-provider-d12179a2374cdda0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/rename-cephfs-native-driver-3d9b4e3c6c78ee98.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/lvm-export-ips-5f73f30df94381d3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-intree-tempest-plugin-9fcf6edbeba47cba.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/3par-fix-get_vfs-driver-bootup-db6b085eb6094f5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/check-thin-provisioning-4bb702535f6b10b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1746202-fix-unicodeDecodeError-when-decode-API-input-4e4502fb50b69502.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1734127-a239d022bef4a002.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bp-netapp-ontap-storage-based-cryptograpy-bb7e28896e2a2539.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1733494-allow-user-group-name-with-blank-access-fix-665b3e42bdc985ac.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1818081-fix-inferred-script-name-in-case-of-proxy-urls-e33466af856708b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1634734-fix-backend-extraspec-for-replication-d611d2227997ae3e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/glusterfs-handle-new-volume-option-xml-schema-dad06253453c572c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1730509-netapp-ipv6-hostname-39abc7f40d48c844.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1698250-netapp-cdot-fix-share-server-deletion-494ab3ad1c0a97c0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/deprecate-service-instance-network-helper-option-82ff62a038f2bfa3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-huawei-exception-a09b73234ksd94kd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1772026-nve-license-not-present-fix-e5d2e0d6c5df9227.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-cdot-use-security-service-ou-4dc5835c9e00ad9d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-172112-fix-drives-private-storage-update-deleted-entries-7516ba624da2dda7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1872873-fix-consume-from-share-eea5941de17a5bcc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1795463-fix-pagination-slowness-8fcda3746aa13940.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/vlan-enhancement-in-unity-driver-0f1d972f2f6d00d9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/revert-switch-to-use-glanceclient-bc462a5477d6b8cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/estimate-provisioned-capacity-34f0d2d7c6c56621.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1706137-netapp-manila-set-valid-qos-during-migration-4405fff02bd6fa83.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-cdot-optimized-migration-within-share-server-92cfa1bcf0c317fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1848889-netapp-fix-share-replica-update-check-failure-90aa964417e7734c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1794402-fix-share-stats-container-driver-b3cb1fa2987ad4b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1816420-validate-access-type-for-ganehas-c42ce6f859fa0c8c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/nexenta-manila-drivers-cbd0b376a076ec50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-ipv6-support-f448e99a7c112362.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/dell-emc-unity-use-user-capacity-322f8bbb7c536453.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix_limit_formating_routes-1b0e1a475de6ac44.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1714691-decimal-separators-in-locales-392c0c794c49c1c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1129 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bp-ocata-migration-improvements-c8c5675e266100da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/disable-share-groups-api-by-default-0627b97ac2cda4cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/manage-unmanage-replicated-share-fa90ce34372b6df5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1649782-fixed-incorrect-exportfs-exportfs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/hitachi-driver-cifs-user-support-3f1a8b894fe3e9bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1663300-554e9c78ca2ba992.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1880747-netapp-fix-do-not-delete-default-ipspace-aee638279e0f8e93.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/gpfs-nfs-server-type-default-value-change-58890adba373737c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1661266-add-consistent-snapshot-support-attr-to-share-groups-DB-model-daa1d05129802796.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1707943-make-lvm-revert-synchronous-0ef5baee3367fd27.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp_cdot_performance_utilization-aff1b498a159470e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/cephfs-native-add-readonly-shares-support-067ccab0217ab5f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/powermax-rebrand-manila-a46a0c2ac0aa77ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/unity-vnx-rename-options-1656168dd4bdba70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/delete_vlan_on_vserver_delete-a7acd145c0b8236d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/blueprint-netapp-snapshot-visibility-4f090a20145fbf34.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/share-mount-snapshots-b52bf3433d1e7afb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-deprecated-default-options-00fed1238fb6dca0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1774159-0afe3dbc39e3c6b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/hnas-mountable-snapshots-4fbffa05656112c4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/container-driver-hardening-against-races-30c9f517a6392b9d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/infortrend-manila-driver-a1a2af20de6368cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-race-condition-netapp-5a36f6ba95a49c5e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1845135-fix-Unity-cannot-use-mgmt-ipv6-9407710a3fc7f4aa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/generic-route-racing-adf92d212f1ab4de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1704622-netapp-cdot-fix-share-specs-on-migration-bfbbebec26533652.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1662615-hnas-snapshot-concurrency-2147159ea6b086c5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1736370-qnap-fix-access-rule-override-1b79b70ae48ad9e6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/inspur-as13000-driver-41f6b7caea82e46e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1665002-hnas-driver-version-f3a8f6bff3dbe054.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/ganesha-store-exports-and-export-counter-in-ceph-rados-052b925f8ea460f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-share-access-metadata-4fda2c06e750e83c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1767430-access-control-raise-ip-address-conflict-on-host-routes-0c298125fee4a640.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/inspur-support-rwx-for-cifs-permission-4279f1fe7a59fd00.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/share-network-with-multiple-subnets-a56be8b646b9e463.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/emc-unity-manila-support-d4f5a410501cfdae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1664201-fix-share-replica-status-update-concurrency-in-replica-promotion-feature-63b15d96106c65da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/manage-snapshot-in-zfsonlinux-driver-6478d8d5b3c6a97f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/error-share-set-size-ff5d4f4ac2d56755.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/huawei-driver-replication-8ed62c8d26ad5060.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix_cephx_validation-cba4df77f9f45c6e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1870751-cleanup-share-type-and-group-type-project-access-when-deleted-4fcd49ba6e6c40bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/deprecate-memcached-servers-config-option-f4456382b9b4d6db.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-huawei-driver-qos-deletion-9ad62db3d7415980.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1696000-netapp-fix-security-style-on-cifs-shares-cbdd557a27d11961.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/qnap-tds-support-qes-24704313a0881c8c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1626249-reintroduce-per-share-instance-access-rule-state-7c08a91373b21557.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/switch-to-use-glanceclient-dde019b0b141caf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/per-backend-az-590c68be0e2cb4bd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1703581-cifs-extension-failing-because-of-volume-in-use-3fea31c4a58e2f1b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/share-revert-to-snapshot-in-netapp-cdot-driver-37f645ec3c14313c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bugfix-1771958-1771970-bcec841e7ae6b9f6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/container-manage-unmanage-share-servers-880d889828ee7ce3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-like-filter-4c1d6dc02f40d5a5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1869712-fix-increased-scheduled-time-for-non-thin-provisioned-backends-1da2cc33d365ba4f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/share-server-delete-failure-ca29d6b286a2c790.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/manage-unmanage-snapshot-bd92164472638f44.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/huawei-pool-disktype-support-0a52ba5d44da55f9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1634278-unmount-orig-active-after-promote-8e24c099ddc1e564.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1704971-fix-name-description-filter-85935582e89a72a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1694768-fix-netapp-cdot-revert-to-snapshot-5e1be65260454988.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/3par-pool-support-fb43b368214c9eda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1765420-netapp-fix-delete-share-for-vsadmins-b5dc9e0224cb3ba2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1815532-supply-request-id-in-all-apis-74419bc1b1feea1e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/qnap-fix-share-and-snapshot-inconsistant-bd628c6e14eeab14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1684032-6e4502fdceb693dr7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-is-default-e49727d276dd9bc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1626523-migration-rw-access-fix-7da3365c7b5b90a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/guru-meditation-support-7872da69f529a6c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-host-field-from-shares-and-replicas-a087f85bc4a4ba45.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1777551-security-services-api-all-tenants-fix-e820ec370d7df473.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1869148-if-only-pyc-exist-the-extension-API-cannot-be-loaded-172cb9153ebd4b56.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/zfssa-driver-add-share-manage-unmanage-9bd6d2e25cc86c35.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1639662-fix-share-service-VM-restart-problem-1110f9133cc294e8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1850264-add-async-error-when-share-extend-error-a0c458204b395994.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-export-location-filter-92ead37b728db654.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add_gateway_into_db-1f3cd3f392ae81cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1858328-netapp-fix-shrinking-error-48bcfffe694f5e81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1785180-zfsonlinux-retry-unmounting-during-manage-872cf46313c5a4ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/unity-manila-ipv6-support-dd9bcf23064baceb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1661381-migration-snapshot-export-locations-169786dcec386402.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      312 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1721787-fix-getting-share-networks-and-security-services-error-7e5e7981fcbf2b53.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/ibm-gpfs-ces-support-3498e35d9fea1b55.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1717263-netapp-ontap-fix-size-for-share-from-snapshot-02385baa7e085f39.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1750074-fix-rabbitmq-password-in-debug-mode-4e136ff86223c4ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/support-qes-114-5881c0ff0e7da512.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1798219-fix-snapshot-creation-lvm-and-generic-driver-55e349e02e7fa370.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix_access_level_managed_shares_hnas-c76a09beed365b46.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/vnx-ssl-verification-2d26a24e7e73bf81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/qnap-support-qes-200-639f3ad70687023d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1888915-harden-lvm-deletions-2a735ab0ee4a4903.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1831092-netapp-fix-race-condition-524555133aaa6ca8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1707084-netapp-manila-driver-to-honour-std-extra-specs-d32fae4e9411b503.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-nova-net-support-from-service-instance-module-dd7559803fa01d45.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/user-messages-api-589ee7d68ccba70c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/cephfs-native-enhance-update-access-support-e1a1258084c997ca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1682795-share-access-list-api-5b1e86218959f796.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1659023-netapp-cg-fix-56bb77b7bc61c3f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1859775-snapshot-over-quota-exception-bb6691612af03ddf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix_policy_file-4a382ac241c718c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/hybrid-aggregates-in-netapp-cdot-drivers-e7c90fb62426c281.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/manage-unmanage-snapshot-in-netapp-cdot-driver-5cb4b1619c39625a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/cephfs-add-nfs-protocol-support-44764094c9d784d8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-cast-rules-to-readonly-field-62ead37b728db654.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-share-migration-support-in-zfsonlinux-driver-88e6da5692b50810.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/migration-share-type-98e3d3c4c6f47bd9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/multi-segment-support-fa171a8e3201d54e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-deprecated-size-limiter-9d7c8ab69cf85aea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/hpe3par-rw-snapshot-shares-f7c33b4bf528bf00.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1638896-missing-migration-completing-state-1e4926ed56eb268c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/Huawei-driver-utilize-requests-lib-67f2c4e7ae0d2efa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1746723-8b89633062885f0b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1660321-fix-default-approach-for-share-group-snapshot-creation-3e843155c395e861.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-replication-dhss-true-5b2887de8e9a2cb5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1645746-fix-inheritance-of-access-rules-from-parent-share-by-zfsonlinux-child-shares-4f85908c8e9871ef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bp-export-locations-az-api-changes-c8aa1a3a5bc86312.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-cdot-quality-of-service-limits-c1fe8601d00cb5a8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1887643-netapp-add-cifs-dc-add-skip-check-c8ea9b952cedb643.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/clean-expired-messages-6161094d0c108aa7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/enhance-ensure-share-58fc14ffc099f481.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1624526-netapp-cdot-filter-root-aggregates-c30ac5064d530b86.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fixed-netapp-cdot-autosupport-3fabd8ac2e407f70.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/limiting-ssh-access-from-tenant-network-6519efd6d6895076.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1773761-qnap-fix-manage-share-size-override-a18acdf1a41909b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1613303-fix-config-generator-18b9f9be40d7eee6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/unity-drvier-support-1gb-share-48f032dff8a6a789.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1804659-speed-up-pools-detail-18f539a96042099a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/hnas-driver-rename-7ef74fe720f7e04b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1678524-check-snaprestore-license-for-snapshot-revert-6d32afdc5d0b2b51.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/manila-status-upgrade-check-framework-aef9b5cf9d8e3bda.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-policy-in-code-c31a24ee045d8d21.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1607029-fix-share-server-deletion-when-interfaces-dont-exist-4d00fe9dafadc252.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/qnap-fix-manage-snapshot-not-exist-4b111982ddc5fdae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/move-emc-share-driver-to-dell-emc-dir-1ec34dee0544270d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/vmax-rename-options-44d8123d14a23f94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-huawei-driver-cifs-mount-issue-2d7bff5a7e6e3ad6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1578328-fix-replica-deletion-in-cDOT-7e4502fb50b69507.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-cleanup-create-from-snap-hnas-0e0431f1fc861a4e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/qnap-support-qes-210-8775e6c210f3ca9f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-gathering-usage-size-8454sd45deopb14e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-default-ipv6-route-13a9fd4959928524.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/huawei-support-access-all-ip-4994c10ff75ac683.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-share-type-quotas-33a6b36c0f4c88b1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add_user_id_and_project_id_to_snapshot_APIs-157614b4b8d01e15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/migration-empty-files-01d1a3caa2e9705e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1735832-43e9291ddd73286d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/unity-revert-to-snapshot-support-1cffc3914982003d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug_1564623_change-e286060a27b02f64.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/ganesha-dynamic-update-access-be80bd1cb785e733.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1660425-snapshot-access-in-error-bce279ee310060f5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/cephfs-native-fix-evict-c45fd2de8f520757.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/windows-smb-fix-default-access-d4b9eee899e400a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/use-tooz-heartbeat-c6aa7e15444e63c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/vmax-manila-support-7c655fc094c09367.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/driver-filter-91e2c60c9d1a48dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1777551-security-networks-api-all-tenants-fix-a061274afe15180d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/hnas_allow_managed_fix-4ec7794e2035d3f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-ipv6-32d89161a9a1e0b4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/support-ipv6-in-drivers-and-network-plugins-1833121513edb13d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1813054-remove-share-usage-size-audit-period-conf-opt-7331013d1cdb7b43.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/3par-add-update-access-68fc12ffc099f480.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-manage-unmanage-share-servers-635496b46e306920.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/glusterfs-add-directory-layout-extend-shrink-fd2a008f152edbf5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/share-replication-81ecf4a32a5c83b6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/change_user_project_length-93cc8d1c32926e75.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-manage-db-purge-b32a24ee045d8d45.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-cdot-switch-volume-efficiency-bd22733445d146f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1674908-allow-user-access-fix-495b3e42bdc985ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-access-key-to-share-access-map-2fda4c06a750e24e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1700871-ontap-allow-extend-of-replicated-share-2c9709180d954308.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/added-possibility-to-run-manila-api-with-web-servers-that-support-wsgi-apps-cfffe0b789f8670a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1777126-netapp-skip-route-setup-if-no-gateway-e841635dcd20fd12.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/config-for-cephfs-volume-prefix-67f2513f603cb614.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/deprecate-old-ks-opts-in-nova-neutron-cinder-groups-e395015088d93fdc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fixing-driver-filter-14022294c8c04d2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-os-region-name-82e3cd4c7fb05ff4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/hnas-revert-to-snapshot-a2405cd6653b1e85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bp-update-share-type-name-or-description-a39c5991b930932f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1717392-fix-downgrade-share-access-map-bbd5fe9cc7002f2d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/qb-bug-1733807-581e71e6581de28e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/vnx-manila-ipv6-support-9ae986431549cc63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1661271-hnas-snapshot-readonly-4e50183100ed2b19.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/manage-share-in-zfsonlinux-driver-e80921081206f75b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/maprfs-manila-drivers-1541296f26cf78fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/qnap-manila-driver-a30fe4011cb90801.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1699836-disallow-share-type-deletion-with-active-share-group-types-83809532d06ef0dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1690159-retry-backend-init-58486ea420feaf51.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-export-locations-api-6fc6086c6a081faa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-share-type-filter-to-pool-list-api-267614b4d93j12de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-hsp-default-filter-function-0af60a819faabfec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1772647-b98025c07553e35d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-cdot-ss-multiple-dns-ip-df42a217977ce44d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/1841035-dellemc-unity-fix-ace-enable-error-b00281bb306d176b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-update-host-command-to-manila-manage-b32ad5017b564c9e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1716922-security-group-creation-failed-d46085d11370d918.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-ganesha-allow-access-for-all-ips-09773a79dc76ad44.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1650043-gpfs-access-bugs-8c10f26ff1f795f4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1882590-fix-svm-scoped-netapp-85b53830135f7558.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-AllocType-from-huawei-driver-8b279802f36efb00.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1666541-quobyte-resize-list-param-bc5b9c42bdc94c9f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-support-filtering-api-tracing-02d1f4271f44d24c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1591357-fix-cannot-remove-user-rule-for-NFS-8e1130e2accabd56.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-user-id-echo-8f42db469b27ff14.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1645751-fixed-shares-created-from-snapshots-for-lvm-and-generic-drivers-94a1161a9e0b5a85.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1774604-qb-driver-b7e717cbc71d6189.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-root-helper-config-option-fd517b0603031afa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/remove-confusing-deprecation-warnings-a17c20d8973ef2bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1879754-teardown-network-d1887cdf6eb83388.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/hnas-manage-unmanage-snapshot-support-0d939e1764c9ebb9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add_mtu_info_db-3c1d6dc02f40d5a6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1872243-netapp-fix-vserver-peer-with-same-vserver-8bc65816f1764784.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1651587-deny-access-verify-563ef2f3f6b8c13b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/inspur-instorage-driver-51d7a67f253f3ecd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/share-revert-to-snapshot-3d028fa00620651e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-ability-to-check-tenant-quota-usages-7fs17djahy61nsd6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/huawei-driver-support-snapshot-revert-1208c586bd8db98e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/cephfs-set-mode-b7fb3ec51300c220.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1861485-fix-share-network-retrieval-31768dcda5aeeaaa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1873963-netapp-fix-vserver-peer-intra-cluster-966398cf3a621edd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1859785-share-list-speed-6b09e7717624e037.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-share-group-quotas-4e426907eed4c000.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1700346-new-exception-for-no-default-share-type-b1dd9bbe8c9cb3df.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/cephfs-nfs-ipv6-support-2ffd9c0448c2f47e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/hsp-driver-e00aff5bc89d4b54.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/unity-un-handles-share-server-mode-support-e179c092ab148948.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/Use-http_proxy_to_wsgi-instead-of-ssl-middleware-df533a2c2d9c3a61.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/rules-for-managed-share-f28a26ffc980f6fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-tegile-driver-1859114513edb13e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml-5655800975cec5d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/newton-migration-improvements-cf9d3d6e37e19c94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1801763-gate-public-share-creation-by-policy-a0ad84e4127a3fc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/infinidat-delete-datasets-with-snapshots-4d18f8c197918606.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-consistency-groups-api-dd9b5b99138e22eb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/manage-unmanage-share-servers-cd4a6523d8e9fbdf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/add-two-new-fields-to-share-groups-api-bc576dddd58a3086.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1846836-fix-share-network-update-unexpected-success-eba8f40db392c467.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix_manage_snapshots_hnas-2c0e1a47b5e6ac33.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1749184-eb06929e76a14fce.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/netapp-cdot-configure-nfs-versions-83e3f319c4592c39.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/emc_vnx_interface_ports_configuration-00d454b3003ef981.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1773929-a5cb52c8417ec5fc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/infinidat-add-infinibox-driver-ec652258e710d6a0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/generic-driver-noop-interface-driver-24abcf7af1e08ff9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/fix-py3-netapp-a9815186ddc865d4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/notes/bug-1640169-check-ceph-connection-on-setup-c92bde41ced43326.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/ocata.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/mitaka.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/liberty.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/releasenotes/source/locale/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/releasenotes/source/locale/es/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/releasenotes/source/locale/es/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3126 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/releasenotes/source/locale/fr/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/releasenotes/source/locale/fr/LC_MESSAGES/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1464 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/_static/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8849 2020-07-31 09:55:01.000000 manila-9.1.4/releasenotes/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/ext/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/doc/ext/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2020-07-31 09:55:01.000000 manila-9.1.4/doc/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5834 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/development.environment.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8003 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/pool-aware-manila-scheduler.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8734 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/development-environment-devstack.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/share.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11338 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/driver_filter_goodness_weigher.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2105 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/api_microversion_history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/database.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/gerrit.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5056 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/manila-review-policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2425 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/services.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/manila.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8722 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/documenting_your_work.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/user_messages.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6923 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/adding_release_notes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14011 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/share_replication.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/contributor/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1727 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/samples/generic_local.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1417 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/samples/container_local.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/samples/zfsonlinux_local.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/samples/lvm_local.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/samples/cephfs_local.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/launchpad.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2691 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/commit_message_tags.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/auth.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1928 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/intro.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/i18n.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13395 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/rpc.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4368 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/guru_meditation_report.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5736 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/tempest_tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6089 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/scheduler.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2823 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/addmethod.openstackapi.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3087 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/architecture.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/threading.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11790 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/ganesha.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9531 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/driver_requirements.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1820 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/fakes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17007 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/share_migration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10987 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/api_microversion_dev.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3406 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/experimental_apis.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2538 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/unit_tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/contributor/share_hooks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3845 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/install/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/install/figures/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4026 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/figures/hwreqs.graffle
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41667 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/figures/hwreqs.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    90834 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/figures/hwreqs.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/verify.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2772 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/post-install.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/install-controller-debian.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/install-share-node.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1512 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/install-controller-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1700 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/install-controller-ubuntu.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/install/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1976 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/common/share-node-share-server-modes.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9829 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/common/controller-node-prerequisites.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17241 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/common/dhss-true-mode-using-shared-file-systems.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/common/dhss-false-mode-intro.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2956 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/common/dhss-true-mode-configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10613 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/common/dhss-false-mode-using-shared-file-systems.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3289 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/common/dhss-false-mode-configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/common/dhss-true-mode-intro.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2339 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/common/controller-node-common-configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2453 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/common/share-node-common-configuration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1705 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/get-started-with-shared-file-systems.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/install-controller-node.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2486 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/install-share-obs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/install-controller-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2469 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/install-share-debian.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9951 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2960 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/install-share-rdo.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2685 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/install-share-ubuntu.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/install/next-steps.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/cli/manila-status.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/cli/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    93595 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/cli/manila.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2947 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/cli/manila-manage.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41327 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/user/create-and-manage-shares.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/user/API.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28568 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/user/troubleshooting-asynchronous-failures.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25834 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/user/share-network-operations.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9633 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/user/share-network-subnet-operations.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/images/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/images/rpc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44964 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/images/rpc/rabt.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35906 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/images/rpc/flow1.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26690 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/images/rpc/arch.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30650 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/images/rpc/flow2.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38543 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/images/rpc/state.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40982 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/images/rpc/flow1.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33799 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/images/rpc/rabt.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18472 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/images/rpc/arch.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24552 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/images/rpc/flow2.svg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   161826 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/images/rpc/hds_network.jpg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/admin/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14569 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/capabilities_and_extra_specs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-share-management.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8112 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-share-server-management.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52434 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/share_back_ends_feature_support_mapping.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10105 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-manage-and-unmanage-share.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6001 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/zfs_on_linux_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44384 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-crud-share.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3119 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-troubleshoot.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7412 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-quotas.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6481 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/glusterfs_native_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13443 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-share-migration.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8312 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/emc_unity_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2939 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13285 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/emc_vnx_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4548 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-manage-and-unmanage-snapshot.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8579 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-security-services.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4568 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/container_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-multi-backend.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/nexentastor5_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18893 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/cephfs_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-share-resize.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9514 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/huawei_nas_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7286 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-share-types.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4877 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-key-concepts.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32359 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-share-replication.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4747 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-network-plugins.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21609 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/hitachi_hnas_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11690 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/hpe_3par_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/export_location_metadata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7752 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-snapshots.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4484 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/generic_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-networking.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3118 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/emc_isilon_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/hdfs_native_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4392 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/group_capabilities_and_extra_specs.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3561 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/gpfs_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7261 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/tegile_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3743 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/netapp_cluster_mode_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21261 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-share-networks.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-services-manage.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7697 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/glusterfs_driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/admin/shared-file-systems-scheduling.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/reference/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/reference/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3705 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/reference/glossary.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/configuration/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/configuration/figures/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   155457 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/figures/hsp_network.png
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77400 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/figures/openstack-spectrumscale-setup.JPG
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   161826 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/figures/hds_network.jpg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/configuration/tables/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-infinidat.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1105 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-powermax.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-quota.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2640 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-nexentastor5.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3625 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-netapp.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-glusterfs.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-san.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2204 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-zfssa.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-hnas.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1080 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-vnx.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1854 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-compute.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-spectrumscale_ces.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-hds_hsp.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-spectrumscale_knfs.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1273 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-hdfs.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-tegile.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-emc.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9644 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-generic.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2121 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-hpe3par.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-lvm.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3223 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-zfs.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2711 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-hds_hnas.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1365 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-winrm.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-redis.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-cephfs.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8295 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-common.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-quobyte.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5686 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-share.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-maprfs.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2114 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-scheduler.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-huawei.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-api.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-unity.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1472 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-ganesha.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/tables/manila-ca.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4221 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/overview.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25612 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/hpe-3par-share-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7044 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/hitachi-hsp-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11586 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/dell-emc-unity-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/windows-smb-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8932 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/cephfs-native-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4022 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/maprfs-native-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1997 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/netapp-cluster-mode-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2506 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/glusterfs-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16789 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/hitachi-hnas-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3672 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/huawei-nas-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18527 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/dell-emc-powermax-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/lvm-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/quobyte-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4702 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/zfssa-manila-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4385 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/glusterfs-native-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2213 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/hdfs-native-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3990 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/infinidat-share-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/nexentastor5-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3399 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/generic-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/emc-isilon-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9970 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/dell-emc-vnx-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5402 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/ibm-spectrumscale-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5358 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/zfs-on-linux-driver.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/api.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/samples/policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/samples/api-paste.ini.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/samples/rootwrap.conf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/samples/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/samples/manila.conf.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/samples/sample_policy.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/config-options.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/log-files.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/configuration/shared-file-systems/drivers.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8757 2020-07-31 09:55:01.000000 manila-9.1.4/doc/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2020-07-31 09:55:01.000000 manila-9.1.4/doc/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   124905 2020-07-31 09:56:46.000000 manila-9.1.4/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4125 2020-07-31 09:55:01.000000 manila-9.1.4/HACKING.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2401 2020-07-31 09:55:01.000000 manila-9.1.4/tools/install_venv.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2472 2020-07-31 09:55:01.000000 manila-9.1.4/tools/cover.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      198 2020-07-31 09:55:01.000000 manila-9.1.4/tools/with_venv.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5959 2020-07-31 09:55:01.000000 manila-9.1.4/tools/install_venv_common.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1197 2020-07-31 09:55:01.000000 manila-9.1.4/tools/check_exec.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1883 2020-07-31 09:55:01.000000 manila-9.1.4/tools/coding-checks.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2020-07-31 09:55:01.000000 manila-9.1.4/tools/fast8.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      435 2020-07-31 09:55:01.000000 manila-9.1.4/tools/check_logging.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1991 2020-07-31 09:55:01.000000 manila-9.1.4/tools/test-setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2020-07-31 09:55:01.000000 manila-9.1.4/tools/validate-json-files.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1223 2020-07-31 09:55:01.000000 manila-9.1.4/tools/enable-pre-commit-hook.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-07-31 09:56:46.000000 manila-9.1.4/manila.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2020-07-31 09:56:46.000000 manila-9.1.4/manila.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2020-07-31 09:56:46.000000 manila-9.1.4/manila.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2653 2020-07-31 09:56:46.000000 manila-9.1.4/manila.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2207 2020-07-31 09:56:46.000000 manila-9.1.4/manila.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      887 2020-07-31 09:56:46.000000 manila-9.1.4/manila.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2020-07-31 09:56:46.000000 manila-9.1.4/manila.egg-info/top_level.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    87355 2020-07-31 09:56:47.000000 manila-9.1.4/manila.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3945 2020-07-31 09:56:47.000000 manila-9.1.4/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15015 2020-07-31 09:55:01.000000 manila-9.1.4/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2524 2020-07-31 09:55:01.000000 manila-9.1.4/lower-constraints.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2207 2020-07-31 09:56:47.000000 manila-9.1.4/PKG-INFO
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/contrib/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/contrib/ci/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11564 2020-07-31 09:55:01.000000 manila-9.1.4/contrib/ci/pre_test_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18768 2020-07-31 09:55:01.000000 manila-9.1.4/contrib/ci/post_test_hook.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3249 2020-07-31 09:55:01.000000 manila-9.1.4/contrib/ci/common.sh
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/contrib/share_driver_hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3264 2020-07-31 09:55:01.000000 manila-9.1.4/contrib/share_driver_hooks/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2020-07-31 09:55:01.000000 manila-9.1.4/contrib/share_driver_hooks/zaqarclientwrapper.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7606 2020-07-31 09:55:01.000000 manila-9.1.4/contrib/share_driver_hooks/zaqar_notification_example_consumer.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2020-07-31 09:55:01.000000 manila-9.1.4/contrib/share_driver_hooks/zaqar_notification.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5462 2020-07-31 09:55:01.000000 manila-9.1.4/manila/manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/testing/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2033 2020-07-31 09:55:01.000000 manila-9.1.4/manila/testing/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14124 2020-07-31 09:55:01.000000 manila-9.1.4/manila/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9218 2020-07-31 09:55:01.000000 manila-9.1.4/manila/opts.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2038 2020-07-31 09:55:01.000000 manila-9.1.4/manila/cmd/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2020-07-31 09:55:01.000000 manila-9.1.4/manila/cmd/status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2324 2020-07-31 09:55:01.000000 manila-9.1.4/manila/cmd/share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1993 2020-07-31 09:55:01.000000 manila-9.1.4/manila/cmd/scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16773 2020-07-31 09:55:01.000000 manila-9.1.4/manila/cmd/manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1824 2020-07-31 09:55:01.000000 manila-9.1.4/manila/cmd/data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6623 2020-07-31 09:55:01.000000 manila-9.1.4/manila/coordination.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9216 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/integrated/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4074 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/integrated/integrated_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/integrated/test_extensions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/integrated/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7943 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/integrated/api/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/integrated/api/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/integrated/test_login.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/integrated/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/monkey_patch_example/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/monkey_patch_example/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/monkey_patch_example/example_b.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/monkey_patch_example/example_a.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2516 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_context.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2638 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7439 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/fake_volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6461 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/fake_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31543 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/declare_conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28595 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_quota.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/var/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/var/certificate.crt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3243 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/var/privatekey.key
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/var/ca.crt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/cmd/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/cmd/test_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/cmd/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/cmd/test_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16568 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/cmd/test_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2650 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/cmd/test_share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/cmd/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1930 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/cmd/test_scheduler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7087 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3813 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/fake_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23735 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_exception.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/message/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4034 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/message/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/message/test_message_field.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/message/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12928 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/test_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17041 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/test_common.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7242 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/middleware/test_faults.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/middleware/test_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/middleware/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10291 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6482 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43534 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11173 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   123281 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5253 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_access_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31485 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10091 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14201 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3061 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8250 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    42707 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24584 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14031 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_group_type_specs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41142 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6756 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_quota_class_sets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/stubs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29183 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7500 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20279 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4272 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19617 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4264 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5162 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_accesses.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28145 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_quota_sets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43485 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v2/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6444 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/test_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/test_wsgi.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/api/extensions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/extensions/foxinsocks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/extensions/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10737 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/test_share_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12231 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50009 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12711 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/test_share_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16809 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29297 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9179 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/test_share_unmanage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3997 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/stubs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19856 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/test_security_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21264 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15491 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/v1/test_share_types_extra_specs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/api/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36783 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/openstack/test_wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1318 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/openstack/test_versioned_method.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7204 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/openstack/test_api_version_request.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/api/views/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4505 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/views/test_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9174 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/views/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3123 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/views/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3449 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/views/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/views/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2672 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/views/test_quota_class_sets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/views/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3676 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/views/test_share_accesses.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3032 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/views/test_quota_sets.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/api/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6426 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/contrib/stubs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9021 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3303 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/api/test_middleware.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2940 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/compute/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14787 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/compute/test_nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5187 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/policy.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3768 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_coordination.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22395 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/network/test_standalone_network_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/network/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29629 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/network/linux/test_ip_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10810 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/network/linux/test_interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/network/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2879 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/network/linux/test_ovs_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/network/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/network/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25079 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/network/neutron/test_neutron_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/network/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    80282 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/network/neutron/test_neutron_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3734 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/fake_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8315 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10226 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/fake_share.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/common/test_config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/common/test_client_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share_group/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67039 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share_group/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share_group/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5205 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share_group/test_share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/fake_client_exception_class.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/scheduler/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/scheduler/weighers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6096 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/weighers/test_goodness.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2310 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/weighers/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6734 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/weighers/test_pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/weighers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11604 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/weighers/test_capacity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1932 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/test_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/scheduler/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3941 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/drivers/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24866 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/drivers/test_filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/drivers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7227 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/drivers/test_simple.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/scheduler/filters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5506 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5041 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_share_replication.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6789 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3977 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1813 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13678 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_json.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2535 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_extra_specs_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13943 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_capacity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_base_host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1961 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_ignore_attempted_hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5002 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/filters/test_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/scheduler/evaluator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/evaluator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6397 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/evaluator/test_evaluator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5397 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/test_rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5241 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/test_scheduler_options.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17325 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50972 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/test_host_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18215 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/scheduler/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11513 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/data/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12362 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/data/test_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/data/test_rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17101 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/data/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/xenapi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/xenapi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   185082 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   112216 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/test_service_instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/ns4/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/ns4/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/ns4/test_jsonrpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21864 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/ns4/test_nexenta_nas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/ns5/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/ns5/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43244 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/ns5/test_jsonrpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21901 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/nexenta/ns5/test_nexenta_nas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29267 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dummy.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/cephfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/cephfs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34637 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/cephfs/test_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/quobyte/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/quobyte/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30335 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/quobyte/test_quobyte.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9274 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/quobyte/test_jsonrpc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/veritas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23062 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/veritas/test_veritas_isa.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/veritas/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/infinidat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/infinidat/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34428 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/infinidat/test_infinidat.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    81517 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/test_generic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/glusterfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34537 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/glusterfs/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/glusterfs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12949 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/glusterfs/test_layout.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11019 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/glusterfs/test_glusterfs_native.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20419 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/glusterfs/test_layout_directory.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    43974 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/glusterfs/test_layout_volume.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16422 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/windows/test_service_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11513 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/windows/test_winrm_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16819 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/windows/test_windows_smb_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16351 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/windows/test_windows_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12572 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/windows/test_windows_smb_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/common/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/common/enas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5480 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/common/enas/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/common/enas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8039 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/common/enas/test_connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5426 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/common/enas/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    62668 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/common/enas/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/powermax/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   129908 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/powermax/test_object_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/powermax/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    97801 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/powermax/test_connection.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32726 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/mocked_unity.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4165 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10005 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9948 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/mocked_manila.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29576 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/test_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1852 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/fake_exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1188 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12845 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/res_mock.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/vnx/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   129829 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/vnx/test_object_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/vnx/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    97830 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/vnx/test_connection.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/isilon/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47173 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/isilon/test_isilon.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/isilon/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33695 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/isilon/test_isilon_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5427 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/dell_emc/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34944 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/test_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26861 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/test_ganesha.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/netapp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17245 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6384 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/protocols/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/protocols/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8233 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/protocols/test_nfs_cmode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/protocols/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8193 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/protocols/test_cifs_cmode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2140 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/protocols/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/client/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10300 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/client/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   251283 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/client/test_client_cmode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/client/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    89414 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/client/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6708 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/client/test_client_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44077 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8723 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_single_svm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    34182 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_performance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27411 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_data_motion.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   234139 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46881 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_multi_svm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_driver_interfaces.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/zfsonlinux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19480 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/zfsonlinux/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/zfsonlinux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   105631 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/zfsonlinux/test_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/huawei/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   195581 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/huawei/test_huawei_nas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/huawei/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/maprfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/maprfs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    38617 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/maprfs/test_maprfs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/infortrend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13722 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/infortrend/fake_infortrend_nas_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/infortrend/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15687 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/infortrend/fake_infortrend_manila_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22147 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/infortrend/test_infortrend_nas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/hpe/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    41497 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hpe/test_hpe_3par_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hpe/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   129857 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hpe/test_hpe_3par_mediator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7526 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hpe/test_hpe_3par_constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/ganesha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5410 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/ganesha/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/ganesha/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    48140 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/ganesha/test_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/qnap/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36904 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/qnap/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    64958 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/qnap/test_qnap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/qnap/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23015 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/qnap/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/zfssa/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/zfssa/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18386 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/zfssa/test_zfssarest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20186 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/zfssa/test_zfssashare.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19168 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/test_glusterfs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/tegile/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32531 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/tegile/test_tegile.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/tegile/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/container/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12495 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/container/test_protocol_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8047 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/container/test_storage_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11362 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/container/test_container_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/container/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3526 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/container/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21069 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/container/test_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/ibm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    76139 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/ibm/test_gpfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/ibm/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/hsp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12853 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/hsp/test_rest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/hsp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/hsp/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22885 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/hsp/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/hnas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/hnas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    65624 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/hnas/test_ssh.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53836 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hitachi/hnas/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    29240 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/test_lvm.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/inspur/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/inspur/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/inspur/instorage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51564 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/inspur/instorage/test_instorage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/inspur/instorage/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/inspur/as13000/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50841 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/inspur/as13000/test_as13000_nas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/inspur/as13000/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/share/drivers/hdfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hdfs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22812 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/drivers/hdfs/test_hdfs_native.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12927 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5780 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_drivers_private_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16750 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7019 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_snapshot_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   345716 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36129 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8533 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_share_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12744 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_hook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19883 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47730 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/share/test_driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2504 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/fake_notifier.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5309 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_misc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3748 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/conf_fixture.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13859 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_hacking.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4343 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3083 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/fake_compute.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2124 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/test_api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/db/migrations/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/db/migrations/alembic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7533 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/migrations/alembic/test_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   114195 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/migrations/alembic/migrations_data_checks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/migrations/alembic/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/migrations/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2852 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/test_migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   162221 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/sqlalchemy/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11647 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/sqlalchemy/test_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/db/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/runtime_conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1920 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/fake_service_instance.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/volume/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/volume/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11477 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/volume/test_cinder.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/test_rpc.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/tests/wsgi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1473 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/wsgi/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1847 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/wsgi/test_wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/wsgi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2967 2020-07-31 09:55:01.000000 manila-9.1.4/manila/tests/fake_zfssa.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/message/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3363 2020-07-31 09:55:01.000000 manila-9.1.4/manila/message/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5607 2020-07-31 09:55:01.000000 manila-9.1.4/manila/message/message_field.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/message/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2020-07-31 09:55:01.000000 manila-9.1.4/manila/message/message_levels.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2020-07-31 09:55:01.000000 manila-9.1.4/manila/i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/api/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16382 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/common.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/api/middleware/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/middleware/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5673 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/middleware/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/middleware/fault.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/api/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3475 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/quota_class_sets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14159 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/quota_sets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4156 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3105 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8977 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17104 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2529 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2933 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_access_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5259 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_group_type_specs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2270 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3238 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22855 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8331 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2874 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2967 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_accesses.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3987 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21285 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10250 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12328 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19581 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8237 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12518 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8303 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v2/share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10216 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/urlmap.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/api/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3316 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3440 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/share_unmanage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7611 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/share_types_extra_specs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8598 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/security_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/router.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5466 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/share_manage.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5539 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/share_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23487 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5974 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8173 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14157 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/v1/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/api/openstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/openstack/versioned_method.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/openstack/urlmap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50581 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/openstack/wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4857 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/openstack/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7945 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/openstack/rest_api_version_history.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12499 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/openstack/api_version_request.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11726 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/extensions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/api/views/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/quota_class_sets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2086 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/quota_sets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1203 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1818 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3418 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2245 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4043 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2821 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/security_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4412 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3732 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_accesses.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3592 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4795 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2238 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2226 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3724 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7544 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2899 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4136 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3737 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4927 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2470 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/views/share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/versions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/api/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2020-07-31 09:55:01.000000 manila-9.1.4/manila/api/auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5521 2020-07-31 09:55:01.000000 manila-9.1.4/manila/context.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1150 2020-07-31 09:55:01.000000 manila-9.1.4/manila/compute/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10118 2020-07-31 09:55:01.000000 manila-9.1.4/manila/compute/nova.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    46004 2020-07-31 09:55:01.000000 manila-9.1.4/manila/quota.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/network/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16423 2020-07-31 09:55:01.000000 manila-9.1.4/manila/network/standalone_network_plugin.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/network/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2111 2020-07-31 09:55:01.000000 manila-9.1.4/manila/network/linux/ovs_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9322 2020-07-31 09:55:01.000000 manila-9.1.4/manila/network/linux/interface.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/network/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15327 2020-07-31 09:55:01.000000 manila-9.1.4/manila/network/linux/ip_lib.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5316 2020-07-31 09:55:01.000000 manila-9.1.4/manila/network/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/network/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15309 2020-07-31 09:55:01.000000 manila-9.1.4/manila/network/neutron/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/network/neutron/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28372 2020-07-31 09:55:01.000000 manila-9.1.4/manila/network/neutron/neutron_network_plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2020-07-31 09:55:01.000000 manila-9.1.4/manila/network/neutron/constants.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3404 2020-07-31 09:55:01.000000 manila-9.1.4/manila/common/client_auth.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7441 2020-07-31 09:55:01.000000 manila-9.1.4/manila/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8041 2020-07-31 09:55:01.000000 manila-9.1.4/manila/common/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share_group/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21589 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share_group/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share_group/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5764 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share_group/share_group_types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/scheduler/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/scheduler/weighers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4577 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/weighers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4385 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/weighers/goodness.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1290 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/weighers/base_host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/weighers/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/weighers/pool.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4353 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/weighers/capacity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12735 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/scheduler/drivers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5148 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/drivers/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3213 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/drivers/simple.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2669 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/drivers/chance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19053 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/drivers/filter.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/scheduler/filters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1949 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/ignore_attempted_hosts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3722 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5018 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/json.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/base_host.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3768 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/scheduler/filters/share_group_filters/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1367 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/share_group_filters/consistent_snapshot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/share_group_filters/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2005 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/capabilities.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/share_replication.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5628 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/capacity.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/retry.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2476 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/filters/extra_specs_ops.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/base_handler.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3492 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/scheduler_options.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/scheduler/evaluator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7963 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/evaluator/evaluator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/evaluator/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5892 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28039 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/host_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7141 2020-07-31 09:55:01.000000 manila-9.1.4/manila/scheduler/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12023 2020-07-31 09:55:01.000000 manila-9.1.4/manila/data/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11255 2020-07-31 09:55:01.000000 manila-9.1.4/manila/data/helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2020-07-31 09:55:01.000000 manila-9.1.4/manila/data/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/data/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6520 2020-07-31 09:55:01.000000 manila-9.1.4/manila/data/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7514 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policy.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14081 2020-07-31 09:55:01.000000 manila-9.1.4/manila/test.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    92369 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   193858 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14049 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/share_types.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/nexenta/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/nexenta/ns4/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3015 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/nexenta/ns4/jsonrpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/nexenta/ns4/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9280 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/nexenta/ns4/nexenta_nfs_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5591 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/nexenta/ns4/nexenta_nas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/nexenta/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/nexenta/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5500 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/nexenta/options.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/nexenta/ns5/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22259 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/nexenta/ns5/jsonrpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/nexenta/ns5/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23368 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/nexenta/ns5/nexenta_nas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47119 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/generic.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/cephfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24279 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/cephfs/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/cephfs/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/cephfs/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/cephfs/conf/cephfs-export-template.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23003 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/lvm.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/quobyte/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4594 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/quobyte/jsonrpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/quobyte/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17458 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/quobyte/quobyte.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/veritas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/veritas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24817 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/veritas/veritas_isa.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/infinidat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20747 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/infinidat/infinibox.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/infinidat/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/glusterfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17160 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/glusterfs/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26056 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/glusterfs/layout_volume.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10105 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/glusterfs/layout.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12210 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/glusterfs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10092 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/glusterfs/layout_directory.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/glusterfs/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/glusterfs/conf/10-glusterfs-export-template.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9092 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/glusterfs/glusterfs_native.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6507 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/windows/winrm_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9382 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/windows/windows_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12818 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/windows/service_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11152 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/windows/windows_smb_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7586 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/windows/windows_smb_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/dell_emc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/dell_emc/common/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/dell_emc/common/enas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/common/enas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6518 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/common/enas/connector.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/common/enas/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5662 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/common/enas/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9979 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/common/enas/xml_api_parser.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8666 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/powermax/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    36163 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/powermax/connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/powermax/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    78716 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/powermax/object_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/unity/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13644 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/unity/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30083 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/unity/connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/unity/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/unity/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3053 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/vnx/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35440 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/vnx/connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/vnx/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    78121 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/vnx/object_manager.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/isilon/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13008 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/isilon/isilon_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/isilon/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20978 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugins/isilon/isilon.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1138 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/dell_emc/plugin_manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47925 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/service_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/netapp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7993 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8290 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/options.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/protocols/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2222 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/protocols/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6757 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/protocols/cifs_cmode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7363 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/protocols/nfs_cmode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/protocols/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/client/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23736 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/client/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   149686 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/client/client_cmode.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4329 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/client/client_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/client/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13137 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/drv_single_svm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19626 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/data_motion.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6360 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/lib_single_svm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23714 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/lib_multi_svm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13332 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/drv_multi_svm.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17313 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/performance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   107590 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/lib_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/zfsonlinux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67550 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/zfsonlinux/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/zfsonlinux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12003 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/zfsonlinux/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/huawei/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/huawei/v3/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52116 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/v3/helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7976 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/v3/smartx.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    77516 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/v3/connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1619 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/v3/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/v3/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10021 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/v3/replication.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4353 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/huawei_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3997 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11551 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/huawei/huawei_nas.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/maprfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19661 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/maprfs/maprfs_native.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/maprfs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13643 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/maprfs/driver_util.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/infortrend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26123 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/infortrend/infortrend_nas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10278 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/infortrend/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/infortrend/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25463 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/helpers.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/hpe/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    70114 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hpe/hpe_3par_mediator.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hpe/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26264 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hpe/hpe_3par_driver.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/ganesha/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22754 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/ganesha/manager.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12216 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/ganesha/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/ganesha/conf/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1180 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/ganesha/conf/00-base-export-template.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4819 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/ganesha/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/qnap/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40927 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/qnap/qnap.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27023 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/qnap/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/qnap/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/zfssa/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/zfssa/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12840 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/zfssa/restclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20977 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/zfssa/zfssashare.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18122 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/zfssa/zfssarest.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/tegile/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/tegile/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    19637 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/tegile/tegile.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/container/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7797 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/container/container_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16349 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/container/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/container/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5950 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/container/storage_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5656 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/container/protocol_helper.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/ibm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51201 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/ibm/gpfs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/ibm/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/hitachi/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/hitachi/hsp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7508 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hitachi/hsp/rest.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14434 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hitachi/hsp/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hitachi/hsp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hitachi/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/hitachi/hnas/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    55534 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hitachi/hnas/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hitachi/hnas/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    35481 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hitachi/hnas/ssh.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/inspur/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/inspur/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/inspur/instorage/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16234 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/inspur/instorage/cli_helper.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/inspur/instorage/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21558 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/inspur/instorage/instorage.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/inspur/as13000/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33764 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/inspur/as13000/as13000_nas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/inspur/as13000/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/drivers/hdfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16931 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hdfs/hdfs_native.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers/hdfs/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7399 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6143 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/drivers_private_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17684 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/rpcapi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   116258 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/driver.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2540 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/configuration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/hook.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24651 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7311 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/snapshot_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5258 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/share/hooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/share/hooks/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    25285 2020-07-31 09:55:01.000000 manila-9.1.4/manila/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/db/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    52848 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/db/migrations/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/db/migrations/alembic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1325 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/env.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2382 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/migration.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/db/migrations/alembic/versions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/211836bf835c_add_access_level.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9401 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/03da71c0e321_convert_cgs_to_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1701 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/d5db24264f5c_add_consistent_snapshot_support_attr_to_share_group_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/27cb96d991fa_add_description_for_share_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2040 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/87ce15c59bbe_add_revert_to_snapshot_support.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/55761e5f59c5_add_snapshot_support_extra_spec_to_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5841 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/3e7d62517afa_add_create_share_from_snapshot_support.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4836 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/1f0bd302c1a6_add_availability_zones_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/5155c7077f99_add_more_network_info_attributes_to_network_allocations_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2660 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/59eb64046740_add_required_extra_spec.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4287 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/344c1ac4747f_add_share_instance_access_rules_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5372 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/38e632621e5a_change_volume_type_to_share_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1771 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/3db9992c30f3_transform_statuses_to_lowercase.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3965 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/dda6de06349_add_export_locations_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2519 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/ef0c02b4366_add_share_type_projects.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5174 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/e1949a93157a_add_share_group_types_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16924 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/162a3e673105_manila_init.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/927920b37453_add_provider_location_for_share_group_snapshot_members_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/323840a08dc4_add_shares_task_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1511 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/829a09b0ddd4_fix_project_share_type_quotas_unique_constraint.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2027 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/238720805ce1_add_messages_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/533646c7af38_remove_unused_attr_status.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/95e3cf760840_remove_nova_net_id_column_from_share_.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1336 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/30cb96d995fa_add_is_public_column_for_share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3874 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/56cdbe267881_add_share_export_locations_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3211 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/48a7beae3117_move_share_type_id_to_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/221a83cfd85b_change_user_project_id_length.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7864 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/3651e16d7c43_add_consistency_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9838 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/805685098bd2_add_share_network_subnets_table_and_modify_share_servers_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/fdfb668d19e1_add_gateway_to_network_allocations_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/63809d875e32_add_access_key.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/493eaffd79e1_add_mtu_network_allocations_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3655 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/e9f79621d83f_add_cast_rules_to_readonly_to_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/17115072e1c3_add_nova_net_id_column_to_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/e8ea58723178_remove_host_from_driver_private_data.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3742 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/a77e2ad5012d_add_share_snapshot_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4145 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/579c267fbb4d_add_share_instances_access_map.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2086 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/11ee96se625f3_add_metadata_for_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6517 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/b10fb432c042_squash_share_group_snapshot_members_and_share_snapshot_instance_models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/293fac1130ca_add_replication_attrs.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/7d142971c4ef_add_reservation_expire_index.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/5237b6625330_add_availability_zone_id_field_to_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/6a3fd2984bc31_add_is_auto_deletable_and_identifier_fields_for_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/097fad24d2fc_add_share_instances_share_id_index.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/4ee2cf4be19a_remove_share_snapshots_export_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2090 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/3a482171410f_add_drivers_private_data_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/b516de97bfee_add_quota_per_share_type_model.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11818 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/5077ffcc5f1c_add_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/0274d20c560f_add_ou_to_security_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3675 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/54667b9cade7_restore_share_instance_access_map_state.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/eb6d5544cbbd_add_provider_location_to_share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/versions/4a482571410f_add_backends_info_table.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic/script.py.mako
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/alembic.ini
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migrations/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1366 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/migration.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/db/sqlalchemy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   184468 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/sqlalchemy/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/sqlalchemy/query.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    50263 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/sqlalchemy/models.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/sqlalchemy/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2020-07-31 09:55:01.000000 manila-9.1.4/manila/db/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/volume/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2020-07-31 09:55:01.000000 manila-9.1.4/manila/volume/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12923 2020-07-31 09:55:01.000000 manila-9.1.4/manila/volume/cinder.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/policies/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_group_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3049 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/quota_set.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_group_types_spec.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1513 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_export_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/availability_zone.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2015 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_instance_export_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2360 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_snapshot_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1553 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_access_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_network_subnet.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3972 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_replica.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1708 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_snapshot_instance_export_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2173 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_instance.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1549 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3695 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3390 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/security_service.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1744 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/message.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2463 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_types_extra_spec.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3206 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3270 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_group.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1614 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_replica_export_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_snapshot_export_location.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1624 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/quota_class_set.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3561 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_group_snapshot.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12283 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3091 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3967 2020-07-31 09:55:01.000000 manila-9.1.4/manila/policies/share_snapshot.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/hacking/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/hacking/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11630 2020-07-31 09:55:01.000000 manila-9.1.4/manila/hacking/checks.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/manila/wsgi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5145 2020-07-31 09:55:01.000000 manila-9.1.4/manila/wsgi/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2020-07-31 09:55:01.000000 manila-9.1.4/manila/wsgi/wsgi.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:55:01.000000 manila-9.1.4/manila/wsgi/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2020-07-31 09:55:01.000000 manila-9.1.4/manila/wsgi/eventlet_server.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2020-07-31 09:55:01.000000 manila-9.1.4/manila/version.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27060 2020-07-31 09:55:01.000000 manila-9.1.4/manila/exception.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4561 2020-07-31 09:55:01.000000 manila-9.1.4/manila/rpc.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1536 2020-07-31 09:55:01.000000 manila-9.1.4/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2020-07-31 09:55:01.000000 manila-9.1.4/babel.cfg
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-native/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-native/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3119 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-native/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3535 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3107 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-generic-scenario-custom-image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-generic-scenario-custom-image/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4252 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-generic-scenario-custom-image/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-zfsonlinux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-zfsonlinux/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3613 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-zfsonlinux/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-dummy/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-dummy/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3439 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-dummy/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-container/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-container/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3609 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-container/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-hdfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-hdfs/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2687 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-hdfs/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native-centos-7/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native-centos-7/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4571 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native-centos-7/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-native-heketi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-native-heketi/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3140 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-native-heketi/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4586 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-generic-singlebackend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-generic-singlebackend/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3571 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-generic-singlebackend/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-mysql-generic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-mysql-generic/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3535 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-mysql-generic/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-container-scenario-custom-image/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-container-scenario-custom-image/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4322 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-container-scenario-custom-image/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-nfs-centos-7/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-nfs-centos-7/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3771 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-nfs-centos-7/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs-heketi/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs-heketi/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3139 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs-heketi/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-dummy-py2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-dummy-py2/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-dummy-py2/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-scenario/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-scenario/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3530 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-scenario/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-native-centos-7/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-native-centos-7/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3786 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-native-centos-7/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/grenade-dsvm-manila/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/grenade-dsvm-manila/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2475 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/grenade-dsvm-manila/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs-centos-7/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs-centos-7/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4616 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs-centos-7/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4602 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/run.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4697 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/run-ipv6.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-generic-no-share-servers/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-generic-no-share-servers/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3559 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-generic-no-share-servers/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/playbooks/manila-tox-genconfig/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2020-07-31 09:55:01.000000 manila-9.1.4/playbooks/manila-tox-genconfig/post.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/api-ref/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/api-ref/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3086 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/scheduler-stats.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4148 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-instances.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2401 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-export-locations.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7633 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-groups.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/extensions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10058 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-networks.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1272 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2343 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-instance-export-locations.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3374 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/user-messages.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2685 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/quota-classes.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11193 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/snapshots.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1705 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/status.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15496 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-types.inc
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2020-07-31 09:56:47.000000 manila-9.1.4/api-ref/source/samples/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-network-remove-security-service-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-instances-list-with-detail-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-types-group-specs-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-type-revoke-access-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-types-list-access-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-shrink-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/versions-get-version-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1425 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-instance-actions-force-delete-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-show-metadata-item-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-type-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-replica-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       28 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-list-access-rules-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1168 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/shares-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-extend-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1450 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-manage-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-type-revoke-access-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/export-location-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-unmanage-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/service-enable-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/services-list-with-filters-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-type-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-network-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-force-delete-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/security-service-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-network-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-reset-state-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-list-access-rules-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      927 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/quota-classes-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-types-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/quota-classes-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-replicas-reset-replica-state-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2380 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-types-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-type-set-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-type-grant-access-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1820 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-networks-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1306 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-type-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-snapshot-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-network-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-actions-force-delete-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-access-rules-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-snapshots-list-members-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-show-instance-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-replicas-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-snapshot-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-update-null-metadata-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-access-rules-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-update-null-metadata-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/service-enable-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/quota-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-servers-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/security-service-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-server-manage-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-snapshot-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-types-default-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-revoke-access-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-set-metadata-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-network-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-replica-export-location-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/pools-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-show-metadata-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-replica-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-type-set-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/security-services-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-access-rules-update-metadata-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-snapshot-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3921 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/pools-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-replica-export-location-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-type-grant-access-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-instance-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-set-metadata-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1782 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-snapshots-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-replicas-reset-state-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-actions-reset-state-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-manage-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-grant-access-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-replicas-force-delete-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3373 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/extensions-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-snapshots-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1057 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1180 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/user-messages-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-network-remove-security-service-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1366 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/security-services-list-for-share-network-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-network-add-security-service-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/user-message-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-server-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3351 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/shares-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-network-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-network-add-security-service-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/service-disable-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-actions-unmanage-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-type-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-grant-access-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-reset-state-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/security-service-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-server-reset-state-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-manage-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1197 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-groups-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-type-set-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-instance-actions-reset-state-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-instance-actions-reset-state-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/availability-zones-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1141 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-replicas-list-detail-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-actions-revert-to-snapshot-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1306 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-type-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-snapshot-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/quota-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-type-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1507 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/versions-index-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1230 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/security-services-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/security-service-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-server-manage-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/quota-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/quota-classes-update-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-update-metadata-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/services-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-snapshot-actions-reset-state-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-types-extra-specs-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-access-rules-update-metadata-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1526 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-type-create-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-update-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-networks-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-types-list-access-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1184 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshots-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-instances-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-types-default-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/export-location-show-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/quota-show-detail-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-group-type-set-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      466 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-replicas-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/limits-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-update-metadata-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-server-unmanage-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/share-server-show-details-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/security-service-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-instances-list-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshots-list-detailed-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-manage-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/snapshot-create-request.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/samples/service-disable-response.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-access-rule-metadata.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/experimental.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9718 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-actions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2400 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-replica-export-locations.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7809 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/security-services.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3126 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/services.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4415 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/snapshot-instances.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    76827 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/parameters.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3132 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/versions.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8587 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-group-snapshots.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2006 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/limits.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17568 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/shares.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6517 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/quota-sets.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4605 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-metadata.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8561 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-servers.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/availability-zones.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9611 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-group-types.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3048 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-migration.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-access-rules.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10400 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/share-replicas.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9877 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3764 2020-07-31 09:55:01.000000 manila-9.1.4/api-ref/source/os-share-manage.inc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2020-07-31 09:55:01.000000 manila-9.1.4/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.339374 manila-9.1.5/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-02-01 17:27:42.000000 manila-9.1.5/.coveragerc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5470 2021-02-01 17:27:42.000000 manila-9.1.5/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-02-01 17:27:42.000000 manila-9.1.5/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15015 2021-02-01 17:27:42.000000 manila-9.1.5/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14110 2021-02-01 17:28:23.000000 manila-9.1.5/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2021-02-01 17:27:42.000000 manila-9.1.5/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   125696 2021-02-01 17:28:23.000000 manila-9.1.5/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4125 2021-02-01 17:27:42.000000 manila-9.1.5/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2021-02-01 17:27:42.000000 manila-9.1.5/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2207 2021-02-01 17:28:24.339374 manila-9.1.5/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1072 2021-02-01 17:27:42.000000 manila-9.1.5/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:23.987306 manila-9.1.5/api-ref/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.023313 manila-9.1.5/api-ref/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/availability-zones.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9877 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      476 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/experimental.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      821 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/extensions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1272 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2006 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/limits.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3764 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/os-share-manage.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    76827 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/parameters.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2685 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/quota-classes.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6517 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/quota-sets.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.051318 manila-9.1.5/api-ref/source/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/availability-zones-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/export-location-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      399 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/export-location-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3373 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/extensions-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      489 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/limits-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3921 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/pools-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      563 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/pools-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/quota-classes-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/quota-classes-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/quota-classes-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      916 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/quota-show-detail-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/quota-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/quota-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/quota-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/security-service-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/security-service-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      529 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/security-service-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/security-service-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      553 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/security-service-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1230 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/security-services-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1366 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/security-services-list-for-share-network-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/security-services-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/service-disable-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/service-disable-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/service-enable-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/service-enable-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/services-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/services-list-with-filters-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      965 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-access-rules-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      486 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-access-rules-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-access-rules-update-metadata-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      139 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-access-rules-update-metadata-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-extend-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-force-delete-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-grant-access-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-grant-access-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       28 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-list-access-rules-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      525 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-list-access-rules-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-reset-state-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-revert-to-snapshot-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-revoke-access-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-shrink-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-actions-unmanage-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      429 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1426 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1057 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-reset-state-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1112 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-snapshot-actions-reset-state-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-snapshot-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-snapshot-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-snapshot-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-snapshot-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      817 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-snapshot-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1782 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-snapshots-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      685 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-snapshots-list-members-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-snapshots-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-type-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-type-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-type-grant-access-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-type-revoke-access-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-type-set-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-type-set-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-types-default-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-types-group-specs-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-types-list-access-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-types-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1098 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-group-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1197 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-groups-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-instance-actions-force-delete-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-instance-actions-reset-state-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1122 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-instances-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      588 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-manage-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1450 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-manage-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-network-add-security-service-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-network-add-security-service-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      248 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-network-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      599 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-network-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-network-remove-security-service-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      503 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-network-remove-security-service-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      577 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-network-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      255 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-network-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      618 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-network-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1820 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-networks-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      354 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-networks-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-replica-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-replica-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      804 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-replica-export-location-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      473 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-replica-export-location-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-replicas-force-delete-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1141 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-replicas-list-detail-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      466 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-replicas-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-replicas-reset-replica-state-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-replicas-reset-state-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      532 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-replicas-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      268 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-server-manage-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-server-manage-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-server-reset-state-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      421 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-server-show-details-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-server-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       44 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-server-unmanage-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-servers-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-set-metadata-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-set-metadata-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      560 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-show-instance-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       52 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-show-metadata-item-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-show-metadata-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1526 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-type-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1306 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-type-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-type-grant-access-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-type-revoke-access-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-type-set-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-type-set-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      840 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-type-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      136 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-type-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1306 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-type-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      828 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-types-default-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-types-extra-specs-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-types-list-access-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2380 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-types-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-update-metadata-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      133 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-update-metadata-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-update-null-metadata-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-update-null-metadata-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1425 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/share-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3351 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/shares-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1168 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/shares-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       29 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-actions-force-delete-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-actions-reset-state-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       25 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-actions-unmanage-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-create-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-create-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-instance-actions-reset-state-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-instance-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-instances-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      640 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-instances-list-with-detail-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      344 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-manage-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      992 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-manage-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      927 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-update-request.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      961 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshot-update-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2039 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshots-list-detailed-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1184 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/snapshots-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1075 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/user-message-show-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1180 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/user-messages-list-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/versions-get-version-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1507 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/samples/versions-index-response.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3086 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/scheduler-stats.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7809 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/security-services.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3126 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/services.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1725 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-access-rule-metadata.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2301 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-access-rules.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9718 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-actions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2401 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-export-locations.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8587 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-group-snapshots.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9611 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-group-types.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7633 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-groups.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2343 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-instance-export-locations.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4148 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-instances.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4605 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-metadata.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3048 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-migration.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10058 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-networks.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2400 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-replica-export-locations.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10400 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-replicas.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8561 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-servers.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15496 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/share-types.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17568 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/shares.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4415 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/snapshot-instances.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11193 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/snapshots.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1705 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/status.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3374 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/user-messages.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3132 2021-02-01 17:27:42.000000 manila-9.1.5/api-ref/source/versions.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       17 2021-02-01 17:27:42.000000 manila-9.1.5/babel.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2021-02-01 17:27:42.000000 manila-9.1.5/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:23.987306 manila-9.1.5/contrib/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/contrib/ci/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3249 2021-02-01 17:27:42.000000 manila-9.1.5/contrib/ci/common.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18768 2021-02-01 17:27:42.000000 manila-9.1.5/contrib/ci/post_test_hook.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11530 2021-02-01 17:27:42.000000 manila-9.1.5/contrib/ci/pre_test_hook.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/contrib/share_driver_hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3264 2021-02-01 17:27:42.000000 manila-9.1.5/contrib/share_driver_hooks/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4925 2021-02-01 17:27:42.000000 manila-9.1.5/contrib/share_driver_hooks/zaqar_notification.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     7606 2021-02-01 17:27:42.000000 manila-9.1.5/contrib/share_driver_hooks/zaqar_notification_example_consumer.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2808 2021-02-01 17:27:42.000000 manila-9.1.5/contrib/share_driver_hooks/zaqarclientwrapper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/devstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      712 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      829 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/apache-manila.template
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:23.991307 manila-9.1.5/devstack/files/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/devstack/files/debs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/files/debs/manila
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/devstack/files/rpms/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/files/rpms/manila
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/devstack/files/rpms-suse/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        5 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/files/rpms-suse/manila
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    57308 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/plugin.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12058 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/settings
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/devstack/upgrade/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/devstack/upgrade/from-mitaka/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/upgrade/from-mitaka/upgrade-manila
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/devstack/upgrade/from-newton/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      587 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/upgrade/from-newton/upgrade-manila
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    19579 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/upgrade/resources.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/upgrade/settings
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      464 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/upgrade/shutdown.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2189 2021-02-01 17:27:42.000000 manila-9.1.5/devstack/upgrade/upgrade.sh
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      865 2021-02-01 17:27:42.000000 manila-9.1.5/doc/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.055319 manila-9.1.5/doc/ext/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/doc/ext/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      561 2021-02-01 17:27:42.000000 manila-9.1.5/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.059320 manila-9.1.5/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.063321 manila-9.1.5/doc/source/admin/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13205 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/capabilities_and_extra_specs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18893 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/cephfs_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4568 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/container_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3118 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/emc_isilon_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8312 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/emc_unity_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13285 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/emc_vnx_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1819 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/export_location_metadata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4484 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/generic_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7697 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/glusterfs_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6481 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/glusterfs_native_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3561 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/gpfs_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1976 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/group_capabilities_and_extra_specs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/hdfs_native_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21609 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/hitachi_hnas_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11690 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/hpe_3par_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9514 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/huawei_nas_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2939 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3743 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/netapp_cluster_mode_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/nexentastor5_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52434 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/share_back_ends_feature_support_mapping.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44384 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-crud-share.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4877 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-key-concepts.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10105 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-manage-and-unmanage-share.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4548 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-manage-and-unmanage-snapshot.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2036 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-multi-backend.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4747 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-network-plugins.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      568 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-networking.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7412 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-quotas.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-scheduling.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8579 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-security-services.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      760 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-services-manage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1282 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-share-management.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13443 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-share-migration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21261 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-share-networks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32359 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-share-replication.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-share-resize.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8112 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-share-server-management.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14500 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-share-types.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7752 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-snapshots.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3119 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/shared-file-systems-troubleshoot.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7261 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/tegile_driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6001 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/admin/zfs_on_linux_driver.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.067321 manila-9.1.5/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      708 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/cli/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2947 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/cli/manila-manage.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1765 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/cli/manila-status.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    93595 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/cli/manila.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8757 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.067321 manila-9.1.5/doc/source/configuration/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.067321 manila-9.1.5/doc/source/configuration/figures/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   161826 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/figures/hds_network.jpg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   155457 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/figures/hsp_network.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77400 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/figures/openstack-spectrumscale-setup.JPG
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      410 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.067321 manila-9.1.5/doc/source/configuration/shared-file-systems/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      602 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/config-options.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.071322 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8932 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/cephfs-native-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18527 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/dell-emc-powermax-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11586 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/dell-emc-unity-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9970 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/dell-emc-vnx-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2023 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/emc-isilon-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3399 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/generic-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2506 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/glusterfs-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4385 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/glusterfs-native-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2213 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/hdfs-native-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16789 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/hitachi-hnas-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7044 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/hitachi-hsp-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25612 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/hpe-3par-share-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3672 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/huawei-nas-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5402 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/ibm-spectrumscale-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3990 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/infinidat-share-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2464 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/lvm-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4022 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/maprfs-native-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1997 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/netapp-cluster-mode-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2136 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/nexentastor5-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/quobyte-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/windows-smb-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5358 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/zfs-on-linux-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4702 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/zfssa-manila-driver.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2153 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/drivers.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      929 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/log-files.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4221 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/overview.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.075323 manila-9.1.5/doc/source/configuration/shared-file-systems/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      223 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/samples/api-paste.ini.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      356 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/samples/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      540 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/samples/manila.conf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      374 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/samples/policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      303 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/samples/rootwrap.conf.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      754 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/shared-file-systems/samples/sample_policy.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.079324 manila-9.1.5/doc/source/configuration/tables/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3311 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-api.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      777 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-ca.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1090 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-cephfs.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8295 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-common.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1854 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-compute.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1460 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-emc.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1472 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-ganesha.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9644 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-generic.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2898 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-glusterfs.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1273 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-hdfs.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2711 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-hds_hnas.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-hds_hsp.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      799 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-hnas.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2121 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-hpe3par.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      814 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-huawei.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      983 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-infinidat.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1373 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-lvm.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1663 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-maprfs.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3625 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-netapp.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2640 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-nexentastor5.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1105 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-powermax.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1482 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-quobyte.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1781 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-quota.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1625 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-redis.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      946 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-san.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2114 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-scheduler.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5686 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-share.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-spectrumscale_ces.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2034 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-spectrumscale_knfs.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1044 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-tegile.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-unity.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1080 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-vnx.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1365 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-winrm.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3223 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-zfs.inc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2204 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/configuration/tables/manila-zfssa.inc
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.087325 manila-9.1.5/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6923 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/adding_release_notes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2823 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/addmethod.openstackapi.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3672 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/apache-httpd.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10987 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/api_microversion_dev.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/api_microversion_history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3087 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/architecture.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1435 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/auth.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2691 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/commit_message_tags.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/database.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8734 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/development-environment-devstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5834 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/development.environment.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8722 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/documenting_your_work.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11338 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/driver_filter_goodness_weigher.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14560 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/driver_requirements.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3406 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/experimental_apis.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1820 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/fakes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11790 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/ganesha.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      565 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/gerrit.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4368 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/guru_meditation_report.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1504 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/i18n.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2121 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1928 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/intro.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1645 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/launchpad.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5056 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/manila-review-policy.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1936 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/manila.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8003 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/pool-aware-manila-scheduler.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13395 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/rpc.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.087325 manila-9.1.5/doc/source/contributor/samples/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1433 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/samples/cephfs_local.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1417 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/samples/container_local.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1727 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/samples/generic_local.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1495 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/samples/lvm_local.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1527 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/samples/zfsonlinux_local.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6089 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/scheduler.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2425 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/services.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/share.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/share_hooks.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17007 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/share_migration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14011 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/share_replication.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5736 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/tempest_tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2712 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/threading.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2538 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/unit_tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/contributor/user_messages.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:23.991307 manila-9.1.5/doc/source/images/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.091326 manila-9.1.5/doc/source/images/rpc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26690 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/images/rpc/arch.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18472 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/images/rpc/arch.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40982 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/images/rpc/flow1.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35906 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/images/rpc/flow1.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30650 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/images/rpc/flow2.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24552 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/images/rpc/flow2.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   161826 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/images/rpc/hds_network.jpg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44964 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/images/rpc/rabt.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33799 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/images/rpc/rabt.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38543 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/images/rpc/state.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3845 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.095327 manila-9.1.5/doc/source/install/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.095327 manila-9.1.5/doc/source/install/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2339 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/common/controller-node-common-configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9829 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/common/controller-node-prerequisites.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3289 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/common/dhss-false-mode-configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      497 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/common/dhss-false-mode-intro.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10613 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/common/dhss-false-mode-using-shared-file-systems.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2956 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/common/dhss-true-mode-configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      894 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/common/dhss-true-mode-intro.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17260 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/common/dhss-true-mode-using-shared-file-systems.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2453 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/common/share-node-common-configuration.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1976 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/common/share-node-share-server-modes.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9951 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.095327 manila-9.1.5/doc/source/install/figures/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4026 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/figures/hwreqs.graffle
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    90834 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/figures/hwreqs.png
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41667 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/figures/hwreqs.svg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1705 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/get-started-with-shared-file-systems.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2772 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1476 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/install-controller-debian.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      704 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/install-controller-node.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1512 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/install-controller-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/install-controller-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1700 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/install-controller-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2469 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/install-share-debian.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      900 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/install-share-node.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2486 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/install-share-obs.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2960 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/install-share-rdo.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2685 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/install-share-ubuntu.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      447 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/next-steps.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/post-install.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/install/verify.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.099328 manila-9.1.5/doc/source/reference/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3705 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/reference/glossary.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/reference/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.099328 manila-9.1.5/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/user/API.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44798 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/user/create-and-manage-shares.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      769 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25834 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/user/share-network-operations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9633 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/user/share-network-subnet-operations.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28568 2021-02-01 17:27:42.000000 manila-9.1.5/doc/source/user/troubleshooting-asynchronous-failures.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:23.991307 manila-9.1.5/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.099328 manila-9.1.5/etc/manila/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-02-01 17:27:42.000000 manila-9.1.5/etc/manila/README.manila.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1886 2021-02-01 17:27:42.000000 manila-9.1.5/etc/manila/api-paste.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1271 2021-02-01 17:27:42.000000 manila-9.1.5/etc/manila/logging_sample.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2021-02-01 17:27:42.000000 manila-9.1.5/etc/manila/manila-policy-generator.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      988 2021-02-01 17:27:42.000000 manila-9.1.5/etc/manila/rootwrap.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.099328 manila-9.1.5/etc/manila/rootwrap.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8112 2021-02-01 17:27:42.000000 manila-9.1.5/etc/manila/rootwrap.d/share.filters
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.099328 manila-9.1.5/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      274 2021-02-01 17:27:42.000000 manila-9.1.5/etc/oslo-config-generator/manila.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.099328 manila-9.1.5/httpd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-02-01 17:27:42.000000 manila-9.1.5/httpd/manila-uwsgi.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      569 2021-02-01 17:27:42.000000 manila-9.1.5/httpd/mod_wsgi-manila.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2021-02-01 17:27:42.000000 manila-9.1.5/httpd/uwsgi-manila.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2525 2021-02-01 17:27:42.000000 manila-9.1.5/lower-constraints.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.103328 manila-9.1.5/manila/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.107329 manila-9.1.5/manila/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      885 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1397 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16382 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.107329 manila-9.1.5/manila/api/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1204 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11726 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/extensions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.107329 manila-9.1.5/manila/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5673 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/middleware/auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/middleware/fault.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.107329 manila-9.1.5/manila/api/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4857 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12499 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/openstack/api_version_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7945 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/openstack/rest_api_version_history.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1010 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/openstack/urlmap.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/openstack/versioned_method.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50581 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/openstack/wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10216 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/urlmap.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.111330 manila-9.1.5/manila/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14157 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3316 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8598 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/security_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5871 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/share_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5539 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/share_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5974 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8173 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7611 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/share_types_extra_specs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3440 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/share_unmanage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23487 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v1/shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.115331 manila-9.1.5/manila/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2270 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3238 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3475 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/quota_class_sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14159 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/quota_sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22855 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/router.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4156 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3142 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_access_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2967 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_accesses.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8331 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5259 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_group_type_specs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10250 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12328 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3105 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3987 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8303 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21285 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2933 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8977 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8237 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2529 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2874 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3135 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12518 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17104 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19581 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/v2/shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3487 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.119331 manila-9.1.5/manila/api/views/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3592 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3737 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2821 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/quota_class_sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2086 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/quota_sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1818 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3045 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/security_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1203 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3732 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_accesses.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4412 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2238 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3724 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4043 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2470 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4795 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3418 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2899 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2245 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4136 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7544 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4927 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2226 2021-02-01 17:27:42.000000 manila-9.1.5/manila/api/views/versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.119331 manila-9.1.5/manila/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2038 2021-02-01 17:27:42.000000 manila-9.1.5/manila/cmd/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1824 2021-02-01 17:27:42.000000 manila-9.1.5/manila/cmd/data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16773 2021-02-01 17:27:42.000000 manila-9.1.5/manila/cmd/manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1993 2021-02-01 17:27:42.000000 manila-9.1.5/manila/cmd/scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2324 2021-02-01 17:27:42.000000 manila-9.1.5/manila/cmd/share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2021-02-01 17:27:42.000000 manila-9.1.5/manila/cmd/status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.123332 manila-9.1.5/manila/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3404 2021-02-01 17:27:42.000000 manila-9.1.5/manila/common/client_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8041 2021-02-01 17:27:42.000000 manila-9.1.5/manila/common/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7441 2021-02-01 17:27:42.000000 manila-9.1.5/manila/common/constants.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.123332 manila-9.1.5/manila/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1150 2021-02-01 17:27:42.000000 manila-9.1.5/manila/compute/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10118 2021-02-01 17:27:42.000000 manila-9.1.5/manila/compute/nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5521 2021-02-01 17:27:42.000000 manila-9.1.5/manila/context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6623 2021-02-01 17:27:42.000000 manila-9.1.5/manila/coordination.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.123332 manila-9.1.5/manila/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11255 2021-02-01 17:27:42.000000 manila-9.1.5/manila/data/helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12023 2021-02-01 17:27:42.000000 manila-9.1.5/manila/data/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2338 2021-02-01 17:27:42.000000 manila-9.1.5/manila/data/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6520 2021-02-01 17:27:42.000000 manila-9.1.5/manila/data/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.123332 manila-9.1.5/manila/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      802 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52848 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1366 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1493 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migration.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.127333 manila-9.1.5/manila/db/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.127333 manila-9.1.5/manila/db/migrations/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1325 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/env.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2382 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      953 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/script.py.mako
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.139335 manila-9.1.5/manila/db/migrations/alembic/versions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1056 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/0274d20c560f_add_ou_to_security_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9401 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/03da71c0e321_convert_cgs_to_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1231 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/097fad24d2fc_add_share_instances_share_id_index.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2086 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/11ee96se625f3_add_metadata_for_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16924 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/162a3e673105_manila_init.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1079 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/17115072e1c3_add_nova_net_id_column_to_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4836 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/1f0bd302c1a6_add_availability_zones_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1146 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/211836bf835c_add_access_level.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1919 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/221a83cfd85b_change_user_project_id_length.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2027 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/238720805ce1_add_messages_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/27cb96d991fa_add_description_for_share_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/293fac1130ca_add_replication_attrs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1336 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/30cb96d995fa_add_is_public_column_for_share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1014 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/323840a08dc4_add_shares_task_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4287 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/344c1ac4747f_add_share_instance_access_rules_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7864 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/3651e16d7c43_add_consistency_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5372 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/38e632621e5a_change_volume_type_to_share_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2090 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/3a482171410f_add_drivers_private_data_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1771 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/3db9992c30f3_transform_statuses_to_lowercase.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5841 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/3e7d62517afa_add_create_share_from_snapshot_support.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3211 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/48a7beae3117_move_share_type_id_to_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/493eaffd79e1_add_mtu_network_allocations_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1842 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/4a482571410f_add_backends_info_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1077 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/4ee2cf4be19a_remove_share_snapshots_export_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11818 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/5077ffcc5f1c_add_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1839 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/5155c7077f99_add_more_network_info_attributes_to_network_allocations_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1173 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/5237b6625330_add_availability_zone_id_field_to_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2133 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/533646c7af38_remove_unused_attr_status.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3675 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/54667b9cade7_restore_share_instance_access_map_state.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4205 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/55761e5f59c5_add_snapshot_support_extra_spec_to_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3874 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/56cdbe267881_add_share_export_locations_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4145 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/579c267fbb4d_add_share_instances_access_map.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2660 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/59eb64046740_add_required_extra_spec.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1000 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/63809d875e32_add_access_key.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2393 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/6a3fd2984bc31_add_is_auto_deletable_and_identifier_fields_for_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/7d142971c4ef_add_reservation_expire_index.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9838 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/805685098bd2_add_share_network_subnets_table_and_modify_share_servers_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1511 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/829a09b0ddd4_fix_project_share_type_quotas_unique_constraint.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2040 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/87ce15c59bbe_add_revert_to_snapshot_support.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/927920b37453_add_provider_location_for_share_group_snapshot_members_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1028 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/95e3cf760840_remove_nova_net_id_column_from_share_.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3742 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/a77e2ad5012d_add_share_snapshot_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6517 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/b10fb432c042_squash_share_group_snapshot_members_and_share_snapshot_instance_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2098 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/b516de97bfee_add_quota_per_share_type_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1701 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/d5db24264f5c_add_consistent_snapshot_support_attr_to_share_group_model.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3965 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/dda6de06349_add_export_locations_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5174 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/e1949a93157a_add_share_group_types_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3777 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/e8ea58723178_remove_host_from_driver_private_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3655 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/e9f79621d83f_add_cast_rules_to_readonly_to_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/eb6d5544cbbd_add_provider_location_to_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2519 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/ef0c02b4366_add_share_type_projects.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic/versions/fdfb668d19e1_add_gateway_to_network_allocations_table.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1127 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/alembic.ini
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      759 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/migrations/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.139335 manila-9.1.5/manila/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   184952 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/sqlalchemy/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50263 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/sqlalchemy/models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1547 2021-02-01 17:27:42.000000 manila-9.1.5/manila/db/sqlalchemy/query.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27060 2021-02-01 17:27:42.000000 manila-9.1.5/manila/exception.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.139335 manila-9.1.5/manila/hacking/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/hacking/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11630 2021-02-01 17:27:42.000000 manila-9.1.5/manila/hacking/checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1041 2021-02-01 17:27:42.000000 manila-9.1.5/manila/i18n.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5462 2021-02-01 17:27:42.000000 manila-9.1.5/manila/manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.139335 manila-9.1.5/manila/message/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/message/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3363 2021-02-01 17:27:42.000000 manila-9.1.5/manila/message/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5607 2021-02-01 17:27:42.000000 manila-9.1.5/manila/message/message_field.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      621 2021-02-01 17:27:42.000000 manila-9.1.5/manila/message/message_levels.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.139335 manila-9.1.5/manila/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5316 2021-02-01 17:27:42.000000 manila-9.1.5/manila/network/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.139335 manila-9.1.5/manila/network/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/network/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9322 2021-02-01 17:27:42.000000 manila-9.1.5/manila/network/linux/interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15327 2021-02-01 17:27:42.000000 manila-9.1.5/manila/network/linux/ip_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2111 2021-02-01 17:27:42.000000 manila-9.1.5/manila/network/linux/ovs_lib.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.143336 manila-9.1.5/manila/network/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/network/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15309 2021-02-01 17:27:42.000000 manila-9.1.5/manila/network/neutron/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      808 2021-02-01 17:27:42.000000 manila-9.1.5/manila/network/neutron/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28372 2021-02-01 17:27:42.000000 manila-9.1.5/manila/network/neutron/neutron_network_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16423 2021-02-01 17:27:42.000000 manila-9.1.5/manila/network/standalone_network_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9218 2021-02-01 17:27:42.000000 manila-9.1.5/manila/opts.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.147337 manila-9.1.5/manila/policies/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3206 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1200 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1172 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1744 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/message.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1624 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/quota_class_set.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3049 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/quota_set.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3390 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/security_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2015 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1549 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1553 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_access_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1513 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_export_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3270 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_group.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3561 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_group_snapshot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_group_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2621 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_group_types_spec.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2173 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1675 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_instance_export_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2268 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_network_subnet.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3972 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_replica.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1614 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_replica_export_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3091 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3967 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_snapshot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1592 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_snapshot_export_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2360 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_snapshot_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1708 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_snapshot_instance_export_location.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3695 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2463 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/share_types_extra_spec.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12283 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policies/shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7514 2021-02-01 17:27:42.000000 manila-9.1.5/manila/policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46004 2021-02-01 17:27:42.000000 manila-9.1.5/manila/quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4561 2021-02-01 17:27:42.000000 manila-9.1.5/manila/rpc.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.147337 manila-9.1.5/manila/scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1809 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/base_handler.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.151337 manila-9.1.5/manila/scheduler/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5148 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/drivers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2669 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/drivers/chance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19053 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/drivers/filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3213 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/drivers/simple.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.151337 manila-9.1.5/manila/scheduler/evaluator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/evaluator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7963 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/evaluator/evaluator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.151337 manila-9.1.5/manila/scheduler/filters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1623 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3722 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1360 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/base_host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2005 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5628 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/capacity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3768 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2476 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/extra_specs_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1949 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/ignore_attempted_hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5018 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/json.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/retry.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.151337 manila-9.1.5/manila/scheduler/filters/share_group_filters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/share_group_filters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1367 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/share_group_filters/consistent_snapshot.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3641 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/filters/share_replication.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28039 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/host_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12735 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5892 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3492 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/scheduler_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7141 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.155338 manila-9.1.5/manila/scheduler/weighers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/weighers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4577 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/weighers/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1290 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/weighers/base_host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4353 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/weighers/capacity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4385 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/weighers/goodness.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1955 2021-02-01 17:27:42.000000 manila-9.1.5/manila/scheduler/weighers/pool.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14124 2021-02-01 17:27:42.000000 manila-9.1.5/manila/service.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.155338 manila-9.1.5/manila/share/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1027 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24651 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    92664 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2540 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/configuration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   116691 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.159339 manila-9.1.5/manila/share/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.159339 manila-9.1.5/manila/share/drivers/cephfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/cephfs/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.159339 manila-9.1.5/manila/share/drivers/cephfs/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       51 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/cephfs/conf/cephfs-export-template.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24279 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/cephfs/driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.159339 manila-9.1.5/manila/share/drivers/container/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/container/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7797 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/container/container_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16349 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/container/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5656 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/container/protocol_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5950 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/container/storage_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.159339 manila-9.1.5/manila/share/drivers/dell_emc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.159339 manila-9.1.5/manila/share/drivers/dell_emc/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.159339 manila-9.1.5/manila/share/drivers/dell_emc/common/enas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/common/enas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6518 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/common/enas/connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1753 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/common/enas/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5822 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/common/enas/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9979 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/common/enas/xml_api_parser.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8666 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1138 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugin_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.159339 manila-9.1.5/manila/share/drivers/dell_emc/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3053 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.159339 manila-9.1.5/manila/share/drivers/dell_emc/plugins/isilon/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/isilon/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20978 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/isilon/isilon.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13008 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/isilon/isilon_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.163340 manila-9.1.5/manila/share/drivers/dell_emc/plugins/powermax/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/powermax/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36229 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/powermax/connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    78716 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/powermax/object_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.163340 manila-9.1.5/manila/share/drivers/dell_emc/plugins/unity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/unity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13644 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/unity/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30220 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/unity/connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/unity/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.163340 manila-9.1.5/manila/share/drivers/dell_emc/plugins/vnx/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/vnx/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35507 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/vnx/connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    78121 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/dell_emc/plugins/vnx/object_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.163340 manila-9.1.5/manila/share/drivers/ganesha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12216 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/ganesha/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.163340 manila-9.1.5/manila/share/drivers/ganesha/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1180 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/ganesha/conf/00-base-export-template.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22754 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/ganesha/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4819 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/ganesha/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47119 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/generic.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.163340 manila-9.1.5/manila/share/drivers/glusterfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12210 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/glusterfs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17160 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/glusterfs/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.167341 manila-9.1.5/manila/share/drivers/glusterfs/conf/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/glusterfs/conf/10-glusterfs-export-template.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9092 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/glusterfs/glusterfs_native.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10105 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/glusterfs/layout.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10092 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/glusterfs/layout_directory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26321 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/glusterfs/layout_volume.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.167341 manila-9.1.5/manila/share/drivers/hdfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hdfs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16931 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hdfs/hdfs_native.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25463 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/helpers.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.167341 manila-9.1.5/manila/share/drivers/hitachi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hitachi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.167341 manila-9.1.5/manila/share/drivers/hitachi/hnas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hitachi/hnas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    55534 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hitachi/hnas/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    35481 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hitachi/hnas/ssh.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.167341 manila-9.1.5/manila/share/drivers/hitachi/hsp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hitachi/hsp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14434 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hitachi/hsp/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7508 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hitachi/hsp/rest.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.167341 manila-9.1.5/manila/share/drivers/hpe/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hpe/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26264 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hpe/hpe_3par_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    70114 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/hpe/hpe_3par_mediator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.167341 manila-9.1.5/manila/share/drivers/huawei/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4353 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3997 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11551 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/huawei_nas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2456 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/huawei_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.171342 manila-9.1.5/manila/share/drivers/huawei/v3/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/v3/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    77516 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/v3/connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    52116 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/v3/helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10021 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/v3/replication.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1619 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/v3/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7976 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/huawei/v3/smartx.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.171342 manila-9.1.5/manila/share/drivers/ibm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/ibm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51201 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/ibm/gpfs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.171342 manila-9.1.5/manila/share/drivers/infinidat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/infinidat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20747 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/infinidat/infinibox.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.171342 manila-9.1.5/manila/share/drivers/infortrend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/infortrend/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10278 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/infortrend/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26123 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/infortrend/infortrend_nas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.171342 manila-9.1.5/manila/share/drivers/inspur/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/inspur/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.171342 manila-9.1.5/manila/share/drivers/inspur/as13000/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/inspur/as13000/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33764 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/inspur/as13000/as13000_nas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.171342 manila-9.1.5/manila/share/drivers/inspur/instorage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/inspur/instorage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16234 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/inspur/instorage/cli_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21558 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/inspur/instorage/instorage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23003 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/lvm.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.175342 manila-9.1.5/manila/share/drivers/maprfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/maprfs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13643 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/maprfs/driver_util.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19661 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/maprfs/maprfs_native.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.175342 manila-9.1.5/manila/share/drivers/netapp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.175342 manila-9.1.5/manila/share/drivers/netapp/dataontap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.175342 manila-9.1.5/manila/share/drivers/netapp/dataontap/client/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/client/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23625 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/client/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4329 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/client/client_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   149867 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/client/client_cmode.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.175342 manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19626 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/data_motion.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13332 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/drv_multi_svm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13137 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/drv_single_svm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   108546 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/lib_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23714 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/lib_multi_svm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6360 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/lib_single_svm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17313 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/performance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.179343 manila-9.1.5/manila/share/drivers/netapp/dataontap/protocols/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/protocols/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2371 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/protocols/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7286 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/protocols/cifs_cmode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7457 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/dataontap/protocols/nfs_cmode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8290 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7993 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/netapp/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.179343 manila-9.1.5/manila/share/drivers/nexenta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/nexenta/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.179343 manila-9.1.5/manila/share/drivers/nexenta/ns4/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/nexenta/ns4/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3015 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/nexenta/ns4/jsonrpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5591 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/nexenta/ns4/nexenta_nas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9280 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/nexenta/ns4/nexenta_nfs_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.179343 manila-9.1.5/manila/share/drivers/nexenta/ns5/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/nexenta/ns5/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22259 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/nexenta/ns5/jsonrpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23368 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/nexenta/ns5/nexenta_nas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5500 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/nexenta/options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1581 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/nexenta/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.183344 manila-9.1.5/manila/share/drivers/qnap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/qnap/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27023 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/qnap/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40927 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/qnap/qnap.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.183344 manila-9.1.5/manila/share/drivers/quobyte/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/quobyte/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4594 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/quobyte/jsonrpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17458 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/quobyte/quobyte.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47925 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/service_instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.183344 manila-9.1.5/manila/share/drivers/tegile/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/tegile/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19637 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/tegile/tegile.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.183344 manila-9.1.5/manila/share/drivers/veritas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/veritas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24817 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/veritas/veritas_isa.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.183344 manila-9.1.5/manila/share/drivers/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12818 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/windows/service_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7586 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/windows/windows_smb_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11152 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/windows/windows_smb_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9382 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/windows/windows_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6507 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/windows/winrm_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.183344 manila-9.1.5/manila/share/drivers/zfsonlinux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/zfsonlinux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67550 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/zfsonlinux/driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12003 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/zfsonlinux/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.187344 manila-9.1.5/manila/share/drivers/zfssa/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/zfssa/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12840 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/zfssa/restclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18122 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/zfssa/zfssarest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20977 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers/zfssa/zfssashare.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6143 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/drivers_private_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5862 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/hook.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.187344 manila-9.1.5/manila/share/hooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/hooks/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   193858 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7399 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17684 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14049 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7311 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/snapshot_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5258 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.187344 manila-9.1.5/manila/share_group/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share_group/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21589 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share_group/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5764 2021-02-01 17:27:42.000000 manila-9.1.5/manila/share_group/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14081 2021-02-01 17:27:42.000000 manila-9.1.5/manila/test.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.187344 manila-9.1.5/manila/testing/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2033 2021-02-01 17:27:42.000000 manila-9.1.5/manila/testing/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.191345 manila-9.1.5/manila/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      925 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.195346 manila-9.1.5/manila/tests/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1198 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/common.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.195346 manila-9.1.5/manila/tests/api/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6426 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/contrib/stubs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.195346 manila-9.1.5/manila/tests/api/extensions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/extensions/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2925 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/extensions/foxinsocks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9021 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.195346 manila-9.1.5/manila/tests/api/middleware/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/middleware/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2306 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/middleware/test_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7242 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/middleware/test_faults.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.195346 manila-9.1.5/manila/tests/api/openstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/openstack/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7204 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/openstack/test_api_version_request.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1318 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/openstack/test_versioned_method.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36783 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/openstack/test_wsgi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17041 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6444 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/test_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3303 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/test_middleware.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12928 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/test_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1792 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/test_wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.199347 manila-9.1.5/manila/tests/api/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3997 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/stubs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29297 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12231 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19856 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/test_security_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11159 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/test_share_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12711 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/test_share_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21264 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16809 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15491 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/test_share_types_extra_specs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9179 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/test_share_unmanage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50009 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v1/test_shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.203348 manila-9.1.5/manila/tests/api/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1656 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/stubs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4036 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7500 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6756 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_quota_class_sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28145 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_quota_sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3061 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11173 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5253 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_access_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5162 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_accesses.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10091 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24584 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14031 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_group_type_specs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29183 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41142 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6482 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14201 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20279 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43534 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8250 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31485 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19617 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4272 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4264 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10291 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    42707 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43485 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   123286 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/v2/test_shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.207348 manila-9.1.5/manila/tests/api/views/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/views/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2672 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/views/test_quota_class_sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3032 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/views/test_quota_sets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3123 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/views/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3676 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/views/test_share_accesses.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2945 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/views/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9174 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/views/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3449 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/views/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4505 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/api/views/test_versions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.207348 manila-9.1.5/manila/tests/cmd/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/cmd/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1877 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/cmd/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/cmd/test_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16568 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/cmd/test_manage.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1930 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/cmd/test_scheduler.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2650 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/cmd/test_share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1020 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/cmd/test_status.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.207348 manila-9.1.5/manila/tests/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4122 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/common/test_client_auth.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1704 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/common/test_config.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.207348 manila-9.1.5/manila/tests/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/compute/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14787 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/compute/test_nova.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3748 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/conf_fixture.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.207348 manila-9.1.5/manila/tests/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/data/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12362 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/data/test_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17101 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/data/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3754 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/data/test_rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11513 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/data/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.211349 manila-9.1.5/manila/tests/db/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1595 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.211349 manila-9.1.5/manila/tests/db/migrations/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/migrations/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.211349 manila-9.1.5/manila/tests/db/migrations/alembic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/migrations/alembic/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   114195 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/migrations/alembic/migrations_data_checks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7533 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/migrations/alembic/test_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1012 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/migrations/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.211349 manila-9.1.5/manila/tests/db/sqlalchemy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/sqlalchemy/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   162221 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/sqlalchemy/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11647 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/sqlalchemy/test_models.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2124 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2852 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db/test_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9216 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/db_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      848 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/declare_conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/fake_client_exception_class.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3083 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/fake_compute.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3813 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/fake_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6461 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/fake_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2504 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/fake_notifier.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1920 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/fake_service_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10226 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/fake_share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3734 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/fake_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1923 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/fake_volume.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2967 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/fake_zfssa.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.211349 manila-9.1.5/manila/tests/integrated/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/integrated/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.211349 manila-9.1.5/manila/tests/integrated/api/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/integrated/api/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7943 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/integrated/api/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4074 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/integrated/integrated_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1440 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/integrated/test_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/integrated/test_login.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.211349 manila-9.1.5/manila/tests/message/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/message/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4034 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/message/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2812 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/message/test_message_field.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.211349 manila-9.1.5/manila/tests/monkey_patch_example/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1106 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/monkey_patch_example/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      911 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/monkey_patch_example/example_a.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      912 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/monkey_patch_example/example_b.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.215350 manila-9.1.5/manila/tests/network/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/network/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.215350 manila-9.1.5/manila/tests/network/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/network/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10810 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/network/linux/test_interface.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29629 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/network/linux/test_ip_lib.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2879 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/network/linux/test_ovs_lib.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.215350 manila-9.1.5/manila/tests/network/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/network/neutron/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25079 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/network/neutron/test_neutron_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    80282 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/network/neutron/test_neutron_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22395 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/network/test_standalone_network_plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5187 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/policy.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      856 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/runtime_conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.215350 manila-9.1.5/manila/tests/scheduler/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.215350 manila-9.1.5/manila/tests/scheduler/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/drivers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3941 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/drivers/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24866 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/drivers/test_filter.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7227 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/drivers/test_simple.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.219351 manila-9.1.5/manila/tests/scheduler/evaluator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/evaluator/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6397 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/evaluator/test_evaluator.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18215 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.219351 manila-9.1.5/manila/tests/scheduler/filters/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3977 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_availability_zone.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5506 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_base_host.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6789 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_capabilities.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13943 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_capacity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5002 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2535 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_extra_specs_ops.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1961 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_ignore_attempted_hosts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13678 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_json.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1813 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_retry.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5041 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/filters/test_share_replication.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50972 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/test_host_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17325 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5397 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/test_rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5241 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/test_scheduler_options.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1932 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.219351 manila-9.1.5/manila/tests/scheduler/weighers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/weighers/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2310 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/weighers/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11604 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/weighers/test_capacity.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6096 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/weighers/test_goodness.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6734 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/scheduler/weighers/test_pool.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.223351 manila-9.1.5/manila/tests/share/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.227352 manila-9.1.5/manila/tests/share/drivers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.227352 manila-9.1.5/manila/tests/share/drivers/cephfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/cephfs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34637 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/cephfs/test_driver.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.227352 manila-9.1.5/manila/tests/share/drivers/container/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/container/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3526 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/container/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11362 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/container/test_container_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21069 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/container/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12495 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/container/test_protocol_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8047 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/container/test_storage_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.227352 manila-9.1.5/manila/tests/share/drivers/dell_emc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.227352 manila-9.1.5/manila/tests/share/drivers/dell_emc/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.227352 manila-9.1.5/manila/tests/share/drivers/dell_emc/common/enas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/common/enas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    62668 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/common/enas/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8039 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/common/enas/test_connector.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6052 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/common/enas/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5426 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/common/enas/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.227352 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.231353 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/isilon/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/isilon/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47173 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/isilon/test_isilon.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33695 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/isilon/test_isilon_api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.231353 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/powermax/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/powermax/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    97958 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/powermax/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   129908 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/powermax/test_object_manager.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.231353 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      740 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1852 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/fake_exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9948 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/mocked_manila.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32726 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/mocked_unity.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12845 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/res_mock.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10005 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29798 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4165 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1188 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.231353 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/vnx/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/vnx/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    97975 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/vnx/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   129829 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/vnx/test_object_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5427 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dell_emc/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29267 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/dummy.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.235354 manila-9.1.5/manila/tests/share/drivers/ganesha/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/ganesha/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48140 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/ganesha/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5410 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/ganesha/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.235354 manila-9.1.5/manila/tests/share/drivers/glusterfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/glusterfs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34537 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/glusterfs/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11019 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/glusterfs/test_glusterfs_native.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12949 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/glusterfs/test_layout.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20419 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/glusterfs/test_layout_directory.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44147 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/glusterfs/test_layout_volume.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.235354 manila-9.1.5/manila/tests/share/drivers/hdfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hdfs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22812 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hdfs/test_hdfs_native.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.235354 manila-9.1.5/manila/tests/share/drivers/hitachi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hitachi/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.235354 manila-9.1.5/manila/tests/share/drivers/hitachi/hnas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hitachi/hnas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53836 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hitachi/hnas/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    65624 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hitachi/hnas/test_ssh.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.235354 manila-9.1.5/manila/tests/share/drivers/hitachi/hsp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hitachi/hsp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2515 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hitachi/hsp/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22885 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hitachi/hsp/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12853 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hitachi/hsp/test_rest.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.239354 manila-9.1.5/manila/tests/share/drivers/hpe/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hpe/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7526 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hpe/test_hpe_3par_constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    41497 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hpe/test_hpe_3par_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   129857 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/hpe/test_hpe_3par_mediator.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.239354 manila-9.1.5/manila/tests/share/drivers/huawei/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/huawei/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   195581 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/huawei/test_huawei_nas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.239354 manila-9.1.5/manila/tests/share/drivers/ibm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/ibm/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    76139 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/ibm/test_gpfs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.239354 manila-9.1.5/manila/tests/share/drivers/infinidat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/infinidat/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34428 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/infinidat/test_infinidat.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.239354 manila-9.1.5/manila/tests/share/drivers/infortrend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/infortrend/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15687 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/infortrend/fake_infortrend_manila_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13722 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/infortrend/fake_infortrend_nas_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22147 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/infortrend/test_infortrend_nas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.239354 manila-9.1.5/manila/tests/share/drivers/inspur/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/inspur/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.239354 manila-9.1.5/manila/tests/share/drivers/inspur/as13000/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/inspur/as13000/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    50841 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/inspur/as13000/test_as13000_nas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.243355 manila-9.1.5/manila/tests/share/drivers/inspur/instorage/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/inspur/instorage/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51564 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/inspur/instorage/test_instorage.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.243355 manila-9.1.5/manila/tests/share/drivers/maprfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/maprfs/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    38617 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/maprfs/test_maprfs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.243355 manila-9.1.5/manila/tests/share/drivers/netapp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.243355 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.243355 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/client/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/client/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    89391 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/client/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10127 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/client/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6708 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/client/test_client_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   251464 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/client/test_client_cmode.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.247356 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27411 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_data_motion.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2625 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_driver_interfaces.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   236116 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    46881 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_multi_svm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8723 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_single_svm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34182 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_performance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44077 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.247356 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/protocols/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/protocols/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2140 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/protocols/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1590 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/protocols/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8414 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/protocols/test_cifs_cmode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8233 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/protocols/test_nfs_cmode.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6384 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17245 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/netapp/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.247356 manila-9.1.5/manila/tests/share/drivers/nexenta/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/nexenta/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.247356 manila-9.1.5/manila/tests/share/drivers/nexenta/ns4/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/nexenta/ns4/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1349 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/nexenta/ns4/test_jsonrpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21864 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/nexenta/ns4/test_nexenta_nas.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.247356 manila-9.1.5/manila/tests/share/drivers/nexenta/ns5/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/nexenta/ns5/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    43244 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/nexenta/ns5/test_jsonrpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21901 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/nexenta/ns5/test_nexenta_nas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/nexenta/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.251357 manila-9.1.5/manila/tests/share/drivers/qnap/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/qnap/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23015 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/qnap/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36904 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/qnap/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    64958 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/qnap/test_qnap.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.251357 manila-9.1.5/manila/tests/share/drivers/quobyte/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/quobyte/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9274 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/quobyte/test_jsonrpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30335 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/quobyte/test_quobyte.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.251357 manila-9.1.5/manila/tests/share/drivers/tegile/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/tegile/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32531 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/tegile/test_tegile.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26861 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/test_ganesha.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    81517 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/test_generic.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19168 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/test_glusterfs.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    34944 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/test_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    29240 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/test_lvm.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   112216 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/test_service_instance.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.251357 manila-9.1.5/manila/tests/share/drivers/veritas/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/veritas/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23062 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/veritas/test_veritas_isa.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.251357 manila-9.1.5/manila/tests/share/drivers/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16422 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/windows/test_service_instance.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12572 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/windows/test_windows_smb_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16819 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/windows/test_windows_smb_helper.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16351 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/windows/test_windows_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11513 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/windows/test_winrm_helper.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.251357 manila-9.1.5/manila/tests/share/drivers/zfsonlinux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/zfsonlinux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   105631 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/zfsonlinux/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19480 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/zfsonlinux/test_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.255358 manila-9.1.5/manila/tests/share/drivers/zfssa/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share/drivers/zfssa/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18386 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/zfssa/test_zfssarest.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20186 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/drivers/zfssa/test_zfssashare.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    36129 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   185495 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    48930 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_driver.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5780 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_drivers_private_data.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12744 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_hook.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   345716 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12927 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_migration.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16750 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_rpcapi.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    19883 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8533 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_share_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7019 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share/test_snapshot_access.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.255358 manila-9.1.5/manila/tests/share_group/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/share_group/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    67039 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share_group/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5205 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/share_group/test_share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2638 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2940 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/test_conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2516 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/test_context.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3768 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/test_coordination.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23735 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/test_exception.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13859 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/test_hacking.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5309 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/test_manager.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2201 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/test_misc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7087 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/test_network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7439 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/test_policy.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28595 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/test_quota.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1479 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/test_rpc.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8315 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/test_service.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/test_test.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1029 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/test_test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31543 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4343 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.255358 manila-9.1.5/manila/tests/var/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2159 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/var/ca.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1858 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/var/certificate.crt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3243 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/var/privatekey.key
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.255358 manila-9.1.5/manila/tests/volume/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/volume/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11477 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/volume/test_cinder.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.255358 manila-9.1.5/manila/tests/wsgi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/wsgi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1473 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/wsgi/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1847 2021-02-01 17:27:43.000000 manila-9.1.5/manila/tests/wsgi/test_wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.255358 manila-9.1.5/manila/tests/xenapi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/tests/xenapi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    25285 2021-02-01 17:27:42.000000 manila-9.1.5/manila/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      892 2021-02-01 17:27:42.000000 manila-9.1.5/manila/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.255358 manila-9.1.5/manila/volume/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1165 2021-02-01 17:27:42.000000 manila-9.1.5/manila/volume/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12923 2021-02-01 17:27:42.000000 manila-9.1.5/manila/volume/cinder.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.255358 manila-9.1.5/manila/wsgi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/manila/wsgi/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5145 2021-02-01 17:27:42.000000 manila-9.1.5/manila/wsgi/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2021-02-01 17:27:42.000000 manila-9.1.5/manila/wsgi/eventlet_server.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1121 2021-02-01 17:27:42.000000 manila-9.1.5/manila/wsgi/wsgi.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.103328 manila-9.1.5/manila.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2207 2021-02-01 17:28:23.000000 manila-9.1.5/manila.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    88130 2021-02-01 17:28:23.000000 manila-9.1.5/manila.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-01 17:28:23.000000 manila-9.1.5/manila.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2653 2021-02-01 17:28:23.000000 manila-9.1.5/manila.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2021-02-01 17:28:23.000000 manila-9.1.5/manila.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2021-02-01 17:28:23.000000 manila-9.1.5/manila.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      859 2021-02-01 17:28:23.000000 manila-9.1.5/manila.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2021-02-01 17:28:23.000000 manila-9.1.5/manila.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.011311 manila-9.1.5/playbooks/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.011311 manila-9.1.5/playbooks/legacy/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.255358 manila-9.1.5/playbooks/legacy/grenade-dsvm-manila/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/grenade-dsvm-manila/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2414 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/grenade-dsvm-manila/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-container-scenario-custom-image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-container-scenario-custom-image/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4322 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-container-scenario-custom-image/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-generic-no-share-servers/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-generic-no-share-servers/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3559 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-generic-no-share-servers/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-generic-scenario-custom-image/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-generic-scenario-custom-image/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4252 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-generic-scenario-custom-image/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-native/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-native/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3119 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-native/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-native-heketi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-native-heketi/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3140 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-native-heketi/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3107 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs-heketi/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs-heketi/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3139 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs-heketi/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-hdfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-hdfs/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2687 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-hdfs/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-mysql-generic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-mysql-generic/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3535 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-mysql-generic/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-container/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-container/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3609 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-container/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.259358 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-generic-singlebackend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-generic-singlebackend/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3571 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-generic-singlebackend/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.263359 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-zfsonlinux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-zfsonlinux/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3613 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-zfsonlinux/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.263359 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-scenario/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-scenario/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3530 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-scenario/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.263359 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3535 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.263359 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native-centos-7/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native-centos-7/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4571 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native-centos-7/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.263359 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4586 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.263359 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs-centos-7/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs-centos-7/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4616 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs-centos-7/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.263359 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-dummy/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-dummy/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3439 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-dummy/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.263359 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-dummy-py2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-dummy-py2/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3394 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-dummy-py2/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.263359 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4697 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/run-ipv6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4602 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.267360 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-native-centos-7/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-native-centos-7/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3786 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-native-centos-7/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.267360 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-nfs-centos-7/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      411 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-nfs-centos-7/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3771 2021-02-01 17:27:43.000000 manila-9.1.5/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-nfs-centos-7/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.267360 manila-9.1.5/playbooks/manila-tox-genconfig/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2021-02-01 17:27:42.000000 manila-9.1.5/playbooks/manila-tox-genconfig/post.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.267360 manila-9.1.5/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2021-02-01 17:27:42.000000 manila-9.1.5/rally-jobs/rally-manila-no-ss.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2021-02-01 17:27:42.000000 manila-9.1.5/rally-jobs/rally-manila.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.015311 manila-9.1.5/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.335373 manila-9.1.5/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/1841035-dellemc-unity-fix-ace-enable-error-b00281bb306d176b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/3par-add-update-access-68fc12ffc099f480.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      365 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/3par-fix-get_vfs-driver-bootup-db6b085eb6094f5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/3par-pool-support-fb43b368214c9eda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/Huawei-driver-utilize-requests-lib-67f2c4e7ae0d2efa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      418 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/Use-http_proxy_to_wsgi-instead-of-ssl-middleware-df533a2c2d9c3a61.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-ability-to-check-tenant-quota-usages-7fs17djahy61nsd6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      192 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-access-key-to-share-access-map-2fda4c06a750e24e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      308 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-cast-rules-to-readonly-field-62ead37b728db654.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-cleanup-create-from-snap-hnas-0e0431f1fc861a4e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-create_share_from_snapshot_support-extra-spec-9b1c3ad6796dd07d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-export-location-filter-92ead37b728db654.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-export-locations-api-6fc6086c6a081faa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-gathering-usage-size-8454sd45deopb14e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-hsp-default-filter-function-0af60a819faabfec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-ipv6-32d89161a9a1e0b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-is-default-e49727d276dd9bc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-like-filter-4c1d6dc02f40d5a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-manage-db-purge-b32a24ee045d8d45.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-perodic-task-7454sd45deopb13e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      682 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-policy-in-code-c31a24ee045d8d21.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      886 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-share-access-metadata-4fda2c06e750e83c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-share-group-quotas-4e426907eed4c000.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-share-migration-support-in-zfsonlinux-driver-88e6da5692b50810.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-share-type-filter-to-pool-list-api-267614b4d93j12de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-share-type-quotas-33a6b36c0f4c88b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-snapshot-instances-admin-api-959a1121aa407629.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml-5655800975cec5d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       64 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-tegile-driver-1859114513edb13e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-two-new-fields-to-share-groups-api-bc576dddd58a3086.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-update-host-command-to-manila-manage-b32ad5017b564c9e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add-user-id-echo-8f42db469b27ff14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add_gateway_into_db-1f3cd3f392ae81cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add_mtu_info_db-3c1d6dc02f40d5a6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/add_user_id_and_project_id_to_snapshot_APIs-157614b4b8d01e15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/added-possibility-to-run-manila-api-with-web-servers-that-support-wsgi-apps-cfffe0b789f8670a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      732 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/api-versions-mark-v1-deprecated-3540d39279fbd60e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      426 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/blueprint-netapp-snapshot-visibility-4f090a20145fbf34.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bp-admin-network-hnas-9b714736e521101e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1178 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bp-export-locations-az-api-changes-c8aa1a3a5bc86312.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bp-netapp-ontap-storage-based-cryptograpy-bb7e28896e2a2539.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1129 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bp-ocata-migration-improvements-c8c5675e266100da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bp-share-type-supported-azs-2e12ed406f181b3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      174 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bp-update-share-type-name-or-description-a39c5991b930932f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1578328-fix-replica-deletion-in-cDOT-7e4502fb50b69507.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1591357-fix-cannot-remove-user-rule-for-NFS-8e1130e2accabd56.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1597940-fix-hpe3par-delete-share-0daf75193f318c41.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1602525-port_binding_mandatory-2aaba0fa72b82676.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1607029-fix-share-server-deletion-when-interfaces-dont-exist-4d00fe9dafadc252.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1613303-fix-config-generator-18b9f9be40d7eee6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1624526-netapp-cdot-filter-root-aggregates-c30ac5064d530b86.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1370 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1626249-reintroduce-per-share-instance-access-rule-state-7c08a91373b21557.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1626523-migration-rw-access-fix-7da3365c7b5b90a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1634278-unmount-orig-active-after-promote-8e24c099ddc1e564.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      342 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1634734-fix-backend-extraspec-for-replication-d611d2227997ae3e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1638896-missing-migration-completing-state-1e4926ed56eb268c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1638994-drop-fake-cg-support-from-generic-driver-16efce98f94b1b6b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1639188-fix-extend-operation-of-shrinked-share-in-generic-driver-5c7f82faefaf26ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1639662-fix-share-service-VM-restart-problem-1110f9133cc294e8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1640169-check-ceph-connection-on-setup-c92bde41ced43326.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      230 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1645746-fix-inheritance-of-access-rules-from-parent-share-by-zfsonlinux-child-shares-4f85908c8e9871ef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      283 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1645751-fixed-shares-created-from-snapshots-for-lvm-and-generic-drivers-94a1161a9e0b5a85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1646603-netapp-broadcast-domains-411a626d38835177.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      113 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1649782-fixed-incorrect-exportfs-exportfs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      253 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1650043-gpfs-access-bugs-8c10f26ff1f795f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1651578-gpfs-prepend-beb99f408cf20bb5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1651587-deny-access-verify-563ef2f3f6b8c13b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1654598-enforce-policy-checks-for-share-export-locations-a5cea1ec123b1469.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1657033-fix-share-metadata-error-when-deleting-share.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1658133-fix-lvm-revert-34a90e70c9aa7354.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1659023-netapp-cg-fix-56bb77b7bc61c3f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1660319-1660336-migration-share-groups-e66a1478634947ad.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      296 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1660321-fix-default-approach-for-share-group-snapshot-creation-3e843155c395e861.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1660425-snapshot-access-in-error-bce279ee310060f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1660686-snapshot-export-locations-mount-not-supported-cdc2f5a3b57a9319.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1660726-migration-export-locations-5670734670435015.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1661266-add-consistent-snapshot-support-attr-to-share-groups-DB-model-daa1d05129802796.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1661271-hnas-snapshot-readonly-4e50183100ed2b19.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1661381-migration-snapshot-export-locations-169786dcec386402.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      114 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1662615-hnas-snapshot-concurrency-2147159ea6b086c5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1663300-554e9c78ca2ba992.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      416 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1664201-fix-share-replica-status-update-concurrency-in-replica-promotion-feature-63b15d96106c65da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1665002-hnas-driver-version-f3a8f6bff3dbe054.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1665072-migration-success-fix-3da1e80fbab666de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1666541-quobyte-resize-list-param-bc5b9c42bdc94c9f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1667450-migration-stale-source-9c092fee267a7a0f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1674908-allow-user-access-fix-495b3e42bdc985ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1678524-check-snaprestore-license-for-snapshot-revert-6d32afdc5d0b2b51.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1682795-share-access-list-api-5b1e86218959f796.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1684032-6e4502fdceb693dr7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1688620-netapp-migration-cancelation-fb913131eb8eb82a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1690159-retry-backend-init-58486ea420feaf51.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1690785-fix-gpfs-path-91a354bc69bf6a47.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1694768-fix-netapp-cdot-revert-to-snapshot-5e1be65260454988.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1696000-netapp-fix-security-style-on-cifs-shares-cbdd557a27d11961.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1696669-add-ou-to-security-service-06b69615bd417d40.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1698250-netapp-cdot-fix-share-server-deletion-494ab3ad1c0a97c0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      334 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1698258-netapp-fix-tenant-network-gateways-85935582e89a72a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1699836-disallow-share-type-deletion-with-active-share-group-types-83809532d06ef0dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1700346-new-exception-for-no-default-share-type-b1dd9bbe8c9cb3df.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1700871-ontap-allow-extend-of-replicated-share-2c9709180d954308.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      151 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1703581-cifs-extension-failing-because-of-volume-in-use-3fea31c4a58e2f1b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      198 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1703660-fix-netapp-driver-preferred-state-0ce1a62961cded35.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      210 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1704622-netapp-cdot-fix-share-specs-on-migration-bfbbebec26533652.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      630 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1704971-fix-name-description-filter-85935582e89a72a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       60 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1705533-manage-api-error-message-fix-967b0d44c09b914a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1706137-netapp-manila-set-valid-qos-during-migration-4405fff02bd6fa83.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1707066-deny-ipv6-access-in-error-bce379ee310060f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1707084-netapp-manila-driver-to-honour-std-extra-specs-d32fae4e9411b503.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1707943-make-lvm-revert-synchronous-0ef5baee3367fd27.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      208 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1707946-nfs-helper-0-netmask-224da94b82056f93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1714691-decimal-separators-in-locales-392c0c794c49c1c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1716922-security-group-creation-failed-d46085d11370d918.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1717135-ganesha-cleanup-of-tmp-config-files-66082b2384ace0a5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1717263-netapp-ontap-fix-size-for-share-from-snapshot-02385baa7e085f39.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1717392-fix-downgrade-share-access-map-bbd5fe9cc7002f2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-172112-fix-drives-private-storage-update-deleted-entries-7516ba624da2dda7.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      312 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1721787-fix-getting-share-networks-and-security-services-error-7e5e7981fcbf2b53.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1730509-netapp-ipv6-hostname-39abc7f40d48c844.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1733494-allow-user-group-name-with-blank-access-fix-665b3e42bdc985ac.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      106 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1734127-a239d022bef4a002.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1735832-43e9291ddd73286d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1736370-qnap-fix-access-rule-override-1b79b70ae48ad9e6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1745436-78c46f8a0c96cbca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      297 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1745436-remove-data-node-access-ip-config-opt-709f330c57cdb0d5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1746202-fix-unicodeDecodeError-when-decode-API-input-4e4502fb50b69502.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1746723-8b89633062885f0b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1747695-fixed-ip-version-in-neutron-bind-network-plugin-526958e2d83df072.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1749184-eb06929e76a14fce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1750074-fix-rabbitmq-password-in-debug-mode-4e136ff86223c4ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      173 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1765420-netapp-fix-delete-share-for-vsadmins-b5dc9e0224cb3ba2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      266 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1767430-access-control-raise-ip-address-conflict-on-host-routes-0c298125fee4a640.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1772026-nve-license-not-present-fix-e5d2e0d6c5df9227.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1772647-b98025c07553e35d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1773761-qnap-fix-manage-share-size-override-a18acdf1a41909b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1773929-a5cb52c8417ec5fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1774159-0afe3dbc39e3c6b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1774604-qb-driver-b7e717cbc71d6189.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      225 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1777126-netapp-skip-route-setup-if-no-gateway-e841635dcd20fd12.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1777551-security-networks-api-all-tenants-fix-a061274afe15180d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      325 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1777551-security-services-api-all-tenants-fix-e820ec370d7df473.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1785129-fix-sighup-behavior-with-scheduler-8ee803ad0e543cce.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1785180-zfsonlinux-retry-unmounting-during-manage-872cf46313c5a4ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      215 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1794402-fix-share-stats-container-driver-b3cb1fa2987ad4b1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1795463-fix-pagination-slowness-8fcda3746aa13940.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      307 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1798219-fix-snapshot-creation-lvm-and-generic-driver-55e349e02e7fa370.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1143 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1801763-gate-public-share-creation-by-policy-a0ad84e4127a3fc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      349 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1804651-netapp-cdot-add-peferred-dc-to-cifs-ad-99072ce663762e83.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1804656-netapp-cdot-add-port-ids-to-share-server-backend-424ca11a1eb44826.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1804659-speed-up-pools-detail-18f539a96042099a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      287 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1811680-destroy-quotas-usages-reservations-when-deleting-share-type-a18f2e00a65fe922.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      449 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1813054-remove-share-usage-size-audit-period-conf-opt-7331013d1cdb7b43.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      213 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1815038-extend-remove_version_from_href-support-ea479daaaf5c5700.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      127 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1815532-supply-request-id-in-all-apis-74419bc1b1feea1e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      361 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1816420-validate-access-type-for-ganehas-c42ce6f859fa0c8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1818081-fix-inferred-script-name-in-case-of-proxy-urls-e33466af856708b4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1822099-fix-multisegment-mtu.yaml-ac2e31c084d8bbb6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1831092-netapp-fix-race-condition-524555133aaa6ca8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1845135-fix-Unity-cannot-use-mgmt-ipv6-9407710a3fc7f4aa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1845452-unity--fix-fail-to-delete-cifs-share-c502a10ae306e506.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1846836-fix-share-network-update-unexpected-success-eba8f40db392c467.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      552 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1848608-1893718-fix-manage-api-for-shares-with-multiple-export-locations-32ade25e9d82535b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      404 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1848889-netapp-fix-share-replica-update-check-failure-90aa964417e7734c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1850264-add-async-error-when-share-extend-error-a0c458204b395994.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1858328-netapp-fix-shrinking-error-48bcfffe694f5e81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      167 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1859775-snapshot-over-quota-exception-bb6691612af03ddf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1859785-share-list-speed-6b09e7717624e037.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1861485-fix-share-network-retrieval-31768dcda5aeeaaa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1869148-if-only-pyc-exist-the-extension-API-cannot-be-loaded-172cb9153ebd4b56.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1869712-fix-increased-scheduled-time-for-non-thin-provisioned-backends-1da2cc33d365ba4f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      286 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1870751-cleanup-share-type-and-group-type-project-access-when-deleted-4fcd49ba6e6c40bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1872243-netapp-fix-vserver-peer-with-same-vserver-8bc65816f1764784.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      370 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1872872-fix-quota-checking-b06fd372be143101.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      264 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1872873-fix-consume-from-share-eea5941de17a5bcc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      451 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1873963-netapp-fix-vserver-peer-intra-cluster-966398cf3a621edd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1878993-netapp-fix-https-3eddf9eb5b762f3a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1879368-netapp-fix-cifs-promote-back-issue-d8fe28466f9dde49.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1879754-teardown-network-d1887cdf6eb83388.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1880747-netapp-fix-do-not-delete-default-ipspace-aee638279e0f8e93.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      185 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1882590-fix-svm-scoped-netapp-85b53830135f7558.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1885956-enforce-policy-check-getting-share-type-by-name-5eca17b02bea5261.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      226 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1886010-Glusterfs-fix-del-share-89dabc8751ed4fec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1887643-netapp-add-cifs-dc-add-skip-check-c8ea9b952cedb643.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1888905-fix-group-snapshot-create-delete-0595f9d7a4c0c343.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1888915-harden-lvm-deletions-2a735ab0ee4a4903.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      252 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1894362-fix-Glusterfs-del-share-3c8467e1d9f0c6e4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-1901937-netapp-nfs-for-windows-465e704524277ea2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug-667744-fix-c64071e6e5a098f7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug_1564623_change-e286060a27b02f64.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bug_1582931-1437eae20fa544d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/bugfix-1771958-1771970-bcec841e7ae6b9f6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/cephfs-add-nfs-protocol-support-44764094c9d784d8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/cephfs-native-add-readonly-shares-support-067ccab0217ab5f5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      227 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/cephfs-native-enhance-update-access-support-e1a1258084c997ca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/cephfs-native-fix-evict-c45fd2de8f520757.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/cephfs-nfs-ipv6-support-2ffd9c0448c2f47e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      311 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/cephfs-set-mode-b7fb3ec51300c220.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/change_user_project_length-93cc8d1c32926e75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      317 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/check-thin-provisioning-4bb702535f6b10b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/clean-expired-messages-6161094d0c108aa7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/config-for-cephfs-volume-prefix-67f2513f603cb614.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      468 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/container-driver-5d972cc40e314663.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      121 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/container-driver-hardening-against-races-30c9f517a6392b9d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      162 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/container-manage-unmanage-share-servers-880d889828ee7ce3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/dedupe-support-hnas-driver-017d2f2a93a8b487.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/delete_vlan_on_vserver_delete-a7acd145c0b8236d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      239 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/dell-emc-unity-use-user-capacity-322f8bbb7c536453.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/dellemc-fix-capacity-report-25f75a6c96e12b40.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/deprecate-memcached-servers-config-option-f4456382b9b4d6db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      941 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/deprecate-old-ks-opts-in-nova-neutron-cinder-groups-e395015088d93fdc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      191 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/deprecate-service-instance-network-helper-option-82ff62a038f2bfa3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      689 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/disable-share-groups-api-by-default-0627b97ac2cda4cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      435 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/driver-filter-91e2c60c9d1a48dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/drop-support-for-lvm-share-export-ip-e031ef4c5f95b534.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      402 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/emc-unity-manila-support-d4f5a410501cfdae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/emc_vnx_interface_ports_configuration-00d454b3003ef981.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/enhance-ensure-share-58fc14ffc099f481.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      187 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/error-share-set-size-ff5d4f4ac2d56755.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/estimate-provisioned-capacity-34f0d2d7c6c56621.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      309 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-consistency-groups-api-dd9b5b99138e22eb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-ganesha-allow-access-for-all-ips-09773a79dc76ad44.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-hds-hnas-unconfined-09b79f3bdb24a83c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-hnas-mount-on-manage-snapshot-91e094c579ddf1a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-huawei-driver-cifs-mount-issue-2d7bff5a7e6e3ad6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-huawei-driver-qos-deletion-9ad62db3d7415980.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-huawei-exception-a09b73234ksd94kd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-managing-twice-hnas-4956a7653d27e320.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-py3-netapp-a9815186ddc865d4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-race-condition-netapp-5a36f6ba95a49c5e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-share-instance-list-with-limit-db7b5b99138e22ee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix-volume-efficiency-status-2102ad630c5407a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      116 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix_access_level_managed_shares_hnas-c76a09beed365b46.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix_cephx_validation-cba4df77f9f45c6e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix_limit_formating_routes-1b0e1a475de6ac44.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      101 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix_manage_snapshots_hnas-2c0e1a47b5e6ac33.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fix_policy_file-4a382ac241c718c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fixed-netapp-cdot-autosupport-3fabd8ac2e407f70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      382 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/fixing-driver-filter-14022294c8c04d2d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      403 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/ganesha-dynamic-update-access-be80bd1cb785e733.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/ganesha-store-exports-and-export-counter-in-ceph-rados-052b925f8ea460f4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/generic-driver-noop-interface-driver-24abcf7af1e08ff9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/generic-route-racing-adf92d212f1ab4de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/glusterfs-add-directory-layout-extend-shrink-fd2a008f152edbf5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/glusterfs-handle-new-volume-option-xml-schema-dad06253453c572c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/gpfs-nfs-server-type-default-value-change-58890adba373737c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      330 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/guru-meditation-support-7872da69f529a6c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/hitachi-driver-cifs-user-support-3f1a8b894fe3e9bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/hnas-driver-rename-7ef74fe720f7e04b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/hnas-manage-unmanage-snapshot-support-0d939e1764c9ebb9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/hnas-mountable-snapshots-4fbffa05656112c4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/hnas-revert-to-snapshot-a2405cd6653b1e85.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      305 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/hnas_allow_managed_fix-4ec7794e2035d3f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/hpe3par-rw-snapshot-shares-f7c33b4bf528bf00.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/hsp-driver-e00aff5bc89d4b54.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/huawei-driver-replication-8ed62c8d26ad5060.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      244 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/huawei-driver-sectorsize-config-da776132ba6da2a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/huawei-driver-support-snapshot-revert-1208c586bd8db98e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/huawei-pool-disktype-support-0a52ba5d44da55f9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/huawei-support-access-all-ip-4994c10ff75ac683.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/hybrid-aggregates-in-netapp-cdot-drivers-e7c90fb62426c281.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      513 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/ibm-gpfs-ces-support-3498e35d9fea1b55.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/ibm-gpfs-manage-support-c110120c350728e3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/infinidat-add-infinibox-driver-ec652258e710d6a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/infinidat-balance-network-spaces-ips-25a9f1e587b87156.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/infinidat-delete-datasets-with-snapshots-4d18f8c197918606.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/infortrend-manila-driver-a1a2af20de6368cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      176 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/inspur-as13000-driver-41f6b7caea82e46e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/inspur-instorage-driver-51d7a67f253f3ecd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/inspur-support-rwx-for-cifs-permission-4279f1fe7a59fd00.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      715 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/introduce-tooz-library-5fed75b8caffcf42.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/limiting-ssh-access-from-tenant-network-6519efd6d6895076.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       71 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/lv-mounting-inside-containers-af8f84d1fab256d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      622 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/lvm-export-ips-5f73f30df94381d3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       80 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/manage-share-in-zfsonlinux-driver-e80921081206f75b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       67 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/manage-share-snapshot-in-huawei-driver-007b2c763fbdf480.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/manage-snapshot-in-zfsonlinux-driver-6478d8d5b3c6a97f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      388 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/manage-unmanage-replicated-share-fa90ce34372b6df5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1092 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/manage-unmanage-share-servers-cd4a6523d8e9fbdf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       48 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/manage-unmanage-snapshot-bd92164472638f44.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/manage-unmanage-snapshot-in-netapp-cdot-driver-5cb4b1619c39625a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      467 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/manila-status-upgrade-check-framework-aef9b5cf9d8e3bda.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/maprfs-manila-drivers-1541296f26cf78fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      240 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/migration-access-fix-71a0f52ea7a152a3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/migration-empty-files-01d1a3caa2e9705e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/migration-share-type-98e3d3c4c6f47bd9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      232 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/move-emc-share-driver-to-dell-emc-dir-1ec34dee0544270d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/multi-segment-support-fa171a8e3201d54e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-cdot-apply-mtu-from-network-provider-d12179a2374cdda0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      353 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-cdot-clone-split-control-a68b5fc80f1fc368.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-cdot-configure-nfs-versions-83e3f319c4592c39.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-cdot-optimized-migration-within-share-server-92cfa1bcf0c317fc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      644 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-cdot-quality-of-service-limits-c1fe8601d00cb5a8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      222 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-cdot-ss-multiple-dns-ip-df42a217977ce44d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      281 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-cdot-switch-volume-efficiency-bd22733445d146f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-cdot-use-security-service-ou-4dc5835c9e00ad9d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-default-ipv6-route-13a9fd4959928524.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-ipv6-support-f448e99a7c112362.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      236 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-manage-unmanage-share-servers-635496b46e306920.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-replication-dhss-true-5b2887de8e9a2cb5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      282 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp-support-filtering-api-tracing-02d1f4271f44d24c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/netapp_cdot_performance_utilization-aff1b498a159470e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       62 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/neutron-binding-driver-43f01565051b031b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1337 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/newton-migration-improvements-cf9d3d6e37e19c94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       89 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/nexenta-manila-drivers-cbd0b376a076ec50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1275 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/nexentastor5-v1.1-1ad6c8f7b5cc11b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      713 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/per-backend-az-590c68be0e2cb4bd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      926 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/powermax-rebrand-manila-a46a0c2ac0aa77ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      109 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/qb-bug-1733807-581e71e6581de28e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      169 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/qnap-enhance-support-53848fda525b7ea4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/qnap-fix-manage-snapshot-not-exist-4b111982ddc5fdae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      158 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/qnap-fix-share-and-snapshot-inconsistant-bd628c6e14eeab14.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/qnap-manila-driver-a30fe4011cb90801.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/qnap-support-qes-200-639f3ad70687023d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       75 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/qnap-support-qes-210-8775e6c210f3ca9f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/qnap-tds-support-qes-24704313a0881c8c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-AllocType-from-huawei-driver-8b279802f36efb00.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      316 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-confusing-deprecation-warnings-a17c20d8973ef2bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-deprecated-default-options-00fed1238fb6dca0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      436 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-deprecated-size-limiter-9d7c8ab69cf85aea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      585 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-host-field-from-shares-and-replicas-a087f85bc4a4ba45.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-intree-tempest-plugin-9fcf6edbeba47cba.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-nova-net-support-from-service-instance-module-dd7559803fa01d45.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-nova-network-support-f5bcb8b2fcd38581.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      131 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-os-region-name-82e3cd4c7fb05ff4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      260 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-root-helper-config-option-fd517b0603031afa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/remove-standalone-network-plugin-ip-version-440ebcf27ffd22f8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      514 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/rename-cephfs-native-driver-3d9b4e3c6c78ee98.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/reset_tap_device_after_node_restart-0690a6beca077b95.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/revert-switch-to-use-glanceclient-bc462a5477d6b8cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/rules-for-managed-share-f28a26ffc980f6fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/share-mount-snapshots-b52bf3433d1e7afb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1076 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/share-network-with-multiple-subnets-a56be8b646b9e463.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/share-replication-81ecf4a32a5c83b6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      142 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/share-revert-to-snapshot-3d028fa00620651e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/share-revert-to-snapshot-in-netapp-cdot-driver-37f645ec3c14313c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/share-server-delete-failure-ca29d6b286a2c790.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/snapshot-force-delete-4432bebfb5a0bbc9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/support-ipv6-in-drivers-and-network-plugins-1833121513edb13d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/support-qes-114-5881c0ff0e7da512.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/switch-to-use-glanceclient-dde019b0b141caf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/unexpected-data-of-share-from-snap-134189fc0f3eeedf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/unity-drvier-support-1gb-share-48f032dff8a6a789.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/unity-manila-ipv6-support-dd9bcf23064baceb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/unity-revert-to-snapshot-support-1cffc3914982003d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/unity-shrink-share-support-cc748daebfe8f562.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/unity-un-handles-share-server-mode-support-e179c092ab148948.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      717 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/unity-vnx-rename-options-1656168dd4bdba70.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      105 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/use-oslo-logging-for-config-options-388da64bb4ce45db.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      289 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/use-tooz-heartbeat-c6aa7e15444e63c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      321 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/user-messages-api-589ee7d68ccba70c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/veritas-access-manila-driver-d75558c01ce6d428.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      490 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/vlan-enhancement-in-unity-driver-0f1d972f2f6d00d9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/vmax-manila-support-7c655fc094c09367.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      366 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/vmax-rename-options-44d8123d14a23f94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/vnx-manila-ipv6-support-9ae986431549cc63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/vnx-ssl-verification-2d26a24e7e73bf81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      148 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/windows-smb-fix-default-access-d4b9eee899e400a0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      194 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/notes/zfssa-driver-add-share-manage-unmanage-9bd6d2e25cc86c35.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.339374 manila-9.1.5/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.339374 manila-9.1.5/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.339374 manila-9.1.5/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8849 2021-02-01 17:27:43.000000 manila-9.1.5/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      841 2021-02-01 17:27:43.000000 manila-9.1.5/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      141 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/liberty.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.015311 manila-9.1.5/releasenotes/source/locale/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.015311 manila-9.1.5/releasenotes/source/locale/es/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.339374 manila-9.1.5/releasenotes/source/locale/es/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3126 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.015311 manila-9.1.5/releasenotes/source/locale/fr/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.339374 manila-9.1.5/releasenotes/source/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1464 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/mitaka.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      125 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2021-02-01 17:27:42.000000 manila-9.1.5/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1508 2021-02-01 17:27:43.000000 manila-9.1.5/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3945 2021-02-01 17:28:24.343375 manila-9.1.5/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2021-02-01 17:27:43.000000 manila-9.1.5/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      950 2021-02-01 17:27:43.000000 manila-9.1.5/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2021-02-01 17:28:24.339374 manila-9.1.5/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1197 2021-02-01 17:27:43.000000 manila-9.1.5/tools/check_exec.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      435 2021-02-01 17:27:43.000000 manila-9.1.5/tools/check_logging.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1883 2021-02-01 17:27:42.000000 manila-9.1.5/tools/coding-checks.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2472 2021-02-01 17:27:42.000000 manila-9.1.5/tools/cover.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1223 2021-02-01 17:27:42.000000 manila-9.1.5/tools/enable-pre-commit-hook.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      299 2021-02-01 17:27:42.000000 manila-9.1.5/tools/fast8.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2401 2021-02-01 17:27:43.000000 manila-9.1.5/tools/install_venv.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5959 2021-02-01 17:27:43.000000 manila-9.1.5/tools/install_venv_common.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1991 2021-02-01 17:27:43.000000 manila-9.1.5/tools/test-setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1407 2021-02-01 17:27:42.000000 manila-9.1.5/tools/validate-json-files.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      198 2021-02-01 17:27:42.000000 manila-9.1.5/tools/with_venv.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5234 2021-02-01 17:27:43.000000 manila-9.1.5/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `manila-9.1.4/devstack/upgrade/settings` & `manila-9.1.5/devstack/upgrade/settings`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/devstack/upgrade/from-mitaka/upgrade-manila` & `manila-9.1.5/devstack/upgrade/from-mitaka/upgrade-manila`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/devstack/upgrade/upgrade.sh` & `manila-9.1.5/devstack/upgrade/upgrade.sh`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/devstack/upgrade/resources.sh` & `manila-9.1.5/devstack/upgrade/resources.sh`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 set -o xtrace
 
 ################################# Settings ####################################
 
 # Access rules data specific to first enabled backend.
 MANILA_GRENADE_ACCESS_TYPE=${MANILA_GRENADE_ACCESS_TYPE:-"ip"}
-MANILA_GRENADE_ACCESS_TO=${MANILA_GRENADE_ACCESS_TO:-"127.0.0.1"}
+MANILA_GRENADE_ACCESS_TO=${MANILA_GRENADE_ACCESS_TO:-"0.0.0.0/0"}
 
 # Network information that will be used in case DHSS=True driver is used
 # with non-single-network-plugin.
 MANILA_GRENADE_NETWORK_NAME=${MANILA_GRENADE_NETWORK_NAME:-"private"}
 MANILA_GRENADE_SUBNET_NAME=${MANILA_GRENADE_SUBNET_NAME:-"private-subnet"}
 
 # Timeout that will be used for share creation wait operation.
@@ -51,14 +51,16 @@
 
     driver_handles_share_servers=$(iniget $MANILA_CONF $backend driver_handles_share_servers)
 
     create_share_cmd="manila create $share_protocol 1 "
     create_share_cmd+="--share-type $MANILA_GRENADE_SHARE_TYPE_NAME "
     create_share_cmd+="--name $MANILA_GRENADE_SHARE_NAME"
 
+    resource_save manila share_protocol $share_protocol
+
     if [[ $(trueorfalse False driver_handles_share_servers) == True ]]; then
         share_driver=$(iniget $MANILA_CONF $backend share_driver)
         generic_driver='manila.share.drivers.generic.GenericShareDriver'
         windows_driver='manila.share.drivers.windows.windows_smb_driver.WindowsSMBDriver'
         network_plugin=$(iniget $MANILA_CONF $backend network_plugin)
 
         share_network_cmd="manila share-network-create "
@@ -116,14 +118,21 @@
     done
     if [[ $available == 'true' ]]; then
         echo "Share has been created successfully."
     else
         die $LINENO "Share timed out to reach 'available' status."
     fi
 
+    # grab the export location
+    export_path=$(manila share-export-location-list \
+                    $MANILA_GRENADE_SHARE_NAME | grep ":/" | \
+                        cut -d "|" -f 3 | head -1)
+
+    resource_save manila export_path $export_path
+
     # Create some metadata
     manila metadata $MANILA_GRENADE_SHARE_NAME set gre=nade
 
     # Add access rules
     manila access-allow $MANILA_GRENADE_SHARE_NAME \
         $MANILA_GRENADE_ACCESS_TYPE $MANILA_GRENADE_ACCESS_TO
 
@@ -413,45 +422,79 @@
             die $LINENO "Share snapshot timed out to be deleted."
         else
             echo "Share snapshot has been deleted successfully."
         fi
     fi
 }
 
+#####
+
+function scenario_6_do_share_mount_and_write_data {
+
+    mkdir -p /tmp/manila-share
+    export_path=$(resource_get manila export_path)
+    share_protocol=$(resource_get manila share_protocol| awk '{print tolower($0)}')
+    sudo mount -t $share_protocol $export_path /tmp/manila-share
+    test_msg="Hello from the past"
+    echo $test_msg | sudo tee /tmp/manila-share/testfile && sudo sync
+}
+
+function scenario_6_verify_share_mount_and_read_data {
+    export_path=$(resource_get manila export_path)
+    share_is_mounted=$(sudo mount | grep $export_path)
+    [[ -z $share_is_mounted ]] && die $LINENO "Share $export_path is not mounted"
+
+    read_data=$(sudo cat /tmp/manila-share/testfile|xargs)
+    if [[ $read_data == "Hello from the past" ]]; then
+        echo "Share data remains unmodified."
+    else
+        die $LINENO "Share data does not match what was written before upgrade."
+    fi
+}
+
+function scenario_6_destroy_share_mount {
+    export_path=$(resource_get manila export_path)
+    sudo umount -f /tmp/manila-share
+}
+
+
 ################################# Main logic ##################################
 
 function create {
     scenario_1_do_share_with_rules_and_metadata
     scenario_2_do_attach_ss_to_sn
     scenario_3_do_quotas
     scenario_4_do_private_share_types
     scenario_5_do_share_snapshot
+    scenario_6_do_share_mount_and_write_data
     echo "Manila 'create': SUCCESS"
 }
 
 function verify {
     scenario_1_verify_share_with_rules_and_metadata
     scenario_2_verify_attach_ss_to_sn
     scenario_3_verify_quotas
     scenario_4_verify_private_share_types
     scenario_5_verify_share_snapshot
+    scenario_6_verify_share_mount_and_read_data
     echo "Manila 'verify': SUCCESS"
 }
 
 function destroy {
+    scenario_6_destroy_share_mount
     scenario_5_destroy_share_snapshot
     scenario_1_destroy_share_with_rules_and_metadata
     scenario_2_destroy_attach_ss_to_sn
     scenario_3_destroy_quotas
     scenario_4_destroy_private_share_types
     echo "Manila 'destroy': SUCCESS"
 }
 
 function verify_noapi {
-    :
+    scenario_6_verify_share_mount_and_read_data
 }
 
 ################################# Dispatcher ##################################
 
 case $1 in
     "create")
         create
```

### Comparing `manila-9.1.4/devstack/upgrade/from-newton/upgrade-manila` & `manila-9.1.5/devstack/upgrade/from-newton/upgrade-manila`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/devstack/settings` & `manila-9.1.5/devstack/settings`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/devstack/README.rst` & `manila-9.1.5/devstack/README.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/devstack/plugin.sh` & `manila-9.1.5/devstack/plugin.sh`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/devstack/apache-manila.template` & `manila-9.1.5/devstack/apache-manila.template`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/etc/manila/logging_sample.conf` & `manila-9.1.5/etc/manila/logging_sample.conf`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/etc/manila/api-paste.ini` & `manila-9.1.5/etc/manila/api-paste.ini`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/etc/manila/rootwrap.conf` & `manila-9.1.5/etc/manila/rootwrap.conf`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/etc/manila/rootwrap.d/share.filters` & `manila-9.1.5/etc/manila/rootwrap.d/share.filters`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/rally-jobs/rally-manila-no-ss.yaml` & `manila-9.1.5/rally-jobs/rally-manila-no-ss.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/rally-jobs/rally-manila.yaml` & `manila-9.1.5/rally-jobs/rally-manila.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/AUTHORS` & `manila-9.1.5/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 Doug Hellmann <doug@doughellmann.com>
 Douglas Viroel <viroel@gmail.com>
 Duan Jiong <jduan@fiberhome.com>
 Dustin Schoenbrun <dschoenb@redhat.com>
 Emilien Macchi <emilien@redhat.com>
 Eric Harney <eharney@redhat.com>
 Felipe Rodrigues <felipe_futty@hotmail.com>
+Felipe Rodrigues <felipefuty01@gmail.com>
 Flavio Percoco <flaper87@gmail.com>
 Gaurang Tapase <gaurang.tapase@in.ibm.com>
 George Melikov <mail@gmelikov.ru>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Goutham Pacha Ravi <gouthampravi@gmail.com>
 Goutham Pacha Ravi <gouthamr@netapp.com>
 Graham Hayes <graham.hayes@hpe.com>
@@ -290,14 +291,15 @@
 kavithahr <kavitha.r@nectechnologies.in>
 kedy <zhao.kaiA@h3c.com>
 kutner <kutner@netapp.com>
 leiyashuai <leiyashuai@inspur.com>
 li,chen <chen.li@intel.com>
 lijunbo <lijunbo@fiberhome.com>
 lijunjie <lijunjie@cloudin.cn>
+linpeiwen <linpeiwen@troila.com>
 liucheng <liucheng20@huawei.com>
 liujiong <liujiong@gohighsec.com>
 liuke2 <liuke2@huawei.com>
 liumengwen <jelan1022@163.com>
 liushi <liu.shi@navercorp.com>
 liuyamin <liuyamin@fiberhome.com>
 liyanhang <liyh@gohighsec.com>
```

### Comparing `manila-9.1.4/test-requirements.txt` & `manila-9.1.5/test-requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # The order of packages is significant, because pip processes them in the order
 # of appearance. Changing the order has an impact on the overall integration
 # process, which may cause wedges in the gate later.
 
 # hacking should be first
 hacking!=0.13.0,<0.14,>=0.12.0 # Apache-2.0
 
-bashate>=0.5.1 # Apache-2.0
+bashate>=0.6.0 # Apache-2.0
 coverage!=4.4,>=4.0 # Apache-2.0
 ddt>=1.0.1 # MIT
 fixtures>=3.0.0 # Apache-2.0/BSD
 mock>=2.0.0 # BSD
 iso8601>=0.1.11 # MIT
 oslotest>=3.2.0 # Apache-2.0
 
 # Do not remove 'PyMySQL' and 'psycopg2' dependencies. They are used
 # by oslo_db lib for running MySQL and PostgreSQL DB migration tests.
 # See https://docs.openstack.org/oslo.db/latest/contributor/index.html#how-to-run-unit-tests
 PyMySQL>=0.7.6 # MIT License
-psycopg2-binary>=2.6.2 # LGPL/ZPL
+psycopg2-binary>=2.8.3 # LGPL/ZPL
 
 requests-mock>=1.2.0 # Apache-2.0
 os-api-ref>=1.4.0 # Apache-2.0
 os-testr>=1.0.0 # Apache-2.0
 testresources>=2.0.0 # Apache-2.0/BSD
 testscenarios>=0.4 # Apache-2.0/BSD
 testtools>=2.2.0 # MIT
```

### Comparing `manila-9.1.4/setup.py` & `manila-9.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/tox.ini` & `manila-9.1.5/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 minversion = 2.0
 skipsdist = True
 envlist = py3,py27,pep8
 
 [testenv]
 setenv = VIRTUAL_ENV={envdir}
 usedevelop = True
-install_command = pip install -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train} {opts} {packages}
 whitelist_externals = find
-deps = -r{toxinidir}/requirements.txt
-       -r{toxinidir}/test-requirements.txt
+deps =
+  -c{env:UPPER_CONSTRAINTS_FILE:https://releases.openstack.org/constraints/upper/train}
+  -r{toxinidir}/requirements.txt
+  -r{toxinidir}/test-requirements.txt
 commands =
   find . -type f -name "*.py[c|o]" -delete
   stestr run {posargs}
   stestr slowest
 
 [testenv:releasenotes]
 basepython = python3
```

### Comparing `manila-9.1.4/README.rst` & `manila-9.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/CONTRIBUTING.rst` & `manila-9.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/.pylintrc` & `manila-9.1.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/LICENSE` & `manila-9.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/introduce-tooz-library-5fed75b8caffcf42.yaml` & `manila-9.1.5/releasenotes/notes/introduce-tooz-library-5fed75b8caffcf42.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/nexentastor5-v1.1-1ad6c8f7b5cc11b6.yaml` & `manila-9.1.5/releasenotes/notes/nexentastor5-v1.1-1ad6c8f7b5cc11b6.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/bp-share-type-supported-azs-2e12ed406f181b3b.yaml` & `manila-9.1.5/releasenotes/notes/bp-share-type-supported-azs-2e12ed406f181b3b.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/api-versions-mark-v1-deprecated-3540d39279fbd60e.yaml` & `manila-9.1.5/releasenotes/notes/api-versions-mark-v1-deprecated-3540d39279fbd60e.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/bug-1688620-netapp-migration-cancelation-fb913131eb8eb82a.yaml` & `manila-9.1.5/releasenotes/notes/bug-1688620-netapp-migration-cancelation-fb913131eb8eb82a.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/rename-cephfs-native-driver-3d9b4e3c6c78ee98.yaml` & `manila-9.1.5/releasenotes/notes/rename-cephfs-native-driver-3d9b4e3c6c78ee98.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/lvm-export-ips-5f73f30df94381d3.yaml` & `manila-9.1.5/releasenotes/notes/lvm-export-ips-5f73f30df94381d3.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/bp-ocata-migration-improvements-c8c5675e266100da.yaml` & `manila-9.1.5/releasenotes/notes/bp-ocata-migration-improvements-c8c5675e266100da.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/disable-share-groups-api-by-default-0627b97ac2cda4cb.yaml` & `manila-9.1.5/releasenotes/notes/disable-share-groups-api-by-default-0627b97ac2cda4cb.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/powermax-rebrand-manila-a46a0c2ac0aa77ed.yaml` & `manila-9.1.5/releasenotes/notes/powermax-rebrand-manila-a46a0c2ac0aa77ed.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/unity-vnx-rename-options-1656168dd4bdba70.yaml` & `manila-9.1.5/releasenotes/notes/unity-vnx-rename-options-1656168dd4bdba70.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/add-share-access-metadata-4fda2c06e750e83c.yaml` & `manila-9.1.5/releasenotes/notes/add-share-access-metadata-4fda2c06e750e83c.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/share-network-with-multiple-subnets-a56be8b646b9e463.yaml` & `manila-9.1.5/releasenotes/notes/share-network-with-multiple-subnets-a56be8b646b9e463.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/bug-1626249-reintroduce-per-share-instance-access-rule-state-7c08a91373b21557.yaml` & `manila-9.1.5/releasenotes/notes/bug-1626249-reintroduce-per-share-instance-access-rule-state-7c08a91373b21557.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/per-backend-az-590c68be0e2cb4bd.yaml` & `manila-9.1.5/releasenotes/notes/per-backend-az-590c68be0e2cb4bd.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/bug-1704971-fix-name-description-filter-85935582e89a72a0.yaml` & `manila-9.1.5/releasenotes/notes/bug-1704971-fix-name-description-filter-85935582e89a72a0.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/remove-host-field-from-shares-and-replicas-a087f85bc4a4ba45.yaml` & `manila-9.1.5/releasenotes/notes/remove-host-field-from-shares-and-replicas-a087f85bc4a4ba45.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/ibm-gpfs-ces-support-3498e35d9fea1b55.yaml` & `manila-9.1.5/releasenotes/notes/ibm-gpfs-ces-support-3498e35d9fea1b55.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/bp-export-locations-az-api-changes-c8aa1a3a5bc86312.yaml` & `manila-9.1.5/releasenotes/notes/bp-export-locations-az-api-changes-c8aa1a3a5bc86312.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/netapp-cdot-quality-of-service-limits-c1fe8601d00cb5a8.yaml` & `manila-9.1.5/releasenotes/notes/netapp-cdot-quality-of-service-limits-c1fe8601d00cb5a8.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/hnas-driver-rename-7ef74fe720f7e04b.yaml` & `manila-9.1.5/releasenotes/notes/hnas-driver-rename-7ef74fe720f7e04b.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/add-policy-in-code-c31a24ee045d8d21.yaml` & `manila-9.1.5/releasenotes/notes/add-policy-in-code-c31a24ee045d8d21.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/deprecate-old-ks-opts-in-nova-neutron-cinder-groups-e395015088d93fdc.yaml` & `manila-9.1.5/releasenotes/notes/deprecate-old-ks-opts-in-nova-neutron-cinder-groups-e395015088d93fdc.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/newton-migration-improvements-cf9d3d6e37e19c94.yaml` & `manila-9.1.5/releasenotes/notes/newton-migration-improvements-cf9d3d6e37e19c94.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/bug-1801763-gate-public-share-creation-by-policy-a0ad84e4127a3fc3.yaml` & `manila-9.1.5/releasenotes/notes/bug-1801763-gate-public-share-creation-by-policy-a0ad84e4127a3fc3.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/notes/manage-unmanage-share-servers-cd4a6523d8e9fbdf.yaml` & `manila-9.1.5/releasenotes/notes/manage-unmanage-share-servers-cd4a6523d8e9fbdf.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/source/index.rst` & `manila-9.1.5/releasenotes/source/index.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po` & `manila-9.1.5/releasenotes/source/locale/es/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po` & `manila-9.1.5/releasenotes/source/locale/fr/LC_MESSAGES/releasenotes.po`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/releasenotes/source/conf.py` & `manila-9.1.5/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/README.rst` & `manila-9.1.5/doc/README.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/development.environment.rst` & `manila-9.1.5/doc/source/contributor/development.environment.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/pool-aware-manila-scheduler.rst` & `manila-9.1.5/doc/source/contributor/pool-aware-manila-scheduler.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/development-environment-devstack.rst` & `manila-9.1.5/doc/source/contributor/development-environment-devstack.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/share.rst` & `manila-9.1.5/doc/source/contributor/share.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/driver_filter_goodness_weigher.rst` & `manila-9.1.5/doc/source/contributor/driver_filter_goodness_weigher.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/index.rst` & `manila-9.1.5/doc/source/contributor/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -24,25 +24,25 @@
 Programming HowTos and Tutorials
 --------------------------------
 .. toctree::
     :maxdepth: 3
 
     development.environment
     development-environment-devstack
+    apache-httpd
     unit_tests
     tempest_tests
     addmethod.openstackapi
     documenting_your_work
     adding_release_notes
     commit_message_tags
     guru_meditation_report
     user_messages
     ganesha
 
-
 Background Concepts for manila
 ------------------------------
 .. toctree::
    :maxdepth: 3
 
    architecture
    threading
```

### Comparing `manila-9.1.4/doc/source/contributor/database.rst` & `manila-9.1.5/doc/source/contributor/database.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/gerrit.rst` & `manila-9.1.5/doc/source/contributor/gerrit.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/manila-review-policy.rst` & `manila-9.1.5/doc/source/contributor/manila-review-policy.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/services.rst` & `manila-9.1.5/doc/source/contributor/services.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/manila.rst` & `manila-9.1.5/doc/source/contributor/manila.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/documenting_your_work.rst` & `manila-9.1.5/doc/source/contributor/documenting_your_work.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/user_messages.rst` & `manila-9.1.5/doc/source/contributor/user_messages.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/adding_release_notes.rst` & `manila-9.1.5/doc/source/contributor/adding_release_notes.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/share_replication.rst` & `manila-9.1.5/doc/source/contributor/share_replication.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/samples/generic_local.conf` & `manila-9.1.5/doc/source/contributor/samples/generic_local.conf`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/samples/container_local.conf` & `manila-9.1.5/doc/source/contributor/samples/container_local.conf`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/samples/zfsonlinux_local.conf` & `manila-9.1.5/doc/source/contributor/samples/zfsonlinux_local.conf`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/samples/lvm_local.conf` & `manila-9.1.5/doc/source/contributor/samples/lvm_local.conf`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/samples/cephfs_local.conf` & `manila-9.1.5/doc/source/contributor/samples/cephfs_local.conf`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/launchpad.rst` & `manila-9.1.5/doc/source/contributor/launchpad.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/commit_message_tags.rst` & `manila-9.1.5/doc/source/contributor/commit_message_tags.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/auth.rst` & `manila-9.1.5/doc/source/contributor/auth.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/intro.rst` & `manila-9.1.5/doc/source/contributor/intro.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/i18n.rst` & `manila-9.1.5/doc/source/contributor/i18n.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/rpc.rst` & `manila-9.1.5/doc/source/contributor/rpc.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/guru_meditation_report.rst` & `manila-9.1.5/doc/source/contributor/guru_meditation_report.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/tempest_tests.rst` & `manila-9.1.5/doc/source/contributor/tempest_tests.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/scheduler.rst` & `manila-9.1.5/doc/source/contributor/scheduler.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/addmethod.openstackapi.rst` & `manila-9.1.5/doc/source/contributor/addmethod.openstackapi.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/architecture.rst` & `manila-9.1.5/doc/source/contributor/architecture.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/threading.rst` & `manila-9.1.5/doc/source/contributor/threading.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/ganesha.rst` & `manila-9.1.5/doc/source/contributor/ganesha.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/driver_requirements.rst` & `manila-9.1.5/doc/source/admin/emc_unity_driver.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,230 +1,266 @@
 ..
-      Copyright (c) 2015 Hitachi Data Systems
+      Copyright (c) 2014 EMC Corporation
       All Rights Reserved.
 
       Licensed under the Apache License, Version 2.0 (the "License"); you may
       not use this file except in compliance with the License. You may obtain
       a copy of the License at
 
           http://www.apache.org/licenses/LICENSE-2.0
 
       Unless required by applicable law or agreed to in writing, software
       distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
       WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
       License for the specific language governing permissions and limitations
       under the License.
 
-Manila minimum requirements and features since Mitaka
-=====================================================
 
-In order for a driver to be accepted into manila code base, there are certain
-minimum requirements and features that must be met, in order to ensure
-interoperability and standardized manila functionality among cloud providers.
-
-At least one driver mode (:term:`DHSS` true/false)
---------------------------------------------------
-
-Driver modes determine if the driver is managing network resources
-(:term:`DHSS` = true) in an automated way, in order to segregate tenants and
-private networks by making use of manila Share Networks, or if it is up to the
-administrator to manually configure all networks (:term:`DHSS` = false) and be
-responsible for segregation, if that is desired. At least one driver mode must
-be supported. In :term:`DHSS` = true mode, Share Server entities are used, so
-the driver must implement functions that setup and teardown such servers.
-
-At least one file system sharing protocol
------------------------------------------
-
-In order to serve shares as a shared file system service, the driver must
-support at least one file system sharing protocol, which can be a new protocol
-or one of the currently supported protocols. The current list of supported
-protocols is as follows:
-
-- NFS
-- CIFS
-- GlusterFS
-- HDFS
-- MapRFS
-- CephFS
+Unity Driver
+============
 
-Access rules
+EMC manila driver framework (EMCShareDriver) utilizes the EMC storage products
+to provide the shared filesystems to OpenStack. The EMC manila driver is a
+plugin based driver which is designed to use different plugins to manage
+different EMC storage products.
+
+Unity plugin is the plugin which manages the Unity Storage System to provide
+shared filesystems.  EMC driver framework with Unity plugin is referred to as
+Unity driver in this document.
+
+This driver performs the operations on Unity by REST API.  Each backend manages
+one Unity Storage System. Multiple manila backends need to be configured to
+manage multiple Unity Storage Systems.
+
+Requirements
 ------------
 
-Access rules control how shares are accessible, by whom, and what the level of
-access is. Access rule operations include allowing access and denying access
-to a given share. The authentication type should be based on IP, User and/or
-Certificate. Drivers must support read-write and read-only access levels for each
-supported protocol, either through individual access rules or separate export
-locations.
-
-Shares
-------
-
-Share servicing is the core functionality of a shared file system service, so
-a driver must be able to create and delete shares.
-
-Share extending
----------------
-
-In order to best satisfy cloud service requirements, shares must be elastic, so
-drivers must implement a share extend function that allows shares' size to be
-increased.
+- Unity OE 4.0.1 or higher.
+- StorOps 1.1.0 or higher is installed on Manila node.
+- Following licenses are activated on Unity:
+
+  * CIFS/SMB Support
+  * Network File System (NFS)
+  * Thin Provisioning
+  * Fiber Channel (FC)
+  * Internet Small Computer System Interface (iSCSI)
+
+
+Supported Operations
+--------------------
+
+In detail, users are allowed to do following operation with EMC Unity
+Storage Systems.
+
+* Create/delete a NFS share.
+* Create/delete a CIFS share.
+* Extend the size of a share.
+* Shrink the size of a share.
+* Modify the host access privilege of a NFS share.
+* Modify the user access privilege of a CIFS share.
+* Take/Delete snapshot of a share.
+* Create a new share from snapshot.
+* Revert a share to a snapshot.
 
-Capabilities
-------------
 
-In order for manila to function accordingly to the driver being used, the
-driver must provide a set of information to manila, known as capabilities, as
-follows:
-
-- share_backend_name: a name for the backend;
-- driver_handles_share_servers: driver mode, whether this driver instance
-  handles share servers, possible values are true or false;
-- vendor_name: driver vendor name;
-- driver_version: current driver instance version;
-- storage_protocol: list of shared file system protocols supported by this
-  driver instance;
-- total_capacity_gb: total amount of storage space provided, in GB;
-- free_capacity_gb: amount of storage space available for use, in GB;
-- reserved_percentage: percentage of total storage space to be kept from being
-  used.
-
-Certain features, if supported by drivers, need to be reported in order to
-function correctly in manila, such as:
-
-- dedupe: whether the backend supports deduplication;
-- compression: whether the backend supports compressed shares;
-- thin_provisioning: whether the backend is overprovisioning shares;
-- pools: list of storage pools managed by this driver instance;
-- qos: whether the backend supports quality of service for shares;
-- replication_domain: string specifying a common group name for all backends
-  that can replicate between each other;
-- replication_type: string specifying the type of replication supported by
-  the driver. Can be one of ('readable', 'writable' or 'dr').
-
-.. note:: for more information please see https://docs.openstack.org/manila/latest/admin/capabilities_and_extra_specs.html
-
-Continuous Integration systems
-------------------------------
-
-Every driver vendor must supply a CI system that tests its drivers
-continuously for each patch submitted to OpenStack gerrit. This allows for
-better QA and quicker response and notification for driver vendors when a
-patch submitted affects an existing driver. The CI system must run all
-applicable tempest tests, test all patches Jenkins has posted +1 and post its
-test results.
-
-.. note:: for more information please see http://docs.openstack.org/infra/system-config/third_party.html
-
-Unit tests
-----------
-
-All drivers submitted must be contemplated with unit tests covering at least
-90% of the code, preferably 100% if possible. Unit tests must use mock
-framework and be located in-tree using a structure that mirrors the functional
-code, such as directory names and filenames. See template below:
-
-  ::
-
-    manila/[tests/]path/to/brand/new/[test_]driver.py
-
-Documentation
--------------
-
-Drivers submitted must provide and maintain related documentation on
-openstack-manuals, containing instructions on how to properly install and
-configure. The intended audience for this manual is cloud operators and
-administrators. Also, driver maintainers must update the manila share features
-support mapping documentation found at
-https://docs.openstack.org/manila/latest/admin/share_back_ends_feature_support_mapping.html
-
-Manila optional requirements and features since Mitaka
-======================================================
-
-Additional to the minimum required features supported by manila, other optional
-features can be supported by drivers as they are already supported in manila
-and can be accessed through the API.
-
-Snapshots
----------
-
-Share Snapshots allow for data respective to a particular point in time to be
-saved in order to be used later. In manila API, share snapshots taken can only
-be restored by creating new shares from them, thus the original share remains
-unaffected. If Snapshots are supported by drivers, they must be
-crash-consistent.
-
-Managing/Unmanaging shares
---------------------------
-
-If :term:`DHSS` = false mode is used, then drivers may implement a function
-that supports reading existing shares in the backend that were not created by
-manila. After the previously existing share is registered in manila, it is
-completely controlled by manila and should not be handled externally anymore.
-Additionally, a function that de-registers such shares from manila but do
-not delete from backend may also be supported.
-
-Share shrinking
----------------
-
-Manila API supports share shrinking, thus a share can be shrunk in a similar
-way it can be extended, but the driver is responsible for making sure no data
-is compromised.
+Supported Network Topologies
+----------------------------
 
-Share ensuring
---------------
+* flat
+* VLAN
 
-In some situations, such as when the driver is restarted, manila attempts to
-perform maintenance on created shares, on the purpose of ensuring previously
-created shares are available and being serviced correctly. The driver can
-implement this function by checking shares' status and performing maintenance
-operations if needed, such as re-exporting.
 
+Pre-Configurations
+------------------
 
-Manila experimental features since Mitaka
-=========================================
+On Manila Node
+~~~~~~~~~~~~~~
 
-Some features are initially released as experimental and can be accessed by
-including specific additional HTTP Request headers. Those features are not
-recommended for production cloud environments while in experimental stage.
+StorOps library is required to run Unity driver.
+Please install it with the pip command.
+You may need root privilege to install python libraries.
 
-Share Migration
----------------
+::
 
-Shares can be migrated between different backends and pools. Manila implements
-migration using an approach that works for any manufacturer, but driver vendors
-can implement a better optimized migration function for when migration involves
-backends or pools related to the same vendor.
+    pip install storops
 
-Share Groups (since Ocata)
---------------------------
 
-The share groups provides the ability to manage a group of shares together.
-This feature is implemented at the manager level, every driver gets this feature
-by default. If a driver wants to override the default behavior to support
-additional functionalities such as consistent group snapshot, the driver
-vendors may report this capability as a group capability, such as: Ordered
-writes, Consistent snapshots, Group replication.
+On Unity System
+~~~~~~~~~~~~~~~
 
-.. note::
+1. Configure System level NTP Server
 
-  for more information please see
-  `group capabilities <https://docs.openstack.org/manila/latest/admin/group_capabilities_and_extra_specs.html>`_
+Configure the NTP server for your Unity at:
 
-Share Replication
------------------
+.. code-block:: console
 
-Replicas of shares can be created for either data protection (for disaster
-recovery) or for load sharing. In order to utilize this feature, drivers must
-report the ``replication_type`` they support as a capability and implement
-necessary methods.
+    Unisphere -> Settings -> Management -> System Time and NTP
 
-More details can be found at:
-https://docs.openstack.org/manila/latest/admin/shared-file-systems-share-replication.html
+Select "Enable NTP synchronization" and add your NTP server(s).
 
-Update "used_size" of shares
-----------------------------
-Drivers can update, for all the shares created on a particular backend, the
-consumed space in GiB. While the polling interval for drivers to update this
-information is configurable, drivers can choose to submit cached information
-as necessary, but specify a time at which this information was "gathered_at".
+2. Configure System level DNS Server
+
+Configure the DNS server for your Unity at:
+
+.. code-block:: console
+
+    Unisphere -> Settings -> Management -> DNS Server
+
+Select "Configure DNS server address manually" and add your DNS server(s).
+
+
+Configurations
+--------------
+
+Following configurations need to be configured in `/etc/manila/manila.conf`
+for the Unity driver.
+
+.. code-block:: ini
+
+    share_driver = manila.share.drivers.dell_emc.driver.EMCShareDriver
+    emc_share_backend = unity
+    emc_nas_server = <management IP address of the Unity system>
+    emc_nas_login = <user with administrator privilege>
+    emc_nas_password = <password>
+    unity_server_meta_pool = <pool name>
+    unity_share_data_pools = <comma separated pool names>
+    unity_ethernet_ports = <comma separated ports list>
+    driver_handles_share_servers = True/False
+    unity_share_server = <name of NAS server in Unity system>
+
+- `emc_share_backend`
+    The plugin name. Set it to `unity` for the Unity driver.
+
+- `emc_nas_server`
+    The management IP for Unity.
+
+- `unity_server_meta_pool`
+    The name of the pool to persist the meta-data of NAS server.
+    This option is required.
+
+- `unity_share_data_pools`
+    Comma separated list specifying the name of the pools to be used
+    by this backend. Do not set this option if all storage pools
+    on the system can be used.
+    Wild card character is supported.
+
+    Examples:
+
+    .. code-block:: ini
+
+       # Only use pool_1
+       unity_share_data_pools = pool_1
+       # Only use pools whose name stars from pool_
+       unity_share_data_pools = pool_*
+       # Use all pools on Unity
+       unity_share_data_pools = *
+
+- `unity_ethernet_ports`
+    Comma separated list specifying the ethernet ports of Unity system
+    that can be used for share. Do not set this option if all ethernet ports
+    can be used.
+    Wild card character is supported. Both the normal ethernet port and link
+    aggregation port can be used by Unity share driver.
+
+
+    Examples:
+
+    .. code-block:: ini
+
+       # Only use spa_eth1
+       unity_ethernet_ports = spa_eth1
+       # Use port whose name stars from spa_
+       unity_ethernet_ports = spa_*
+       # Use all Link Aggregation ports
+       unity_ethernet_ports = sp*_la_*
+       # Use all available ports
+       unity_ethernet_ports = *
+
+- `driver_handles_share_servers`
+    Unity driver requires this option to be as `True` or `False`.
+    Need to set `unity_share_server` when the value is `False`.
+
+- `unity_share_server`
+    One of NAS server names in Unity, it is used for share creation when
+    the driver is in `DHSS=False` mode.
+
+Restart of :term:`manila-share` service is needed for the configuration changes to take
+effect.
+
+IPv6 support
+------------
+
+IPv6 support for Unity driver is introduced in Queens release. The feature is divided
+into two parts:
+
+1. The driver is able to manage share or snapshot in the Neutron IPv6 network.
+2. The driver is able to connect Unity management interface using its IPv6 address.
+
+Snapshot support
+----------------
+
+In the Mitaka and Newton release of OpenStack, Snapshot support is enabled by default for a newly created share type.
+Starting with the Ocata release, the snapshot_support extra spec must be set to True in order to allow snapshots for
+a share type. If the 'snapshot_support' extra_spec is omitted or if it is set to False, users would not be able to
+create snapshots on shares of this share type. The feature is divided into two parts:
+
+1. The driver is able to create/delete snapshot of share.
+2. The driver is able to create share from snapshot.
+
+Restrictions
+------------
+
+The Unity driver has following restrictions.
+
+- EMC Unity does not support the same IP in different VLANs.
+- Only IP access type is supported for NFS.
+- Only user access type is supported for CIFS.
+
+
+API Implementations
+-------------------
+
+Following driver features are implemented in the plugin.
+
+* create_share: Create a share and export it based on the protocol used
+  (NFS or CIFS).
+* create_share_from_snapshot: Create a share from a snapshot - clone a
+  snapshot.
+* delete_share: Delete a share.
+* extend_share: Extend the maximum size of a share.
+* shrink_share: Shrink the minimum size of a share.
+* create_snapshot: Create a snapshot for the specified share.
+* delete_snapshot: Delete the snapshot of the share.
+* update_access: recover, add or delete user/host access to a share.
+* allow_access: Allow access (read write/read only) of a user to a
+  CIFS share.  Allow access (read write/read only) of a host to a NFS
+  share.
+* deny_access: Remove access (read write/read only) of a user from
+  a CIFS share.  Remove access (read write/read only) of a host from a
+  NFS share.
+* ensure_share: Check whether share exists or not.
+* update_share_stats: Retrieve share related statistics from Unity.
+* get_network_allocations_number: Returns number of network allocations for
+  creating VIFs.
+* setup_server: Set up and configures share server with given network
+  parameters.
+* teardown_server: Tear down the share server.
+* revert_to_snapshot: Revert a share to a snapshot.
+
+
+The :mod:`manila.share.drivers.dell_emc.driver` Module
+------------------------------------------------------
+
+.. automodule:: manila.share.drivers.dell_emc.driver
+    :noindex:
+    :members:
+    :undoc-members:
+    :show-inheritance:
+
+The :mod:`manila.share.drivers.dell_emc.plugins.unity.connection` Module
+------------------------------------------------------------------------
+
+.. automodule:: manila.share.drivers.dell_emc.plugins.unity.connection
+    :noindex:
+    :members:
+    :undoc-members:
+    :show-inheritance:
```

### Comparing `manila-9.1.4/doc/source/contributor/fakes.rst` & `manila-9.1.5/doc/source/contributor/fakes.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/share_migration.rst` & `manila-9.1.5/doc/source/contributor/share_migration.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/api_microversion_dev.rst` & `manila-9.1.5/doc/source/contributor/api_microversion_dev.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/experimental_apis.rst` & `manila-9.1.5/doc/source/contributor/experimental_apis.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/unit_tests.rst` & `manila-9.1.5/doc/source/contributor/unit_tests.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/contributor/share_hooks.rst` & `manila-9.1.5/doc/source/contributor/share_hooks.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/index.rst` & `manila-9.1.5/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/figures/hwreqs.graffle` & `manila-9.1.5/doc/source/install/figures/hwreqs.graffle`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/figures/hwreqs.svg` & `manila-9.1.5/doc/source/install/figures/hwreqs.svg`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/figures/hwreqs.png` & `manila-9.1.5/doc/source/install/figures/hwreqs.png`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/verify.rst` & `manila-9.1.5/doc/source/install/verify.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/index.rst` & `manila-9.1.5/doc/source/install/index.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/post-install.rst` & `manila-9.1.5/doc/source/install/post-install.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/install-controller-debian.rst` & `manila-9.1.5/doc/source/install/install-controller-debian.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/install-share-node.rst` & `manila-9.1.5/doc/source/install/install-share-node.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/install-controller-obs.rst` & `manila-9.1.5/doc/source/install/install-controller-obs.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/install-controller-ubuntu.rst` & `manila-9.1.5/doc/source/install/install-controller-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/common/share-node-share-server-modes.rst` & `manila-9.1.5/doc/source/install/common/share-node-share-server-modes.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/common/controller-node-prerequisites.rst` & `manila-9.1.5/doc/source/install/common/controller-node-prerequisites.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/common/dhss-true-mode-using-shared-file-systems.rst` & `manila-9.1.5/doc/source/install/common/dhss-true-mode-using-shared-file-systems.rst`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,16 @@
       ``service_instance_password`` in your configuration, a key-pair may be
       specified with options ``path_to_public_key`` and
       ``path_to_private_key`` to configure and allow password-less SSH access
       between the `share node` and the share server/s created.
 
    .. code-block:: console
 
-      $ curl https://tarballs.openstack.org/manila-image-elements/images/manila-service-image-master.qcow2 | \
+      $ curl -L \
+      https://tarballs.opendev.org/openstack/manila-image-elements/images/manila-service-image-master.qcow2 | \
       glance image-create \
       --name "manila-service-image" \
       --disk-format qcow2 \
       --container-format bare \
       --visibility public --progress
       %   Total    %   Received %   Xferd  Average  Speed   Time     Time     Time      Current
                                            Dload    Upload  Total    Spent    Left      Speed
```

### Comparing `manila-9.1.4/doc/source/install/common/dhss-true-mode-configuration.rst` & `manila-9.1.5/doc/source/install/common/dhss-true-mode-configuration.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/common/dhss-false-mode-using-shared-file-systems.rst` & `manila-9.1.5/doc/source/install/common/dhss-false-mode-using-shared-file-systems.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/common/dhss-false-mode-configuration.rst` & `manila-9.1.5/doc/source/install/common/dhss-false-mode-configuration.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/common/dhss-true-mode-intro.rst` & `manila-9.1.5/doc/source/install/common/dhss-true-mode-intro.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/common/controller-node-common-configuration.rst` & `manila-9.1.5/doc/source/install/common/controller-node-common-configuration.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/common/share-node-common-configuration.rst` & `manila-9.1.5/doc/source/install/common/share-node-common-configuration.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/get-started-with-shared-file-systems.rst` & `manila-9.1.5/doc/source/install/get-started-with-shared-file-systems.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/install-controller-node.rst` & `manila-9.1.5/doc/source/install/install-controller-node.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/install-share-obs.rst` & `manila-9.1.5/doc/source/install/install-share-obs.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/install-controller-rdo.rst` & `manila-9.1.5/doc/source/install/install-controller-rdo.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/install-share-debian.rst` & `manila-9.1.5/doc/source/install/install-share-debian.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/conf.py` & `manila-9.1.5/doc/source/install/conf.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/install-share-rdo.rst` & `manila-9.1.5/doc/source/install/install-share-rdo.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/install/install-share-ubuntu.rst` & `manila-9.1.5/doc/source/install/install-share-ubuntu.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/cli/manila-status.rst` & `manila-9.1.5/doc/source/cli/manila-status.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/cli/index.rst` & `manila-9.1.5/doc/source/cli/index.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/cli/manila.rst` & `manila-9.1.5/doc/source/cli/manila.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/cli/manila-manage.rst` & `manila-9.1.5/doc/source/cli/manila-manage.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/user/create-and-manage-shares.rst` & `manila-9.1.5/doc/source/user/create-and-manage-shares.rst`

 * *Files 17% similar despite different names*

```diff
@@ -157,72 +157,130 @@
 Allow read-write access
 ~~~~~~~~~~~~~~~~~~~~~~~
 
 #. Allow access.
 
    .. code-block:: console
 
-      $ manila access-allow myshare ip 10.0.0.0/24
+      $ manila access-allow myshare ip 10.0.0.0/24 --metadata key1=value1
       +--------------+--------------------------------------+
       | Property     | Value                                |
       +--------------+--------------------------------------+
+      | id           | 0c8470ca-0d77-490c-9e71-29e1f453bf97 |
       | share_id     | 8d8b854b-ec32-43f1-acc0-1b2efa7c3400 |
-      | access_type  | ip                                   |
-      | access_to    | 10.0.0.0/24                          |
       | access_level | rw                                   |
-      | state        | new                                  |
-      | id           | 0c8470ca-0d77-490c-9e71-29e1f453bf97 |
+      | access_to    | 10.0.0.0/24                          |
+      | access_type  | ip                                   |
+      | state        | queued_to_apply                      |
+      | access_key   | None                                 |
+      | created_at   | 2016-03-24T14:51:36.000000           |
+      | updated_at   | None                                 |
+      | metadata     | {'key1': 'value1'}                   |
       +--------------+--------------------------------------+
 
+   .. note::
+      Since API version 2.45, metadata can be added, removed and updated for
+      share access rules in a form of key=value pairs.
+
+
 #. List access.
 
    .. code-block:: console
 
       $ manila access-list myshare
-      +--------------------------------------+-------------+-------------+--------------+--------+
-      | id                                   | access_type | access_to   | access_level | state  |
-      +--------------------------------------+-------------+-------------+--------------+--------+
-      | 0c8470ca-0d77-490c-9e71-29e1f453bf97 | ip          | 10.0.0.0/24 | rw           | active |
-      +--------------------------------------+-------------+-------------+--------------+--------+
+      +--------------------------------------+-------------+-------------+--------------+--------+------------+----------------------------+------------+
+      | id                                   | access_type | access_to   | access_level | state  | access_key | created_at                 | updated_at |
+      +--------------------------------------+-------------+-------------+--------------+--------+------------+----------------------------+------------+
+      | 0c8470ca-0d77-490c-9e71-29e1f453bf97 | ip          | 10.0.0.0/24 | rw           | active | None       | 2016-03-24T14:51:36.000000 | None       |
+      +--------------------------------------+-------------+-------------+--------------+--------+------------+----------------------------+------------+
 
    The access is created.
 
 Allow read-only access
 ~~~~~~~~~~~~~~~~~~~~~~
 
 #. Allow access.
 
    .. code-block:: console
 
       $ manila access-allow myshare ip 20.0.0.0/24 --access-level ro
       +--------------+--------------------------------------+
       | Property     | Value                                |
       +--------------+--------------------------------------+
+      | id           | f151ad17-654d-40ce-ba5d-98a5df67aadc |
       | share_id     | 8d8b854b-ec32-43f1-acc0-1b2efa7c3400 |
-      | access_type  | ip                                   |
-      | access_to    | 20.0.0.0/24                          |
       | access_level | ro                                   |
-      | state        | new                                  |
-      | id           | f151ad17-654d-40ce-ba5d-98a5df67aadc |
+      | access_to    | 20.0.0.0/24                          |
+      | access_type  | ip                                   |
+      | state        | queued_to_apply                      |
+      | access_key   | None                                 |
+      | created_at   | 2016-03-24T14:54:11.000000           |
+      | updated_at   | None                                 |
+      | metadata     | {}                                   |
       +--------------+--------------------------------------+
 
 #. List access.
 
    .. code-block:: console
 
       $ manila access-list myshare
-      +--------------------------------------+-------------+-------------+--------------+--------+
-      | id                                   | access_type | access_to   | access_level | state  |
-      +--------------------------------------+-------------+-------------+--------------+--------+
-      | 0c8470ca-0d77-490c-9e71-29e1f453bf97 | ip          | 10.0.0.0/24 | rw           | active |
-      | f151ad17-654d-40ce-ba5d-98a5df67aadc | ip          | 20.0.0.0/24 | ro           | active |
-      +--------------------------------------+-------------+-------------+--------------+--------+
+      +--------------------------------------+-------------+-------------+--------------+--------+------------+----------------------------+------------+
+      | id                                   | access_type | access_to   | access_level | state  | access_key | created_at                 | updated_at |
+      +--------------------------------------+-------------+-------------+--------------+--------+------------+----------------------------+------------+
+      | 0c8470ca-0d77-490c-9e71-29e1f453bf97 | ip          | 10.0.0.0/24 | rw           | active | None       | 2016-03-24T14:51:36.000000 | None       |
+      | f151ad17-654d-40ce-ba5d-98a5df67aadc | ip          | 20.0.0.0/24 | ro           | active | None       | 2016-03-24T14:54:11.000000 | None       |
+      +--------------------------------------+-------------+-------------+--------------+--------+------------+----------------------------+------------+
 
    The access is created.
 
+Update access rules metadata
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+#. Add a new metadata.
+
+   .. code-block:: console
+
+      $ manila access-metadata 0c8470ca-0d77-490c-9e71-29e1f453bf97 set key2=value2
+      $ manila access-show 0c8470ca-0d77-490c-9e71-29e1f453bf97
+      +--------------+--------------------------------------+
+      | Property     | Value                                |
+      +--------------+--------------------------------------+
+      | id           | 0c8470ca-0d77-490c-9e71-29e1f453bf97 |
+      | share_id     | 8d8b854b-ec32-43f1-acc0-1b2efa7c3400 |
+      | access_level | rw                                   |
+      | access_to    | 10.0.0.0/24                          |
+      | access_type  | ip                                   |
+      | state        | active                               |
+      | access_key   | None                                 |
+      | created_at   | 2016-03-24T14:51:36.000000           |
+      | updated_at   | None                                 |
+      | metadata     | {'key1': 'value1', 'key2': 'value2'} |
+      +--------------+--------------------------------------+
+
+#. Remove a metadata key value.
+
+   .. code-block:: console
+
+      $ manila access-metadata 0c8470ca-0d77-490c-9e71-29e1f453bf97 unset key
+      $ manila access-show 0c8470ca-0d77-490c-9e71-29e1f453bf97
+      +--------------+--------------------------------------+
+      | Property     | Value                                |
+      +--------------+--------------------------------------+
+      | id           | 0c8470ca-0d77-490c-9e71-29e1f453bf97 |
+      | share_id     | 8d8b854b-ec32-43f1-acc0-1b2efa7c3400 |
+      | access_level | rw                                   |
+      | access_to    | 10.0.0.0/24                          |
+      | access_type  | ip                                   |
+      | state        | active                               |
+      | access_key   | None                                 |
+      | created_at   | 2016-03-24T14:51:36.000000           |
+      | updated_at   | None                                 |
+      | metadata     | {'key2': 'value2'}                   |
+      +--------------+--------------------------------------+
+
 Deny access
 ~~~~~~~~~~~
 
 #. Deny access.
 
    .. code-block:: console
```

### Comparing `manila-9.1.4/doc/source/user/index.rst` & `manila-9.1.5/doc/source/user/index.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/user/troubleshooting-asynchronous-failures.rst` & `manila-9.1.5/doc/source/user/troubleshooting-asynchronous-failures.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/user/share-network-operations.rst` & `manila-9.1.5/doc/source/user/share-network-operations.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/user/share-network-subnet-operations.rst` & `manila-9.1.5/doc/source/user/share-network-subnet-operations.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/images/rpc/rabt.png` & `manila-9.1.5/doc/source/images/rpc/rabt.png`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/images/rpc/flow1.svg` & `manila-9.1.5/doc/source/images/rpc/flow1.svg`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/images/rpc/arch.png` & `manila-9.1.5/doc/source/images/rpc/arch.png`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/images/rpc/flow2.png` & `manila-9.1.5/doc/source/images/rpc/flow2.png`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/images/rpc/state.png` & `manila-9.1.5/doc/source/images/rpc/state.png`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/images/rpc/flow1.png` & `manila-9.1.5/doc/source/images/rpc/flow1.png`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/images/rpc/rabt.svg` & `manila-9.1.5/doc/source/images/rpc/rabt.svg`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/images/rpc/arch.svg` & `manila-9.1.5/doc/source/images/rpc/arch.svg`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/images/rpc/flow2.svg` & `manila-9.1.5/doc/source/images/rpc/flow2.svg`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/images/rpc/hds_network.jpg` & `manila-9.1.5/doc/source/configuration/figures/hds_network.jpg`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/capabilities_and_extra_specs.rst` & `manila-9.1.5/doc/source/admin/capabilities_and_extra_specs.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,101 @@
 .. _capabilities_and_extra_specs:
 
 Capabilities and Extra-Specs
 ============================
-Manila Administrators create share types with extra-specs to allow users
-to request a type of share to create. The Administrator chooses a name
-for the share type and decides how to communicate the significance of
-the different share types in terms that the users should understand or
-need to know. By design, most of the details of a share type (the extra-
-specs) are not exposed to users -- only Administrators.
-
-Share Types
------------
-Refer to the manila client command-line help for information on how to
-create a share type and set "extra-spec" key/value pairs for a share type.
-
-Extra-Specs
------------
-There are 3 types of extra-specs: required, scoped, and un-scoped.
-
-Manila *requires* the driver_handles_share_servers extra-spec.
-
-*Scoped* extra-specs use a prefix followed by a colon to define a namespace
-for scoping the extra-spec. A prefix could be a vendor name or acronym
-and is a hint that this extra-spec key/value only applies to that vendor's
-driver. Scoped extra-specs are not used by the scheduler to determine
-where a share is created (except for the special `capabilities` prefix).
-It is up to each driver implementation to determine how to use scoped
-extra-specs and to document them.
-
-The prefix "capabilities" is a special prefix to indicate extra-specs that
-are treated like un-scoped extra-specs. In the CapabilitiesFilter the
-"capabilities:" is stripped from the key and then the extra-spec key and
-value are used as an un-scoped extra-spec.
-
-*Un-scoped* extra-specs have a key that either starts with "capabilities:" or
-does not contain a colon. When the CapabilitiesFilter is enabled (it is
-enabled by default), the scheduler will only create a share on a backend
-that reports capabilities that match the share type's un-scoped extra-spec
-keys.
+Cloud Administrators create :ref:`shared_file_systems_share_types` with
+extra-specs to:
 
-The CapabilitiesFilter uses the following for matching operators:
+- influence the scheduler's decision to place new shares, and
+- instruct the Shared File System service or its storage driver/s to perform
+  certain special actions with respect to the users' shares.
+
+As an administrator, you can choose a descriptive name or provide good
+descriptions for your share types to convey the share type capabilities to
+end users. End users can view standard ``tenant-visible`` extra-specs that
+can let them seek required behavior and automate their applications
+accordingly. By design, however, all other extra-specs of a share type are not
+exposed to non-privileged users.
+
+Types of Extra-Specs
+--------------------
+
+The Shared File Systems service back-end storage drivers offer a wide range of
+capabilities. The variation in these capabilities allows cloud
+administrators to provide a storage service catalog to their end users.
+Share type extra-specs tie-in with these capabilities.
+
+Some back-end capabilities are very specific to a storage system, and are
+opaque to the Shared File System service or the end users. These
+capabilities are invoked with the help of "scoped" extra-specs. Using scoped
+extra-specs is a way to provide programmatic directives to the concerned
+storage driver to do something during share creation or share manipulation.
+You can learn about the opaque capabilities through driver documentation
+and configure these capabilities within share types as scoped
+extra-specs (e.g.: hpe3par:nfs_options). The Shared File System service
+scheduler ignores scoped extra-specs during its quest to find the right back
+end to provision shares.
+
+There are some back-end capabilities in manila that do matter to the scheduler.
+For our understanding, lets call these non-scoped or non-opaque capabilities.
+All non-scoped capabilities can be directly used as share types extra-specs.
+They are considered by the scheduler’s capabilities filter (and any custom
+filter defined by deployers).
+
+You can get a list of non-scoped capabilities from the scheduler by using:
+
+.. code-block:: console
+
+    $ manila pool-list --detail
+
+The non-scoped capabilities can be of three types:
+
+- **Capabilities pertaining to a specific back end storage system driver**: For
+  example, *huawei_smartcache*.
+  No Shared File System service API relies on non-opaque back end specific
+  capabilities.
+- **Common capabilities that are not visible to end users**: The manila
+  community has standardized some cross-platform capabilities like
+  *thin_provisioning*, *dedupe*, *compression*, *qos*, *ipv6_support* and
+  *ipv4_support*. Values of these options do not matter to any Shared File
+  System service APIs; however, they can signify something to the manila
+  services themselves. For example when a back end supports thin_provisioning,
+  the scheduler service performs over-provisioning, and if a back end does
+  not report *ipv6_support* as True, the share-manager service drops IPv6
+  access rules before invoking the storage driver to update access rules.
+- **Common capabilities that are visible to end users**: Some capabilities
+  affect functionality exposed via the Shared File System service API. For
+  example, not all back ends support snapshots, and even if they do, they
+  may not support all of the snapshot operations. For example, cloning
+  snapshots into new shares, reverting shares in-place to snapshots, etc.
+
+  The support for these capabilities determines whether users would be able
+  to perform certain control-plane operations with manila. For example, a back
+  end driver may report *snapshot_support=True* allowing end users to
+  create share snapshots, however, the driver can report
+  *create_share_from_snapshot_support=False*.
+  This reporting allows cloud administrators to create share types that
+  support snapshots but not creating shares from snapshots. When a user uses
+  such a share type, they will not be able to clone snapshots into new shares.
+  Tenant-visible capabilities aid manila in validating requests and failing
+  fast on requests it cannot accommodate. They also help level set the user
+  expectations on some failures. For example, if snapshot_support is set to
+  False on the share type, since users can see this, they will not invoke
+  the create snapshot API, and even if they do, they will understand the
+  HTTP 400 (and error message) in better context.
+
+.. important::
+
+    All extra-specs are optional, except one: *driver_handles_share_servers*.
+
+Scheduler's treatment of non-scoped extra specs
+-----------------------------------------------
+
+The CapabilitiesFilter in the Shared File System scheduler uses the following
+for matching operators:
 
 * No operator
   This defaults to doing a python ==. Additionally it will match boolean values.
 
 * **<=, >=, ==, !=**
 
   This does a float conversion and then uses the python operators as expected.
@@ -70,225 +122,138 @@
 
   This does a float conversion and chooses a host that has equal to or greater
   than the resource specified. This operator behaves this way for historical
   reasons.
 
 * **s==, s!=, s>=, s>, s<=, s<**
 
-  The "s" indicates it is a string comparison. These choose a host that satisfies
-  the comparison of strings in capability and specification. For example,
-  if "capabilities:replication_type s== dr", a host that reports
-  replication_type of "dr" will be chosen.
-
-For vendor-specific capabilities (which need to be visible to the
-CapabilityFilter), it is recommended to use the vendor prefix followed
-by an underscore. This is not a strict requirement, but will provide a
+  The "s" indicates it is a string comparison. These choose a host that
+  satisfies the comparison of strings in capability and specification. For
+  example, if "capabilities:replication_type s== dr", a host that reports
+  replication_type of "dr" will be chosen. If "share_backend_name s!=
+  cephfs" is used, any host not named "cephfs" can be chosen.
+
+For vendor-specific non-scoped capabilities (which need to be visible to the
+scheduler), drivers are recommended to use the vendor prefix followed
+by an underscore. This is not a strict requirement, but can provide a
 consistent look along-side the scoped extra-specs and will be a clear
 indicator of vendor capabilities vs. common capabilities.
 
 Common Capabilities
 -------------------
-For capabilities that apply to multiple backends a common capability can
-be created. Like all other backend reported capabilities, these capabilities
+Common capabilities apply to multiple backends.
+Like all other backend reported capabilities, these capabilities
 can be used verbatim as extra_specs in share types used to create shares.
 
-* `driver_handles_share_servers` is a special, required, user-visible common
-  capability. Added in Kilo.
+Share type common capability extra-specs that are visible to end users:
+-----------------------------------------------------------------------
 
-* `dedupe` - indicates that a backend/pool can provide shares using some
-  deduplication technology. The default value of the dedupe capability (if a
-  driver doesn't report it) is False. In Liberty, drivers cannot report to the
-  scheduler that they support both dedupe and non-deduped share. For each pool
-  it's either always on or always off, even if the drivers can technically
-  support both dedupe and non-deduped in a pool. Since Mitaka, the logic is
-  changed to allow a driver to report dedupe=[True, False] if it can support
-  both dedupe and non-deduped in a pool. Administrators can make a share type
-  use deduplication by setting this extra-spec to '<is> True'. Administrators
-  can prevent a share type from using deduplication by setting this extra-spec
-  to '<is> False'. Added in Liberty.
+* **driver_handles_share_servers** is a special, required common
+  capability. When set to True, the scheduler matches requests with back ends
+  that can isolate user workloads with dedicated share servers exporting
+  shares on user provided share networks.
 
-* `compression` - indicates that a backend/pool can provide shares using some
-  compression technology. The default value of the compression capability (if a
-  driver doesn't report it) is False. In Liberty, drivers cannot report to the
-  scheduler that they support both compression and non-compression. For each
-  pool it's either always on or always off, even if the drivers can technically
-  support both compression and non-compression in a pool. Since Mitaka, the
-  logic is changed to allow a driver to report compression=[True, False] if it
-  can support both compression and non-compression in a pool. Administrators
-  can make a share type use compression by setting this extra-spec to
-  '<is> True'. Administrators can prevent a share type from using compression
-  by setting this extra-spec to '<is> False'. Added in Liberty.
-
-* `thin_provisioning` - shares will not be space guaranteed and
-  overprovisioning will be enabled. This capability defaults to False.
-  Backends/pools that support thin provisioning must report True for this
-  capability. Administrators can make a share type use thin provisioned shares
-  by setting this extra-spec to '<is> True'. If a driver reports
-  thin_provisioning=False (the default) then it's assumed that the driver is
-  doing thick provisioning and overprovisioning is turned off.
-  This was added in Liberty. In Liberty and Mitaka, the driver was required
-  to configure one pool for thin and another pool for thick and report
-  thin_provisioning as either True or False even if an array can technically
-  support both thin and thick provisioning in a pool. In Newton, the logic is
-  changed to allow a driver to report thin_provisioning=[True, False] if it
-  can support both thin and thick provisioning in a pool. To provision a thick
-  share on a back end that supports both thin and thick provisioning, set one
-  of the following in extra specs:
+* **snapshot_support** indicates whether snapshots are supported for shares
+  created on the pool/backend. When administrators do not set this capability
+  as an extra-spec in a share type, the scheduler can place new shares of that
+  type in pools without regard for whether snapshots are supported, and those
+  shares will not support snapshots.
 
-::
+* **create_share_from_snapshot_support** indicates whether a backend can
+  create a new share from a snapshot. When administrators do not set this
+  capability as an extra-spec in a share type, the scheduler can place new
+  shares of that type in pools without regard for whether creating shares
+  from snapshots is supported, and those shares will not support creating
+  shares from snapshots.
 
-    {'thin_provisioning': 'False'}
-    {'thin_provisioning': '<is> False'}
-    {'capabilities:thin_provisioning': 'False'}
-    {'capabilities:thin_provisioning': '<is> False'}
+* **revert_to_snapshot_support** indicates that a driver is capable of
+  reverting a share in place to its most recent snapshot. When administrators
+  do not set this capability as an extra-spec in a share type, the scheduler
+  can place new shares of that type in pools without regard for whether
+  reverting shares to snapshots is supported, and those shares will not support
+  reverting shares to snapshots.
 
-* `qos` - indicates that a backend/pool can provide shares using some
-  QoS (Quality of Service) specification. The default value of the qos
-  capability (if a driver doesn't report it) is False. Administrators
-  can make a share type use QoS by setting this extra-spec to '<is> True' and
-  also setting the relevant QoS-related extra specs for the drivers being used.
-  Administrators can prevent a share type from using QoS by setting this
-  extra-spec to '<is> False'. Different drivers have different ways of specifying
-  QoS limits (or guarantees) and this extra spec merely allows the scheduler to
-  filter by pools that either have or don't have QoS support enabled. Added in
-  Mitaka.
+* **mount_snapshot_support** indicates that a driver is capable of exporting
+  share snapshots for mounting. Users can provide and revoke access to
+  mountable snapshots just like they can with their shares.
 
-* `replication_type` - indicates the style of replication supported for the
+* **replication_type** indicates the style of replication supported for the
   backend/pool. This extra_spec will have a string value and could be one
   of :term:`writable`, :term:`readable` or :term:`dr`. `writable` replication
   type involves synchronously replicated shares where all replicas are
   writable. Promotion is not supported and not needed. `readable` and `dr`
   replication types involve a single `active` or `primary` replica and one or
   more `non-active` or secondary replicas per share. In `readable` type of
   replication, `non-active` replicas have one or more export_locations and
   can thus be mounted and read while the `active` replica is the only one
   that can be written into. In `dr` style of replication, only
-  the `active` replica can be mounted, read from and written into. Added in
-  Mitaka.
+  the `active` replica can be mounted, read from and written into.
 
-* `snapshot_support` - indicates whether snapshots are supported for shares
-  created on the pool/backend. When administrators do not set this capability
-  as an extra-spec in a share type, the scheduler can place new shares of that
-  type in pools without regard for whether snapshots are supported, and those
-  shares will not support snapshots.
+* **availability_zones** indicates a comma separated list of availability
+  zones that can be used for provisioning. Users can always provide a specific
+  availability zone during share creation, and they will receive a
+  synchronous failure message if they attempt to create a share in an
+  availability zone that the share type does not permit. If you do not set
+  this extra-spec, the share type is assumed to be serviceable in all
+  availability zones known to the Shared File Systems service.
 
-* `create_share_from_snapshot_support` - indicates whether a backend can create
-  a new share from a snapshot. When administrators do not set this capability
-  as an extra-spec in a share type, the scheduler can place new shares of that
-  type in pools without regard for whether creating shares from snapshots is
-  supported, and those shares will not support creating shares from snapshots.
-
-* `revert_to_snapshot_support` - indicates that a driver is capable of
-  reverting a share in place to its most recent snapshot. When administrators
-  do not set this capability as an extra-spec in a share type, the scheduler
-  can place new shares of that type in pools without regard for whether
-  reverting shares to snapshots is supported, and those shares will not support
-  reverting shares to snapshots.
+Share type common capability extra-specs that are not visible to end users:
+---------------------------------------------------------------------------
 
-* `ipv4_support` - indicates whether a back end can create a share that can be
-  accessed via IPv4 protocol. If administrators do not set this capability
-  as an extra-spec in a share type, the scheduler can place new shares of that
-  type in pools without regard for whether IPv4 is supported.
+* **dedupe** indicates that a backend/pool can provide shares using some
+  deduplication technology. The default value of the dedupe capability (if a
+  driver doesn't report it) is False. Drivers can support both dedupe and
+  non-deduped shares in a single storage pool by reporting ``dedupe=[True,
+  False]``. You can make a share type use deduplication by setting this
+  extra-spec to '<is> True', or prevent it by setting this extra-spec
+  to '<is> False'.
 
-* `ipv6_support` - indicates whether a back end can create a share that can be
-  accessed via IPv6 protocol. If administrators do not set this capability
-  as an extra-spec in a share type, the scheduler can place new shares of that
-  type in pools without regard for whether IPv6 is supported.
+* **compression** indicates that a backend/pool can provide shares using some
+  compression technology. The default value of the compression capability (if a
+  driver doesn't report it) is False. Drivers can support compressed and
+  non-compressed shares in a single storage pool by reporting
+  ``compression=[True, False]``. You can make a share type use compression
+  by setting this extra-spec to '<is> True', or prevent it by setting this
+  extra-spec to '<is> False'.
+
+* **thin_provisioning** can be enabled where shares will not be
+  guaranteed space allocations and overprovisioning will be enabled. This
+  capability defaults to False. Back ends/pools that support thin
+  provisioning report True for this capability. Administrators can make a
+  share type use thin provisioned shares by setting this extra-spec
+  to '<is> True'. If a driver reports thin_provisioning=False (the default)
+  then it's assumed that the driver is doing thick provisioning and
+  overprovisioning is turned off. A driver can support thin provisioned
+  and thick provisioned shares in the same pool by reporting
+  ``thin_provisioning=[True, False]``.
 
-Reporting Capabilities
-----------------------
-Drivers report capabilities as part of the updated stats (e.g. capacity)
-for their backend/pools. This is how a backend/pool advertizes its ability
-to provide a share that matches the capabilities requested in the share
-type extra-specs.
-
-Developer impact
-----------------
-
-Developers should update their drivers to include all backend and pool
-capacities and capabilities in the share stats it reports to scheduler.
-Below is an example having multiple pools. "my" is used as an
-example vendor prefix:
+  To provision a thick
+  share on a back end that supports both thin and thick provisioning, set one
+  of the following in extra specs:
 
 ::
 
-    {
-        'driver_handles_share_servers': 'False',  #\
-        'share_backend_name': 'My Backend',       # backend level
-        'vendor_name': 'MY',                      # mandatory/fixed
-        'driver_version': '1.0',                  # stats & capabilities
-        'storage_protocol': 'NFS_CIFS',           #/
-                                                  #\
-        'my_capability_1': 'custom_val',          # "my" optional vendor
-        'my_capability_2': True,                  # stats & capabilities
-                                                  #/
-        'pools': [
-            {'pool_name':
-               'thin-dedupe-compression pool',    #\
-             'total_capacity_gb': 500,            #  mandatory stats for
-             'free_capacity_gb': 230,             #  pools
-             'reserved_percentage': 0,            #/
-                                                  #\
-             'dedupe': True,                      # common capabilities
-             'compression': True,                 #
-             'snapshot_support': True,            #
-             'create_share_from_snapshot_support': True,
-             'revert_to_snapshot_support': True,
-             'qos': True,                         # this backend supports QoS
-             'thin_provisioning': True,           #
-             'max_over_subscription_ratio': 10,   # (mandatory for thin)
-             'provisioned_capacity_gb': 270,      # (mandatory for thin)
-                                                  #
-                                                  #
-             'replication_type': 'dr',            # this backend supports
-                                                  # replication_type 'dr'
-                                                  #/
-             'my_dying_disks': 100,               #\
-             'my_super_hero_1': 'Hulk',           #  "my" optional vendor
-             'my_super_hero_2': 'Spider-Man',     #  stats & capabilities
-                                                  #/
-                                                  #\
-                                                  # can replicate to other
-             'replication_domain': 'asgard',      # backends in
-                                                  # replication_domain 'asgard'
-                                                  #/
-             'ipv4_support': True,
-             'ipv6_support': True,
-
-            },
-            {'pool_name': 'thick pool',
-             'total_capacity_gb': 1024,
-             'free_capacity_gb': 1024,
-             'qos': False,
-             'snapshot_support': True,
-             'create_share_from_snapshot_support': False, # this pool does not
-                                                          # allow creating
-                                                          # shares from
-                                                          # snapshots
-             'revert_to_snapshot_support': True,
-             'reserved_percentage': 0,
-             'dedupe': False,
-             'compression': False,
-             'thin_provisioning': False,
-             'replication_type': None,
-             'my_dying_disks': 200,
-             'my_super_hero_1': 'Batman',
-             'my_super_hero_2': 'Robin',
-             'ipv4_support': True,
-             'ipv6_support': True,
-            },
-         ]
-    }
-
-Work Flow
----------
-
-1) Share Backends report how many pools and what those pools look like and
-   are capable of to scheduler;
-
-2) When request comes in, scheduler picks a pool that fits the need best to
-   serve the request, it passes the request to the backend where the target
-   pool resides;
-
-3) Share driver gets the message and lets the target pool serve the request
-   as scheduler instructed. Share type extra-specs (scoped and un-scoped)
-   are available for the driver implementation to use as-needed.
+    {'thin_provisioning': 'False'}
+    {'thin_provisioning': '<is> False'}
+    {'capabilities:thin_provisioning': 'False'}
+    {'capabilities:thin_provisioning': '<is> False'}
+
+* **qos** indicates that a backend/pool can provide shares using some
+  QoS (Quality of Service) specification. The default value of the qos
+  capability (if a driver doesn't report it) is False. You can make a share
+  type use QoS by setting this extra-spec to '<is> True' and also setting
+  the relevant QoS-related extra specs for the drivers being used.
+  Administrators can prevent a share type from using QoS by setting this
+  extra-spec to '<is> False'. Different drivers have different ways of
+  specifying QoS limits (or guarantees) and this extra spec merely allows
+  the scheduler to filter by pools that either have or don't have QoS
+  support enabled.
+
+* **ipv4_support** indicates whether a back end can create a share that
+  can be accessed via IPv4 protocol. If administrators do not set this
+  capability as an extra-spec in a share type, the scheduler can place new
+  shares of that type in pools without regard for whether IPv4 is supported.
+
+* **ipv6_support** - indicates whether a back end can create a share that
+  can be accessed via IPv6 protocol. If administrators do not set this
+  capability as an extra-spec in a share type, the scheduler can place new
+  shares of that type in pools without regard for whether IPv6 is supported.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-share-management.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-share-management.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-share-server-management.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-share-server-management.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/share_back_ends_feature_support_mapping.rst` & `manila-9.1.5/doc/source/admin/share_back_ends_feature_support_mapping.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-manage-and-unmanage-share.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-manage-and-unmanage-share.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/zfs_on_linux_driver.rst` & `manila-9.1.5/doc/source/admin/zfs_on_linux_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-crud-share.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-crud-share.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-troubleshoot.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-troubleshoot.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-quotas.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-quotas.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/glusterfs_native_driver.rst` & `manila-9.1.5/doc/source/admin/glusterfs_native_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-share-migration.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-share-migration.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/emc_unity_driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/cephfs-native-driver.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,266 +1,294 @@
-..
-      Copyright (c) 2014 EMC Corporation
-      All Rights Reserved.
-
-      Licensed under the Apache License, Version 2.0 (the "License"); you may
-      not use this file except in compliance with the License. You may obtain
-      a copy of the License at
-
-          http://www.apache.org/licenses/LICENSE-2.0
-
-      Unless required by applicable law or agreed to in writing, software
-      distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
-      WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
-      License for the specific language governing permissions and limitations
-      under the License.
-
-
-Unity Driver
-============
-
-EMC manila driver framework (EMCShareDriver) utilizes the EMC storage products
-to provide the shared filesystems to OpenStack. The EMC manila driver is a
-plugin based driver which is designed to use different plugins to manage
-different EMC storage products.
-
-Unity plugin is the plugin which manages the Unity Storage System to provide
-shared filesystems.  EMC driver framework with Unity plugin is referred to as
-Unity driver in this document.
-
-This driver performs the operations on Unity by REST API.  Each backend manages
-one Unity Storage System. Multiple manila backends need to be configured to
-manage multiple Unity Storage Systems.
+====================
+CephFS Native driver
+====================
+
+The CephFS Native driver enables the Shared File Systems service to export
+shared file systems to guests using the Ceph network protocol. Guests require a
+Ceph client in order to mount the file system.
+
+Access is controlled via Ceph's cephx authentication system. When a user
+requests share access for an ID, Ceph creates a corresponding Ceph auth ID and
+a secret key, if they do not already exist, and authorizes the ID to access
+the share. The client can then mount the share using the ID and the secret
+key.
+
+To learn more about configuring Ceph clients to access the shares created
+using this driver, please see the Ceph documentation (
+http://docs.ceph.com/docs/master/cephfs/). If you choose to use the kernel
+client rather than the FUSE client, the share size limits set in the
+Shared File Systems service may not be obeyed.
+
+Supported shared file systems and operations
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+The driver supports CephFS shares.
+
+The following operations are supported with CephFS back end:
+
+- Create a share.
+
+- Delete a share.
+
+- Allow share access.
+
+  - ``read-only`` access level is supported.
+
+  - ``read-write`` access level is supported.
+
+
+  Note the following limitation for CephFS shares:
+
+  - Only ``cephx`` access type is supported.
+
+- Deny share access.
+
+- Create a snapshot.
+
+- Delete a snapshot.
+
+- Create a consistency group (CG).
+
+- Delete a CG.
+
+- Create a CG snapshot.
+
+- Delete a CG snapshot.
 
 Requirements
-------------
+~~~~~~~~~~~~
+
+- Mitaka or later versions of manila.
+
+- Jewel or later versions of Ceph.
+
+- A Ceph cluster with a file system configured (
+  http://docs.ceph.com/docs/master/cephfs/createfs/)
+
+- ``ceph-common`` package installed in the servers running the
+  ``manila-share`` service.
 
-- Unity OE 4.0.1 or higher.
-- StorOps 1.1.0 or higher is installed on Manila node.
-- Following licenses are activated on Unity:
+- Ceph client installed in the guest, preferably the FUSE based client,
+  ``ceph-fuse``.
 
-  * CIFS/SMB Support
-  * Network File System (NFS)
-  * Thin Provisioning
-  * Fiber Channel (FC)
-  * Internet Small Computer System Interface (iSCSI)
+- Network connectivity between your Ceph cluster's public network and the
+  servers running the ``manila-share`` service.
 
+- Network connectivity between your Ceph cluster's public network and guests.
+
+.. important:: A manila share backed onto CephFS is only as good as the
+               underlying file system. Take care when configuring your Ceph
+               cluster, and consult the latest guidance on the use of
+               CephFS in the Ceph documentation (
+               http://docs.ceph.com/docs/master/cephfs/).
+
+Authorize the driver to communicate with Ceph
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Run the following commands to create a Ceph identity for the Shared File
+Systems service to use:
+
+.. code-block:: console
 
-Supported Operations
---------------------
+    read -d '' MON_CAPS << EOF
+    allow r,
+    allow command "auth del",
+    allow command "auth caps",
+    allow command "auth get",
+    allow command "auth get-or-create"
+    EOF
+
+    ceph auth get-or-create client.manila -o manila.keyring \
+    mds 'allow *' \
+    osd 'allow rw' \
+    mon "$MON_CAPS"
+
+
+``manila.keyring``, along with your ``ceph.conf`` file, then needs to be placed
+on the server running the ``manila-share`` service.
+
+Enable snapshots in Ceph if you want to use them in the Shared File Systems
+service:
+
+.. code-block:: console
+
+    ceph mds set allow_new_snaps true --yes-i-really-mean-it
+
+In the server running the ``manila-share`` service, you can place the
+``ceph.conf`` and ``manila.keyring`` files in the ``/etc/ceph`` directory. Set
+the same owner for the ``manila-share`` process and the ``manila.keyring``
+file. Add the following section to the ``ceph.conf`` file.
+
+.. code-block:: ini
 
-In detail, users are allowed to do following operation with EMC Unity
-Storage Systems.
+    [client.manila]
+    client mount uid = 0
+    client mount gid = 0
+    log file = /opt/stack/logs/ceph-client.manila.log
+    admin socket = /opt/stack/status/stack/ceph-$name.$pid.asok
+    keyring = /etc/ceph/manila.keyring
 
-* Create/delete a NFS share.
-* Create/delete a CIFS share.
-* Extend the size of a share.
-* Shrink the size of a share.
-* Modify the host access privilege of a NFS share.
-* Modify the user access privilege of a CIFS share.
-* Take/Delete snapshot of a share.
-* Create a new share from snapshot.
-* Revert a share to a snapshot.
+It is advisable to modify the Ceph client's admin socket file and log file
+locations so that they are co-located with the Shared File Systems services'
+pid files and log files respectively.
 
 
-Supported Network Topologies
-----------------------------
+Configure CephFS back end in ``manila.conf``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-* flat
-* VLAN
+#. Add CephFS to ``enabled_share_protocols`` (enforced at the Shared File
+   Systems service's API layer). In this example we leave NFS and CIFS enabled,
+   although you can remove these if you only use CephFS:
 
+   .. code-block:: ini
 
-Pre-Configurations
-------------------
+       enabled_share_protocols = NFS,CIFS,CEPHFS
 
-On Manila Node
-~~~~~~~~~~~~~~
+#. Refer to the following table for the list of all the ``cephfs_native``
+   driver-specific configuration options.
 
-StorOps library is required to run Unity driver.
-Please install it with the pip command.
-You may need root privilege to install python libraries.
+   .. include:: ../../tables/manila-cephfs.inc
 
-::
+   Create a section to define a CephFS back end:
 
-    pip install storops
+   .. code-block:: ini
 
+       [cephfs1]
+       driver_handles_share_servers = False
+       share_backend_name = CEPHFS1
+       share_driver = manila.share.drivers.cephfs.cephfs_native.CephFSNativeDriver
+       cephfs_conf_path = /etc/ceph/ceph.conf
+       cephfs_auth_id = manila
+       cephfs_cluster_name = ceph
+       cephfs_enable_snapshots = False
 
-On Unity System
+   To let the driver perform snapshot related operations, set
+   cephfs_enable_snapshots to True . Also set the
+   ``driver-handles-share-servers`` to ``False`` as the driver does not manage
+   the lifecycle of ``share-servers``.
+
+#. Edit ``enabled_share_backends`` to point to the driver's back-end section
+   using the section name. In this example we are also including another
+   back end (``generic1``), you would include whatever other back ends you have
+   configured.
+
+   .. code-block:: ini
+
+       enabled_share_backends = generic1,cephfs1
+
+
+Creating shares
 ~~~~~~~~~~~~~~~
 
-1. Configure System level NTP Server
+The default share type may have ``driver_handles_share_servers`` set to
+``True``. Configure a share type suitable for CephFS:
 
-Configure the NTP server for your Unity at:
+.. code-block:: console
+
+     manila type-create cephfstype false
+
+     manila type-set cephfstype set share_backend_name='CEPHFS1'
+
+Then create a share:
 
 .. code-block:: console
 
-    Unisphere -> Settings -> Management -> System Time and NTP
+    manila create --share-type cephfstype --name cephshare1 cephfs 1
 
-Select "Enable NTP synchronization" and add your NTP server(s).
+Note the export location of the share:
 
-2. Configure System level DNS Server
+.. code-block:: console
 
-Configure the DNS server for your Unity at:
+    manila share-export-location-list cephshare1
+
+The export location of the share contains the Ceph monitor (mon) addresses and
+ports, and the path to be mounted. It is of the form,
+``{mon ip addr:port}[,{mon ip addr:port}]:{path to be mounted}``
+
+
+Allowing access to shares
+~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Allow Ceph auth ID ``alice`` access to the share using ``cephx`` access type.
 
 .. code-block:: console
 
-    Unisphere -> Settings -> Management -> DNS Server
+    manila access-allow cephshare1 cephx alice
+
+Note the access status and the secret access key of ``alice``.
+
+.. code-block:: console
+
+    manila access-list cephshare1
+
 
-Select "Configure DNS server address manually" and add your DNS server(s).
+Mounting shares using FUSE client
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
+Using the secret key of the authorized ID ``alice``, create a keyring file
+``alice.keyring``.
 
-Configurations
---------------
+.. code-block:: ini
+
+    [client.alice]
+            key = AQA8+ANW/4ZWNRAAOtWJMFPEihBA1unFImJczA==
 
-Following configurations need to be configured in `/etc/manila/manila.conf`
-for the Unity driver.
+Using the monitor IP addresses from the share's export location, create a
+configuration file, ``ceph.conf``:
 
 .. code-block:: ini
 
-    share_driver = manila.share.drivers.dell_emc.driver.EMCShareDriver
-    emc_share_backend = unity
-    emc_nas_server = <management IP address of the Unity system>
-    emc_nas_login = <user with administrator privilege>
-    emc_nas_password = <password>
-    unity_server_meta_pool = <pool name>
-    unity_share_data_pools = <comma separated pool names>
-    unity_ethernet_ports = <comma separated ports list>
-    driver_handles_share_servers = True/False
-    unity_share_server = <name of NAS server in Unity system>
-
-- `emc_share_backend`
-    The plugin name. Set it to `unity` for the Unity driver.
-
-- `emc_nas_server`
-    The management IP for Unity.
-
-- `unity_server_meta_pool`
-    The name of the pool to persist the meta-data of NAS server.
-    This option is required.
-
-- `unity_share_data_pools`
-    Comma separated list specifying the name of the pools to be used
-    by this backend. Do not set this option if all storage pools
-    on the system can be used.
-    Wild card character is supported.
-
-    Examples:
-
-    .. code-block:: ini
-
-       # Only use pool_1
-       unity_share_data_pools = pool_1
-       # Only use pools whose name stars from pool_
-       unity_share_data_pools = pool_*
-       # Use all pools on Unity
-       unity_share_data_pools = *
-
-- `unity_ethernet_ports`
-    Comma separated list specifying the ethernet ports of Unity system
-    that can be used for share. Do not set this option if all ethernet ports
-    can be used.
-    Wild card character is supported. Both the normal ethernet port and link
-    aggregation port can be used by Unity share driver.
-
-
-    Examples:
-
-    .. code-block:: ini
-
-       # Only use spa_eth1
-       unity_ethernet_ports = spa_eth1
-       # Use port whose name stars from spa_
-       unity_ethernet_ports = spa_*
-       # Use all Link Aggregation ports
-       unity_ethernet_ports = sp*_la_*
-       # Use all available ports
-       unity_ethernet_ports = *
-
-- `driver_handles_share_servers`
-    Unity driver requires this option to be as `True` or `False`.
-    Need to set `unity_share_server` when the value is `False`.
-
-- `unity_share_server`
-    One of NAS server names in Unity, it is used for share creation when
-    the driver is in `DHSS=False` mode.
-
-Restart of :term:`manila-share` service is needed for the configuration changes to take
-effect.
-
-IPv6 support
-------------
-
-IPv6 support for Unity driver is introduced in Queens release. The feature is divided
-into two parts:
-
-1. The driver is able to manage share or snapshot in the Neutron IPv6 network.
-2. The driver is able to connect Unity management interface using its IPv6 address.
-
-Snapshot support
-----------------
-
-In the Mitaka and Newton release of OpenStack, Snapshot support is enabled by default for a newly created share type.
-Starting with the Ocata release, the snapshot_support extra spec must be set to True in order to allow snapshots for
-a share type. If the 'snapshot_support' extra_spec is omitted or if it is set to False, users would not be able to
-create snapshots on shares of this share type. The feature is divided into two parts:
-
-1. The driver is able to create/delete snapshot of share.
-2. The driver is able to create share from snapshot.
-
-Restrictions
-------------
-
-The Unity driver has following restrictions.
-
-- EMC Unity does not support the same IP in different VLANs.
-- Only IP access type is supported for NFS.
-- Only user access type is supported for CIFS.
-
-
-API Implementations
--------------------
-
-Following driver features are implemented in the plugin.
-
-* create_share: Create a share and export it based on the protocol used
-  (NFS or CIFS).
-* create_share_from_snapshot: Create a share from a snapshot - clone a
-  snapshot.
-* delete_share: Delete a share.
-* extend_share: Extend the maximum size of a share.
-* shrink_share: Shrink the minimum size of a share.
-* create_snapshot: Create a snapshot for the specified share.
-* delete_snapshot: Delete the snapshot of the share.
-* update_access: recover, add or delete user/host access to a share.
-* allow_access: Allow access (read write/read only) of a user to a
-  CIFS share.  Allow access (read write/read only) of a host to a NFS
+    [client]
+            client quota = true
+            mon host = 192.168.1.7:6789, 192.168.1.8:6789, 192.168.1.9:6789
+
+Finally, mount the file system, substituting the file names of the keyring and
+configuration files you just created, and substituting the path to be mounted
+from the share's export location:
+
+.. code-block:: console
+
+    sudo ceph-fuse ~/mnt \
+    --id=alice \
+    --conf=./ceph.conf \
+    --keyring=./alice.keyring \
+    --client-mountpoint=/volumes/_nogroup/4c55ad20-9c55-4a5e-9233-8ac64566b98c
+
+
+Known restrictions
+~~~~~~~~~~~~~~~~~~
+
+Consider the driver as a building block for supporting multi-tenant workloads
+in the future. However, it can be used in private cloud deployments.
+
+- The guests have direct access to Ceph's public network.
+
+- The snapshot support of the driver is disabled by default.
+  ``cephfs_enable_snapshots`` configuration option needs to be set to ``True``
+  to allow snapshot operations.
+
+- Snapshots are read-only. A user can read a snapshot's contents from the
+  ``.snap/{manila-snapshot-id}_{unknown-id}`` folder within the mounted
   share.
-* deny_access: Remove access (read write/read only) of a user from
-  a CIFS share.  Remove access (read write/read only) of a host from a
-  NFS share.
-* ensure_share: Check whether share exists or not.
-* update_share_stats: Retrieve share related statistics from Unity.
-* get_network_allocations_number: Returns number of network allocations for
-  creating VIFs.
-* setup_server: Set up and configures share server with given network
-  parameters.
-* teardown_server: Tear down the share server.
-* revert_to_snapshot: Revert a share to a snapshot.
-
-
-The :mod:`manila.share.drivers.dell_emc.driver` Module
-------------------------------------------------------
-
-.. automodule:: manila.share.drivers.dell_emc.driver
-    :noindex:
-    :members:
-    :undoc-members:
-    :show-inheritance:
-
-The :mod:`manila.share.drivers.dell_emc.plugins.unity.connection` Module
-------------------------------------------------------------------------
-
-.. automodule:: manila.share.drivers.dell_emc.plugins.unity.connection
-    :noindex:
-    :members:
-    :undoc-members:
-    :show-inheritance:
+
+- To restrict share sizes, CephFS uses quotas that are enforced in the client
+  side. The CephFS clients are relied on to respect quotas.
+
+
+Security
+~~~~~~~~
+
+- Each share's data is mapped to a distinct Ceph RADOS namespace. A guest is
+  restricted to access only that particular RADOS namespace.
+
+- An additional level of resource isolation can be provided by mapping a
+  share's contents to a separate RADOS pool. This layout would be preferred
+  only for cloud deployments with a limited number of shares needing strong
+  resource separation. You can do this by setting a share type specification,
+  ``cephfs:data_isolated`` for the share type used by the cephfs driver.
+
+  .. code-block:: console
+
+       manila type-key cephfstype set cephfs:data_isolated=True
+
+- Untrusted manila guests pose security risks to the Ceph storage cluster as
+  they would have direct access to the cluster's public network.
```

### Comparing `manila-9.1.4/doc/source/admin/index.rst` & `manila-9.1.5/doc/source/admin/index.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -41,19 +41,19 @@
 deployment.
 
 .. toctree::
    :maxdepth: 1
 
    shared-file-systems-key-concepts.rst
    shared-file-systems-share-management.rst
-   shared-file-systems-share-server-management.rst
-   shared-file-systems-share-migration.rst
    shared-file-systems-share-types.rst
    shared-file-systems-snapshots.rst
+   shared-file-systems-share-server-management.rst
    shared-file-systems-security-services.rst
+   shared-file-systems-share-migration.rst
    shared-file-systems-share-replication.rst
    shared-file-systems-multi-backend.rst
    shared-file-systems-networking.rst
    shared-file-systems-troubleshoot.rst
    share_back_ends_feature_support_mapping
    capabilities_and_extra_specs
    group_capabilities_and_extra_specs
```

### Comparing `manila-9.1.4/doc/source/admin/emc_vnx_driver.rst` & `manila-9.1.5/doc/source/admin/emc_vnx_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-manage-and-unmanage-snapshot.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-manage-and-unmanage-snapshot.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-security-services.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-security-services.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/container_driver.rst` & `manila-9.1.5/doc/source/admin/container_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-multi-backend.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-multi-backend.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/nexentastor5_driver.rst` & `manila-9.1.5/doc/source/admin/nexentastor5_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/cephfs_driver.rst` & `manila-9.1.5/doc/source/admin/cephfs_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-share-resize.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-share-resize.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/huawei_nas_driver.rst` & `manila-9.1.5/doc/source/admin/huawei_nas_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-key-concepts.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-key-concepts.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-share-replication.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-share-replication.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-network-plugins.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-network-plugins.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/hitachi_hnas_driver.rst` & `manila-9.1.5/doc/source/admin/hitachi_hnas_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/hpe_3par_driver.rst` & `manila-9.1.5/doc/source/admin/hpe_3par_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/export_location_metadata.rst` & `manila-9.1.5/doc/source/admin/export_location_metadata.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-snapshots.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-snapshots.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/generic_driver.rst` & `manila-9.1.5/doc/source/admin/generic_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-networking.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-networking.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/emc_isilon_driver.rst` & `manila-9.1.5/doc/source/admin/emc_isilon_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/hdfs_native_driver.rst` & `manila-9.1.5/doc/source/admin/hdfs_native_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/gpfs_driver.rst` & `manila-9.1.5/doc/source/admin/gpfs_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/tegile_driver.rst` & `manila-9.1.5/doc/source/admin/tegile_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/netapp_cluster_mode_driver.rst` & `manila-9.1.5/doc/source/admin/netapp_cluster_mode_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-share-networks.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-share-networks.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-services-manage.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-services-manage.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/glusterfs_driver.rst` & `manila-9.1.5/doc/source/admin/glusterfs_driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/admin/shared-file-systems-scheduling.rst` & `manila-9.1.5/doc/source/admin/shared-file-systems-scheduling.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/reference/index.rst` & `manila-9.1.5/doc/source/reference/index.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/reference/glossary.rst` & `manila-9.1.5/doc/source/reference/glossary.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/figures/hsp_network.png` & `manila-9.1.5/doc/source/configuration/figures/hsp_network.png`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/figures/openstack-spectrumscale-setup.JPG` & `manila-9.1.5/doc/source/configuration/figures/openstack-spectrumscale-setup.JPG`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/figures/hds_network.jpg` & `manila-9.1.5/doc/source/images/rpc/hds_network.jpg`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-infinidat.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-infinidat.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-powermax.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-powermax.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-quota.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-quota.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-nexentastor5.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-nexentastor5.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-netapp.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-netapp.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-glusterfs.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-glusterfs.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-san.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-san.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-zfssa.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-zfssa.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-hnas.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-hnas.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-vnx.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-vnx.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-compute.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-compute.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-spectrumscale_ces.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-spectrumscale_ces.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-hds_hsp.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-hds_hsp.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-spectrumscale_knfs.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-spectrumscale_knfs.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-hdfs.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-hdfs.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-tegile.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-tegile.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-emc.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-emc.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-generic.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-generic.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-hpe3par.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-hpe3par.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-lvm.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-lvm.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-zfs.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-zfs.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-hds_hnas.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-hds_hnas.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-winrm.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-winrm.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-redis.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-redis.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-cephfs.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-cephfs.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-common.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-common.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-quobyte.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-quobyte.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-share.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-share.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-maprfs.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-maprfs.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-scheduler.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-scheduler.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-huawei.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-huawei.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-api.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-api.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-unity.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-unity.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-ganesha.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-ganesha.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/tables/manila-ca.inc` & `manila-9.1.5/doc/source/configuration/tables/manila-ca.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/overview.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/overview.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/hpe-3par-share-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/hpe-3par-share-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/hitachi-hsp-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/hitachi-hsp-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/dell-emc-unity-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/dell-emc-unity-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/windows-smb-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/windows-smb-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/maprfs-native-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/maprfs-native-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/netapp-cluster-mode-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/netapp-cluster-mode-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/glusterfs-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/glusterfs-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/hitachi-hnas-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/hitachi-hnas-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/huawei-nas-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/huawei-nas-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/dell-emc-powermax-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/dell-emc-powermax-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/lvm-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/lvm-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/quobyte-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/quobyte-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/zfssa-manila-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/zfssa-manila-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/glusterfs-native-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/glusterfs-native-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/hdfs-native-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/hdfs-native-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/infinidat-share-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/infinidat-share-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/nexentastor5-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/nexentastor5-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/generic-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/generic-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/emc-isilon-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/emc-isilon-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/dell-emc-vnx-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/dell-emc-vnx-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/ibm-spectrumscale-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/ibm-spectrumscale-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers/zfs-on-linux-driver.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers/zfs-on-linux-driver.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/samples/manila.conf.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/samples/manila.conf.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/samples/sample_policy.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/samples/sample_policy.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/config-options.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/config-options.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/log-files.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/log-files.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/configuration/shared-file-systems/drivers.rst` & `manila-9.1.5/doc/source/configuration/shared-file-systems/drivers.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/source/conf.py` & `manila-9.1.5/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/doc/requirements.txt` & `manila-9.1.5/doc/requirements.txt`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/ChangeLog` & `manila-9.1.5/ChangeLog`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 CHANGES
 =======
 
+9.1.5
+-----
+
+* Update doc for manila-service-image download
+* [stable/train] Update requirements and constraints
+* Fix logic that determines a share exists before manage
+* [NetApp] Support NFS shares on windows
+* fix reno file location and indention
+* [NetApp] Fix CIFS promote back issue
+* [NetApp] Fix HTTPS connection for python 3.7
+* [Glusterfs] Fix delete share, Couldn't find the 'gluster\_used\_vols'
+* [Glusterfs] Fix delete share, mount point not disconnected
+* Fix documentation for types and extra specs
+* Update access rules documentation for user guide
+* Add mod\_wsgi configuration samples
+* Add uWSGI configuration samples
+* Fix wrong capacity in pool\_stat for DellEMC manila drivers
+
 9.1.4
 -----
 
+* Fix fallback share group snapshot implementation
+* Add verify-noapi testcase to grenade
 * Harden LVM driver deletion paths
 * Update LVM volume extend
 * [ci] Remove explicit compression of log files
 * [NetApp] Fix default ipspace deletion issue
 * [NetApp] Fix falsely report migration cancelation success
 * Monkey patch original current\_thread \_active
 * [NetApp] update set\_preferred\_dc for ontapi 1.150
```

### Comparing `manila-9.1.4/HACKING.rst` & `manila-9.1.5/HACKING.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/tools/install_venv.py` & `manila-9.1.5/tools/install_venv.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/tools/cover.sh` & `manila-9.1.5/tools/cover.sh`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/tools/install_venv_common.py` & `manila-9.1.5/tools/install_venv_common.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/tools/check_exec.py` & `manila-9.1.5/tools/check_exec.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/tools/coding-checks.sh` & `manila-9.1.5/tools/coding-checks.sh`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/tools/test-setup.sh` & `manila-9.1.5/tools/test-setup.sh`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/tools/validate-json-files.py` & `manila-9.1.5/tools/validate-json-files.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/tools/enable-pre-commit-hook.sh` & `manila-9.1.5/tools/enable-pre-commit-hook.sh`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila.egg-info/entry_points.txt` & `manila-9.1.5/manila.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila.egg-info/PKG-INFO` & `manila-9.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: manila
-Version: 9.1.4
+Version: 9.1.5
 Summary: Shared Storage for OpenStack
 Home-page: https://docs.openstack.org/manila/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `manila-9.1.4/manila.egg-info/requires.txt` & `manila-9.1.5/manila.egg-info/requires.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 Babel!=2.4.0,>=2.3.4
 Paste>=2.0.2
 PasteDeploy>=1.5.0
 Routes>=2.3.1
 SQLAlchemy!=1.1.5,!=1.1.6,!=1.1.7,!=1.1.8,>=1.0.10
 WebOb>=1.7.1
 alembic>=0.8.10
-eventlet!=0.18.3,!=0.20.1,>=0.18.2
+eventlet>=0.24.1
 greenlet>=0.4.10
 keystoneauth1>=3.4.0
 keystonemiddleware>=4.17.0
 lxml!=3.7.0,>=3.4.1
 netaddr>=0.7.18
 oslo.concurrency>=3.26.0
 oslo.config>=5.2.0
 oslo.context>=2.19.2
 oslo.db>=4.27.0
 oslo.i18n>=3.15.3
 oslo.log>=3.36.0
-oslo.messaging>=5.29.0
+oslo.messaging>=6.4.1
 oslo.middleware>=3.31.0
 oslo.policy>=1.30.0
 oslo.reports>=1.18.0
 oslo.rootwrap>=5.8.0
 oslo.serialization!=2.19.1,>=2.18.0
-oslo.service!=1.28.1,>=1.24.0
+oslo.service>=1.31.0
 oslo.upgradecheck>=0.1.0
 oslo.utils>=3.33.0
 paramiko>=2.0.0
 pbr!=2.1.0,>=2.0.0
 pyparsing>=2.1.0
 python-cinderclient!=4.0.0,>=3.3.0
 python-neutronclient>=6.7.0
```

### Comparing `manila-9.1.4/manila.egg-info/SOURCES.txt` & `manila-9.1.5/manila.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -344,14 +344,15 @@
 doc/source/configuration/tables/manila-unity.inc
 doc/source/configuration/tables/manila-vnx.inc
 doc/source/configuration/tables/manila-winrm.inc
 doc/source/configuration/tables/manila-zfs.inc
 doc/source/configuration/tables/manila-zfssa.inc
 doc/source/contributor/adding_release_notes.rst
 doc/source/contributor/addmethod.openstackapi.rst
+doc/source/contributor/apache-httpd.rst
 doc/source/contributor/api_microversion_dev.rst
 doc/source/contributor/api_microversion_history.rst
 doc/source/contributor/architecture.rst
 doc/source/contributor/auth.rst
 doc/source/contributor/commit_message_tags.rst
 doc/source/contributor/database.rst
 doc/source/contributor/development-environment-devstack.rst
@@ -438,14 +439,17 @@
 etc/manila/README.manila.conf
 etc/manila/api-paste.ini
 etc/manila/logging_sample.conf
 etc/manila/manila-policy-generator.conf
 etc/manila/rootwrap.conf
 etc/manila/rootwrap.d/share.filters
 etc/oslo-config-generator/manila.conf
+httpd/manila-uwsgi.ini
+httpd/mod_wsgi-manila.conf
+httpd/uwsgi-manila.conf
 manila/__init__.py
 manila/context.py
 manila/coordination.py
 manila/exception.py
 manila/i18n.py
 manila/manager.py
 manila/opts.py
@@ -1426,33 +1430,40 @@
 releasenotes/notes/bug-1816420-validate-access-type-for-ganehas-c42ce6f859fa0c8c.yaml
 releasenotes/notes/bug-1818081-fix-inferred-script-name-in-case-of-proxy-urls-e33466af856708b4.yaml
 releasenotes/notes/bug-1822099-fix-multisegment-mtu.yaml-ac2e31c084d8bbb6.yaml
 releasenotes/notes/bug-1831092-netapp-fix-race-condition-524555133aaa6ca8.yaml
 releasenotes/notes/bug-1845135-fix-Unity-cannot-use-mgmt-ipv6-9407710a3fc7f4aa.yaml
 releasenotes/notes/bug-1845452-unity--fix-fail-to-delete-cifs-share-c502a10ae306e506.yaml
 releasenotes/notes/bug-1846836-fix-share-network-update-unexpected-success-eba8f40db392c467.yaml
+releasenotes/notes/bug-1848608-1893718-fix-manage-api-for-shares-with-multiple-export-locations-32ade25e9d82535b.yaml
 releasenotes/notes/bug-1848889-netapp-fix-share-replica-update-check-failure-90aa964417e7734c.yaml
 releasenotes/notes/bug-1850264-add-async-error-when-share-extend-error-a0c458204b395994.yaml
 releasenotes/notes/bug-1858328-netapp-fix-shrinking-error-48bcfffe694f5e81.yaml
 releasenotes/notes/bug-1859775-snapshot-over-quota-exception-bb6691612af03ddf.yaml
 releasenotes/notes/bug-1859785-share-list-speed-6b09e7717624e037.yaml
 releasenotes/notes/bug-1861485-fix-share-network-retrieval-31768dcda5aeeaaa.yaml
 releasenotes/notes/bug-1869148-if-only-pyc-exist-the-extension-API-cannot-be-loaded-172cb9153ebd4b56.yaml
 releasenotes/notes/bug-1869712-fix-increased-scheduled-time-for-non-thin-provisioned-backends-1da2cc33d365ba4f.yaml
 releasenotes/notes/bug-1870751-cleanup-share-type-and-group-type-project-access-when-deleted-4fcd49ba6e6c40bd.yaml
 releasenotes/notes/bug-1872243-netapp-fix-vserver-peer-with-same-vserver-8bc65816f1764784.yaml
 releasenotes/notes/bug-1872872-fix-quota-checking-b06fd372be143101.yaml
 releasenotes/notes/bug-1872873-fix-consume-from-share-eea5941de17a5bcc.yaml
 releasenotes/notes/bug-1873963-netapp-fix-vserver-peer-intra-cluster-966398cf3a621edd.yaml
+releasenotes/notes/bug-1878993-netapp-fix-https-3eddf9eb5b762f3a.yaml
+releasenotes/notes/bug-1879368-netapp-fix-cifs-promote-back-issue-d8fe28466f9dde49.yaml
 releasenotes/notes/bug-1879754-teardown-network-d1887cdf6eb83388.yaml
 releasenotes/notes/bug-1880747-netapp-fix-do-not-delete-default-ipspace-aee638279e0f8e93.yaml
 releasenotes/notes/bug-1882590-fix-svm-scoped-netapp-85b53830135f7558.yaml
 releasenotes/notes/bug-1885956-enforce-policy-check-getting-share-type-by-name-5eca17b02bea5261.yaml
+releasenotes/notes/bug-1886010-Glusterfs-fix-del-share-89dabc8751ed4fec.yaml
 releasenotes/notes/bug-1887643-netapp-add-cifs-dc-add-skip-check-c8ea9b952cedb643.yaml
+releasenotes/notes/bug-1888905-fix-group-snapshot-create-delete-0595f9d7a4c0c343.yaml
 releasenotes/notes/bug-1888915-harden-lvm-deletions-2a735ab0ee4a4903.yaml
+releasenotes/notes/bug-1894362-fix-Glusterfs-del-share-3c8467e1d9f0c6e4.yaml
+releasenotes/notes/bug-1901937-netapp-nfs-for-windows-465e704524277ea2.yaml
 releasenotes/notes/bug-667744-fix-c64071e6e5a098f7.yaml
 releasenotes/notes/bug_1564623_change-e286060a27b02f64.yaml
 releasenotes/notes/bug_1582931-1437eae20fa544d1.yaml
 releasenotes/notes/bugfix-1771958-1771970-bcec841e7ae6b9f6.yaml
 releasenotes/notes/cephfs-add-nfs-protocol-support-44764094c9d784d8.yaml
 releasenotes/notes/cephfs-native-add-readonly-shares-support-067ccab0217ab5f5.yaml
 releasenotes/notes/cephfs-native-enhance-update-access-support-e1a1258084c997ca.yaml
@@ -1465,14 +1476,15 @@
 releasenotes/notes/config-for-cephfs-volume-prefix-67f2513f603cb614.yaml
 releasenotes/notes/container-driver-5d972cc40e314663.yaml
 releasenotes/notes/container-driver-hardening-against-races-30c9f517a6392b9d.yaml
 releasenotes/notes/container-manage-unmanage-share-servers-880d889828ee7ce3.yaml
 releasenotes/notes/dedupe-support-hnas-driver-017d2f2a93a8b487.yaml
 releasenotes/notes/delete_vlan_on_vserver_delete-a7acd145c0b8236d.yaml
 releasenotes/notes/dell-emc-unity-use-user-capacity-322f8bbb7c536453.yaml
+releasenotes/notes/dellemc-fix-capacity-report-25f75a6c96e12b40.yaml
 releasenotes/notes/deprecate-memcached-servers-config-option-f4456382b9b4d6db.yaml
 releasenotes/notes/deprecate-old-ks-opts-in-nova-neutron-cinder-groups-e395015088d93fdc.yaml
 releasenotes/notes/deprecate-service-instance-network-helper-option-82ff62a038f2bfa3.yaml
 releasenotes/notes/disable-share-groups-api-by-default-0627b97ac2cda4cb.yaml
 releasenotes/notes/driver-filter-91e2c60c9d1a48dd.yaml
 releasenotes/notes/drop-support-for-lvm-share-export-ip-e031ef4c5f95b534.yaml
 releasenotes/notes/emc-unity-manila-support-d4f5a410501cfdae.yaml
```

### Comparing `manila-9.1.4/setup.cfg` & `manila-9.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/.zuul.yaml` & `manila-9.1.5/.zuul.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/lower-constraints.txt` & `manila-9.1.5/lower-constraints.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 alabaster==0.7.10
 alembic==0.8.10
 amqp==2.2.2
 appdirs==1.4.3
 asn1crypto==0.24.0
 Babel==2.3.4
-bashate==0.5.1
+bashate==0.6.0
 bcrypt==3.1.4
 cachetools==2.0.1
 certifi==2018.1.18
 cffi==1.11.5
 chardet==3.0.4
 cliff==2.11.0
 cmd2==0.8.1
@@ -19,15 +19,15 @@
 debtcollector==1.19.0
 decorator==4.2.1
 deprecation==2.0
 docutils==0.14
 dogpile.cache==0.6.5
 dulwich==0.19.0
 enum-compat==0.0.2
-eventlet==0.18.2
+eventlet==0.24.1
 extras==1.0.0
 fasteners==0.14.1
 fixtures==3.0.0
 flake8==2.5.5
 future==0.16.0
 futurist==1.6.0
 greenlet==0.4.10
@@ -42,15 +42,15 @@
 jsonpointer==2.0
 keystoneauth1==3.4.0
 keystonemiddleware==4.17.0
 kombu==4.1.0
 linecache2==1.0.0
 lxml==3.4.1
 Mako==1.0.7
-MarkupSafe==1.0
+MarkupSafe==1.1.1
 mccabe==0.2.1
 mock==2.0.0
 monotonic==1.4
 mox3==0.25.0
 msgpack==0.5.6
 munch==2.2.0
 netaddr==0.7.18
@@ -65,35 +65,35 @@
 oslo.cache==1.29.0
 oslo.concurrency==3.26.0
 oslo.config==5.2.0
 oslo.context==2.19.2
 oslo.db==4.27.0
 oslo.i18n==3.15.3
 oslo.log==3.36.0
-oslo.messaging==5.29.0
+oslo.messaging==6.4.1
 oslo.middleware==3.31.0
 oslo.policy==1.30.0
 oslo.reports==1.18.0
 oslo.rootwrap==5.8.0
 oslo.serialization==2.18.0
-oslo.service==1.24.0
+oslo.service==1.31.0
 oslo.upgradecheck==0.1.0
 oslo.utils==3.33.0
 oslotest==3.2.0
 packaging==17.1
 paramiko==2.0.0
 Paste==2.0.2
 PasteDeploy==1.5.0
 pbr==2.0.0
 pep8==1.5.7
 pika==0.10.0
 pika-pool==0.1.3
 prettytable==0.7.2
-psutil==5.4.3
-psycopg2-binary==2.6.2
+psutil==5.6.3
+psycopg2-binary==2.8.3
 pyasn1==0.4.2
 pycadf==2.7.0
 pycparser==2.18
 pyflakes==0.8.1
 Pygments==2.2.0
 pyinotify==0.9.6
 PyMySQL==0.7.6
```

### Comparing `manila-9.1.4/PKG-INFO` & `manila-9.1.5/manila.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: manila
-Version: 9.1.4
+Version: 9.1.5
 Summary: Shared Storage for OpenStack
 Home-page: https://docs.openstack.org/manila/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
```

### Comparing `manila-9.1.4/contrib/ci/pre_test_hook.sh` & `manila-9.1.5/contrib/ci/pre_test_hook.sh`

 * *Files 1% similar despite different names*

```diff
@@ -151,15 +151,14 @@
 
 elif [[ "$DRIVER" == "lvm" ]]; then
     MANILA_SERVICE_IMAGE_ENABLED=True
     DEFAULT_EXTRA_SPECS="'snapshot_support=True create_share_from_snapshot_support=True revert_to_snapshot_support=True mount_snapshot_support=True'"
 
     echo "SHARE_DRIVER=manila.share.drivers.lvm.LVMShareDriver" >> $localconf
     echo "SHARE_BACKING_FILE_SIZE=32000M" >> $localconf
-    export MANILA_SETUP_IPV6=True
 elif [[ "$DRIVER" == "zfsonlinux" ]]; then
     MANILA_SERVICE_IMAGE_ENABLED=True
     echo "SHARE_DRIVER=manila.share.drivers.zfsonlinux.driver.ZFSonLinuxShareDriver" >> $localconf
     echo "RUN_MANILA_REPLICATION_TESTS=True" >> $localconf
     # Set the replica_state_update_interval to 60 seconds to make
     # replication tests run faster. The default is 300, which is greater than
     # the build timeout for ZFS on the gate.
```

### Comparing `manila-9.1.4/contrib/ci/post_test_hook.sh` & `manila-9.1.5/contrib/ci/post_test_hook.sh`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/contrib/ci/common.sh` & `manila-9.1.5/contrib/ci/common.sh`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/contrib/share_driver_hooks/README.rst` & `manila-9.1.5/contrib/share_driver_hooks/README.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/contrib/share_driver_hooks/zaqarclientwrapper.py` & `manila-9.1.5/contrib/share_driver_hooks/zaqarclientwrapper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/contrib/share_driver_hooks/zaqar_notification_example_consumer.py` & `manila-9.1.5/contrib/share_driver_hooks/zaqar_notification_example_consumer.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/contrib/share_driver_hooks/zaqar_notification.py` & `manila-9.1.5/contrib/share_driver_hooks/zaqar_notification.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/manager.py` & `manila-9.1.5/manila/manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/testing/README.rst` & `manila-9.1.5/manila/testing/README.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/service.py` & `manila-9.1.5/manila/service.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/opts.py` & `manila-9.1.5/manila/opts.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/cmd/api.py` & `manila-9.1.5/manila/cmd/api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/cmd/status.py` & `manila-9.1.5/manila/cmd/status.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/cmd/share.py` & `manila-9.1.5/manila/cmd/share.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/cmd/scheduler.py` & `manila-9.1.5/manila/cmd/scheduler.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/cmd/manage.py` & `manila-9.1.5/manila/cmd/manage.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/cmd/data.py` & `manila-9.1.5/manila/cmd/data.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/coordination.py` & `manila-9.1.5/manila/coordination.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/db_utils.py` & `manila-9.1.5/manila/tests/db_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/integrated/integrated_helpers.py` & `manila-9.1.5/manila/tests/integrated/integrated_helpers.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/integrated/test_extensions.py` & `manila-9.1.5/manila/tests/integrated/test_extensions.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/integrated/api/client.py` & `manila-9.1.5/manila/tests/integrated/api/client.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/integrated/test_login.py` & `manila-9.1.5/manila/tests/integrated/test_login.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/monkey_patch_example/__init__.py` & `manila-9.1.5/manila/tests/monkey_patch_example/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/monkey_patch_example/example_b.py` & `manila-9.1.5/manila/tests/monkey_patch_example/example_b.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/monkey_patch_example/example_a.py` & `manila-9.1.5/manila/tests/monkey_patch_example/example_a.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_context.py` & `manila-9.1.5/manila/tests/test_context.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_api.py` & `manila-9.1.5/manila/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_policy.py` & `manila-9.1.5/manila/tests/test_policy.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/fake_volume.py` & `manila-9.1.5/manila/tests/fake_volume.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/fake_network.py` & `manila-9.1.5/manila/tests/fake_network.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_utils.py` & `manila-9.1.5/manila/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/declare_conf.py` & `manila-9.1.5/manila/tests/declare_conf.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_quota.py` & `manila-9.1.5/manila/tests/test_quota.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/var/certificate.crt` & `manila-9.1.5/manila/tests/var/certificate.crt`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/var/privatekey.key` & `manila-9.1.5/manila/tests/var/privatekey.key`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/var/ca.crt` & `manila-9.1.5/manila/tests/var/ca.crt`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/cmd/test_data.py` & `manila-9.1.5/manila/tests/cmd/test_data.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/cmd/test_api.py` & `manila-9.1.5/manila/tests/cmd/test_api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/cmd/test_status.py` & `manila-9.1.5/manila/tests/cmd/test_status.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/cmd/test_manage.py` & `manila-9.1.5/manila/tests/cmd/test_manage.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/cmd/test_share.py` & `manila-9.1.5/manila/tests/cmd/test_share.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/cmd/test_scheduler.py` & `manila-9.1.5/manila/tests/cmd/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_network.py` & `manila-9.1.5/manila/tests/test_network.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/fake_driver.py` & `manila-9.1.5/manila/tests/fake_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_exception.py` & `manila-9.1.5/manila/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/message/test_api.py` & `manila-9.1.5/manila/tests/message/test_api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/message/test_message_field.py` & `manila-9.1.5/manila/tests/message/test_message_field.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/common.py` & `manila-9.1.5/manila/tests/api/common.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/test_versions.py` & `manila-9.1.5/manila/tests/api/test_versions.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/test_common.py` & `manila-9.1.5/manila/tests/api/test_common.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/middleware/test_faults.py` & `manila-9.1.5/manila/tests/api/middleware/test_faults.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/middleware/test_auth.py` & `manila-9.1.5/manila/tests/api/middleware/test_auth.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_snapshot_instances.py` & `manila-9.1.5/manila/tests/api/v2/test_share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_instance_export_locations.py` & `manila-9.1.5/manila/tests/api/v2/test_share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_networks.py` & `manila-9.1.5/manila/tests/api/v2/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_services.py` & `manila-9.1.5/manila/tests/api/v2/test_services.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_shares.py` & `manila-9.1.5/manila/tests/api/v2/test_shares.py`

 * *Files 0% similar despite different names*

```diff
@@ -2888,15 +2888,15 @@
         self.mock_object(
             share_api.API, 'manage', return_share)
         self.mock_object(
             common, 'validate_public_share_policy',
             mock.Mock(side_effect=lambda *args, **kwargs: args[1]))
         share = {
             'host': data['share']['service_host'],
-            'export_location': data['share']['export_path'],
+            'export_location_path': data['share']['export_path'],
             'share_proto': data['share']['protocol'].upper(),
             'share_type_id': 'fake',
             'display_name': 'foo',
             'display_description': 'bar',
         }
         driver_options = data['share'].get('driver_options', {})
```

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_access_metadata.py` & `manila-9.1.5/manila/tests/api/v2/test_share_access_metadata.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_replicas.py` & `manila-9.1.5/manila/tests/api/v2/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_export_locations.py` & `manila-9.1.5/manila/tests/api/v2/test_share_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_instances.py` & `manila-9.1.5/manila/tests/api/v2/test_share_instances.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_security_services.py` & `manila-9.1.5/manila/tests/api/v2/test_security_services.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_replica_export_locations.py` & `manila-9.1.5/manila/tests/api/v2/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_snapshots.py` & `manila-9.1.5/manila/tests/api/v2/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_group_snapshots.py` & `manila-9.1.5/manila/tests/api/v2/test_share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_group_type_specs.py` & `manila-9.1.5/manila/tests/api/v2/test_share_group_type_specs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_groups.py` & `manila-9.1.5/manila/tests/api/v2/test_share_groups.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_quota_class_sets.py` & `manila-9.1.5/manila/tests/api/v2/test_quota_class_sets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/stubs.py` & `manila-9.1.5/manila/tests/api/v2/stubs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_availability_zones.py` & `manila-9.1.5/manila/tests/api/v2/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_group_types.py` & `manila-9.1.5/manila/tests/api/v2/test_share_group_types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_messages.py` & `manila-9.1.5/manila/tests/api/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_network_subnets.py` & `manila-9.1.5/manila/tests/api/v2/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_snapshot_export_locations.py` & `manila-9.1.5/manila/tests/api/v2/test_share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_servers.py` & `manila-9.1.5/manila/tests/api/v2/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_snapshot_instance_export_locations.py` & `manila-9.1.5/manila/tests/api/v2/test_share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_accesses.py` & `manila-9.1.5/manila/tests/api/v2/test_share_accesses.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_quota_sets.py` & `manila-9.1.5/manila/tests/api/v2/test_quota_sets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v2/test_share_types.py` & `manila-9.1.5/manila/tests/api/v2/test_share_types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/test_extensions.py` & `manila-9.1.5/manila/tests/api/test_extensions.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/test_wsgi.py` & `manila-9.1.5/manila/tests/api/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/extensions/foxinsocks.py` & `manila-9.1.5/manila/tests/api/extensions/foxinsocks.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v1/test_share_manage.py` & `manila-9.1.5/manila/tests/api/v1/test_share_manage.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,15 +55,17 @@
             policy, 'check_policy', mock.Mock(return_value=True))
         self.mock_object(
             common, 'validate_public_share_policy',
             mock.Mock(side_effect=lambda *args, **kwargs: args[1]))
 
     @ddt.data({},
               {'shares': {}},
-              {'share': get_fake_manage_body('', None, None)})
+              {'share': get_fake_manage_body('', None, None)},
+              {'share': get_fake_manage_body(
+                  export_path={'not_path': '/fake'})})
     def test_share_manage_invalid_body(self, body):
         self.assertRaises(webob.exc.HTTPUnprocessableEntity,
                           self.controller.create,
                           self.request,
                           body)
         self.mock_policy_check.assert_called_once_with(
             self.context, self.resource_name, 'manage')
@@ -188,30 +190,36 @@
     @ddt.data(
         get_fake_manage_body(name='foo', description='bar'),
         get_fake_manage_body(display_name='foo', description='bar'),
         get_fake_manage_body(name='foo', display_description='bar'),
         get_fake_manage_body(display_name='foo', display_description='bar'),
         get_fake_manage_body(display_name='foo', display_description='bar',
                              driver_options=dict(volume_id='quuz')),
+        get_fake_manage_body(display_name='foo', display_description='bar',
+                             export_path={'path': '/fake'}),
     )
     def test_share_manage(self, data):
         self._setup_manage_mocks()
         return_share = {'share_type_id': '', 'id': 'fake'}
         self.mock_object(
             share_api.API, 'manage', mock.Mock(return_value=return_share))
         share = {
             'host': data['share']['service_host'],
-            'export_location': data['share']['export_path'],
+            'export_location_path': data['share']['export_path'],
             'share_proto': data['share']['protocol'].upper(),
             'share_type_id': 'fake',
             'display_name': 'foo',
             'display_description': 'bar',
         }
         data['share']['is_public'] = 'foo'
         driver_options = data['share'].get('driver_options', {})
+        if isinstance(share['export_location_path'], dict):
+            share['export_location_path'] = (
+                share['export_location_path']['path']
+            )
 
         actual_result = self.controller.create(self.request, data)
 
         share_api.API.manage.assert_called_once_with(
             mock.ANY, share, driver_options)
         self.assertIsNotNone(actual_result)
         self.mock_policy_check.assert_called_once_with(
@@ -221,15 +229,15 @@
         self._setup_manage_mocks()
         data = get_fake_manage_body(name='foo', description='bar')
         return_share = {'share_type_id': '', 'id': 'fake'}
         self.mock_object(
             share_api.API, 'manage', mock.Mock(return_value=return_share))
         share = {
             'host': data['share']['service_host'],
-            'export_location': data['share']['export_path'],
+            'export_location_path': data['share']['export_path'],
             'share_proto': data['share']['protocol'].upper(),
             'share_type_id': 'fake',
             'display_name': 'foo',
             'display_description': 'bar',
             'share_server_id': 'fake'
         }
         data['share']['share_server_id'] = 'fake'
```

### Comparing `manila-9.1.4/manila/tests/api/v1/test_scheduler_stats.py` & `manila-9.1.5/manila/tests/api/v1/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v1/test_shares.py` & `manila-9.1.5/manila/tests/api/v1/test_shares.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v1/test_share_metadata.py` & `manila-9.1.5/manila/tests/api/v1/test_share_metadata.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v1/test_share_snapshots.py` & `manila-9.1.5/manila/tests/api/v1/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v1/test_limits.py` & `manila-9.1.5/manila/tests/api/v1/test_limits.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v1/test_share_unmanage.py` & `manila-9.1.5/manila/tests/api/v1/test_share_unmanage.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v1/stubs.py` & `manila-9.1.5/manila/tests/api/v1/stubs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v1/test_security_service.py` & `manila-9.1.5/manila/tests/api/v1/test_security_service.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v1/test_share_servers.py` & `manila-9.1.5/manila/tests/api/v1/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/v1/test_share_types_extra_specs.py` & `manila-9.1.5/manila/tests/api/v1/test_share_types_extra_specs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/openstack/test_wsgi.py` & `manila-9.1.5/manila/tests/api/openstack/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/openstack/test_versioned_method.py` & `manila-9.1.5/manila/tests/api/openstack/test_versioned_method.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/openstack/test_api_version_request.py` & `manila-9.1.5/manila/tests/api/openstack/test_api_version_request.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/views/test_versions.py` & `manila-9.1.5/manila/tests/api/views/test_versions.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/views/test_share_networks.py` & `manila-9.1.5/manila/tests/api/views/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/views/test_scheduler_stats.py` & `manila-9.1.5/manila/tests/api/views/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/views/test_shares.py` & `manila-9.1.5/manila/tests/api/views/test_shares.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/views/test_quota_class_sets.py` & `manila-9.1.5/manila/tests/api/views/test_quota_class_sets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/views/test_share_network_subnets.py` & `manila-9.1.5/manila/tests/api/views/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/views/test_share_accesses.py` & `manila-9.1.5/manila/tests/api/views/test_share_accesses.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/views/test_quota_sets.py` & `manila-9.1.5/manila/tests/api/views/test_quota_sets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/contrib/stubs.py` & `manila-9.1.5/manila/tests/api/contrib/stubs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/fakes.py` & `manila-9.1.5/manila/tests/api/fakes.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/api/test_middleware.py` & `manila-9.1.5/manila/tests/api/test_middleware.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_conf.py` & `manila-9.1.5/manila/tests/test_conf.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/compute/test_nova.py` & `manila-9.1.5/manila/tests/compute/test_nova.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/policy.json` & `manila-9.1.5/manila/tests/policy.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_coordination.py` & `manila-9.1.5/manila/tests/test_coordination.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/network/test_standalone_network_plugin.py` & `manila-9.1.5/manila/tests/network/test_standalone_network_plugin.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/network/linux/test_ip_lib.py` & `manila-9.1.5/manila/tests/network/linux/test_ip_lib.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/network/linux/test_interface.py` & `manila-9.1.5/manila/tests/network/linux/test_interface.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/network/linux/test_ovs_lib.py` & `manila-9.1.5/manila/tests/network/linux/test_ovs_lib.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/network/neutron/test_neutron_api.py` & `manila-9.1.5/manila/tests/network/neutron/test_neutron_api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/network/neutron/test_neutron_plugin.py` & `manila-9.1.5/manila/tests/network/neutron/test_neutron_plugin.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/fake_utils.py` & `manila-9.1.5/manila/tests/fake_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_service.py` & `manila-9.1.5/manila/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/fake_share.py` & `manila-9.1.5/manila/tests/fake_share.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/common/test_config.py` & `manila-9.1.5/manila/tests/common/test_config.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/common/test_client_auth.py` & `manila-9.1.5/manila/tests/common/test_client_auth.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/__init__.py` & `manila-9.1.5/manila/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share_group/test_api.py` & `manila-9.1.5/manila/tests/share_group/test_api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share_group/test_share_group_types.py` & `manila-9.1.5/manila/tests/share_group/test_share_group_types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/fake_client_exception_class.py` & `manila-9.1.5/manila/tests/fake_client_exception_class.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_test_utils.py` & `manila-9.1.5/manila/tests/test_test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/weighers/test_goodness.py` & `manila-9.1.5/manila/tests/scheduler/weighers/test_goodness.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/weighers/test_base.py` & `manila-9.1.5/manila/tests/scheduler/weighers/test_base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/weighers/test_pool.py` & `manila-9.1.5/manila/tests/scheduler/weighers/test_pool.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/weighers/test_capacity.py` & `manila-9.1.5/manila/tests/scheduler/weighers/test_capacity.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/test_utils.py` & `manila-9.1.5/manila/tests/scheduler/test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/drivers/test_base.py` & `manila-9.1.5/manila/tests/scheduler/drivers/test_base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/drivers/test_filter.py` & `manila-9.1.5/manila/tests/scheduler/drivers/test_filter.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/drivers/test_simple.py` & `manila-9.1.5/manila/tests/scheduler/drivers/test_simple.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_base.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_share_replication.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_share_replication.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_capabilities.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_capabilities.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_availability_zone.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_availability_zone.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_retry.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_retry.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_json.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_json.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_extra_specs_ops.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_extra_specs_ops.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_capacity.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_capacity.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_base_host.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_base_host.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_ignore_attempted_hosts.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_ignore_attempted_hosts.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/filters/test_driver.py` & `manila-9.1.5/manila/tests/scheduler/filters/test_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/evaluator/test_evaluator.py` & `manila-9.1.5/manila/tests/scheduler/evaluator/test_evaluator.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/test_rpcapi.py` & `manila-9.1.5/manila/tests/scheduler/test_rpcapi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/test_scheduler_options.py` & `manila-9.1.5/manila/tests/scheduler/test_scheduler_options.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/test_manager.py` & `manila-9.1.5/manila/tests/scheduler/test_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/test_host_manager.py` & `manila-9.1.5/manila/tests/scheduler/test_host_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/scheduler/fakes.py` & `manila-9.1.5/manila/tests/scheduler/fakes.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/data/test_utils.py` & `manila-9.1.5/manila/tests/data/test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/data/test_helper.py` & `manila-9.1.5/manila/tests/data/test_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/data/test_rpcapi.py` & `manila-9.1.5/manila/tests/data/test_rpcapi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/data/test_manager.py` & `manila-9.1.5/manila/tests/data/test_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_test.py` & `manila-9.1.5/manila/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_api.py` & `manila-9.1.5/manila/tests/share/test_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -997,15 +997,15 @@
         {'replication_type': None, 'dhss': False, 'share_server_id': None},
         {'replication_type': None, 'dhss': True, 'share_server_id': 'fake'}
     )
     @ddt.unpack
     def test_manage_new(self, replication_type, dhss, share_server_id):
         share_data = {
             'host': 'fake',
-            'export_location': 'fake',
+            'export_location_path': 'fake',
             'share_proto': 'fake',
             'share_type_id': 'fake',
         }
         if dhss:
             share_data['share_server_id'] = share_server_id
         driver_options = {}
         date = datetime.datetime(1, 1, 1, 1, 1, 1)
@@ -1041,15 +1041,16 @@
                          mock.Mock(return_value=share))
         self.mock_object(share_types, 'get_share_type',
                          mock.Mock(return_value=fake_type))
         self.mock_object(db_api, 'share_server_get',
                          mock.Mock(return_value=share_server))
         self.mock_object(db_api, 'share_network_subnet_get',
                          mock.Mock(return_value=fake_subnet))
-        self.mock_object(self.api, 'get_all', mock.Mock(return_value=[]))
+        self.mock_object(db_api, 'share_instances_get_all',
+                         mock.Mock(return_value=[]))
 
         self.api.manage(self.context, copy.deepcopy(share_data),
                         driver_options)
 
         share_data.update({
             'user_id': self.context.user_id,
             'project_id': self.context.project_id,
@@ -1068,21 +1069,26 @@
         expected_request_spec = self._get_request_spec_dict(
             share, fake_type, size=0, share_proto=share_data['share_proto'],
             host=share_data['host'])
 
         if dhss:
             share_data.update({
                 'share_network_id': fake_subnet['share_network_id']})
-        export_location = share_data.pop('export_location')
-        self.api.get_all.assert_called_once_with(self.context, mock.ANY)
+        export_location = share_data.pop('export_location_path')
+        filters = {'export_location_path': export_location,
+                   'host': share_data['host']
+                   }
+        if share_server_id:
+            filters['share_server_id'] = share_server_id
+        db_api.share_instances_get_all.assert_called_once_with(
+            self.context, filters=filters)
         db_api.share_create.assert_called_once_with(self.context, share_data)
         db_api.share_get.assert_called_once_with(self.context, share['id'])
         db_api.share_export_locations_update.assert_called_once_with(
-            self.context, share.instance['id'], export_location
-        )
+            self.context, share.instance['id'], export_location)
         self.scheduler_rpcapi.manage_share.assert_called_once_with(
             self.context, share['id'], driver_options, expected_request_spec)
         if dhss:
             db_api.share_server_get.assert_called_once_with(
                 self.context, share_data['share_server_id'])
             db_api.share_network_subnet_get.assert_called_once_with(
                 self.context, share_server['share_network_subnet_id'])
@@ -1092,15 +1098,15 @@
               (False, exception.InvalidInput, True),
               (True, exception.InvalidInput, True))
     @ddt.unpack
     def test_manage_new_dhss_true_and_false(self, dhss, exception_type,
                                             has_share_server_id):
         share_data = {
             'host': 'fake',
-            'export_location': 'fake',
+            'export_location_path': 'fake',
             'share_proto': 'fake',
             'share_type_id': 'fake',
         }
         if has_share_server_id:
             share_data['share_server_id'] = 'fake'
 
         driver_options = {}
@@ -1115,38 +1121,38 @@
                 'mount_snapshot_support': False,
                 'driver_handles_share_servers': dhss,
             },
         }
 
         self.mock_object(share_types, 'get_share_type',
                          mock.Mock(return_value=fake_type))
-        self.mock_object(self.api, 'get_all', mock.Mock(return_value=[]))
+        self.mock_object(db_api, 'share_instances_get_all',
+                         mock.Mock(return_value=[]))
 
         self.assertRaises(exception_type,
                           self.api.manage,
                           self.context,
                           share_data=share_data,
                           driver_options=driver_options
                           )
         share_types.get_share_type.assert_called_once_with(
             self.context, share_data['share_type_id']
         )
-        self.api.get_all.assert_called_once_with(
-            self.context, {
-                'host': share_data['host'],
-                'export_location': share_data['export_location'],
-                'share_proto': share_data['share_proto'],
-                'share_type_id': share_data['share_type_id']
-            }
-        )
+        filters = {'export_location_path': share_data['export_location_path'],
+                   'host': share_data['host']
+                   }
+        if has_share_server_id:
+            filters['share_server_id'] = 'fake'
+        db_api.share_instances_get_all.assert_called_once_with(
+            self.context, filters=filters)
 
     def test_manage_new_share_server_not_found(self):
         share_data = {
             'host': 'fake',
-            'export_location': 'fake',
+            'export_location_path': 'fake',
             'share_proto': 'fake',
             'share_type_id': 'fake',
             'share_server_id': 'fake'
 
         }
         driver_options = {}
         date = datetime.datetime(1, 1, 1, 1, 1, 1)
@@ -1162,38 +1168,38 @@
                 'mount_snapshot_support': False,
                 'driver_handles_share_servers': True,
             },
         }
 
         self.mock_object(share_types, 'get_share_type',
                          mock.Mock(return_value=fake_type))
-        self.mock_object(self.api, 'get_all', mock.Mock(return_value=[]))
+        self.mock_object(db_api, 'share_instances_get_all',
+                         mock.Mock(return_value=[]))
 
         self.assertRaises(exception.InvalidInput,
                           self.api.manage,
                           self.context,
                           share_data=share_data,
                           driver_options=driver_options
                           )
         share_types.get_share_type.assert_called_once_with(
             self.context, share_data['share_type_id']
         )
-        self.api.get_all.assert_called_once_with(
-            self.context, {
+        db_api.share_instances_get_all.assert_called_once_with(
+            self.context, filters={
+                'export_location_path': share_data['export_location_path'],
                 'host': share_data['host'],
-                'export_location': share_data['export_location'],
-                'share_proto': share_data['share_proto'],
-                'share_type_id': share_data['share_type_id']
+                'share_server_id': share_data['share_server_id']
             }
         )
 
     def test_manage_new_share_server_not_active(self):
         share_data = {
             'host': 'fake',
-            'export_location': 'fake',
+            'export_location_path': 'fake',
             'share_proto': 'fake',
             'share_type_id': 'fake',
             'share_server_id': 'fake'
 
         }
         fake_share_data = {
             'id': 'fakeid',
@@ -1215,59 +1221,59 @@
             },
         }
 
         share = db_api.share_create(self.context, fake_share_data)
 
         self.mock_object(share_types, 'get_share_type',
                          mock.Mock(return_value=fake_type))
-        self.mock_object(self.api, 'get_all', mock.Mock(return_value=[]))
+        self.mock_object(db_api, 'share_instances_get_all',
+                         mock.Mock(return_value=[]))
         self.mock_object(db_api, 'share_server_get',
                          mock.Mock(return_value=share))
 
         self.assertRaises(exception.InvalidShareServer,
                           self.api.manage,
                           self.context,
                           share_data=share_data,
                           driver_options=driver_options
                           )
         share_types.get_share_type.assert_called_once_with(
             self.context, share_data['share_type_id']
         )
-        self.api.get_all.assert_called_once_with(
-            self.context, {
+        db_api.share_instances_get_all.assert_called_once_with(
+            self.context, filters={
+                'export_location_path': share_data['export_location_path'],
                 'host': share_data['host'],
-                'export_location': share_data['export_location'],
-                'share_proto': share_data['share_proto'],
-                'share_type_id': share_data['share_type_id']
+                'share_server_id': share_data['share_server_id']
             }
         )
         db_api.share_server_get.assert_called_once_with(
             self.context, share_data['share_server_id']
         )
 
     @ddt.data(constants.STATUS_MANAGE_ERROR, constants.STATUS_AVAILABLE)
     def test_manage_duplicate(self, status):
         share_data = {
             'host': 'fake',
-            'export_location': 'fake',
+            'export_location_path': 'fake',
             'share_proto': 'fake',
             'share_type_id': 'fake',
         }
         driver_options = {}
         fake_type = {
             'id': 'fake_type_id',
             'extra_specs': {
                 'snapshot_support': False,
                 'create_share_from_snapshot_support': False,
                 'driver_handles_share_servers': False,
             },
         }
-        shares = [{'id': 'fake', 'status': status}]
-        self.mock_object(self.api, 'get_all',
-                         mock.Mock(return_value=shares))
+        already_managed = [{'id': 'fake', 'status': status}]
+        self.mock_object(db_api, 'share_instances_get_all',
+                         mock.Mock(return_value=already_managed))
         self.mock_object(share_types, 'get_share_type',
                          mock.Mock(return_value=fake_type))
         self.assertRaises(exception.InvalidShare, self.api.manage,
                           self.context, share_data, driver_options)
 
     def _get_request_spec_dict(self, share, share_type, **kwargs):
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/test_service_instance.py` & `manila-9.1.5/manila/tests/share/drivers/test_service_instance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/nexenta/ns4/test_jsonrpc.py` & `manila-9.1.5/manila/tests/share/drivers/nexenta/ns4/test_jsonrpc.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/nexenta/ns4/test_nexenta_nas.py` & `manila-9.1.5/manila/tests/share/drivers/nexenta/ns4/test_nexenta_nas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/nexenta/test_utils.py` & `manila-9.1.5/manila/tests/share/drivers/nexenta/test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/nexenta/ns5/test_jsonrpc.py` & `manila-9.1.5/manila/tests/share/drivers/nexenta/ns5/test_jsonrpc.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/nexenta/ns5/test_nexenta_nas.py` & `manila-9.1.5/manila/tests/share/drivers/nexenta/ns5/test_nexenta_nas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dummy.py` & `manila-9.1.5/manila/tests/share/drivers/dummy.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/cephfs/test_driver.py` & `manila-9.1.5/manila/tests/share/drivers/cephfs/test_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/quobyte/test_quobyte.py` & `manila-9.1.5/manila/tests/share/drivers/quobyte/test_quobyte.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/quobyte/test_jsonrpc.py` & `manila-9.1.5/manila/tests/share/drivers/quobyte/test_jsonrpc.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/veritas/test_veritas_isa.py` & `manila-9.1.5/manila/tests/share/drivers/veritas/test_veritas_isa.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/infinidat/test_infinidat.py` & `manila-9.1.5/manila/tests/share/drivers/infinidat/test_infinidat.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/test_generic.py` & `manila-9.1.5/manila/tests/share/drivers/test_generic.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/glusterfs/test_common.py` & `manila-9.1.5/manila/tests/share/drivers/glusterfs/test_common.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/glusterfs/test_layout.py` & `manila-9.1.5/manila/tests/share/drivers/glusterfs/test_layout.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/glusterfs/test_glusterfs_native.py` & `manila-9.1.5/manila/tests/share/drivers/glusterfs/test_glusterfs_native.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/glusterfs/test_layout_directory.py` & `manila-9.1.5/manila/tests/share/drivers/glusterfs/test_layout_directory.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/glusterfs/test_layout_volume.py` & `manila-9.1.5/manila/tests/share/drivers/glusterfs/test_layout_volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -583,29 +583,33 @@
     def test_delete_share(self, clone_of):
         self._layout._push_gluster_vol = mock.Mock()
         self._layout._wipe_gluster_vol = mock.Mock()
         gmgr = common.GlusterManager
         gmgr1 = gmgr(self.glusterfs_target1, self._execute, None, None)
         gmgr1.set_vol_option = mock.Mock()
         gmgr1.get_vol_option = mock.Mock(return_value=clone_of)
+        new_vol_addr = self.glusterfs_target1
         self.mock_object(self._layout, '_glustermanager',
                          mock.Mock(return_value=gmgr1))
         self._layout.gluster_used_vols = set([self.glusterfs_target1])
 
         self._layout.delete_share(self._context, self.share1)
 
         gmgr1.get_vol_option.assert_called_once_with(
             'user.manila-cloned-from')
         self._layout._wipe_gluster_vol.assert_called_once_with(gmgr1)
+        self.assertIn(new_vol_addr, self._layout.gluster_used_vols)
         self._layout._push_gluster_vol.assert_called_once_with(
             self.glusterfs_target1)
         self._layout.private_storage.delete.assert_called_once_with(
             self.share1['id'])
-        gmgr1.set_vol_option.assert_called_once_with(
-            'user.manila-share', 'NONE')
+        gmgr1.set_vol_option.assert_has_calls([
+            mock.call('user.manila-share', 'NONE'),
+            mock.call('nfs.disable', 'on')
+        ])
 
     def test_delete_share_clone(self):
         self._layout._push_gluster_vol = mock.Mock()
         self._layout._wipe_gluster_vol = mock.Mock()
         gmgr = common.GlusterManager
         gmgr1 = gmgr(self.glusterfs_target1, self._execute, None, None)
         gmgr1.gluster_call = mock.Mock()
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/windows/test_service_instance.py` & `manila-9.1.5/manila/tests/share/drivers/windows/test_service_instance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/windows/test_winrm_helper.py` & `manila-9.1.5/manila/tests/share/drivers/windows/test_winrm_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/windows/test_windows_smb_helper.py` & `manila-9.1.5/manila/tests/share/drivers/windows/test_windows_smb_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/windows/test_windows_utils.py` & `manila-9.1.5/manila/tests/share/drivers/windows/test_windows_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/windows/test_windows_smb_driver.py` & `manila-9.1.5/manila/tests/share/drivers/windows/test_windows_smb_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/common/enas/test_utils.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/common/enas/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -135,7 +135,23 @@
               {'ip_addr': '192.168.1.100/32'},
               {'ip_addr': 'fdf8:f53b:82e4::55/64'},
               {'ip_addr': 'fdf8:f53b:82e4::55/128'},
               {'ip_addr': '[fdf8:f53b:82e4::55]'})
     @ddt.unpack
     def test_invalid_ipv6_addr(self, ip_addr):
         self.assertEqual(ip_addr, utils.export_unc_path(ip_addr))
+
+
+@ddt.ddt
+class SizeToGbTestCase(test.TestCase):
+
+    @ddt.data({'size_in_bytes': 1073741824, 'size_in_gb': 1.0},
+              {'size_in_bytes': 5610301030, 'size_in_gb': 5.22})
+    @ddt.unpack
+    def test_bytes_to_gb(self, size_in_bytes, size_in_gb):
+        self.assertEqual(size_in_gb, utils.bytes_to_gb(size_in_bytes))
+
+    @ddt.data({'size_in_mb': 1024, 'size_in_gb': 1.0},
+              {'size_in_mb': 5346, 'size_in_gb': 5.22})
+    @ddt.unpack
+    def test_mb_to_gb(self, size_in_mb, size_in_gb):
+        self.assertEqual(size_in_gb, utils.mb_to_gb(size_in_mb))
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/common/enas/test_connector.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/common/enas/test_connector.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/common/enas/utils.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/common/enas/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/common/enas/fakes.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/common/enas/fakes.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/powermax/test_object_manager.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/powermax/test_object_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/powermax/test_connection.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/powermax/test_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import ddt
 import mock
 from oslo_log import log
 
 from manila import exception
 from manila.share.drivers.dell_emc.common.enas import connector
+from manila.share.drivers.dell_emc.common.enas import utils as enas_utils
 from manila.share.drivers.dell_emc.plugins.vnx import connection
 from manila.share.drivers.dell_emc.plugins.vnx import object_manager
 from manila import test
 from manila.tests import fake_share
 from manila.tests.share.drivers.dell_emc.common.enas import fakes
 from manila.tests.share.drivers.dell_emc.common.enas import utils
 
@@ -2208,20 +2209,22 @@
             mock.call(self.mover.req_get_ref()),
             mock.call(self.pool.req_get()),
         ]
         xml_req_mock.assert_has_calls(expected_calls)
 
         for pool in fakes.STATS['pools']:
             if pool['pool_name'] == fakes.FakeData.pool_name:
-                self.assertEqual(fakes.FakeData.pool_total_size,
-                                 pool['total_capacity_gb'])
+                self.assertEqual(
+                    enas_utils.mb_to_gb(fakes.FakeData.pool_total_size),
+                    pool['total_capacity_gb'])
 
                 free_size = (fakes.FakeData.pool_total_size -
                              fakes.FakeData.pool_used_size)
-                self.assertEqual(free_size, pool['free_capacity_gb'])
+                self.assertEqual(enas_utils.mb_to_gb(free_size),
+                                 pool['free_capacity_gb'])
 
     def test_update_share_stats_without_matched_config_pools(self):
         self.connection.pools = set('fake_pool')
 
         hook = utils.RequestSideEffect()
         hook.append(self.mover.resp_get_ref_succeed())
         hook.append(self.pool.resp_get_succeed())
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/mocked_unity.yaml` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/mocked_unity.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/test_utils.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/test_client.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/test_client.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/__init__.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/mocked_manila.yaml` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/mocked_manila.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/test_connection.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/test_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,22 +12,23 @@
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import copy
 import ddt
 import mock
-from oslo_utils import units
 import six
 
 from manila import exception
+from manila.share.drivers.dell_emc.common.enas import utils as enas_utils
 from manila import test
 from manila.tests.share.drivers.dell_emc.plugins.unity import fake_exceptions
 from manila.tests.share.drivers.dell_emc.plugins.unity import res_mock
 from manila.tests.share.drivers.dell_emc.plugins.unity import utils
+from oslo_utils import units
 
 
 @ddt.ddt
 class TestConnection(test.TestCase):
     client = None
 
     @classmethod
@@ -285,22 +286,26 @@
     @res_mock.patch_connection
     def test_update_share_stats(self, connection):
         stat_dict = copy.deepcopy(res_mock.STATS)
         connection.update_share_stats(stat_dict)
         self.assertEqual(5, len(stat_dict))
         pool = stat_dict['pools'][0]
         self.assertEqual('pool_1', pool['pool_name'])
-        self.assertEqual(500000.0, pool['total_capacity_gb'])
+        self.assertEqual(
+            enas_utils.bytes_to_gb(500000.0), pool['total_capacity_gb'])
         self.assertEqual(False, pool['qos'])
-        self.assertEqual(30000.0, pool['provisioned_capacity_gb'])
+        self.assertEqual(
+            enas_utils.bytes_to_gb(30000.0), pool['provisioned_capacity_gb'])
         self.assertEqual(20, pool['max_over_subscription_ratio'])
-        self.assertEqual(10000.0, pool['allocated_capacity_gb'])
+        self.assertEqual(
+            enas_utils.bytes_to_gb(10000.0), pool['allocated_capacity_gb'])
         self.assertEqual(0, pool['reserved_percentage'])
         self.assertTrue(pool['thin_provisioning'])
-        self.assertEqual(490000.0, pool['free_capacity_gb'])
+        self.assertEqual(
+            enas_utils.bytes_to_gb(490000.0), pool['free_capacity_gb'])
 
     @res_mock.patch_connection
     def test_update_share_stats__nonexistent_pools(self, connection):
         stat_dict = copy.deepcopy(res_mock.STATS)
 
         self.assertRaises(exception.EMCUnityError,
                           connection.update_share_stats,
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/fake_exceptions.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/fake_exceptions.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/utils.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/unity/res_mock.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/unity/res_mock.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/vnx/test_object_manager.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/vnx/test_object_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/vnx/test_connection.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/vnx/test_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 
 import ddt
 import mock
 from oslo_log import log
 
 from manila import exception
 from manila.share.drivers.dell_emc.common.enas import connector
+from manila.share.drivers.dell_emc.common.enas import utils as enas_utils
 from manila.share.drivers.dell_emc.plugins.vnx import connection
 from manila.share.drivers.dell_emc.plugins.vnx import object_manager
 from manila import test
 from manila.tests import fake_share
 from manila.tests.share.drivers.dell_emc.common.enas import fakes
 from manila.tests.share.drivers.dell_emc.common.enas import utils
 
@@ -2208,20 +2209,22 @@
             mock.call(self.mover.req_get_ref()),
             mock.call(self.pool.req_get()),
         ]
         xml_req_mock.assert_has_calls(expected_calls)
 
         for pool in fakes.STATS['pools']:
             if pool['pool_name'] == fakes.FakeData.pool_name:
-                self.assertEqual(fakes.FakeData.pool_total_size,
-                                 pool['total_capacity_gb'])
+                self.assertEqual(
+                    enas_utils.mb_to_gb(fakes.FakeData.pool_total_size),
+                    pool['total_capacity_gb'])
 
                 free_size = (fakes.FakeData.pool_total_size -
                              fakes.FakeData.pool_used_size)
-                self.assertEqual(free_size, pool['free_capacity_gb'])
+                self.assertEqual(
+                    enas_utils.mb_to_gb(free_size), pool['free_capacity_gb'])
 
     def test_update_share_stats_without_matched_config_pools(self):
         self.connection.pools = set('fake_pool')
 
         hook = utils.RequestSideEffect()
         hook.append(self.mover.resp_get_ref_succeed())
         hook.append(self.pool.resp_get_succeed())
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/isilon/test_isilon.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/isilon/test_isilon.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/plugins/isilon/test_isilon_api.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/plugins/isilon/test_isilon_api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/dell_emc/test_driver.py` & `manila-9.1.5/manila/tests/share/drivers/dell_emc/test_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/test_helpers.py` & `manila-9.1.5/manila/tests/share/drivers/test_helpers.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/test_ganesha.py` & `manila-9.1.5/manila/tests/share/drivers/test_ganesha.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/test_utils.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/test_common.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/test_common.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/fakes.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/fakes.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/protocols/test_base.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/protocols/test_base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/protocols/test_nfs_cmode.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/protocols/test_nfs_cmode.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/protocols/test_cifs_cmode.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/protocols/test_cifs_cmode.py`

 * *Files 6% similar despite different names*

```diff
@@ -210,7 +210,13 @@
         share = fake.CIFS_SHARE.copy()
         share['export_location'] = location
 
         result_ip, result_share_name = self.helper._get_export_location(share)
 
         self.assertEqual(ip, result_ip)
         self.assertEqual(share_name, result_share_name)
+
+    def test_cleanup_demoted_replica(self):
+        self.helper.cleanup_demoted_replica(fake.CIFS_SHARE, fake.SHARE_NAME)
+
+        self.mock_client.remove_cifs_share.assert_called_once_with(
+            fake.SHARE_NAME)
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/protocols/fakes.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/protocols/fakes.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/client/test_api.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/client/test_api.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #    License for the specific language governing permissions and limitations
 #    under the License.
 """
 Tests for NetApp API layer
 """
 import ddt
 import mock
-from six.moves import urllib
+import requests
 
 from manila import exception
 from manila.share.drivers.netapp.dataontap.client import api
 from manila import test
 from manila.tests.share.drivers.netapp.dataontap.client import fakes as fake
 
 
@@ -184,50 +184,48 @@
 
         self.assertRaises(ValueError, self.root.invoke_elem, na_element)
 
     def test_invoke_elem_http_error(self):
         """Tests handling of HTTPError"""
         na_element = fake.FAKE_NA_ELEMENT
         self.mock_object(self.root, '_create_request', mock.Mock(
-            return_value=('abc', fake.FAKE_NA_ELEMENT)))
+            return_value=fake.FAKE_NA_ELEMENT))
         self.mock_object(api, 'LOG')
-        self.root._opener = fake.FAKE_HTTP_OPENER
-        self.mock_object(self.root, '_build_opener')
-        self.mock_object(self.root._opener, 'open', mock.Mock(
-            side_effect=urllib.error.HTTPError(url='', hdrs='',
-                                               fp=None, code='401',
-                                               msg='httperror')))
+        self.root._session = fake.FAKE_HTTP_SESSION
+        self.mock_object(self.root, '_build_session')
+        self.mock_object(self.root._session, 'post', mock.Mock(
+            side_effect=requests.HTTPError()))
 
         self.assertRaises(api.NaApiError, self.root.invoke_elem,
                           na_element)
 
     def test_invoke_elem_urlerror(self):
         """Tests handling of URLError"""
         na_element = fake.FAKE_NA_ELEMENT
         self.mock_object(self.root, '_create_request', mock.Mock(
-            return_value=('abc', fake.FAKE_NA_ELEMENT)))
+            return_value=fake.FAKE_NA_ELEMENT))
         self.mock_object(api, 'LOG')
-        self.root._opener = fake.FAKE_HTTP_OPENER
-        self.mock_object(self.root, '_build_opener')
-        self.mock_object(self.root._opener, 'open', mock.Mock(
-            side_effect=urllib.error.URLError(reason='urlerror')))
+        self.root._session = fake.FAKE_HTTP_SESSION
+        self.mock_object(self.root, '_build_session')
+        self.mock_object(self.root._session, 'post', mock.Mock(
+            side_effect=requests.URLRequired()))
 
         self.assertRaises(exception.StorageCommunicationException,
                           self.root.invoke_elem,
                           na_element)
 
     def test_invoke_elem_unknown_exception(self):
         """Tests handling of Unknown Exception"""
         na_element = fake.FAKE_NA_ELEMENT
         self.mock_object(self.root, '_create_request', mock.Mock(
-            return_value=('abc', fake.FAKE_NA_ELEMENT)))
+            return_value=fake.FAKE_NA_ELEMENT))
         self.mock_object(api, 'LOG')
-        self.root._opener = fake.FAKE_HTTP_OPENER
-        self.mock_object(self.root, '_build_opener')
-        self.mock_object(self.root._opener, 'open', mock.Mock(
+        self.root._session = fake.FAKE_HTTP_SESSION
+        self.mock_object(self.root, '_build_session')
+        self.mock_object(self.root._session, 'post', mock.Mock(
             side_effect=Exception))
 
         exception = self.assertRaises(api.NaApiError, self.root.invoke_elem,
                                       na_element)
         self.assertEqual('unknown', exception.code)
 
     @ddt.data({'trace_enabled': False,
@@ -241,21 +239,24 @@
     @ddt.unpack
     def test_invoke_elem_valid(self, trace_enabled, trace_pattern, log):
         """Tests the method invoke_elem with valid parameters"""
         na_element = fake.FAKE_NA_ELEMENT
         self.root._trace = trace_enabled
         self.root._api_trace_pattern = trace_pattern
         self.mock_object(self.root, '_create_request', mock.Mock(
-            return_value=('abc', fake.FAKE_NA_ELEMENT)))
+            return_value=fake.FAKE_NA_ELEMENT))
         self.mock_object(api, 'LOG')
-        self.root._opener = fake.FAKE_HTTP_OPENER
-        self.mock_object(self.root, '_build_opener')
+        self.root._session = fake.FAKE_HTTP_SESSION
+        self.mock_object(self.root, '_build_session')
         self.mock_object(self.root, '_get_result', mock.Mock(
             return_value=fake.FAKE_NA_ELEMENT))
-        opener_mock = self.mock_object(
-            self.root._opener, 'open', mock.Mock())
-        opener_mock.read.side_effect = ['resp1', 'resp2']
+
+        response = mock.Mock()
+        response.text = 'res1'
+        self.mock_object(
+            self.root._session, 'post', mock.Mock(
+                return_value=response))
 
         self.root.invoke_elem(na_element)
 
         expected_log_count = 2 if log else 0
         self.assertEqual(expected_log_count, api.LOG.debug.call_count)
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/client/test_client_cmode.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/client/test_client_cmode.py`

 * *Files 1% similar despite different names*

```diff
@@ -2427,14 +2427,18 @@
 
         self.client._enable_nfs_protocols(versions)
 
         nfs_service_modify_args = {
             'is-nfsv3-enabled': 'true' if v3 else 'false',
             'is-nfsv40-enabled': 'true' if v40 else 'false',
             'is-nfsv41-enabled': 'true' if v41 else 'false',
+            'showmount': 'true',
+            'is-v3-ms-dos-client-enabled': 'true',
+            'is-nfsv3-connection-drop-enabled': 'false',
+            'enable-ejukebox': 'false',
         }
         self.client.send_request.assert_called_once_with(
             'nfs-service-modify', nfs_service_modify_args)
 
     def test_create_default_nfs_export_rules(self):
 
         class CopyingMock(mock.Mock):
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/client/fakes.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/client/fakes.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 from lxml import etree
 import mock
-from six.moves import urllib
+import requests
 
 from manila.share.drivers.netapp.dataontap.client import api
 
 
 CONNECTION_INFO = {
     'hostname': 'hostname',
     'transport_type': 'https',
@@ -2593,15 +2593,15 @@
 
 FAKE_RESULT_API_ERRNO_VALID = api.NaElement('result')
 FAKE_RESULT_API_ERRNO_VALID.add_attr('errno', '14956')
 
 FAKE_RESULT_SUCCESS = api.NaElement('result')
 FAKE_RESULT_SUCCESS.add_attr('status', 'passed')
 
-FAKE_HTTP_OPENER = urllib.request.build_opener()
+FAKE_HTTP_SESSION = requests.Session()
 
 FAKE_MANAGE_VOLUME = {
     'aggregate': SHARE_AGGREGATE_NAME,
     'name': SHARE_NAME,
     'owning-vserver-name': VSERVER_NAME,
     'junction_path': VOLUME_JUNCTION_PATH,
     'style': 'fake_style',
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/client/test_client_base.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/client/test_client_base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/fakes.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/fakes.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_single_svm.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_single_svm.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_performance.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_performance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_data_motion.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_data_motion.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_base.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -3024,27 +3024,29 @@
         self.assertEqual(constants.REPLICA_STATE_OUT_OF_SYNC, result)
 
     def test_promote_replica(self):
         self.mock_object(self.library,
                          '_get_vserver',
                          mock.Mock(return_value=(fake.VSERVER1,
                                                  mock.Mock())))
+        protocol_helper = mock.Mock()
         self.mock_object(self.library,
                          '_get_helper',
-                         mock.Mock(return_value=mock.Mock()))
+                         mock.Mock(return_value=protocol_helper))
         self.mock_object(self.library, '_create_export',
                          mock.Mock(return_value='fake_export_location'))
         self.mock_object(self.library, '_unmount_orig_active_replica')
         self.mock_object(self.library, '_handle_qos_on_replication_change')
 
         mock_dm_session = mock.Mock()
         self.mock_object(data_motion, "DataMotionSession",
                          mock.Mock(return_value=mock_dm_session))
         self.mock_object(mock_dm_session, 'get_vserver_from_share',
                          mock.Mock(return_value=fake.VSERVER1))
+        self.mock_object(self.client, 'cleanup_demoted_replica')
 
         replicas = self.library.promote_replica(
             None, [self.fake_replica, self.fake_replica_2],
             self.fake_replica_2, [], share_server=None)
 
         mock_dm_session.change_snapmirror_source.assert_called_once_with(
             self.fake_replica, self.fake_replica, self.fake_replica_2,
@@ -3062,14 +3064,52 @@
         self.assertEqual('fake_export_location',
                          actual_replica_2['export_locations'])
         self.assertEqual(constants.STATUS_ACTIVE,
                          actual_replica_2['access_rules_status'])
         self.library._unmount_orig_active_replica.assert_called_once_with(
             self.fake_replica, fake.VSERVER1)
         self.library._handle_qos_on_replication_change.assert_called_once()
+        protocol_helper.cleanup_demoted_replica.assert_called_once_with(
+            self.fake_replica, fake.SHARE['name'])
+
+    def test_promote_replica_cleanup_demoted_storage_error(self):
+        self.mock_object(self.library,
+                         '_get_vserver',
+                         mock.Mock(return_value=(fake.VSERVER1,
+                                                 mock.Mock())))
+        protocol_helper = mock.Mock()
+        self.mock_object(self.library,
+                         '_get_helper',
+                         mock.Mock(return_value=protocol_helper))
+        self.mock_object(self.library, '_create_export',
+                         mock.Mock(return_value='fake_export_location'))
+        self.mock_object(self.library, '_unmount_orig_active_replica')
+        self.mock_object(self.library, '_handle_qos_on_replication_change')
+
+        mock_dm_session = mock.Mock()
+        self.mock_object(data_motion, "DataMotionSession",
+                         mock.Mock(return_value=mock_dm_session))
+        self.mock_object(mock_dm_session, 'get_vserver_from_share',
+                         mock.Mock(return_value=fake.VSERVER1))
+        self.mock_object(
+            protocol_helper, 'cleanup_demoted_replica',
+            mock.Mock(side_effect=exception.StorageCommunicationException))
+        mock_log = self.mock_object(lib_base.LOG, 'exception')
+
+        self.library.promote_replica(
+            None, [self.fake_replica, self.fake_replica_2],
+            self.fake_replica_2, [], share_server=None)
+
+        mock_dm_session.change_snapmirror_source.assert_called_once_with(
+            self.fake_replica, self.fake_replica, self.fake_replica_2,
+            mock.ANY
+        )
+        protocol_helper.cleanup_demoted_replica.assert_called_once_with(
+            self.fake_replica, fake.SHARE['name'])
+        mock_log.assert_called_once()
 
     def test_promote_replica_destination_unreachable(self):
         self.mock_object(self.library,
                          '_get_vserver',
                          mock.Mock(return_value=(fake.VSERVER1,
                                                  mock.Mock())))
         self.mock_object(self.library,
```

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_multi_svm.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_lib_multi_svm.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_driver_interfaces.py` & `manila-9.1.5/manila/tests/share/drivers/netapp/dataontap/cluster_mode/test_driver_interfaces.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/zfsonlinux/test_utils.py` & `manila-9.1.5/manila/tests/share/drivers/zfsonlinux/test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/zfsonlinux/test_driver.py` & `manila-9.1.5/manila/tests/share/drivers/zfsonlinux/test_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/huawei/test_huawei_nas.py` & `manila-9.1.5/manila/tests/share/drivers/huawei/test_huawei_nas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/maprfs/test_maprfs.py` & `manila-9.1.5/manila/tests/share/drivers/maprfs/test_maprfs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/infortrend/fake_infortrend_nas_data.py` & `manila-9.1.5/manila/tests/share/drivers/infortrend/fake_infortrend_nas_data.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/infortrend/fake_infortrend_manila_data.py` & `manila-9.1.5/manila/tests/share/drivers/infortrend/fake_infortrend_manila_data.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/infortrend/test_infortrend_nas.py` & `manila-9.1.5/manila/tests/share/drivers/infortrend/test_infortrend_nas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/hpe/test_hpe_3par_driver.py` & `manila-9.1.5/manila/tests/share/drivers/hpe/test_hpe_3par_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/hpe/test_hpe_3par_mediator.py` & `manila-9.1.5/manila/tests/share/drivers/hpe/test_hpe_3par_mediator.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/hpe/test_hpe_3par_constants.py` & `manila-9.1.5/manila/tests/share/drivers/hpe/test_hpe_3par_constants.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/ganesha/test_utils.py` & `manila-9.1.5/manila/tests/share/drivers/ganesha/test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/ganesha/test_manager.py` & `manila-9.1.5/manila/tests/share/drivers/ganesha/test_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/qnap/test_api.py` & `manila-9.1.5/manila/tests/share/drivers/qnap/test_api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/qnap/test_qnap.py` & `manila-9.1.5/manila/tests/share/drivers/qnap/test_qnap.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/qnap/fakes.py` & `manila-9.1.5/manila/tests/share/drivers/qnap/fakes.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/zfssa/test_zfssarest.py` & `manila-9.1.5/manila/tests/share/drivers/zfssa/test_zfssarest.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/zfssa/test_zfssashare.py` & `manila-9.1.5/manila/tests/share/drivers/zfssa/test_zfssashare.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/test_glusterfs.py` & `manila-9.1.5/manila/tests/share/drivers/test_glusterfs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/tegile/test_tegile.py` & `manila-9.1.5/manila/tests/share/drivers/tegile/test_tegile.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/container/test_protocol_helper.py` & `manila-9.1.5/manila/tests/share/drivers/container/test_protocol_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/container/test_storage_helper.py` & `manila-9.1.5/manila/tests/share/drivers/container/test_storage_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/container/test_container_helper.py` & `manila-9.1.5/manila/tests/share/drivers/container/test_container_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/container/fakes.py` & `manila-9.1.5/manila/tests/share/drivers/container/fakes.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/container/test_driver.py` & `manila-9.1.5/manila/tests/share/drivers/container/test_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/ibm/test_gpfs.py` & `manila-9.1.5/manila/tests/share/drivers/ibm/test_gpfs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/hitachi/hsp/test_rest.py` & `manila-9.1.5/manila/tests/share/drivers/hitachi/hsp/test_rest.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/hitachi/hsp/fakes.py` & `manila-9.1.5/manila/tests/share/drivers/hitachi/hsp/fakes.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/hitachi/hsp/test_driver.py` & `manila-9.1.5/manila/tests/share/drivers/hitachi/hsp/test_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/hitachi/hnas/test_ssh.py` & `manila-9.1.5/manila/tests/share/drivers/hitachi/hnas/test_ssh.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/hitachi/hnas/test_driver.py` & `manila-9.1.5/manila/tests/share/drivers/hitachi/hnas/test_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/test_lvm.py` & `manila-9.1.5/manila/tests/share/drivers/test_lvm.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/inspur/instorage/test_instorage.py` & `manila-9.1.5/manila/tests/share/drivers/inspur/instorage/test_instorage.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/inspur/as13000/test_as13000_nas.py` & `manila-9.1.5/manila/tests/share/drivers/inspur/as13000/test_as13000_nas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/drivers/hdfs/test_hdfs_native.py` & `manila-9.1.5/manila/tests/share/drivers/hdfs/test_hdfs_native.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_migration.py` & `manila-9.1.5/manila/tests/share/test_migration.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_drivers_private_data.py` & `manila-9.1.5/manila/tests/share/test_drivers_private_data.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_rpcapi.py` & `manila-9.1.5/manila/tests/share/test_rpcapi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_snapshot_access.py` & `manila-9.1.5/manila/tests/share/test_snapshot_access.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_manager.py` & `manila-9.1.5/manila/tests/share/test_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_access.py` & `manila-9.1.5/manila/tests/share/test_access.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_share_utils.py` & `manila-9.1.5/manila/tests/share/test_share_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_hook.py` & `manila-9.1.5/manila/tests/share/test_hook.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_share_types.py` & `manila-9.1.5/manila/tests/share/test_share_types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/share/test_driver.py` & `manila-9.1.5/manila/tests/share/test_driver.py`

 * *Files 3% similar despite different names*

```diff
@@ -805,26 +805,30 @@
     def test_create_share_group_snapshot(self):
         fake_snap_member_1 = {
             'id': '6813e06b-a8f5-4784-b17d-f3e91afa370e',
             'share_id': 'a3ebdba5-b4e1-46c8-a0ea-a9ac8daf5296',
             'share_group_snapshot_id': 'fake_share_group_snapshot_id',
             'share_instance_id': 'fake_share_instance_id_1',
             'provider_location': 'should_not_be_used_1',
+            'share_name': 'share_fake_share_instance_id_1',
+            'name': 'share-snapshot-6813e06b-a8f5-4784-b17d-f3e91afa370e',
             'share': {
                 'id': '420f978b-dbf6-4b3c-92fe-f5b17a0bb5e2',
                 'size': 3,
                 'share_proto': 'fake_share_proto',
             },
         }
         fake_snap_member_2 = {
             'id': '1e010dfe-545b-432d-ab95-4ef03cd82f89',
             'share_id': 'a3ebdba5-b4e1-46c8-a0ea-a9ac8daf5296',
             'share_group_snapshot_id': 'fake_share_group_snapshot_id',
             'share_instance_id': 'fake_share_instance_id_2',
             'provider_location': 'should_not_be_used_2',
+            'share_name': 'share_fake_share_instance_id_2',
+            'name': 'share-snapshot-1e010dfe-545b-432d-ab95-4ef03cd82f89',
             'share': {
                 'id': '420f978b-dbf6-4b3c-92fe-f5b17a0bb5e2',
                 'size': '2',
                 'share_proto': 'fake_share_proto',
             },
         }
         fake_snap_dict = {
@@ -855,14 +859,16 @@
             mock.call(
                 'fake_context',
                 {'snapshot_id': member['share_group_snapshot_id'],
                  'share_id': member['share_id'],
                  'share_instance_id': member['share']['id'],
                  'id': member['id'],
                  'share': member['share'],
+                 'share_name': member['share_name'],
+                 'name': member['name'],
                  'size': member['share']['size'],
                  'share_size': member['share']['size'],
                  'share_proto': member['share']['share_proto'],
                  'provider_location': None},
                 share_server=None)
             for member in (fake_snap_member_1, fake_snap_member_2)
         ])
@@ -877,26 +883,30 @@
     def test_create_share_group_snapshot_failed_snapshot(self):
         fake_snap_member_1 = {
             'id': '6813e06b-a8f5-4784-b17d-f3e91afa370e',
             'share_id': 'a3ebdba5-b4e1-46c8-a0ea-a9ac8daf5296',
             'share_group_snapshot_id': 'fake_share_group_snapshot_id',
             'share_instance_id': 'fake_share_instance_id_1',
             'provider_location': 'should_not_be_used_1',
+            'share_name': 'share_fake_share_instance_id_1',
+            'name': 'share-snapshot-6813e06b-a8f5-4784-b17d-f3e91afa370e',
             'share': {
                 'id': '420f978b-dbf6-4b3c-92fe-f5b17a0bb5e2',
                 'size': 3,
                 'share_proto': 'fake_share_proto',
             },
         }
         fake_snap_member_2 = {
             'id': '1e010dfe-545b-432d-ab95-4ef03cd82f89',
             'share_id': 'a3ebdba5-b4e1-46c8-a0ea-a9ac8daf5296',
             'share_group_snapshot_id': 'fake_share_group_snapshot_id',
             'share_instance_id': 'fake_share_instance_id_2',
             'provider_location': 'should_not_be_used_2',
+            'share_name': 'share_fake_share_instance_id_2',
+            'name': 'share-snapshot-1e010dfe-545b-432d-ab95-4ef03cd82f89',
             'share': {
                 'id': '420f978b-dbf6-4b3c-92fe-f5b17a0bb5e2',
                 'size': '2',
                 'share_proto': 'fake_share_proto',
             },
         }
         fake_snap_dict = {
@@ -928,27 +938,31 @@
 
         fake_snap_member_1_expected = {
             'snapshot_id': fake_snap_member_1['share_group_snapshot_id'],
             'share_id': fake_snap_member_1['share_id'],
             'share_instance_id': fake_snap_member_1['share']['id'],
             'id': fake_snap_member_1['id'],
             'share': fake_snap_member_1['share'],
+            'share_name': fake_snap_member_1['share_name'],
+            'name': fake_snap_member_1['name'],
             'size': fake_snap_member_1['share']['size'],
             'share_size': fake_snap_member_1['share']['size'],
             'share_proto': fake_snap_member_1['share']['share_proto'],
             'provider_location': None,
         }
         mock_create_snap.assert_has_calls([
             mock.call(
                 'fake_context',
                 {'snapshot_id': member['share_group_snapshot_id'],
                  'share_id': member['share_id'],
                  'share_instance_id': member['share']['id'],
                  'id': member['id'],
                  'share': member['share'],
+                 'share_name': member['share_name'],
+                 'name': member['name'],
                  'size': member['share']['size'],
                  'share_size': member['share']['size'],
                  'share_proto': member['share']['share_proto'],
                  'provider_location': None},
                 share_server=None)
             for member in (fake_snap_member_1, fake_snap_member_2)
         ])
@@ -1016,26 +1030,30 @@
     def test_delete_share_group_snapshot(self):
         fake_snap_member_1 = {
             'id': '6813e06b-a8f5-4784-b17d-f3e91afa370e',
             'share_id': 'a3ebdba5-b4e1-46c8-a0ea-a9ac8daf5296',
             'share_group_snapshot_id': 'fake_share_group_snapshot_id',
             'share_instance_id': 'fake_share_instance_id_1',
             'provider_location': 'fake_provider_location_2',
+            'share_name': 'share_fake_share_instance_id_1',
+            'name': 'share-snapshot-6813e06b-a8f5-4784-b17d-f3e91afa370e',
             'share': {
                 'id': '420f978b-dbf6-4b3c-92fe-f5b17a0bb5e2',
                 'size': 3,
                 'share_proto': 'fake_share_proto',
             },
         }
         fake_snap_member_2 = {
             'id': '1e010dfe-545b-432d-ab95-4ef03cd82f89',
             'share_id': 'a3ebdba5-b4e1-46c8-a0ea-a9ac8daf5296',
             'share_group_snapshot_id': 'fake_share_group_snapshot_id',
             'share_instance_id': 'fake_share_instance_id_2',
             'provider_location': 'fake_provider_location_2',
+            'share_name': 'share_fake_provider_location_2',
+            'name': 'share-snapshot-1e010dfe-545b-432d-ab95-4ef03cd82f89',
             'share': {
                 'id': '420f978b-dbf6-4b3c-92fe-f5b17a0bb5e2',
                 'size': '2',
                 'share_proto': 'fake_share_proto',
             },
         }
         fake_snap_dict = {
@@ -1066,14 +1084,16 @@
                 {'snapshot_id': member['share_group_snapshot_id'],
                  'share_id': member['share_id'],
                  'share_instance_id': member['share']['id'],
                  'id': member['id'],
                  'share': member['share'],
                  'size': member['share']['size'],
                  'share_size': member['share']['size'],
+                 'share_name': member['share_name'],
+                 'name': member['name'],
                  'share_proto': member['share']['share_proto'],
                  'provider_location': member['provider_location']},
                 share_server=None)
             for member in (fake_snap_member_1, fake_snap_member_2)
         ])
         self.assertIsNone(share_group_snapshot_update)
         self.assertIsNone(member_update_list)
```

### Comparing `manila-9.1.4/manila/tests/fake_notifier.py` & `manila-9.1.5/manila/tests/fake_notifier.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_manager.py` & `manila-9.1.5/manila/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_misc.py` & `manila-9.1.5/manila/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/conf_fixture.py` & `manila-9.1.5/manila/tests/conf_fixture.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_hacking.py` & `manila-9.1.5/manila/tests/test_hacking.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/utils.py` & `manila-9.1.5/manila/tests/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/fake_compute.py` & `manila-9.1.5/manila/tests/fake_compute.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/db/test_api.py` & `manila-9.1.5/manila/tests/db/test_api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/db/migrations/alembic/test_migration.py` & `manila-9.1.5/manila/tests/db/migrations/alembic/test_migration.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/db/migrations/alembic/migrations_data_checks.py` & `manila-9.1.5/manila/tests/db/migrations/alembic/migrations_data_checks.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/db/migrations/test_utils.py` & `manila-9.1.5/manila/tests/db/migrations/test_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/db/test_migration.py` & `manila-9.1.5/manila/tests/db/test_migration.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/db/sqlalchemy/test_api.py` & `manila-9.1.5/manila/tests/db/sqlalchemy/test_api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/db/sqlalchemy/test_models.py` & `manila-9.1.5/manila/tests/db/sqlalchemy/test_models.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/db/fakes.py` & `manila-9.1.5/manila/tests/db/fakes.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/runtime_conf.py` & `manila-9.1.5/manila/tests/runtime_conf.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/fake_service_instance.py` & `manila-9.1.5/manila/tests/fake_service_instance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/volume/test_cinder.py` & `manila-9.1.5/manila/tests/volume/test_cinder.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/test_rpc.py` & `manila-9.1.5/manila/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/wsgi/test_common.py` & `manila-9.1.5/manila/tests/wsgi/test_common.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/wsgi/test_wsgi.py` & `manila-9.1.5/manila/tests/wsgi/test_wsgi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/tests/fake_zfssa.py` & `manila-9.1.5/manila/tests/fake_zfssa.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/message/api.py` & `manila-9.1.5/manila/message/api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/message/message_field.py` & `manila-9.1.5/manila/message/message_field.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/message/message_levels.py` & `manila-9.1.5/manila/message/message_levels.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/i18n.py` & `manila-9.1.5/manila/i18n.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/common.py` & `manila-9.1.5/manila/api/common.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/middleware/auth.py` & `manila-9.1.5/manila/api/middleware/auth.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/middleware/fault.py` & `manila-9.1.5/manila/api/middleware/fault.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/quota_class_sets.py` & `manila-9.1.5/manila/api/v2/quota_class_sets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/quota_sets.py` & `manila-9.1.5/manila/api/v2/quota_sets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/services.py` & `manila-9.1.5/manila/api/v2/services.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_instance_export_locations.py` & `manila-9.1.5/manila/api/v2/share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_replicas.py` & `manila-9.1.5/manila/api/v2/share_replicas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_types.py` & `manila-9.1.5/manila/api/v2/share_types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_snapshot_export_locations.py` & `manila-9.1.5/manila/api/v2/share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_replica_export_locations.py` & `manila-9.1.5/manila/api/v2/share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_access_metadata.py` & `manila-9.1.5/manila/api/v2/share_access_metadata.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_group_type_specs.py` & `manila-9.1.5/manila/api/v2/share_group_type_specs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/availability_zones.py` & `manila-9.1.5/manila/api/v2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/messages.py` & `manila-9.1.5/manila/api/v2/messages.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/router.py` & `manila-9.1.5/manila/api/v2/router.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_group_snapshots.py` & `manila-9.1.5/manila/api/v2/share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_snapshot_instance_export_locations.py` & `manila-9.1.5/manila/api/v2/share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_export_locations.py` & `manila-9.1.5/manila/api/v2/share_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_accesses.py` & `manila-9.1.5/manila/api/v2/share_accesses.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_instances.py` & `manila-9.1.5/manila/api/v2/share_instances.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_networks.py` & `manila-9.1.5/manila/api/v2/share_networks.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_group_types.py` & `manila-9.1.5/manila/api/v2/share_group_types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_groups.py` & `manila-9.1.5/manila/api/v2/share_groups.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/shares.py` & `manila-9.1.5/manila/api/v2/shares.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_servers.py` & `manila-9.1.5/manila/api/v2/share_servers.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_snapshots.py` & `manila-9.1.5/manila/api/v2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_snapshot_instances.py` & `manila-9.1.5/manila/api/v2/share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v2/share_network_subnets.py` & `manila-9.1.5/manila/api/v2/share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/urlmap.py` & `manila-9.1.5/manila/api/urlmap.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v1/scheduler_stats.py` & `manila-9.1.5/manila/api/v1/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v1/share_unmanage.py` & `manila-9.1.5/manila/api/v1/share_unmanage.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v1/share_types_extra_specs.py` & `manila-9.1.5/manila/api/v1/share_types_extra_specs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v1/security_service.py` & `manila-9.1.5/manila/api/v1/security_service.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v1/router.py` & `manila-9.1.5/manila/api/v1/router.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v1/share_manage.py` & `manila-9.1.5/manila/api/v1/share_manage.py`

 * *Files 4% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         # appropriately.
         name = share_data.get('display_name', share_data.get('name'))
         description = share_data.get(
             'display_description', share_data.get('description'))
 
         share = {
             'host': share_data['service_host'],
-            'export_location': share_data['export_path'],
+            'export_location_path': share_data['export_path'],
             'share_proto': share_data['protocol'].upper(),
             'share_type_id': share_data['share_type_id'],
             'display_name': name,
             'display_description': description,
         }
 
         if share_data.get('is_public') is not None:
@@ -82,14 +82,23 @@
             if parameter not in data:
                 msg = _("Required parameter %s not found") % parameter
                 raise exc.HTTPUnprocessableEntity(explanation=msg)
             if not data.get(parameter):
                 msg = _("Required parameter %s is empty") % parameter
                 raise exc.HTTPUnprocessableEntity(explanation=msg)
 
+        if isinstance(data['export_path'], dict):
+            # the path may be inside this dictionary
+            try:
+                data['export_path'] = data['export_path']['path']
+            except KeyError:
+                msg = ("Export path must be a string, or a dictionary "
+                       "with a 'path' item")
+                raise exc.HTTPUnprocessableEntity(explanation=msg)
+
         if not share_utils.extract_host(data['service_host'], 'pool'):
             msg = _("service_host parameter should contain pool.")
             raise exc.HTTPBadRequest(explanation=msg)
 
         try:
             utils.validate_service_host(
                 context, share_utils.extract_host(data['service_host']))
```

### Comparing `manila-9.1.4/manila/api/v1/share_metadata.py` & `manila-9.1.5/manila/api/v1/share_metadata.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v1/shares.py` & `manila-9.1.5/manila/api/v1/shares.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v1/share_servers.py` & `manila-9.1.5/manila/api/v1/share_servers.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v1/share_snapshots.py` & `manila-9.1.5/manila/api/v1/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/v1/limits.py` & `manila-9.1.5/manila/api/v1/limits.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/__init__.py` & `manila-9.1.5/manila/api/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/openstack/versioned_method.py` & `manila-9.1.5/manila/api/openstack/versioned_method.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/openstack/urlmap.py` & `manila-9.1.5/manila/api/openstack/urlmap.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/openstack/wsgi.py` & `manila-9.1.5/manila/api/openstack/wsgi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/openstack/__init__.py` & `manila-9.1.5/manila/api/openstack/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/openstack/rest_api_version_history.rst` & `manila-9.1.5/manila/api/openstack/rest_api_version_history.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/openstack/api_version_request.py` & `manila-9.1.5/manila/api/openstack/api_version_request.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/extensions.py` & `manila-9.1.5/manila/api/extensions.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/quota_class_sets.py` & `manila-9.1.5/manila/api/views/quota_class_sets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/quota_sets.py` & `manila-9.1.5/manila/api/views/quota_sets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/services.py` & `manila-9.1.5/manila/api/views/services.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/scheduler_stats.py` & `manila-9.1.5/manila/api/views/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_replicas.py` & `manila-9.1.5/manila/api/views/share_replicas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_migration.py` & `manila-9.1.5/manila/api/views/share_migration.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_snapshot_export_locations.py` & `manila-9.1.5/manila/api/views/share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/availability_zones.py` & `manila-9.1.5/manila/api/views/availability_zones.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_instance.py` & `manila-9.1.5/manila/api/views/share_instance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/messages.py` & `manila-9.1.5/manila/api/views/messages.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/security_service.py` & `manila-9.1.5/manila/api/views/security_service.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_group_snapshots.py` & `manila-9.1.5/manila/api/views/share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_accesses.py` & `manila-9.1.5/manila/api/views/share_accesses.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/export_locations.py` & `manila-9.1.5/manila/api/views/export_locations.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_networks.py` & `manila-9.1.5/manila/api/views/share_networks.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_group_types.py` & `manila-9.1.5/manila/api/views/share_group_types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/versions.py` & `manila-9.1.5/manila/api/views/versions.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_groups.py` & `manila-9.1.5/manila/api/views/share_groups.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/shares.py` & `manila-9.1.5/manila/api/views/shares.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_servers.py` & `manila-9.1.5/manila/api/views/share_servers.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_snapshots.py` & `manila-9.1.5/manila/api/views/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/limits.py` & `manila-9.1.5/manila/api/views/limits.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_snapshot_instances.py` & `manila-9.1.5/manila/api/views/share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/types.py` & `manila-9.1.5/manila/api/views/types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/views/share_network_subnets.py` & `manila-9.1.5/manila/api/views/share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/versions.py` & `manila-9.1.5/manila/api/versions.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/contrib/__init__.py` & `manila-9.1.5/manila/api/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/api/auth.py` & `manila-9.1.5/manila/api/auth.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/context.py` & `manila-9.1.5/manila/context.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/compute/__init__.py` & `manila-9.1.5/manila/compute/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/compute/nova.py` & `manila-9.1.5/manila/compute/nova.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/quota.py` & `manila-9.1.5/manila/quota.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/network/standalone_network_plugin.py` & `manila-9.1.5/manila/network/standalone_network_plugin.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/network/linux/ovs_lib.py` & `manila-9.1.5/manila/network/linux/ovs_lib.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/network/linux/interface.py` & `manila-9.1.5/manila/network/linux/interface.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/network/linux/ip_lib.py` & `manila-9.1.5/manila/network/linux/ip_lib.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/network/__init__.py` & `manila-9.1.5/manila/network/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/network/neutron/api.py` & `manila-9.1.5/manila/network/neutron/api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/network/neutron/neutron_network_plugin.py` & `manila-9.1.5/manila/network/neutron/neutron_network_plugin.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/network/neutron/constants.py` & `manila-9.1.5/manila/network/neutron/constants.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/common/client_auth.py` & `manila-9.1.5/manila/common/client_auth.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/common/constants.py` & `manila-9.1.5/manila/common/constants.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/common/config.py` & `manila-9.1.5/manila/common/config.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share_group/api.py` & `manila-9.1.5/manila/share_group/api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share_group/share_group_types.py` & `manila-9.1.5/manila/share_group/share_group_types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/weighers/base.py` & `manila-9.1.5/manila/scheduler/weighers/base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/weighers/goodness.py` & `manila-9.1.5/manila/scheduler/weighers/goodness.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/weighers/base_host.py` & `manila-9.1.5/manila/scheduler/weighers/base_host.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/weighers/pool.py` & `manila-9.1.5/manila/scheduler/weighers/pool.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/weighers/capacity.py` & `manila-9.1.5/manila/scheduler/weighers/capacity.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/manager.py` & `manila-9.1.5/manila/scheduler/manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/drivers/base.py` & `manila-9.1.5/manila/scheduler/drivers/base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/drivers/simple.py` & `manila-9.1.5/manila/scheduler/drivers/simple.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/drivers/chance.py` & `manila-9.1.5/manila/scheduler/drivers/chance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/drivers/filter.py` & `manila-9.1.5/manila/scheduler/drivers/filter.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/ignore_attempted_hosts.py` & `manila-9.1.5/manila/scheduler/filters/ignore_attempted_hosts.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/availability_zone.py` & `manila-9.1.5/manila/scheduler/filters/availability_zone.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/base.py` & `manila-9.1.5/manila/scheduler/filters/base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/json.py` & `manila-9.1.5/manila/scheduler/filters/json.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/base_host.py` & `manila-9.1.5/manila/scheduler/filters/base_host.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/driver.py` & `manila-9.1.5/manila/scheduler/filters/driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/share_group_filters/consistent_snapshot.py` & `manila-9.1.5/manila/scheduler/filters/share_group_filters/consistent_snapshot.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/capabilities.py` & `manila-9.1.5/manila/scheduler/filters/capabilities.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/share_replication.py` & `manila-9.1.5/manila/scheduler/filters/share_replication.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/capacity.py` & `manila-9.1.5/manila/scheduler/filters/capacity.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/retry.py` & `manila-9.1.5/manila/scheduler/filters/retry.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/filters/extra_specs_ops.py` & `manila-9.1.5/manila/scheduler/filters/extra_specs_ops.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/base_handler.py` & `manila-9.1.5/manila/scheduler/base_handler.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/scheduler_options.py` & `manila-9.1.5/manila/scheduler/scheduler_options.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/evaluator/evaluator.py` & `manila-9.1.5/manila/scheduler/evaluator/evaluator.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/rpcapi.py` & `manila-9.1.5/manila/scheduler/rpcapi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/host_manager.py` & `manila-9.1.5/manila/scheduler/host_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/scheduler/utils.py` & `manila-9.1.5/manila/scheduler/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/data/manager.py` & `manila-9.1.5/manila/data/manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/data/helper.py` & `manila-9.1.5/manila/data/helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/data/rpcapi.py` & `manila-9.1.5/manila/data/rpcapi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/data/utils.py` & `manila-9.1.5/manila/data/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policy.py` & `manila-9.1.5/manila/policy.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/test.py` & `manila-9.1.5/manila/test.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/api.py` & `manila-9.1.5/manila/share/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -662,26 +662,36 @@
         if not share_replica['host']:
             msg = _("Share replica does not have a valid host.")
             raise exception.InvalidHost(reason=msg)
 
         self.share_rpcapi.update_share_replica(context, share_replica)
 
     def manage(self, context, share_data, driver_options):
-        shares = self.get_all(context, {
+
+        # Check whether there's a share already with the provided options:
+        filters = {
+            'export_location_path': share_data['export_location_path'],
             'host': share_data['host'],
-            'export_location': share_data['export_location'],
-            'share_proto': share_data['share_proto'],
-            'share_type_id': share_data['share_type_id']
-        })
+        }
+        share_server_id = share_data.get('share_server_id')
+        if share_server_id:
+            filters['share_server_id'] = share_data['share_server_id']
+
+        already_managed = self.db.share_instances_get_all(context,
+                                                          filters=filters)
+
+        if already_managed:
+            LOG.error("Found an existing share with export location %s!",
+                      share_data['export_location_path'])
+            msg = _("A share already exists with the export path specified.")
+            raise exception.InvalidShare(reason=msg)
 
         share_type_id = share_data['share_type_id']
         share_type = share_types.get_share_type(context, share_type_id)
 
-        share_server_id = share_data.get('share_server_id')
-
         dhss = share_types.parse_boolean_extra_spec(
             'driver_handles_share_servers',
             share_type['extra_specs']['driver_handles_share_servers'])
 
         if dhss and not share_server_id:
             msg = _("Share Server ID parameter is required when managing a "
                     "share using a share type with "
@@ -713,26 +723,19 @@
             'project_id': context.project_id,
             'status': constants.STATUS_MANAGING,
             'scheduled_at': timeutils.utcnow(),
         })
         share_data.update(
             self.get_share_attributes_from_share_type(share_type))
 
-        LOG.debug("Manage: Found shares %s.", len(shares))
-
-        export_location = share_data.pop('export_location')
-
-        if len(shares) == 0:
-            share = self.db.share_create(context, share_data)
-        else:
-            msg = _("Share already exists.")
-            raise exception.InvalidShare(reason=msg)
+        share = self.db.share_create(context, share_data)
 
+        export_location_path = share_data.pop('export_location_path')
         self.db.share_export_locations_update(context, share.instance['id'],
-                                              export_location)
+                                              export_location_path)
 
         request_spec = self._get_request_spec_dict(
             share, share_type, size=0, share_proto=share_data['share_proto'],
             host=share_data['host'])
 
         # NOTE(ganso): Scheduler is called to validate if share type
         # provided can fit in host provided. It will invoke manage upon
```

### Comparing `manila-9.1.4/manila/share/manager.py` & `manila-9.1.5/manila/share/manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/share_types.py` & `manila-9.1.5/manila/share/share_types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/nexenta/ns4/jsonrpc.py` & `manila-9.1.5/manila/share/drivers/nexenta/ns4/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/nexenta/ns4/nexenta_nfs_helper.py` & `manila-9.1.5/manila/share/drivers/nexenta/ns4/nexenta_nfs_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/nexenta/ns4/nexenta_nas.py` & `manila-9.1.5/manila/share/drivers/nexenta/ns4/nexenta_nas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/nexenta/utils.py` & `manila-9.1.5/manila/share/drivers/nexenta/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/nexenta/options.py` & `manila-9.1.5/manila/share/drivers/nexenta/options.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/nexenta/ns5/jsonrpc.py` & `manila-9.1.5/manila/share/drivers/nexenta/ns5/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/nexenta/ns5/nexenta_nas.py` & `manila-9.1.5/manila/share/drivers/nexenta/ns5/nexenta_nas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/generic.py` & `manila-9.1.5/manila/share/drivers/generic.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/cephfs/driver.py` & `manila-9.1.5/manila/share/drivers/cephfs/driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/lvm.py` & `manila-9.1.5/manila/share/drivers/lvm.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/quobyte/jsonrpc.py` & `manila-9.1.5/manila/share/drivers/quobyte/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/quobyte/quobyte.py` & `manila-9.1.5/manila/share/drivers/quobyte/quobyte.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/veritas/veritas_isa.py` & `manila-9.1.5/manila/share/drivers/veritas/veritas_isa.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/infinidat/infinibox.py` & `manila-9.1.5/manila/share/drivers/infinidat/infinibox.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/glusterfs/common.py` & `manila-9.1.5/manila/share/drivers/glusterfs/common.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/glusterfs/layout_volume.py` & `manila-9.1.5/manila/share/drivers/glusterfs/layout_volume.py`

 * *Files 2% similar despite different names*

```diff
@@ -429,15 +429,20 @@
                 # created by us (as snapshot clones) ...
                 gmgr.gluster_call('volume', 'delete', gmgr.volume)
             else:
                 # ... for volumes that come from the pool, we return
                 # them to the pool (after some purification rituals)
                 self._wipe_gluster_vol(gmgr)
                 gmgr.set_vol_option(USER_MANILA_SHARE, 'NONE')
+                gmgr.set_vol_option('nfs.disable', 'on')
 
+            # When deleting the share instance, we need to
+            # update'self.gluster_used_vols' again
+            self.gluster_used_vols = set()
+            self.gluster_used_vols.add(gmgr.qualified)
             self._push_gluster_vol(gmgr.qualified)
         except exception.GlusterfsException:
             msg = ("Error during delete_share request for "
                    "share %(share_id)s", {'share_id': share['id']})
             LOG.error(msg)
             raise
```

### Comparing `manila-9.1.4/manila/share/drivers/glusterfs/layout.py` & `manila-9.1.5/manila/share/drivers/glusterfs/layout.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/glusterfs/__init__.py` & `manila-9.1.5/manila/share/drivers/glusterfs/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/glusterfs/layout_directory.py` & `manila-9.1.5/manila/share/drivers/glusterfs/layout_directory.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/glusterfs/glusterfs_native.py` & `manila-9.1.5/manila/share/drivers/glusterfs/glusterfs_native.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/windows/winrm_helper.py` & `manila-9.1.5/manila/share/drivers/windows/winrm_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/windows/windows_utils.py` & `manila-9.1.5/manila/share/drivers/windows/windows_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/windows/service_instance.py` & `manila-9.1.5/manila/share/drivers/windows/service_instance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/windows/windows_smb_helper.py` & `manila-9.1.5/manila/share/drivers/windows/windows_smb_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/windows/windows_smb_driver.py` & `manila-9.1.5/manila/share/drivers/windows/windows_smb_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/common/enas/connector.py` & `manila-9.1.5/manila/share/drivers/dell_emc/common/enas/connector.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/common/enas/constants.py` & `manila-9.1.5/manila/share/drivers/dell_emc/common/enas/constants.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/common/enas/utils.py` & `manila-9.1.5/manila/share/drivers/dell_emc/common/enas/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 import types
 
 from oslo_config import cfg
 from oslo_log import log
 from oslo_utils import fnmatch
 from oslo_utils import netutils
 from oslo_utils import timeutils
+from oslo_utils import units
 import ssl
 
 CONF = cfg.CONF
 LOG = log.getLogger(__name__)
 
 
 def decorate_all_methods(decorator, debug_only=False):
@@ -175,7 +176,15 @@
     :param ip_addr: IPv6 address.
     :return: UNC path.
     """
     unc_suffix = '.ipv6-literal.net'
     if netutils.is_valid_ipv6(ip_addr):
         ip_addr = ip_addr.replace(':', '-') + unc_suffix
     return ip_addr
+
+
+def bytes_to_gb(size):
+    return round(float(size) / units.Gi, 2)
+
+
+def mb_to_gb(size):
+    return bytes_to_gb(size * units.Mi)
```

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/common/enas/xml_api_parser.py` & `manila-9.1.5/manila/share/drivers/dell_emc/common/enas/xml_api_parser.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/driver.py` & `manila-9.1.5/manila/share/drivers/dell_emc/driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugins/powermax/connection.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugins/powermax/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -627,16 +627,17 @@
         for name, pool in pools.items():
             if not self.pools or pool['name'] in self.pools:
                 total_size = float(pool['total_size'])
                 used_size = float(pool['used_size'])
 
                 pool_stat = {
                     'pool_name': pool['name'],
-                    'total_capacity_gb': total_size,
-                    'free_capacity_gb': total_size - used_size,
+                    'total_capacity_gb': enas_utils.mb_to_gb(total_size),
+                    'free_capacity_gb':
+                        enas_utils.mb_to_gb(total_size - used_size),
                     'qos': False,
                     'reserved_percentage': self.reserved_percentage,
                     'snapshot_support': True,
                     'create_share_from_snapshot_support': True,
                     'revert_to_snapshot_support': False,
                     'ipv6_support': True
                 }
```

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugins/powermax/object_manager.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugins/powermax/object_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugins/unity/client.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugins/unity/client.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugins/unity/connection.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugins/unity/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,18 +414,20 @@
                 # the unit of following numbers are GB
                 total_size = float(pool.size_total)
                 used_size = float(pool.size_used)
 
                 pool_stat = {
                     'pool_name': pool.name,
                     'thin_provisioning': True,
-                    'total_capacity_gb': total_size,
-                    'free_capacity_gb': total_size - used_size,
-                    'allocated_capacity_gb': used_size,
-                    'provisioned_capacity_gb': float(pool.size_subscribed),
+                    'total_capacity_gb': enas_utils.bytes_to_gb(total_size),
+                    'free_capacity_gb':
+                        enas_utils.bytes_to_gb(total_size - used_size),
+                    'allocated_capacity_gb': enas_utils.bytes_to_gb(used_size),
+                    'provisioned_capacity_gb':
+                        enas_utils.bytes_to_gb(pool.size_subscribed),
                     'qos': False,
                     'reserved_percentage': self.reserved_percentage,
                     'max_over_subscription_ratio':
                         self.max_over_subscription_ratio,
                 }
                 stats_dict['pools'].append(pool_stat)
```

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugins/unity/utils.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugins/unity/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugins/base.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugins/base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugins/vnx/connection.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugins/vnx/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -620,16 +620,17 @@
         for name, pool in pools.items():
             if not self.pools or pool['name'] in self.pools:
                 total_size = float(pool['total_size'])
                 used_size = float(pool['used_size'])
 
                 pool_stat = dict(
                     pool_name=pool['name'],
-                    total_capacity_gb=total_size,
-                    free_capacity_gb=total_size - used_size,
+                    total_capacity_gb=enas_utils.mb_to_gb(total_size),
+                    free_capacity_gb=enas_utils.mb_to_gb(
+                        total_size - used_size),
                     qos=False,
                     reserved_percentage=self.reserved_percentage,
                 )
                 stats_dict['pools'].append(pool_stat)
 
         if not stats_dict['pools']:
             message = _("Failed to update storage pool.")
```

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugins/vnx/object_manager.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugins/vnx/object_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugins/isilon/isilon_api.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugins/isilon/isilon_api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugins/isilon/isilon.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugins/isilon/isilon.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/dell_emc/plugin_manager.py` & `manila-9.1.5/manila/share/drivers/dell_emc/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/service_instance.py` & `manila-9.1.5/manila/share/drivers/service_instance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/common.py` & `manila-9.1.5/manila/share/drivers/netapp/common.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/utils.py` & `manila-9.1.5/manila/share/drivers/netapp/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/options.py` & `manila-9.1.5/manila/share/drivers/netapp/options.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/protocols/base.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/protocols/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,7 +67,11 @@
     @abc.abstractmethod
     def get_target(self, share):
         """Returns host where the share located."""
 
     @abc.abstractmethod
     def get_share_name_for_share(self, share):
         """Returns the flexvol name that hosts a share."""
+
+    @abc.abstractmethod
+    def cleanup_demoted_replica(self, share, share_name):
+        """Do some cleanup regarding the former active replica"""
```

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/protocols/cifs_cmode.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/protocols/cifs_cmode.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,7 +159,17 @@
         export_location = share['export_location'] or '\\\\\\'
         regex = r'^(?:\\\\|//)(?P<host_ip>.*)(?:\\|/)(?P<share_name>.*)$'
         match = re.match(regex, export_location)
         if match:
             return match.group('host_ip'), match.group('share_name')
         else:
             return '', ''
+
+    @na_utils.trace
+    def cleanup_demoted_replica(self, share, share_name):
+        """Cleans up some things regarding a demoted replica."""
+        # NOTE(carloss): This is necessary due to bug 1879368. If we do not
+        # remove this CIFS share, in case the demoted replica is promoted
+        # back, the promotion will fail due to a duplicated entry for the
+        # share, since a create share request is sent to the backend every
+        # time a promotion occurs.
+        self._client.remove_cifs_share(share_name)
```

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/protocols/nfs_cmode.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/protocols/nfs_cmode.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,7 +178,11 @@
         elif actual_export_policy == 'default':
             self._client.create_nfs_export_policy(expected_export_policy)
             self._client.set_nfs_export_policy_for_volume(
                 share_name, expected_export_policy)
         else:
             self._client.rename_nfs_export_policy(actual_export_policy,
                                                   expected_export_policy)
+
+    @na_utils.trace
+    def cleanup_demoted_replica(self, share, share_name):
+        return
```

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/client/api.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/client/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,17 @@
 """
 
 import copy
 import re
 
 from lxml import etree
 from oslo_log import log
+import requests
+from requests import auth
 import six
-from six.moves import urllib
 
 from manila import exception
 from manila.i18n import _
 from manila.share.drivers.netapp import utils
 
 LOG = log.getLogger(__name__)
 
@@ -57,14 +58,15 @@
 
 
 class NaServer(object):
     """Encapsulates server connection logic."""
 
     TRANSPORT_TYPE_HTTP = 'http'
     TRANSPORT_TYPE_HTTPS = 'https'
+    SSL_CERT_DEFAULT = "/etc/ssl/certs/"
     SERVER_TYPE_FILER = 'filer'
     SERVER_TYPE_DFM = 'dfm'
     URL_FILER = 'servlets/netapp.servlets.admin.XMLrequest_filer'
     URL_DFM = 'apis/XMLrequest'
     NETAPP_NS = 'http://www.netapp.com/filer/admin'
     STYLE_LOGIN_PASSWORD = 'basic_auth'
     STYLE_CERTIFICATE = 'certificate_auth'
@@ -228,41 +230,44 @@
         self._password = password
         self._refresh_conn = True
 
     def invoke_elem(self, na_element, enable_tunneling=False):
         """Invoke the API on the server."""
         if na_element and not isinstance(na_element, NaElement):
             ValueError('NaElement must be supplied to invoke API')
-        request, request_element = self._create_request(na_element,
-                                                        enable_tunneling)
+        request_element = self._create_request(na_element, enable_tunneling)
+        request_d = request_element.to_string()
 
         api_name = na_element.get_name()
         api_name_matches_regex = (re.match(self._api_trace_pattern, api_name)
                                   is not None)
 
         if self._trace and api_name_matches_regex:
             LOG.debug("Request: %s", request_element.to_string(pretty=True))
 
-        if (not hasattr(self, '_opener') or not self._opener
+        if (not hasattr(self, '_session') or not self._session
                 or self._refresh_conn):
-            self._build_opener()
+            self._build_session()
         try:
             if hasattr(self, '_timeout'):
-                response = self._opener.open(request, timeout=self._timeout)
+                response = self._session.post(
+                    self._get_url(), data=request_d, timeout=self._timeout)
             else:
-                response = self._opener.open(request)
-        except urllib.error.HTTPError as e:
-            raise NaApiError(e.code, e.msg)
-        except urllib.error.URLError as e:
+                response = self._session.post(
+                    self._get_url(), data=request_d)
+        except requests.HTTPError as e:
+            raise NaApiError(e.errno, e.strerror)
+        except requests.URLRequired as e:
             raise exception.StorageCommunicationException(six.text_type(e))
         except Exception as e:
             raise NaApiError(message=e)
 
-        response_xml = response.read()
-        response_element = self._get_result(response_xml)
+        response_xml = response.text
+        response_element = self._get_result(
+            bytes(bytearray(response_xml, encoding='utf-8')))
 
         if self._trace and api_name_matches_regex:
             LOG.debug("Response: %s", response_element.to_string(pretty=True))
 
         return response_element
 
     def invoke_successfully(self, na_element, enable_tunneling=False):
@@ -292,19 +297,15 @@
         netapp_elem = NaElement('netapp')
         netapp_elem.add_attr('xmlns', self._ns)
         if hasattr(self, '_api_version'):
             netapp_elem.add_attr('version', self._api_version)
         if enable_tunneling:
             self._enable_tunnel_request(netapp_elem)
         netapp_elem.add_child_elem(na_element)
-        request_d = netapp_elem.to_string()
-        request = urllib.request.Request(
-            self._get_url(), data=request_d,
-            headers={'Content-Type': 'text/xml', 'charset': 'utf-8'})
-        return request, netapp_elem
+        return netapp_elem
 
     def _enable_tunnel_request(self, netapp_elem):
         """Enables vserver or vfiler tunneling."""
         if hasattr(self, '_vfiler') and self._vfiler:
             if (hasattr(self, '_api_major_version') and
                     hasattr(self, '_api_minor_version') and
                     self._api_major_version >= 1 and
@@ -337,28 +338,28 @@
 
     def _get_url(self):
         host = self._host
         if ':' in host:
             host = '[%s]' % host
         return '%s://%s:%s/%s' % (self._protocol, host, self._port, self._url)
 
-    def _build_opener(self):
+    def _build_session(self):
         if self._auth_style == NaServer.STYLE_LOGIN_PASSWORD:
             auth_handler = self._create_basic_auth_handler()
         else:
             auth_handler = self._create_certificate_auth_handler()
-        opener = urllib.request.build_opener(auth_handler)
-        self._opener = opener
+
+        self._session = requests.Session()
+        self._session.auth = auth_handler
+        self._session.verify = NaServer.SSL_CERT_DEFAULT
+        self._session.headers = {
+            'Content-Type': 'text/xml', 'charset': 'utf-8'}
 
     def _create_basic_auth_handler(self):
-        password_man = urllib.request.HTTPPasswordMgrWithDefaultRealm()
-        password_man.add_password(None, self._get_url(), self._username,
-                                  self._password)
-        auth_handler = urllib.request.HTTPBasicAuthHandler(password_man)
-        return auth_handler
+        return auth.HTTPBasicAuth(self._username, self._password)
 
     def _create_certificate_auth_handler(self):
         raise NotImplementedError()
 
     def __str__(self):
         return "server: %s" % (self._host)
```

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/client/client_cmode.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/client/client_cmode.py`

 * *Files 0% similar despite different names*

```diff
@@ -1365,14 +1365,18 @@
         nfs40 = 'true' if 'nfs4.0' in versions else 'false'
         nfs41 = 'true' if 'nfs4.1' in versions else 'false'
 
         nfs_service_modify_args = {
             'is-nfsv3-enabled': nfs3,
             'is-nfsv40-enabled': nfs40,
             'is-nfsv41-enabled': nfs41,
+            'showmount': 'true',
+            'is-v3-ms-dos-client-enabled': 'true',
+            'is-nfsv3-connection-drop-enabled': 'false',
+            'enable-ejukebox': 'false',
         }
         self.send_request('nfs-service-modify', nfs_service_modify_args)
 
     @na_utils.trace
     def _create_default_nfs_export_rules(self):
         """Create the default export rule for the NFS service."""
```

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/client/client_base.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/client/client_base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/drv_single_svm.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/drv_single_svm.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/data_motion.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/data_motion.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/lib_single_svm.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/lib_single_svm.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/lib_multi_svm.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/lib_multi_svm.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/drv_multi_svm.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/drv_multi_svm.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/performance.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/performance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/netapp/dataontap/cluster_mode/lib_base.py` & `manila-9.1.5/manila/share/drivers/netapp/dataontap/cluster_mode/lib_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1695,17 +1695,37 @@
             if r['id'] != replica['id']:
                 r = self._safe_change_replica_source(dm_session, r,
                                                      orig_active_replica,
                                                      replica,
                                                      replica_list)
                 new_replica_list.append(r)
 
-        # Unmount the original active replica.
         orig_active_vserver = dm_session.get_vserver_from_share(
             orig_active_replica)
+
+        # Cleanup the original active share if necessary
+        orig_active_replica_backend = (
+            share_utils.extract_host(orig_active_replica['host'],
+                                     level='backend_name'))
+        orig_active_replica_name = self._get_backend_share_name(
+            orig_active_replica['id'])
+        orig_active_vserver_client = data_motion.get_client_for_backend(
+            orig_active_replica_backend, vserver_name=orig_active_vserver)
+
+        orig_active_replica_helper = self._get_helper(orig_active_replica)
+        orig_active_replica_helper.set_client(orig_active_vserver_client)
+
+        try:
+            orig_active_replica_helper.cleanup_demoted_replica(
+                orig_active_replica, orig_active_replica_name)
+        except exception.StorageCommunicationException:
+            LOG.exception("Could not cleanup the original active replica %s.",
+                          orig_active_replica['id'])
+
+        # Unmount the original active replica.
         self._unmount_orig_active_replica(orig_active_replica,
                                           orig_active_vserver)
 
         self._handle_qos_on_replication_change(dm_session,
                                                new_active_replica,
                                                orig_active_replica,
                                                share_server=share_server)
```

### Comparing `manila-9.1.4/manila/share/drivers/zfsonlinux/driver.py` & `manila-9.1.5/manila/share/drivers/zfsonlinux/driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/zfsonlinux/utils.py` & `manila-9.1.5/manila/share/drivers/zfsonlinux/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/huawei/v3/helper.py` & `manila-9.1.5/manila/share/drivers/huawei/v3/helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/huawei/v3/smartx.py` & `manila-9.1.5/manila/share/drivers/huawei/v3/smartx.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/huawei/v3/connection.py` & `manila-9.1.5/manila/share/drivers/huawei/v3/connection.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/huawei/v3/rpcapi.py` & `manila-9.1.5/manila/share/drivers/huawei/v3/rpcapi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/huawei/v3/replication.py` & `manila-9.1.5/manila/share/drivers/huawei/v3/replication.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/huawei/base.py` & `manila-9.1.5/manila/share/drivers/huawei/base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/huawei/huawei_utils.py` & `manila-9.1.5/manila/share/drivers/huawei/huawei_utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/huawei/constants.py` & `manila-9.1.5/manila/share/drivers/huawei/constants.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/huawei/huawei_nas.py` & `manila-9.1.5/manila/share/drivers/huawei/huawei_nas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/maprfs/maprfs_native.py` & `manila-9.1.5/manila/share/drivers/maprfs/maprfs_native.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/maprfs/driver_util.py` & `manila-9.1.5/manila/share/drivers/maprfs/driver_util.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/infortrend/infortrend_nas.py` & `manila-9.1.5/manila/share/drivers/infortrend/infortrend_nas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/infortrend/driver.py` & `manila-9.1.5/manila/share/drivers/infortrend/driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/helpers.py` & `manila-9.1.5/manila/share/drivers/helpers.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/hpe/hpe_3par_mediator.py` & `manila-9.1.5/manila/share/drivers/hpe/hpe_3par_mediator.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/hpe/hpe_3par_driver.py` & `manila-9.1.5/manila/share/drivers/hpe/hpe_3par_driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/ganesha/manager.py` & `manila-9.1.5/manila/share/drivers/ganesha/manager.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/ganesha/__init__.py` & `manila-9.1.5/manila/share/drivers/ganesha/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/ganesha/conf/00-base-export-template.conf` & `manila-9.1.5/manila/share/drivers/ganesha/conf/00-base-export-template.conf`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/ganesha/utils.py` & `manila-9.1.5/manila/share/drivers/ganesha/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/qnap/qnap.py` & `manila-9.1.5/manila/share/drivers/qnap/qnap.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/qnap/api.py` & `manila-9.1.5/manila/share/drivers/qnap/api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/zfssa/restclient.py` & `manila-9.1.5/manila/share/drivers/zfssa/restclient.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/zfssa/zfssashare.py` & `manila-9.1.5/manila/share/drivers/zfssa/zfssashare.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/zfssa/zfssarest.py` & `manila-9.1.5/manila/share/drivers/zfssa/zfssarest.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/tegile/tegile.py` & `manila-9.1.5/manila/share/drivers/tegile/tegile.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/container/container_helper.py` & `manila-9.1.5/manila/share/drivers/container/container_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/container/driver.py` & `manila-9.1.5/manila/share/drivers/container/driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/container/storage_helper.py` & `manila-9.1.5/manila/share/drivers/container/storage_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/container/protocol_helper.py` & `manila-9.1.5/manila/share/drivers/container/protocol_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/ibm/gpfs.py` & `manila-9.1.5/manila/share/drivers/ibm/gpfs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/hitachi/hsp/rest.py` & `manila-9.1.5/manila/share/drivers/hitachi/hsp/rest.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/hitachi/hsp/driver.py` & `manila-9.1.5/manila/share/drivers/hitachi/hsp/driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/hitachi/hnas/driver.py` & `manila-9.1.5/manila/share/drivers/hitachi/hnas/driver.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/hitachi/hnas/ssh.py` & `manila-9.1.5/manila/share/drivers/hitachi/hnas/ssh.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/inspur/instorage/cli_helper.py` & `manila-9.1.5/manila/share/drivers/inspur/instorage/cli_helper.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/inspur/instorage/instorage.py` & `manila-9.1.5/manila/share/drivers/inspur/instorage/instorage.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/inspur/as13000/as13000_nas.py` & `manila-9.1.5/manila/share/drivers/inspur/as13000/as13000_nas.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers/hdfs/hdfs_native.py` & `manila-9.1.5/manila/share/drivers/hdfs/hdfs_native.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/migration.py` & `manila-9.1.5/manila/share/migration.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/drivers_private_data.py` & `manila-9.1.5/manila/share/drivers_private_data.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/rpcapi.py` & `manila-9.1.5/manila/share/rpcapi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/driver.py` & `manila-9.1.5/manila/share/driver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1473,14 +1473,16 @@
                      'share_type_id': 'some_fake_uuid',
                      'user_id': 'a0314a441ca842019b0952224aa39192',
                      'deleted': 'False',
                      'created_at': datetime.datetime(2015, 8, 10, 0, 5, 58),
                      'share': <models.Share>,
                      'updated_at': datetime.datetime(2015, 8, 10, 0, 5, 58),
                      'share_proto': 'NFS',
+                     'share_name': 'share_some_fake_uuid',
+                     'name': 'share-snapshot-some_fake_uuid',
                      'project_id': '13c0be6290934bd98596cfa004650049',
                      'share_group_snapshot_id': 'some_fake_uuid',
                      'deleted_at': None,
                      'share_id': 'some_fake_uuid',
                      'id': 'some_fake_uuid',
                      'size': 1,
                      'provider_location': None,
@@ -1515,14 +1517,16 @@
             for member in snapshot_members:
                 share_snapshot = {
                     'snapshot_id': member['share_group_snapshot_id'],
                     'share_id': member['share_id'],
                     'share_instance_id': member['share']['id'],
                     'id': member['id'],
                     'share': member['share'],
+                    'share_name': member['share_name'],
+                    'name': member['name'],
                     'size': member['share']['size'],
                     'share_size': member['share']['size'],
                     'share_proto': member['share']['share_proto'],
                     'provider_location': None,
                 }
                 try:
                     member_update = self.create_snapshot(
@@ -1577,14 +1581,16 @@
                      'share_id': 'some_fake_uuid',
                      'user_id': 'a0314a441ca842019b0952224aa39192',
                      'deleted': 'False',
                      'created_at': datetime.datetime(2015, 8, 10, 0, 5, 58),
                      'share': <models.Share>,
                      'updated_at': datetime.datetime(2015, 8, 10, 0, 5, 58),
                      'share_proto': 'NFS',
+                     'share_name':'share_some_fake_uuid',
+                     'name': 'share-snapshot-some_fake_uuid',
                      'project_id': '13c0be6290934bd98596cfa004650049',
                      'share_group_snapshot_id': 'some_fake_uuid',
                      'deleted_at': None,
                      'id': 'some_fake_uuid',
                      'size': 1,
                      'provider_location': 'fake_provider_location_value',
                     }
@@ -1604,14 +1610,16 @@
             share_snapshot = {
                 'snapshot_id': member['share_group_snapshot_id'],
                 'share_id': member['share_id'],
                 'share_instance_id': member['share']['id'],
                 'id': member['id'],
                 'share': member['share'],
                 'size': member['share']['size'],
+                'share_name': member['share_name'],
+                'name': member['name'],
                 'share_size': member['share']['size'],
                 'share_proto': member['share']['share_proto'],
                 'provider_location': member['provider_location'],
             }
             self.delete_snapshot(
                 context, share_snapshot, share_server=share_server)
```

### Comparing `manila-9.1.4/manila/share/__init__.py` & `manila-9.1.5/manila/share/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/configuration.py` & `manila-9.1.5/manila/share/configuration.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/hook.py` & `manila-9.1.5/manila/share/hook.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/access.py` & `manila-9.1.5/manila/share/access.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/snapshot_access.py` & `manila-9.1.5/manila/share/snapshot_access.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/share/utils.py` & `manila-9.1.5/manila/share/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/utils.py` & `manila-9.1.5/manila/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/api.py` & `manila-9.1.5/manila/db/api.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/env.py` & `manila-9.1.5/manila/db/migrations/alembic/env.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/migration.py` & `manila-9.1.5/manila/db/migrations/alembic/migration.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/211836bf835c_add_access_level.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/211836bf835c_add_access_level.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/03da71c0e321_convert_cgs_to_share_groups.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/03da71c0e321_convert_cgs_to_share_groups.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/d5db24264f5c_add_consistent_snapshot_support_attr_to_share_group_model.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/d5db24264f5c_add_consistent_snapshot_support_attr_to_share_group_model.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/27cb96d991fa_add_description_for_share_type.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/27cb96d991fa_add_description_for_share_type.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/87ce15c59bbe_add_revert_to_snapshot_support.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/87ce15c59bbe_add_revert_to_snapshot_support.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/55761e5f59c5_add_snapshot_support_extra_spec_to_share_types.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/55761e5f59c5_add_snapshot_support_extra_spec_to_share_types.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/3e7d62517afa_add_create_share_from_snapshot_support.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/3e7d62517afa_add_create_share_from_snapshot_support.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/1f0bd302c1a6_add_availability_zones_table.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/1f0bd302c1a6_add_availability_zones_table.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/5155c7077f99_add_more_network_info_attributes_to_network_allocations_table.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/5155c7077f99_add_more_network_info_attributes_to_network_allocations_table.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/59eb64046740_add_required_extra_spec.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/59eb64046740_add_required_extra_spec.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/344c1ac4747f_add_share_instance_access_rules_status.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/344c1ac4747f_add_share_instance_access_rules_status.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/38e632621e5a_change_volume_type_to_share_type.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/38e632621e5a_change_volume_type_to_share_type.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/3db9992c30f3_transform_statuses_to_lowercase.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/3db9992c30f3_transform_statuses_to_lowercase.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/dda6de06349_add_export_locations_metadata.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/dda6de06349_add_export_locations_metadata.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/ef0c02b4366_add_share_type_projects.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/ef0c02b4366_add_share_type_projects.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/e1949a93157a_add_share_group_types_table.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/e1949a93157a_add_share_group_types_table.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/162a3e673105_manila_init.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/162a3e673105_manila_init.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/927920b37453_add_provider_location_for_share_group_snapshot_members_model.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/927920b37453_add_provider_location_for_share_group_snapshot_members_model.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/323840a08dc4_add_shares_task_state.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/323840a08dc4_add_shares_task_state.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/829a09b0ddd4_fix_project_share_type_quotas_unique_constraint.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/829a09b0ddd4_fix_project_share_type_quotas_unique_constraint.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/238720805ce1_add_messages_table.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/238720805ce1_add_messages_table.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/533646c7af38_remove_unused_attr_status.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/533646c7af38_remove_unused_attr_status.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/95e3cf760840_remove_nova_net_id_column_from_share_.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/95e3cf760840_remove_nova_net_id_column_from_share_.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/30cb96d995fa_add_is_public_column_for_share.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/30cb96d995fa_add_is_public_column_for_share.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/56cdbe267881_add_share_export_locations_table.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/56cdbe267881_add_share_export_locations_table.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/48a7beae3117_move_share_type_id_to_instances.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/48a7beae3117_move_share_type_id_to_instances.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/221a83cfd85b_change_user_project_id_length.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/221a83cfd85b_change_user_project_id_length.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/3651e16d7c43_add_consistency_groups.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/3651e16d7c43_add_consistency_groups.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/805685098bd2_add_share_network_subnets_table_and_modify_share_servers_table.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/805685098bd2_add_share_network_subnets_table_and_modify_share_servers_table.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/fdfb668d19e1_add_gateway_to_network_allocations_table.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/fdfb668d19e1_add_gateway_to_network_allocations_table.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/63809d875e32_add_access_key.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/63809d875e32_add_access_key.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/493eaffd79e1_add_mtu_network_allocations_share_networks.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/493eaffd79e1_add_mtu_network_allocations_share_networks.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/e9f79621d83f_add_cast_rules_to_readonly_to_share_instances.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/e9f79621d83f_add_cast_rules_to_readonly_to_share_instances.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/17115072e1c3_add_nova_net_id_column_to_share_networks.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/17115072e1c3_add_nova_net_id_column_to_share_networks.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/e8ea58723178_remove_host_from_driver_private_data.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/e8ea58723178_remove_host_from_driver_private_data.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/a77e2ad5012d_add_share_snapshot_access.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/a77e2ad5012d_add_share_snapshot_access.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/579c267fbb4d_add_share_instances_access_map.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/579c267fbb4d_add_share_instances_access_map.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/11ee96se625f3_add_metadata_for_access.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/11ee96se625f3_add_metadata_for_access.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/b10fb432c042_squash_share_group_snapshot_members_and_share_snapshot_instance_models.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/b10fb432c042_squash_share_group_snapshot_members_and_share_snapshot_instance_models.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/293fac1130ca_add_replication_attrs.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/293fac1130ca_add_replication_attrs.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/7d142971c4ef_add_reservation_expire_index.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/7d142971c4ef_add_reservation_expire_index.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/5237b6625330_add_availability_zone_id_field_to_share_groups.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/5237b6625330_add_availability_zone_id_field_to_share_groups.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/6a3fd2984bc31_add_is_auto_deletable_and_identifier_fields_for_share_servers.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/6a3fd2984bc31_add_is_auto_deletable_and_identifier_fields_for_share_servers.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/097fad24d2fc_add_share_instances_share_id_index.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/097fad24d2fc_add_share_instances_share_id_index.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/4ee2cf4be19a_remove_share_snapshots_export_location.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/4ee2cf4be19a_remove_share_snapshots_export_location.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/3a482171410f_add_drivers_private_data_table.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/3a482171410f_add_drivers_private_data_table.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/b516de97bfee_add_quota_per_share_type_model.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/b516de97bfee_add_quota_per_share_type_model.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/5077ffcc5f1c_add_share_instances.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/5077ffcc5f1c_add_share_instances.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/0274d20c560f_add_ou_to_security_service.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/0274d20c560f_add_ou_to_security_service.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/54667b9cade7_restore_share_instance_access_map_state.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/54667b9cade7_restore_share_instance_access_map_state.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/eb6d5544cbbd_add_provider_location_to_share_snapshot_instances.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/eb6d5544cbbd_add_provider_location_to_share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/versions/4a482571410f_add_backends_info_table.py` & `manila-9.1.5/manila/db/migrations/alembic/versions/4a482571410f_add_backends_info_table.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic/script.py.mako` & `manila-9.1.5/manila/db/migrations/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/alembic.ini` & `manila-9.1.5/manila/db/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migrations/utils.py` & `manila-9.1.5/manila/db/migrations/utils.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/base.py` & `manila-9.1.5/manila/db/base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/migration.py` & `manila-9.1.5/manila/db/migration.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/sqlalchemy/api.py` & `manila-9.1.5/manila/db/sqlalchemy/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1450,14 +1450,27 @@
                 models.ShareInstanceExportLocations.path ==
                 export_location_path)
         if export_location_id:
             query = query.filter(
                 models.ShareInstanceExportLocations.uuid ==
                 export_location_id)
 
+    # TODO(gouthamr): This DB API method needs to be generalized for all
+    # share instance fields.
+    host = filters.get('host')
+    if host:
+        query = query.filter(
+            or_(models.ShareInstance.host == host,
+                models.ShareInstance.host.like("{0}#%".format(host)))
+        )
+    share_server_id = filters.get('share_server_id')
+    if share_server_id:
+        query = query.filter(
+            models.ShareInstance.share_server_id == share_server_id)
+
     # Returns list of share instances that satisfy filters.
     query = query.all()
     return query
 
 
 @require_context
 def share_instance_delete(context, instance_id, session=None,
```

### Comparing `manila-9.1.4/manila/db/sqlalchemy/query.py` & `manila-9.1.5/manila/db/sqlalchemy/query.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/sqlalchemy/models.py` & `manila-9.1.5/manila/db/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/db/__init__.py` & `manila-9.1.5/manila/db/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/volume/__init__.py` & `manila-9.1.5/manila/volume/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/volume/cinder.py` & `manila-9.1.5/manila/volume/cinder.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_group_type.py` & `manila-9.1.5/manila/policies/share_group_type.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/quota_set.py` & `manila-9.1.5/manila/policies/quota_set.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/scheduler_stats.py` & `manila-9.1.5/manila/policies/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_group_types_spec.py` & `manila-9.1.5/manila/policies/share_group_types_spec.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_export_location.py` & `manila-9.1.5/manila/policies/share_export_location.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/availability_zone.py` & `manila-9.1.5/manila/policies/availability_zone.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/base.py` & `manila-9.1.5/manila/policies/base.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/service.py` & `manila-9.1.5/manila/policies/service.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_instance_export_location.py` & `manila-9.1.5/manila/policies/share_instance_export_location.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_snapshot_instance.py` & `manila-9.1.5/manila/policies/share_snapshot_instance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_access_metadata.py` & `manila-9.1.5/manila/policies/share_access_metadata.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_network_subnet.py` & `manila-9.1.5/manila/policies/share_network_subnet.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_replica.py` & `manila-9.1.5/manila/policies/share_replica.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_snapshot_instance_export_location.py` & `manila-9.1.5/manila/policies/share_snapshot_instance_export_location.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_instance.py` & `manila-9.1.5/manila/policies/share_instance.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_access.py` & `manila-9.1.5/manila/policies/share_access.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_network.py` & `manila-9.1.5/manila/policies/share_network.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_type.py` & `manila-9.1.5/manila/policies/share_type.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/security_service.py` & `manila-9.1.5/manila/policies/security_service.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/message.py` & `manila-9.1.5/manila/policies/message.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_types_extra_spec.py` & `manila-9.1.5/manila/policies/share_types_extra_spec.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/__init__.py` & `manila-9.1.5/manila/policies/__init__.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_group.py` & `manila-9.1.5/manila/policies/share_group.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_replica_export_location.py` & `manila-9.1.5/manila/policies/share_replica_export_location.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_snapshot_export_location.py` & `manila-9.1.5/manila/policies/share_snapshot_export_location.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/quota_class_set.py` & `manila-9.1.5/manila/policies/quota_class_set.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_group_snapshot.py` & `manila-9.1.5/manila/policies/share_group_snapshot.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/shares.py` & `manila-9.1.5/manila/policies/shares.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_server.py` & `manila-9.1.5/manila/policies/share_server.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/policies/share_snapshot.py` & `manila-9.1.5/manila/policies/share_snapshot.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/hacking/checks.py` & `manila-9.1.5/manila/hacking/checks.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/wsgi/common.py` & `manila-9.1.5/manila/wsgi/common.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/wsgi/wsgi.py` & `manila-9.1.5/manila/wsgi/wsgi.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/wsgi/eventlet_server.py` & `manila-9.1.5/manila/wsgi/eventlet_server.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/version.py` & `manila-9.1.5/manila/version.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/exception.py` & `manila-9.1.5/manila/exception.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/manila/rpc.py` & `manila-9.1.5/manila/rpc.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/requirements.txt` & `manila-9.1.5/requirements.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 # process, which may cause wedges in the gate later.
 
 # pbr should be first
 pbr!=2.1.0,>=2.0.0 # Apache-2.0
 
 alembic>=0.8.10 # MIT
 Babel!=2.4.0,>=2.3.4 # BSD
-eventlet!=0.18.3,!=0.20.1,>=0.18.2 # MIT
+eventlet>=0.24.1 # MIT
 greenlet>=0.4.10 # MIT
 ipaddress>=1.0.17;python_version<'3.3' # PSF
 lxml!=3.7.0,>=3.4.1 # BSD
 netaddr>=0.7.18 # BSD
 oslo.config>=5.2.0 # Apache-2.0
 oslo.context>=2.19.2 # Apache-2.0
 oslo.db>=4.27.0 # Apache-2.0
 oslo.i18n>=3.15.3 # Apache-2.0
 oslo.log>=3.36.0 # Apache-2.0
-oslo.messaging>=5.29.0 # Apache-2.0
+oslo.messaging>=6.4.1 # Apache-2.0
 oslo.middleware>=3.31.0 # Apache-2.0
 oslo.policy>=1.30.0 # Apache-2.0
 oslo.reports>=1.18.0 # Apache-2.0
 oslo.rootwrap>=5.8.0 # Apache-2.0
 oslo.serialization!=2.19.1,>=2.18.0 # Apache-2.0
-oslo.service!=1.28.1,>=1.24.0 # Apache-2.0
+oslo.service>=1.31.0 # Apache-2.0
 oslo.upgradecheck>=0.1.0 # Apache-2.0
 oslo.utils>=3.33.0 # Apache-2.0
 oslo.concurrency>=3.26.0 # Apache-2.0
 paramiko>=2.0.0 # LGPLv2.1+
 Paste>=2.0.2 # MIT
 PasteDeploy>=1.5.0 # MIT
 pyparsing>=2.1.0 # MIT
```

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-native/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-native/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-generic-scenario-custom-image/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-generic-scenario-custom-image/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-zfsonlinux/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-zfsonlinux/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-dummy/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-dummy/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-container/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-container/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-hdfs/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-hdfs/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native-centos-7/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-native-centos-7/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-native-heketi/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-native-heketi/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-postgres-generic-singlebackend/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-postgres-generic-singlebackend/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-mysql-generic/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-mysql-generic/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-container-scenario-custom-image/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-container-scenario-custom-image/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-nfs-centos-7/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-nfs-centos-7/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs-heketi/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-glusterfs-nfs-heketi/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-dummy-py2/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-dummy-py2/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-scenario/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-scenario/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-native-centos-7/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-minimal-py35-dsvm-cephfs-native-centos-7/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/grenade-dsvm-manila/run.yaml` & `manila-9.1.5/playbooks/legacy/grenade-dsvm-manila/run.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -47,18 +47,15 @@
           # link should not be used.
           export GRENADE_PLUGINRC="enable_grenade_plugin manila https://opendev.org/openstack/manila"
 
           # Keep localrc to be able to set some vars in pre_test_hook
           export KEEP_LOCALRC=1
 
           function pre_test_hook {
-              source $BASE/new/manila/contrib/ci/pre_test_hook.sh \
-                  True \
-                  dummy \
-                  multibackend
+              source $BASE/new/manila/contrib/ci/pre_test_hook.sh False lvm multibackend
           }
           export -f pre_test_hook
 
           export BRANCH_OVERRIDE=default
           if [ "$BRANCH_OVERRIDE" != "default" ] ; then
               export OVERRIDE_ZUUL_BRANCH=$BRANCH_OVERRIDE
           fi
```

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs-centos-7/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-cephfs-nfs-centos-7/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/run-ipv6.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-minimal-dsvm-lvm/run-ipv6.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/playbooks/legacy/manila-tempest-dsvm-generic-no-share-servers/run.yaml` & `manila-9.1.5/playbooks/legacy/manila-tempest-dsvm-generic-no-share-servers/run.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/scheduler-stats.inc` & `manila-9.1.5/api-ref/source/scheduler-stats.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-instances.inc` & `manila-9.1.5/api-ref/source/share-instances.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-export-locations.inc` & `manila-9.1.5/api-ref/source/share-export-locations.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-groups.inc` & `manila-9.1.5/api-ref/source/share-groups.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/extensions.inc` & `manila-9.1.5/api-ref/source/extensions.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-networks.inc` & `manila-9.1.5/api-ref/source/share-networks.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/index.rst` & `manila-9.1.5/api-ref/source/index.rst`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-instance-export-locations.inc` & `manila-9.1.5/api-ref/source/share-instance-export-locations.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/user-messages.inc` & `manila-9.1.5/api-ref/source/user-messages.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/quota-classes.inc` & `manila-9.1.5/api-ref/source/quota-classes.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/snapshots.inc` & `manila-9.1.5/api-ref/source/snapshots.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/status.yaml` & `manila-9.1.5/api-ref/source/status.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-types.inc` & `manila-9.1.5/api-ref/source/share-types.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/snapshot-instances-list-with-detail-response.json` & `manila-9.1.5/api-ref/source/samples/snapshot-instances-list-with-detail-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/versions-get-version-response.json` & `manila-9.1.5/api-ref/source/samples/versions-get-version-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-update-response.json` & `manila-9.1.5/api-ref/source/samples/share-update-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/snapshot-create-response.json` & `manila-9.1.5/api-ref/source/samples/snapshot-create-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-type-show-response.json` & `manila-9.1.5/api-ref/source/samples/share-type-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/shares-list-response.json` & `manila-9.1.5/api-ref/source/samples/shares-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-manage-response.json` & `manila-9.1.5/api-ref/source/samples/share-manage-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/export-location-list-response.json` & `manila-9.1.5/api-ref/source/samples/export-location-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-network-create-response.json` & `manila-9.1.5/api-ref/source/samples/share-network-create-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/security-service-create-response.json` & `manila-9.1.5/api-ref/source/samples/security-service-create-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/snapshot-update-response.json` & `manila-9.1.5/api-ref/source/samples/snapshot-update-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-actions-list-access-rules-response.json` & `manila-9.1.5/api-ref/source/samples/share-actions-list-access-rules-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/snapshot-show-response.json` & `manila-9.1.5/api-ref/source/samples/snapshot-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-types-list-response.json` & `manila-9.1.5/api-ref/source/samples/share-types-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-networks-list-detailed-response.json` & `manila-9.1.5/api-ref/source/samples/share-networks-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-type-update-response.json` & `manila-9.1.5/api-ref/source/samples/share-type-create-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-group-snapshot-update-response.json` & `manila-9.1.5/api-ref/source/samples/share-group-snapshot-create-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-network-update-response.json` & `manila-9.1.5/api-ref/source/samples/share-network-update-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-access-rules-list-response.json` & `manila-9.1.5/api-ref/source/samples/share-access-rules-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-group-snapshots-list-members-response.json` & `manila-9.1.5/api-ref/source/samples/share-group-snapshots-list-members-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-show-instance-response.json` & `manila-9.1.5/api-ref/source/samples/share-show-instance-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-replicas-show-response.json` & `manila-9.1.5/api-ref/source/samples/share-replicas-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-group-snapshot-create-response.json` & `manila-9.1.5/api-ref/source/samples/share-group-snapshot-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/security-service-update-response.json` & `manila-9.1.5/api-ref/source/samples/security-service-update-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-network-show-response.json` & `manila-9.1.5/api-ref/source/samples/share-network-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/pools-list-response.json` & `manila-9.1.5/api-ref/source/samples/pools-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-group-snapshot-show-response.json` & `manila-9.1.5/api-ref/source/samples/share-group-snapshot-update-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/pools-list-detailed-response.json` & `manila-9.1.5/api-ref/source/samples/pools-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-replica-export-location-list-response.json` & `manila-9.1.5/api-ref/source/samples/share-replica-export-location-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-create-response.json` & `manila-9.1.5/api-ref/source/samples/share-create-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/snapshot-instance-show-response.json` & `manila-9.1.5/api-ref/source/samples/snapshot-instance-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-group-snapshots-list-detailed-response.json` & `manila-9.1.5/api-ref/source/samples/share-group-snapshots-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-manage-request.json` & `manila-9.1.5/api-ref/source/samples/share-manage-request.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/extensions-list-response.json` & `manila-9.1.5/api-ref/source/samples/extensions-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-group-snapshots-list-response.json` & `manila-9.1.5/api-ref/source/samples/share-group-snapshots-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-group-create-response.json` & `manila-9.1.5/api-ref/source/samples/share-group-create-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/user-messages-list-response.json` & `manila-9.1.5/api-ref/source/samples/user-messages-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/security-services-list-for-share-network-response.json` & `manila-9.1.5/api-ref/source/samples/security-services-list-for-share-network-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/user-message-show-response.json` & `manila-9.1.5/api-ref/source/samples/user-message-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-server-show-response.json` & `manila-9.1.5/api-ref/source/samples/share-server-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/shares-list-detailed-response.json` & `manila-9.1.5/api-ref/source/samples/shares-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-groups-list-response.json` & `manila-9.1.5/api-ref/source/samples/share-groups-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-replicas-list-detail-response.json` & `manila-9.1.5/api-ref/source/samples/share-replicas-list-detail-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-type-create-response.json` & `manila-9.1.5/api-ref/source/samples/share-type-update-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-group-show-response.json` & `manila-9.1.5/api-ref/source/samples/share-group-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/versions-index-response.json` & `manila-9.1.5/api-ref/source/samples/versions-index-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/security-services-list-detailed-response.json` & `manila-9.1.5/api-ref/source/samples/security-services-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/security-service-show-response.json` & `manila-9.1.5/api-ref/source/samples/security-service-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-server-manage-response.json` & `manila-9.1.5/api-ref/source/samples/share-server-manage-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/services-list-response.json` & `manila-9.1.5/api-ref/source/samples/services-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-show-response.json` & `manila-9.1.5/api-ref/source/samples/share-show-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-group-update-response.json` & `manila-9.1.5/api-ref/source/samples/share-group-update-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/snapshots-list-response.json` & `manila-9.1.5/api-ref/source/samples/snapshots-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-instances-list-response.json` & `manila-9.1.5/api-ref/source/samples/share-instances-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/share-types-default-list-response.json` & `manila-9.1.5/api-ref/source/samples/share-types-default-list-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/quota-show-detail-response.json` & `manila-9.1.5/api-ref/source/samples/quota-show-detail-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/snapshots-list-detailed-response.json` & `manila-9.1.5/api-ref/source/samples/snapshots-list-detailed-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/samples/snapshot-manage-response.json` & `manila-9.1.5/api-ref/source/samples/snapshot-manage-response.json`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-access-rule-metadata.inc` & `manila-9.1.5/api-ref/source/share-access-rule-metadata.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-actions.inc` & `manila-9.1.5/api-ref/source/share-actions.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-replica-export-locations.inc` & `manila-9.1.5/api-ref/source/share-replica-export-locations.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/security-services.inc` & `manila-9.1.5/api-ref/source/security-services.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/services.inc` & `manila-9.1.5/api-ref/source/services.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/snapshot-instances.inc` & `manila-9.1.5/api-ref/source/snapshot-instances.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/parameters.yaml` & `manila-9.1.5/api-ref/source/parameters.yaml`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/versions.inc` & `manila-9.1.5/api-ref/source/versions.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-group-snapshots.inc` & `manila-9.1.5/api-ref/source/share-group-snapshots.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/limits.inc` & `manila-9.1.5/api-ref/source/limits.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/shares.inc` & `manila-9.1.5/api-ref/source/shares.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/quota-sets.inc` & `manila-9.1.5/api-ref/source/quota-sets.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-metadata.inc` & `manila-9.1.5/api-ref/source/share-metadata.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-servers.inc` & `manila-9.1.5/api-ref/source/share-servers.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/availability-zones.inc` & `manila-9.1.5/api-ref/source/availability-zones.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-group-types.inc` & `manila-9.1.5/api-ref/source/share-group-types.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-migration.inc` & `manila-9.1.5/api-ref/source/share-migration.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-access-rules.inc` & `manila-9.1.5/api-ref/source/share-access-rules.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/share-replicas.inc` & `manila-9.1.5/api-ref/source/share-replicas.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/conf.py` & `manila-9.1.5/api-ref/source/conf.py`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/api-ref/source/os-share-manage.inc` & `manila-9.1.5/api-ref/source/os-share-manage.inc`

 * *Files identical despite different names*

### Comparing `manila-9.1.4/bindep.txt` & `manila-9.1.5/bindep.txt`

 * *Files identical despite different names*

