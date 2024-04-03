# Comparing `tmp/openstack-image-manager-0.5.1.tar.gz` & `tmp/openstack-image-manager-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openstack-image-manager-0.5.1.tar", last modified: Tue Sep 19 15:26:55 2023, max compression
+gzip compressed data, was "openstack-image-manager-0.6.0.tar", last modified: Tue Oct 24 14:50:16 2023, max compression
```

## Comparing `openstack-image-manager-0.5.1.tar` & `openstack-image-manager-0.6.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:26:55.711755 openstack-image-manager-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2023-09-19 15:26:55.711755 openstack-image-manager-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      447 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:26:55.703755 openstack-image-manager-0.5.1/etc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:26:55.707755 openstack-image-manager-0.5.1/etc/images/
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/almalinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3175 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/centos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      987 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/cirros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      910 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/clearlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/debian.yml
--rw-r--r--   0 runner    (1001) docker     (127)      983 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/fedora.yml
--rw-r--r--   0 runner    (1001) docker     (127)      948 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/flatcar.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/gardenlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/kubernetes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      847 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/octavia.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/opensuse.yml
--rw-r--r--   0 runner    (1001) docker     (127)      945 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/opnsense.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2157 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/rockylinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/talos.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9458 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/images/ubuntu.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/etc/schema.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:26:55.711755 openstack-image-manager-0.5.1/openstack_image_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      201 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/openstack_image_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    46123 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/openstack_image_manager/manage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4195 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/openstack_image_manager/mirror.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/openstack_image_manager/table.py
--rw-r--r--   0 runner    (1001) docker     (127)     9698 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/openstack_image_manager/update.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-19 15:26:55.711755 openstack-image-manager-0.5.1/openstack_image_manager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14787 2023-09-19 15:26:55.000000 openstack-image-manager-0.5.1/openstack_image_manager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      887 2023-09-19 15:26:55.000000 openstack-image-manager-0.5.1/openstack_image_manager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-19 15:26:55.000000 openstack-image-manager-0.5.1/openstack_image_manager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2023-09-19 15:26:55.000000 openstack-image-manager-0.5.1/openstack_image_manager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-09-19 15:26:55.000000 openstack-image-manager-0.5.1/openstack_image_manager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2023-09-19 15:26:55.000000 openstack-image-manager-0.5.1/openstack_image_manager.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      191 2023-09-19 15:26:41.000000 openstack-image-manager-0.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-19 15:26:55.711755 openstack-image-manager-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 14:50:16.454199 openstack-image-manager-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    14797 2023-10-24 14:50:16.454199 openstack-image-manager-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 14:50:16.450199 openstack-image-manager-0.6.0/etc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 14:50:16.454199 openstack-image-manager-0.6.0/etc/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/almalinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3175 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/centos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      987 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/cirros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/clearlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3278 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/debian.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      984 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/fedora.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/flatcar.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/gardenlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/kubernetes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/octavia.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/opensuse.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/opnsense.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/rockylinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/talos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9458 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/images/ubuntu.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/etc/schema.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 14:50:16.454199 openstack-image-manager-0.6.0/openstack_image_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/openstack_image_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46990 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/openstack_image_manager/manage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4451 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/openstack_image_manager/mirror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/openstack_image_manager/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10546 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/openstack_image_manager/update.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-24 14:50:16.454199 openstack-image-manager-0.6.0/openstack_image_manager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14797 2023-10-24 14:50:16.000000 openstack-image-manager-0.6.0/openstack_image_manager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2023-10-24 14:50:16.000000 openstack-image-manager-0.6.0/openstack_image_manager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-24 14:50:16.000000 openstack-image-manager-0.6.0/openstack_image_manager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2023-10-24 14:50:16.000000 openstack-image-manager-0.6.0/openstack_image_manager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-24 14:50:16.000000 openstack-image-manager-0.6.0/openstack_image_manager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2023-10-24 14:50:16.000000 openstack-image-manager-0.6.0/openstack_image_manager.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2023-10-24 14:50:06.000000 openstack-image-manager-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-24 14:50:16.458199 openstack-image-manager-0.6.0/setup.cfg
```

### Comparing `openstack-image-manager-0.5.1/LICENSE` & `openstack-image-manager-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/PKG-INFO` & `openstack-image-manager-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-image-manager
-Version: 0.5.1
+Version: 0.6.0
 Summary: OpenStack image manager
 Author-email: OSISM community <info@osism.tech>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,27 +219,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru==0.7.2
-Requires-Dist: minio==7.1.16
+Requires-Dist: minio==7.1.17
 Requires-Dist: munch==4.0.0
 Requires-Dist: natsort==8.4.0
-Requires-Dist: openstacksdk==1.5.0
+Requires-Dist: openstacksdk==2.0.0
 Requires-Dist: paramiko==3.3.1
 Requires-Dist: patool==1.12
 Requires-Dist: requests==2.31.0
-Requires-Dist: ruamel.yaml==0.17.32
+Requires-Dist: ruamel.yaml==0.18.1
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: typer[all]==0.9.0
 Requires-Dist: yamale==4.0.4
 
 # openstack-image-manager
 
 [![PyPi version](https://badgen.net/pypi/v/openstack-image-manager/)](https://pypi.org/project/openstack-image-manager/)
 [![PyPi license](https://badgen.net/pypi/license/openstack-image-manager/)](https://pypi.org/project/openstack-image-manager/)
 
 Easily manage and keep up to date a large number of images on an OpenStack environment
 
-Documentation: <https://docs.scs.community/docs/category/openstack-image-manager/>
+Documentation: <https://osism.github.io/docs/guides/operations-guide/openstack/image-manager>
```

### Comparing `openstack-image-manager-0.5.1/etc/images/almalinux.yml` & `openstack-image-manager-0.6.0/etc/images/almalinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/centos.yml` & `openstack-image-manager-0.6.0/etc/images/centos.yml`

 * *Files 5% similar despite different names*

```diff
@@ -53,19 +53,19 @@
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud.centos.org/centos/8-stream/x86_64/images/CHECKSUM
     latest_url: 
       https://cloud.centos.org/centos/8-stream/x86_64/images/CentOS-Stream-GenericCloud-8-HEREBE\d+\.\dDRAGONS.x86_64.qcow2
     versions:
-      - version: '20230826'
+      - version: '20231003'
         url: 
-          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/centos-stream-8/20230826-centos-stream-8.qcow2
-        checksum: sha256:3d0b45bacb0355d7f0542d302a7a71146b425f41b513782b4dc554daffe72e9e
-        build_date: 2023-08-26
+          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/centos-stream-8/20231003-centos-stream-8.qcow2
+        checksum: sha256:5f98a3018e64ec334be3e350df59db29f6ad822688529304c7905594fff005f4
+        build_date: 2023-10-03
   - name: CentOS Stream 9
     enable: true
     shortname: centos-stream-9
     format: qcow2
     login: centos
     min_disk: 10
     min_ram: 512
@@ -84,12 +84,12 @@
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud.centos.org/centos/9-stream/x86_64/images/CHECKSUM
     latest_url: 
       https://cloud.centos.org/centos/9-stream/x86_64/images/CentOS-Stream-GenericCloud-9-HEREBE\d+\.\dDRAGONS.x86_64.qcow2
     versions:
-      - version: '20230821'
+      - version: '20231002'
         url: 
-          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/centos-stream-9/20230821-centos-stream-9.qcow2
-        checksum: sha256:ce7828ea362f4c63d5a73567ee4adce11248b017473ac3bdfa1c155af8796fe5
-        build_date: 2023-08-21
+          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/centos-stream-9/20231002-centos-stream-9.qcow2
+        checksum: sha256:d12bb6934dd207e242d6aa13f6a4ca4969449c14c3bbdd88a5ce5f5203597a40
+        build_date: 2023-10-02
```

### Comparing `openstack-image-manager-0.5.1/etc/images/cirros.yml` & `openstack-image-manager-0.6.0/etc/images/cirros.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/clearlinux.yml` & `openstack-image-manager-0.6.0/etc/images/clearlinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/debian.yml` & `openstack-image-manager-0.6.0/etc/images/debian.yml`

 * *Files 9% similar despite different names*

```diff
@@ -22,20 +22,20 @@
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cdimage.debian.org/cdimage/cloud/buster/latest/SHA512SUMS
     latest_url: 
       https://cdimage.debian.org/cdimage/cloud/buster/latest/debian-10-genericcloud-amd64.qcow2
     versions:
-      - version: '20230802'
+      - version: '20230917'
         url: 
-          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/debian-10/20230802-debian-10.qcow2
+          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/debian-10/20230917-debian-10.qcow2
         checksum: 
-          sha512:a11252378a9573052b48fcec8cb0e5d6ab11338e81e960442eb8a9bf4504d8e25f5c2cd893c010f63ef99201b96e4f9cae7fce6c8f8132e18f1a561b9afd8eb3
-        build_date: 2023-08-02
+          sha512:5bafe5851a38fe3a00853ee3c3203d5444c05cf81d1e04ac4a5c04500ab45cbd346a3e23aa138d93b4d13de2c0d4cfa7b4d622554d4e5e198817911f2bbd664b
+        build_date: 2023-09-17
   - name: Debian 11
     enable: true
     shortname: debian-11
     format: qcow2
     login: debian
     min_disk: 8
     min_ram: 512
@@ -53,20 +53,20 @@
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cdimage.debian.org/cdimage/cloud/bullseye/latest/SHA512SUMS
     latest_url: 
       https://cdimage.debian.org/cdimage/cloud/bullseye/latest/debian-11-genericcloud-amd64.qcow2
     versions:
-      - version: '20230802'
+      - version: '20231004'
         url: 
-          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/debian-11/20230802-debian-11.qcow2
+          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/debian-11/20231004-debian-11.qcow2
         checksum: 
-          sha512:f16512174452ea49e34d302e86bb11b6f821013dde583bf703550998e87819f98c6e411d7737bd53f16c73007f1c039218f9cd40421ec3a6b5b1fe38044018c0
-        build_date: 2023-08-02
+          sha512:83cb90b44232d6899369fa0980a81baf97a2ac5b188ffe373a74f4aa9ca7a5d13b80f6cc221fc31c3e556efb4f0aa254ea265c2d452d23e2e7f05efc7f3014fe
+        build_date: 2023-10-04
   - name: Debian 12
     enable: true
     shortname: debian-12
     format: qcow2
     login: debian
     min_disk: 8
     min_ram: 512
@@ -84,13 +84,13 @@
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cdimage.debian.org/cdimage/cloud/bookworm/daily/latest/SHA512SUMS
     latest_url: 
       https://cdimage.debian.org/cdimage/cloud/bookworm/daily/latest/debian-12-genericcloud-amd64-daily.qcow2
     versions:
-      - build_date: 2023-08-26
+      - build_date: 2023-10-04
         checksum: 
-          sha512:b9b01448d1572326622e7e5bcf060b995bf5c66326e826f0149c21807cfbda4000224aeb2f43a1991ab486c05d0e184e13de3dd4e0be48611626377fb10d9263
+          sha512:b594a146d0c85aa138b7fd4ba27cdf4c56fcceef2f90d6f4e1553d35c7faeab566df885ccaa2e48b2c9edf1d1926f0b997406f34729708069c6fad9ee1c73397
         url: 
-          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/debian-12/20230826-debian-12.qcow2
-        version: '20230826'
+          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/debian-12/20231004-debian-12.qcow2
+        version: '20231004'
```

### Comparing `openstack-image-manager-0.5.1/etc/images/fedora.yml` & `openstack-image-manager-0.6.0/etc/images/fedora.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 images:
 
   - name: Fedora 37
-    enable: true
+    enable: false
     shortname: fedora-37
     format: qcow2
     login: fedora
     min_disk: 4
     min_ram: 512
     status: active
     visibility: public
```

### Comparing `openstack-image-manager-0.5.1/etc/images/flatcar.yml` & `openstack-image-manager-0.6.0/etc/images/flatcar.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/gardenlinux.yml` & `openstack-image-manager-0.6.0/etc/images/gardenlinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/kubernetes.yml` & `openstack-image-manager-0.6.0/etc/images/kubernetes.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/octavia.yml` & `openstack-image-manager-0.6.0/etc/images/octavia.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/opensuse.yml` & `openstack-image-manager-0.6.0/etc/images/opensuse.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/opnsense.yml` & `openstack-image-manager-0.6.0/etc/images/opnsense.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/rockylinux.yml` & `openstack-image-manager-0.6.0/etc/images/rockylinux.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/talos.yml` & `openstack-image-manager-0.6.0/etc/images/talos.yml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/etc/images/ubuntu.yml` & `openstack-image-manager-0.6.0/etc/images/ubuntu.yml`

 * *Files 2% similar despite different names*

```diff
@@ -175,19 +175,19 @@
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/focal/current/SHA256SUMS
     latest_url: https://cloud-images.ubuntu.com/focal/current/focal-server-cloudimg-amd64.img
     versions:
-      - version: '20230823'
+      - version: '20231003'
         url: 
-          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/ubuntu-20.04/20230823-ubuntu-20.04.qcow2
-        checksum: sha256:ecfb2e07fce2a273e845ca328b96b64390a0bf0efad70fd1d57a0ebbc0549717
-        build_date: 2023-08-23
+          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/ubuntu-20.04/20231003-ubuntu-20.04.qcow2
+        checksum: sha256:9ad6b034f5cbb3492eb0148caee16cd73b63f2478bd2a6bc64503042b0f4035b
+        build_date: 2023-10-03
   - name: Ubuntu 20.04 Minimal
     enable: true
     shortname: ubuntu-20.04-minimal
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
@@ -206,19 +206,19 @@
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/minimal/releases/focal/release/SHA256SUMS
     latest_url: 
       https://cloud-images.ubuntu.com/minimal/releases/focal/release/ubuntu-20.04-minimal-cloudimg-amd64.img
     versions:
-      - version: '20230811'
+      - version: '20230921'
         url: 
-          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/ubuntu-20.04-minimal/20230811-ubuntu-20.04-minimal.qcow2
-        checksum: sha256:95536fe95112fff650012867afbf36d31f61ec06dea4269f8133bd6a1596bf95
-        build_date: 2023-08-11
+          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/ubuntu-20.04-minimal/20230921-ubuntu-20.04-minimal.qcow2
+        checksum: sha256:a809d42ff539812149bd3dd9b8e2dfba611dff4fcfe14818423b32dc54d46bf9
+        build_date: 2023-09-21
   - name: Ubuntu 22.04
     enable: true
     shortname: ubuntu-22.04
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
@@ -236,19 +236,19 @@
       replace_frequency: quarterly
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/jammy/current/SHA256SUMS
     latest_url: https://cloud-images.ubuntu.com/jammy/current/jammy-server-cloudimg-amd64.img
     versions:
-      - version: '20230823'
+      - version: '20230929'
         url: 
-          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/ubuntu-22.04/20230823-ubuntu-22.04.qcow2
-        checksum: sha256:a7845be05e3a5c9e031be35d27ecb6f4c1cdab8df89475cd1943d57ff94294c9
-        build_date: 2023-08-23
+          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/ubuntu-22.04/20230929-ubuntu-22.04.qcow2
+        checksum: sha256:9d43e0311466f60b152059f97b75036e84bb20c1c3d8e0e2af7070e065b91c52
+        build_date: 2023-09-29
   - name: Ubuntu 22.04 Minimal
     enable: true
     shortname: ubuntu-22.04-minimal
     format: qcow2
     login: ubuntu
     min_disk: 8
     min_ram: 512
@@ -267,12 +267,12 @@
       uuid_validity: last-3
       provided_until: none
     tags: []
     latest_checksum_url: https://cloud-images.ubuntu.com/minimal/releases/jammy/release/SHA256SUMS
     latest_url: 
       https://cloud-images.ubuntu.com/minimal/releases/jammy/release/ubuntu-22.04-minimal-cloudimg-amd64.img
     versions:
-      - version: '20230815'
+      - version: '20231003'
         url: 
-          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/ubuntu-22.04-minimal/20230815-ubuntu-22.04-minimal.qcow2
-        checksum: sha256:72ca6ba4f8b7305479ed32ed79890a52aec4f0629762286dbc9a5e5b3997489c
-        build_date: 2023-08-15
+          https://swift.services.a.regiocloud.tech/swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/openstack-images/ubuntu-22.04-minimal/20231003-ubuntu-22.04-minimal.qcow2
+        checksum: sha256:f18fb7ceb7624545a4c70c1b683b3cfca70815afa1b92ebc08f8a9e49356c5d2
+        build_date: 2023-10-03
```

### Comparing `openstack-image-manager-0.5.1/etc/schema.yaml` & `openstack-image-manager-0.6.0/etc/schema.yaml`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/openstack_image_manager/manage.py` & `openstack-image-manager-0.6.0/openstack_image_manager/manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 import time
 import openstack
 import requests
 import yaml
 import os
 import re
 import sys
@@ -288,30 +290,40 @@
 
             try:
                 versions = dict()
                 for version in image["versions"]:
                     versions[str(version["version"])] = {"url": version["url"]}
 
                     if "mirror_url" in version:
-                        versions[version["version"]]["mirror_url"] = version["mirror_url"]
+                        versions[version["version"]]["mirror_url"] = version[
+                            "mirror_url"
+                        ]
 
                     if "visibility" in version:
-                        versions[version["version"]]["visibility"] = version["visibility"]
+                        versions[version["version"]]["visibility"] = version[
+                            "visibility"
+                        ]
 
                     if "os_version" in version:
-                        versions[version["version"]]["os_version"] = version["os_version"]
+                        versions[version["version"]]["os_version"] = version[
+                            "os_version"
+                        ]
 
                     if "hidden" in version:
                         versions[version["version"]]["hidden"] = version["hidden"]
 
-                    if version["version"] == "latest":#
+                    if version["version"] == "latest":  #
                         if "checksums_url" in version:
-                            versions[version["version"]]["checksums_url"] = version["checksums_url"]
+                            versions[version["version"]]["checksums_url"] = version[
+                                "checksums_url"
+                            ]
                         else:
-                            raise ValueError('Key "checksums_url" is required when using version "latest"')
+                            raise ValueError(
+                                'Key "checksums_url" is required when using version "latest"'
+                            )
 
                     if "meta" in version:
                         versions[version["version"]]["meta"] = version["meta"]
                     else:
                         versions[version["version"]]["meta"] = {}
 
                     if "url" in version:
@@ -319,15 +331,17 @@
                         # strip any directory path for file: urls in order to
                         # avoid exposing local filesystem details to other users
                         if url.startswith("file:") and "/" in url:
                             url = "file:%s" % url.rsplit("/", 1)[1]
                         versions[version["version"]]["meta"]["image_source"] = url
 
                     if "build_date" in version:
-                        versions[version["version"]]["meta"]["image_build_date"] = date.isoformat(version["build_date"])
+                        versions[version["version"]]["meta"][
+                            "image_build_date"
+                        ] = date.isoformat(version["build_date"])
 
                     if "id" in version:
                         versions[version["version"]]["id"] = version["id"]
             except ValueError as e:
                 logger.error(str(e))
                 continue
             except Exception as e:
@@ -384,22 +398,25 @@
 
         new_image = self.conn.image.create_image(**properties)
         parsed_url = urllib.parse.urlparse(url)
         if parsed_url.scheme == "file":
             local_file = open(parsed_url.path, "rb")
             with local_file:
                 try:
-                    logger.info("Uploading local file '%s' as image %s"
-                                % (parsed_url.path, name))
+                    logger.info(
+                        "Uploading local file '%s' as image %s"
+                        % (parsed_url.path, name)
+                    )
                     new_image.data = local_file
                     new_image.upload(self.conn.image)
                 except Exception as e:
                     self.conn.image.delete_image(new_image)
-                    logger.error("Failed to upload local file for image %s\n%s"
-                                 % (name, e))
+                    logger.error(
+                        "Failed to upload local file for image %s\n%s" % (name, e)
+                    )
                     self.exit_with_error = True
                     return None
         else:
             self.conn.image.import_image(new_image, method="web-download", uri=url)
 
         return self.wait_for_image(new_image)
 
@@ -462,15 +479,16 @@
                 # If an import fails (e.g. web-download task API disabled),
                 # it silently falls back to "queued" state asynchronously in
                 # the background. We need to catch such cases where an image is
                 # indefinitely stuck in "queued" state.
                 if imported_image.status == "queued":
                     if retry_attempts_for_queued_state < 0:
                         logger.error(
-                            "Image %s seems stuck in queued state" % image.name)
+                            "Image %s seems stuck in queued state" % image.name
+                        )
                         self.exit_with_error = True
                         return None
                     else:
                         retry_attempts_for_queued_state -= 1
                         logger.info("Waiting for image to leave queued state...")
                         time.sleep(2.0)
                 elif imported_image.status != "active":
@@ -620,18 +638,21 @@
                         self.exit_with_error = True
                         return existing_images, imported_image, previous_image
 
                 if image["multi"] and image["name"] in cloud_images:
                     previous_image = cloud_images[image["name"]]
 
                 if not self.CONF.dry_run:
-                    import_result = self.import_image(image, name, url, versions, version)
+                    import_result = self.import_image(
+                        image, name, url, versions, version
+                    )
                     if import_result:
                         logger.info(
-                            "Import of '%s' successfully completed, reloading images" % name
+                            "Import of '%s' successfully completed, reloading images"
+                            % name
                         )
                         cloud_images = self.get_images()
                         imported_image = cloud_images.get(name, None)
                 else:
                     logger.info(
                         f"Skipping required import of image '{name}', running in dry-run mode"
                     )
@@ -904,17 +925,15 @@
         """
         Check the age of the images in OpenStack and compare with the
         image definitions. Return a set of image names that are too old.
 
         Returns:
             set: A set of image names that are older than the max age.
         """
-        logger.info(
-            f"Checking for openstack images of age {str(self.CONF.max_age)}"
-        )
+        logger.info(f"Checking for openstack images of age {str(self.CONF.max_age)}")
 
         images = {}
         for d in self.read_image_files(return_all_images=True):
             images[d["name"]] = d
 
         cloud_images = self.get_images()
 
@@ -927,15 +946,17 @@
                 logger.warning(
                     f"No image definition found for '{image_name}', image will be ignored"
                 )
                 continue
 
             image_definition = images[image_name]
 
-            build_date_backend = date.fromisoformat(cloud_image.properties["image_build_date"])
+            build_date_backend = date.fromisoformat(
+                cloud_image.properties["image_build_date"]
+            )
 
             if image_definition["multi"]:
                 build_date_definition_candidates = [
                     x["build_date"] for x in image_definition["versions"]
                 ]
             else:
                 build_date_definition_candidates = []
@@ -1029,31 +1050,43 @@
 
             if self.CONF.keep and not image_definition["multi"]:
                 logger.info(
                     f"Image '{image}' will not be deleted, undefined versions of defined images are kept"
                 )
 
             elif uuid_validity == "none":
-                logger.info(f"Image '{image}' will not be deleted, UUID validity is 'none'")
+                logger.info(
+                    f"Image '{image}' will not be deleted, UUID validity is 'none'"
+                )
             elif counter[image_name] > last:
-                if self.CONF.delete and self.CONF.yes_i_really_know_what_i_do and not self.CONF.dry_run:
+                if (
+                    self.CONF.delete
+                    and self.CONF.yes_i_really_know_what_i_do
+                    and not self.CONF.dry_run
+                ):
                     try:
                         logger.info("Deactivating image '%s'" % image)
                         self.conn.image.deactivate_image(cloud_image.id)
 
                         logger.info("Setting visibility of '%s' to 'community'" % image)
                         self.conn.image.update_image(
                             cloud_image.id, visibility="community"
                         )
 
-                        if "keep" not in image_definition or not image_definition["keep"]:
+                        if (
+                            "keep" not in image_definition
+                            or not image_definition["keep"]
+                        ):
                             logger.info("Deleting %s" % image)
                             self.conn.image.delete_image(cloud_image.id)
                         else:
-                            logger.info("Image '%s' will not be deleted, because 'keep' flag is True" % image)
+                            logger.info(
+                                "Image '%s' will not be deleted, because 'keep' flag is True"
+                                % image
+                            )
                     except Exception as e:
                         logger.info(
                             "%s is still in use and cannot be deleted\n %s" % (image, e)
                         )
 
                 else:
                     logger.warning(
@@ -1070,15 +1103,17 @@
                             )
                             self.conn.image.update_image(
                                 cloud_image.id, visibility="community"
                             )
                     except Exception as e:
                         logger.error("An Exception occurred: \n%s" % e)
                         self.exit_with_error = True
-            elif counter[image_name] < last and self.CONF.hide and not self.CONF.dry_run:
+            elif (
+                counter[image_name] < last and self.CONF.hide and not self.CONF.dry_run
+            ):
                 logger.info("Setting visibility of '%s' to 'community'" % image)
                 self.conn.image.update_image(cloud_image.id, visibility="community")
         return unmanaged_images
 
     def validate_yaml_schema(self):
         """Validate all image.yaml files against the SCS Metadata spec"""
         schema = yamale.make_schema("etc/schema.yaml")
```

### Comparing `openstack-image-manager-0.5.1/openstack_image_manager/mirror.py` & `openstack-image-manager-0.6.0/openstack_image_manager/mirror.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# NOTE(berendt): quick & dirty (but it works for the moment)
+# SPDX-License-Identifier: Apache-2.0
 
 import logging
 import os
 import patoolib
 import requests
 import shutil
 import typer
@@ -45,81 +45,90 @@
     logging.basicConfig(
         format="%(asctime)s - %(message)s", level=level, datefmt="%Y-%m-%d %H:%M:%S"
     )
 
     onlyfiles = []
     for f in listdir(images):
         if isfile(join(images, f)):
+            logging.debug(f"Adding {f} to the list of files")
             onlyfiles.append(f)
 
     all_images = []
     for file in onlyfiles:
         with open(join(images, file)) as fp:
             data = yaml.load(fp, Loader=yaml.SafeLoader)
-            imgs = data.get("images")
-            for image in imgs:
+            for image in data.get("images"):
+                logging.debug(f"Adding {image['name']} to the list of images")
                 all_images.append(image)
 
     client = Minio(
         minio_server,
         access_key=minio_access_key,
         secret_key=minio_secret_key,
     )
 
+    result = client.bucket_exists(minio_bucket)
+    if not result:
+        logging.error(f"Create bucket '{minio_bucket}' first")
+
     for image in all_images:
+        if "versions" not in image:
+            continue
+
         for version in image["versions"]:
             if "source" not in version:
                 continue
+            else:
+                source = version["source"]
 
-            logging.debug("source: %s" % version["source"])
+            logging.debug(f"source: {source}")
 
-            path = urlparse(version["source"])
+            path = urlparse(source)
             url = urlparse(version["url"])
 
-            dirname = "%s/%s" % (image["shortname"], version["version"])
+            dirname = f"{image['shortname']}/{version['version']}"
             filename, fileextension = os.path.splitext(os.path.basename(path.path))
             _, fileextension2 = os.path.splitext(filename)
 
             if fileextension not in [".bz2", ".zip", ".xz", ".gz"]:
                 filename += fileextension
 
             if fileextension2 == ".tar":
                 filename = os.path.basename(url.path)
 
-            logging.debug("dirname: %s" % dirname)
-            logging.debug("filename: %s" % filename)
+            logging.debug(f"dirname: {dirname}")
+            logging.debug(f"filename: {filename}")
 
             try:
                 client.stat_object(minio_bucket, os.path.join(dirname, filename))
-                logging.info("'%s' available in '%s'" % (filename, dirname))
+                logging.info(f"'{filename}' available in '{dirname}'")
             except S3Error:
-                logging.info("'%s' not yet available in '%s'" % (filename, dirname))
+                logging.info(f"'{filename}' not yet available in '{dirname}'")
 
-                logging.info("Downloading '%s'" % version["source"])
+                logging.info(f"Downloading {version['source']}")
                 response = requests.get(
                     version["source"], stream=True, allow_redirects=True
                 )
                 with open(os.path.basename(path.path), "wb") as fp:
                     shutil.copyfileobj(response.raw, fp)
                 del response
 
                 if fileextension in [".bz2", ".zip", ".xz", ".gz"]:
-                    logging.info("Decompressing '%s'" % os.path.basename(path.path))
+                    logging.info(f"Decompressing '{os.path.basename(path.path)}'")
                     patoolib.extract_archive(os.path.basename(path.path), outdir=".")
                     os.remove(os.path.basename(path.path))
 
                 if not dry_run:
-                    logging.info("Uploading '%s' to '%s'" % (filename, dirname))
+                    logging.info(f"Uploading '{filename}' to '{dirname}'")
                     client.fput_object(
                         minio_bucket, os.path.join(dirname, filename), filename
                     )
                 else:
                     logging.info(
-                        "Not uploading '%s' to '%s' (dry-run enabled)"
-                        % (filename, dirname)
+                        f"Not uploading '{filename}' to '{dirname}' (dry-run enabled)"
                     )
 
                 os.remove(filename)
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `openstack-image-manager-0.5.1/openstack_image_manager/table.py` & `openstack-image-manager-0.6.0/openstack_image_manager/table.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# SPDX-License-Identifier: Apache-2.0
+
 import tabulate
 import typer
 import yaml
 
 from munch import Munch
 from os import listdir
 from os.path import isfile, join
```

### Comparing `openstack-image-manager-0.5.1/openstack_image_manager/update.py` & `openstack-image-manager-0.6.0/openstack_image_manager/update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# NOTE(berendt): quick & dirty (but it works for the moment)
+# SPDX-License-Identifier: Apache-2.0
+
 # source of latest URLs: https://gitlab.com/libosinfo/osinfo-db
 
 from datetime import datetime
 import os
 import re
 import shutil
 import sys
-import time
 from urllib.parse import urlparse
 from urllib.request import urlopen
 
 from loguru import logger
 from minio import Minio
 from minio.error import S3Error
 from natsort import natsorted
@@ -19,15 +19,17 @@
 import ruamel.yaml
 import typer
 
 app = typer.Typer()
 DEBUBU_REGEX = r'<a href="([^"]+)/">(?:release-)?([0-9]+)(\-[0-9]+)?/</a>'
 
 
-def get_latest_default(shortname, latest_checksum_url, latest_url, checksum_type="sha256"):
+def get_latest_default(
+    shortname, latest_checksum_url, latest_url, checksum_type="sha256"
+):
     result = requests.get(latest_checksum_url)
     result.raise_for_status()
 
     latest_filename = os.path.basename(urlparse(latest_url).path)
     filename_pattern = None
     if shortname in ["centos-stream-8", "centos-stream-9", "centos-7"]:
         filename_pattern = latest_filename.replace("HEREBE", "")
@@ -39,16 +41,18 @@
         if shortname in ["rocky-8", "rocky-9"]:
             if len(cs) == 4 and cs[0] == "SHA256":
                 checksums[latest_filename] = cs[3]
         elif shortname in ["centos-7"]:
             if len(cs) == 2 and re.search(filename_pattern, cs[1]):
                 checksums[cs[1]] = cs[0]
         elif shortname in ["centos-stream-8", "centos-stream-9"]:
-            if len(cs) == 4 and cs[0] == "SHA256" and re.search(
-                filename_pattern, cs[1][1:-1]
+            if (
+                len(cs) == 4
+                and cs[0] == "SHA256"
+                and re.search(filename_pattern, cs[1][1:-1])
             ):
                 checksums[cs[1][1:-1]] = cs[3]
         else:
             if len(cs) == 2:
                 checksums[cs[1]] = cs[0]
 
     if filename_pattern:
@@ -72,58 +76,67 @@
     return latest_folder, latest_date, latest_build
 
 
 def get_latest_debubu(shortname, latest_checksum_url, latest_url, checksum_type=None):
     base_url, _, filename = latest_url.rsplit("/", 2)
     latest_folder, latest_date, latest_build = resolve_debubu(base_url)
     current_base_url = f"{base_url}/{latest_folder}"
-    current_checksum_url = f"{current_base_url}/{latest_checksum_url.rsplit('/', 1)[-1]}"
+    current_checksum_url = (
+        f"{current_base_url}/{latest_checksum_url.rsplit('/', 1)[-1]}"
+    )
     result = requests.get(current_checksum_url)
     result.raise_for_status()
     current_checksum = None
     current_filename = filename
     if latest_build:  # Debian includes date-build in file name
-        fn_pre, fn_suf = filename.rsplit('.', 1)
+        fn_pre, fn_suf = filename.rsplit(".", 1)
         current_filename = f"{fn_pre}-{latest_date}{latest_build}.{fn_suf}"
     for line in result.text.splitlines():
         cs = line.split()
         if len(cs) != 2:
             continue
         if cs[1].startswith("*"):  # Ubuntu has the asterisk in front of the name
             cs[1] = cs[1][1:]
         if cs[1] != current_filename:
             continue
         if checksum_type is None:  # use heuristics to distinguish sha256/sha512
             checksum_type = "sha256" if len(cs[0]) == 64 else "sha512"
         current_checksum = f"{checksum_type}:{cs[0]}"
         break
     if current_checksum is None:
-        raise RuntimeError(f"{current_checksum_url} does not contain {current_filename}")
+        raise RuntimeError(
+            f"{current_checksum_url} does not contain {current_filename}"
+        )
     current_url = f"{current_base_url}/{current_filename}"
     return current_checksum, current_url, latest_date
 
 
 IMAGES = {
     "almalinux": get_latest_default,
     "centos": get_latest_default,
-    "debian": get_latest_debubu, 
-    "rockylinux": get_latest_default, 
+    "debian": get_latest_debubu,
+    "rockylinux": get_latest_default,
     "ubuntu": get_latest_debubu,
 }
 
 
 def mirror_image(
-    image, minio_server, minio_bucket, minio_access_key, minio_secret_key
+    image, latest_url, minio_server, minio_bucket, minio_access_key, minio_secret_key
 ):
     client = Minio(
         minio_server,
         access_key=minio_access_key,
         secret_key=minio_secret_key,
     )
 
+    result = client.bucket_exists(minio_bucket)
+    if not result:
+        logger.error(f"Create bucket '{minio_bucket}' first")
+        return
+
     version = image["versions"][0]
 
     path = urlparse(version["url"])
     dirname = image["shortname"]
     filename, fileextension = os.path.splitext(os.path.basename(path.path))
 
     if fileextension not in [".bz2", ".zip", ".xz", ".gz"]:
@@ -135,16 +148,17 @@
     new_filename = f"{new_version}-{shortname}.{format}"
 
     try:
         client.stat_object(minio_bucket, os.path.join(dirname, new_filename))
         logger.info("'%s' available in '%s'" % (new_filename, dirname))
     except S3Error:
         logger.info("'%s' not yet available in '%s'" % (new_filename, dirname))
-        logger.info("Downloading '%s'" % version["url"])
-        response = requests.get(version["url"], stream=True)
+        logger.info("Downloading '%s'" % latest_url)
+
+        response = requests.get(latest_url, stream=True)
         with open(os.path.basename(path.path), "wb") as fp:
             shutil.copyfileobj(response.raw, fp)
         del response
 
         if fileextension in [".bz2", ".zip", ".xz", ".gz"]:
             logger.info("Decompressing '%s'" % os.path.basename(path.path))
             patoolib.extract_archive(os.path.basename(path.path), outdir=".")
@@ -154,28 +168,41 @@
             "Uploading '%s' to '%s' as '%s'" % (filename, dirname, new_filename)
         )
 
         client.fput_object(minio_bucket, os.path.join(dirname, new_filename), filename)
         os.remove(filename)
 
 
-def update_image(image, getter, minio_server, minio_bucket, minio_access_key, minio_secret_key):
+def update_image(
+    image,
+    getter,
+    minio_server,
+    minio_bucket,
+    minio_access_key,
+    minio_secret_key,
+    dry_run=False,
+    swift_prefix="",
+):
     name = image["name"]
     logger.info(f"Checking image {name}")
 
     latest_url = image["latest_url"]
     logger.info(f"Latest download URL is {latest_url}")
 
     latest_checksum_url = image["latest_checksum_url"]
     logger.info(f"Getting checksums from {latest_checksum_url}")
-    
+
     shortname = image["shortname"]
-    current_checksum, current_url, current_version = getter(shortname, latest_checksum_url, latest_url)
+    current_checksum, current_url, current_version = getter(
+        shortname, latest_checksum_url, latest_url
+    )
 
-    logger.info(f"Checksum of current {current_url.rsplit('/', 1)[-1]} is {current_checksum}")
+    logger.info(
+        f"Checksum of current {current_url.rsplit('/', 1)[-1]} is {current_checksum}"
+    )
 
     if not image["versions"]:
         logger.info("No image available so far")
         image["versions"].append(
             {
                 "build_date": None,
                 "checksum": None,
@@ -210,41 +237,53 @@
     image["versions"][0].update(new_values)
 
     shortname = image["shortname"]
     format = image["format"]
 
     minio_server = str(minio_server)
     minio_bucket = str(minio_bucket)
-    new_url = f"https://{minio_server}/{minio_bucket}/{shortname}/{current_version}-{shortname}.{format}"
+    new_url = f"https://{minio_server}/{swift_prefix}{minio_bucket}/{shortname}/{current_version}-{shortname}.{format}"
     logger.info(f"New URL is {new_url}")
-    image["versions"][0]["mirror_url"] = new_url
+    image["versions"][0]["url"] = new_url
 
-    mirror_image(
-        image,
-        minio_server,
-        minio_bucket,
-        minio_access_key,
-        minio_secret_key,
-    )
+    if dry_run:
+        logger.info(f"Not mirroring {new_url}, dry-run enabled")
+    else:
+        mirror_image(
+            image,
+            current_url,
+            minio_server,
+            minio_bucket,
+            minio_access_key,
+            minio_secret_key,
+        )
     return 1
 
 
 @app.command()
 def main(
     debug: bool = typer.Option(False, "--debug", help="Enable debug logging"),
+    dry_run: bool = typer.Option(False, "--dry-run", help="Do not perform any changes"),
     minio_access_key: str = typer.Option(
         None, help="Minio access key", envvar="MINIO_ACCESS_KEY"
     ),
     minio_secret_key: str = typer.Option(
         None, help="Minio secret key", envvar="MINIO_SECRET_KEY"
     ),
     minio_server: str = typer.Option(
-        "swift.services.a.regiocloud.tech", help="Minio server"
+        "swift.services.a.regiocloud.tech", help="Minio server", envvar="MINIO_SERVER"
+    ),
+    minio_bucket: str = typer.Option(
+        "openstack-images", help="Minio bucket", envvar="MINIO_BUCKET"
+    ),
+    swift_prefix: str = typer.Option(
+        "swift/v1/AUTH_b182637428444b9aa302bb8d5a5a418c/",
+        help="Swift prefix",
+        envvar="SWIFT_PREFIX",
     ),
-    minio_bucket: str = typer.Option("openstack-images", help="Minio bucket"),
 ):
 
     if debug:
         level = "DEBUG"
     else:
         level = "INFO"
 
@@ -253,34 +292,39 @@
         "<green>{time:YYYY-MM-DD HH:mm:ss}</green> | <level>{level: <8}</level> | "
         "<cyan>{function}</cyan>:<cyan>{line}</cyan> - <level>{message}</level>"
     )
     logger.add(sys.stderr, format=log_fmt, level=level, colorize=True)
 
     for image, getter in IMAGES.items():
         p = f"etc/images/{image}.yml"
+        logger.info(f"Processing file {p}")
 
         ryaml = ruamel.yaml.YAML()
         with open(p) as fp:
             data = ryaml.load(fp)
 
         updates = 0
         for index, image in enumerate(data["images"]):
             if "latest_url" not in image:
                 continue
+
             updates += update_image(
                 image,
                 getter,
                 minio_server,
                 minio_bucket,
                 minio_access_key,
                 minio_secret_key,
+                dry_run,
+                swift_prefix,
             )
 
         if not updates:
             continue
+
         with open(p, "w+") as fp:
             ryaml.explicit_start = True
             ryaml.indent(sequence=4, offset=2)
             ryaml.dump(data, fp)
 
 
 if __name__ == "__main__":
```

### Comparing `openstack-image-manager-0.5.1/openstack_image_manager.egg-info/PKG-INFO` & `openstack-image-manager-0.6.0/openstack_image_manager.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openstack-image-manager
-Version: 0.5.1
+Version: 0.6.0
 Summary: OpenStack image manager
 Author-email: OSISM community <info@osism.tech>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -219,27 +219,27 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: loguru==0.7.2
-Requires-Dist: minio==7.1.16
+Requires-Dist: minio==7.1.17
 Requires-Dist: munch==4.0.0
 Requires-Dist: natsort==8.4.0
-Requires-Dist: openstacksdk==1.5.0
+Requires-Dist: openstacksdk==2.0.0
 Requires-Dist: paramiko==3.3.1
 Requires-Dist: patool==1.12
 Requires-Dist: requests==2.31.0
-Requires-Dist: ruamel.yaml==0.17.32
+Requires-Dist: ruamel.yaml==0.18.1
 Requires-Dist: tabulate==0.9.0
 Requires-Dist: typer[all]==0.9.0
 Requires-Dist: yamale==4.0.4
 
 # openstack-image-manager
 
 [![PyPi version](https://badgen.net/pypi/v/openstack-image-manager/)](https://pypi.org/project/openstack-image-manager/)
 [![PyPi license](https://badgen.net/pypi/license/openstack-image-manager/)](https://pypi.org/project/openstack-image-manager/)
 
 Easily manage and keep up to date a large number of images on an OpenStack environment
 
-Documentation: <https://docs.scs.community/docs/category/openstack-image-manager/>
+Documentation: <https://osism.github.io/docs/guides/operations-guide/openstack/image-manager>
```

### Comparing `openstack-image-manager-0.5.1/openstack_image_manager.egg-info/SOURCES.txt` & `openstack-image-manager-0.6.0/openstack_image_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openstack-image-manager-0.5.1/pyproject.toml` & `openstack-image-manager-0.6.0/pyproject.toml`

 * *Files identical despite different names*

