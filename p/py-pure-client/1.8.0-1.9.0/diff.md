# Comparing `tmp/py-pure-client-1.8.0.tar.gz` & `tmp/py-pure-client-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-pure-client-1.8.0.tar", last modified: Mon Sep 28 18:31:09 2020, max compression
+gzip compressed data, was "dist/py-pure-client-1.9.0.tar", last modified: Thu Oct 22 23:31:21 2020, max compression
```

## Comparing `py-pure-client-1.8.0.tar` & `py-pure-client-1.9.0.tar`

### file list

```diff
@@ -1,1308 +1,1311 @@
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:09.125295 py-pure-client-1.8.0/
--rw-r--r--   0 yxu        (502) staff       (20)     1871 2020-09-28 18:31:09.114207 py-pure-client-1.8.0/PKG-INFO
--rw-r--r--   0 yxu        (502) staff       (20)     1032 2020-09-28 17:43:20.000000 py-pure-client-1.8.0/README.md
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:52.590819 py-pure-client-1.8.0/py_pure_client.egg-info/
--rw-r--r--   0 yxu        (502) staff       (20)     1871 2020-09-28 18:30:51.000000 py-pure-client-1.8.0/py_pure_client.egg-info/PKG-INFO
--rw-r--r--   0 yxu        (502) staff       (20)    76573 2020-09-28 18:30:52.000000 py-pure-client-1.8.0/py_pure_client.egg-info/SOURCES.txt
--rw-r--r--   0 yxu        (502) staff       (20)        1 2020-09-28 18:30:51.000000 py-pure-client-1.8.0/py_pure_client.egg-info/dependency_links.txt
--rw-r--r--   0 yxu        (502) staff       (20)      111 2020-09-28 18:30:51.000000 py-pure-client-1.8.0/py_pure_client.egg-info/requires.txt
--rw-r--r--   0 yxu        (502) staff       (20)       13 2020-09-28 18:30:51.000000 py-pure-client-1.8.0/py_pure_client.egg-info/top_level.txt
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:52.693894 py-pure-client-1.8.0/pypureclient/
--rw-r--r--   0 yxu        (502) staff       (20)      200 2020-09-24 18:29:11.000000 py-pure-client-1.8.0/pypureclient/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     2073 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/api_token_manager.py
--rw-r--r--   0 yxu        (502) staff       (20)      276 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/exceptions.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:52.723775 py-pure-client-1.8.0/pypureclient/flasharray/
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:52.782371 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/
--rw-r--r--   0 yxu        (502) staff       (20)     3768 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/__init__.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:52.871858 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/
--rw-r--r--   0 yxu        (502) staff       (20)      328 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)    14706 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/authorization_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    21406 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/connections_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    40358 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/host_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    40650 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/hosts_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    32502 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/volume_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    57311 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/volumes_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    24491 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api_client.py
--rw-r--r--   0 yxu        (502) staff       (20)   141512 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/client.py
--rw-r--r--   0 yxu        (502) staff       (20)     7677 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/configuration.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:54.031689 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/
--rw-r--r--   0 yxu        (502) staff       (20)     4537 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     3153 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/api_version_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3352 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/built_in.py
--rw-r--r--   0 yxu        (502) staff       (20)     4154 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/chap.py
--rw-r--r--   0 yxu        (502) staff       (20)     5563 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/connection.py
--rw-r--r--   0 yxu        (502) staff       (20)     4202 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/connection_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4664 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/connection_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3287 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/connection_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3534 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/destroyed_patch_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3349 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/fixed_reference.py
--rw-r--r--   0 yxu        (502) staff       (20)     3153 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/fixed_reference_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     6860 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host.py
--rw-r--r--   0 yxu        (502) staff       (20)     4160 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4261 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     4141 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3092 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19335 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19612 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     3226 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7782 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19315 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19592 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     3549 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_port_connectivity.py
--rw-r--r--   0 yxu        (502) staff       (20)     5382 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3245 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/inline_response400.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/inline_response401.py
--rw-r--r--   0 yxu        (502) staff       (20)     3262 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/member.py
--rw-r--r--   0 yxu        (502) staff       (20)     3430 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all.py
--rw-r--r--   0 yxu        (502) staff       (20)     4169 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3254 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3064 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/new_name.py
--rw-r--r--   0 yxu        (502) staff       (20)     4342 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/oauth_token_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3779 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/page_info.py
--rw-r--r--   0 yxu        (502) staff       (20)    18814 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     4245 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/qos.py
--rw-r--r--   0 yxu        (502) staff       (20)     3329 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/reference.py
--rw-r--r--   0 yxu        (502) staff       (20)     3133 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/reference_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     3361 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource.py
--rw-r--r--   0 yxu        (502) staff       (20)     3128 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)    19331 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19608 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4690 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_by_array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4598 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    19098 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)    19375 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4730 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_by_array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4638 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3857 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     4622 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_space_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5869 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     8620 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/space.py
--rw-r--r--   0 yxu        (502) staff       (20)     4703 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/username.py
--rw-r--r--   0 yxu        (502) staff       (20)     3116 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/username_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7705 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume.py
--rw-r--r--   0 yxu        (502) staff       (20)     6702 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_common.py
--rw-r--r--   0 yxu        (502) staff       (20)     4552 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4887 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19323 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19600 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4667 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3259 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7257 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     4632 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3730 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     4009 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3315 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5244 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     4712 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3371 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3849 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_space.py
--rw-r--r--   0 yxu        (502) staff       (20)    13088 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/rest.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:54.107850 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/
--rw-r--r--   0 yxu        (502) staff       (20)     7691 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/__init__.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:54.365144 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/
--rw-r--r--   0 yxu        (502) staff       (20)      875 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)    20392 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/api_clients_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    14706 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/authorization_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    22009 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/connections_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    75517 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/host_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    75649 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/hosts_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    15870 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/offloads_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    76932 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/pods_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    30197 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/protection_group_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)   126965 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/protection_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7987 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/remote_pods_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    26280 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/remote_protection_group_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    18457 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/remote_protection_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    18899 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/remote_volume_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    54326 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/volume_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    33102 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/volume_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    84705 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/volumes_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    24491 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api_client.py
--rw-r--r--   0 yxu        (502) staff       (20)   474676 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/client.py
--rw-r--r--   0 yxu        (502) staff       (20)     7679 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/configuration.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:56.851111 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/
--rw-r--r--   0 yxu        (502) staff       (20)     9408 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     3483 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/aggregate_replication_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     6448 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_client.py
--rw-r--r--   0 yxu        (502) staff       (20)     4901 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_client_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3223 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_client_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     5443 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_client_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3226 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_client_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3153 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_version_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3352 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/built_in.py
--rw-r--r--   0 yxu        (502) staff       (20)     3151 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/built_in_resource_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     4154 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/chap.py
--rw-r--r--   0 yxu        (502) staff       (20)     5364 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/connection.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/connection_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4664 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/connection_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/connection_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3534 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/destroyed_patch_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3349 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/fixed_reference.py
--rw-r--r--   0 yxu        (502) staff       (20)     3153 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/fixed_reference_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     7232 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host.py
--rw-r--r--   0 yxu        (502) staff       (20)     4866 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4261 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     4901 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3092 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19335 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19612 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     3226 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3522 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     7782 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19315 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19592 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     3549 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_port_connectivity.py
--rw-r--r--   0 yxu        (502) staff       (20)     5382 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3191 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3502 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/inline_response400.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/inline_response401.py
--rw-r--r--   0 yxu        (502) staff       (20)     3262 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member.py
--rw-r--r--   0 yxu        (502) staff       (20)     4934 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3430 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all.py
--rw-r--r--   0 yxu        (502) staff       (20)     4929 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3254 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_no_id_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     3259 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3064 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/new_name.py
--rw-r--r--   0 yxu        (502) staff       (20)     4342 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/oauth_token_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5861 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload.py
--rw-r--r--   0 yxu        (502) staff       (20)     4175 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_azure.py
--rw-r--r--   0 yxu        (502) staff       (20)     5268 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4257 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_nfs.py
--rw-r--r--   0 yxu        (502) staff       (20)     3543 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3212 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6121 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_s3.py
--rw-r--r--   0 yxu        (502) staff       (20)     4539 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/page_info.py
--rw-r--r--   0 yxu        (502) staff       (20)    18814 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     7362 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod.py
--rw-r--r--   0 yxu        (502) staff       (20)     7481 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_array_status.py
--rw-r--r--   0 yxu        (502) staff       (20)     5228 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5355 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19311 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19588 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4466 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3184 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     8632 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     7747 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     5402 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3955 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     4425 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4986 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_array_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4433 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4954 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3322 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5991 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     5428 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5624 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     5798 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3324 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5387 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5508 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3380 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3546 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3861 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_target.py
--rw-r--r--   0 yxu        (502) staff       (20)     4985 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_target_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_target_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4245 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/qos.py
--rw-r--r--   0 yxu        (502) staff       (20)     3329 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/reference.py
--rw-r--r--   0 yxu        (502) staff       (20)     3133 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/reference_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     3581 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_pod.py
--rw-r--r--   0 yxu        (502) staff       (20)     4893 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_pods_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5722 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     4985 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5472 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     5041 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3366 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5411 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5465 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3319 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6402 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     4875 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3200 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5624 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5375 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3256 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4175 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/replication_schedule.py
--rw-r--r--   0 yxu        (502) staff       (20)     3361 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource.py
--rw-r--r--   0 yxu        (502) staff       (20)     3128 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)    19331 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19608 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     5450 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_by_array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5358 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    19098 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)    19375 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     5490 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_by_array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5398 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3857 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     5382 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_space_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3534 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_space_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     4854 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_space_no_id_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3707 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/retention_policy.py
--rw-r--r--   0 yxu        (502) staff       (20)     5869 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     3834 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/snapshot_schedule.py
--rw-r--r--   0 yxu        (502) staff       (20)     8620 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3773 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/target_protection_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     3951 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/target_protection_group_post_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3494 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/time_window.py
--rw-r--r--   0 yxu        (502) staff       (20)     5059 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/username.py
--rw-r--r--   0 yxu        (502) staff       (20)     3116 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/username_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7705 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume.py
--rw-r--r--   0 yxu        (502) staff       (20)     6702 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_common.py
--rw-r--r--   0 yxu        (502) staff       (20)     5312 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5114 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     5205 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    19343 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     4850 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3137 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3869 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     4887 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19323 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19600 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4667 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3259 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7257 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     5392 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3730 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     4009 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3315 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5600 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5472 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3371 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3849 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_space.py
--rw-r--r--   0 yxu        (502) staff       (20)    13088 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/rest.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:56.927967 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/
--rw-r--r--   0 yxu        (502) staff       (20)    12907 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/__init__.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:30:57.450563 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/
--rw-r--r--   0 yxu        (502) staff       (20)     1540 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)    58610 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/administrators_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    20753 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/alerts_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    20392 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/api_clients_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    18819 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/apps_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    42836 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/arrays_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     8049 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/audits_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    14706 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/authorization_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    22035 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/connections_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7737 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/controllers_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    31766 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/directory_services_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    10127 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/dns_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    11156 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/hardware_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    75510 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/host_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    75642 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/hosts_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    22891 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/kmip_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    15865 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/maintenance_windows_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    15864 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/offloads_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    63516 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/pod_replica_links_api.py
--rw-r--r--   0 yxu        (502) staff       (20)   101781 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/pods_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    14048 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/ports_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    30174 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/protection_group_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)   126965 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/protection_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7987 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/remote_pods_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    26280 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/remote_protection_group_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    18457 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/remote_protection_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    18899 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/remote_volume_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    10154 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/smi_s_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    32959 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/software_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    19422 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/subnets_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    17289 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/support_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    54326 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/volume_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    50371 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/volume_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)   101901 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/volumes_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    24491 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api_client.py
--rw-r--r--   0 yxu        (502) staff       (20)   763246 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/client.py
--rw-r--r--   0 yxu        (502) staff       (20)     7679 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/configuration.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:01.477095 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/
--rw-r--r--   0 yxu        (502) staff       (20)    16731 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     5100 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin.py
--rw-r--r--   0 yxu        (502) staff       (20)     3357 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_api_token.py
--rw-r--r--   0 yxu        (502) staff       (20)     4826 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_api_token_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3151 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_api_token_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3591 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_cache.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_cache_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_cache_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4770 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5367 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3296 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3117 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_role.py
--rw-r--r--   0 yxu        (502) staff       (20)     5080 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_settings.py
--rw-r--r--   0 yxu        (502) staff       (20)     3151 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_settings_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3483 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/aggregate_replication_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     7730 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert.py
--rw-r--r--   0 yxu        (502) staff       (20)     6208 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert_event.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert_event_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert_event_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4770 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6448 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_client.py
--rw-r--r--   0 yxu        (502) staff       (20)     4901 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_client_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3223 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_client_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     5443 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_client_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3226 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_client_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3568 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_token.py
--rw-r--r--   0 yxu        (502) staff       (20)     3153 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_version_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4864 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app.py
--rw-r--r--   0 yxu        (502) staff       (20)     4756 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4051 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app_node.py
--rw-r--r--   0 yxu        (502) staff       (20)     4784 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app_node_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3109 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app_node_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5865 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4773 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    21752 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     4847 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_performance_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3098 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4242 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_space_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5869 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/arrays.py
--rw-r--r--   0 yxu        (502) staff       (20)     5197 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/audit.py
--rw-r--r--   0 yxu        (502) staff       (20)     4770 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/audit_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/audit_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3352 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/built_in.py
--rw-r--r--   0 yxu        (502) staff       (20)     3124 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/built_in_relationship.py
--rw-r--r--   0 yxu        (502) staff       (20)     3151 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/built_in_resource_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     4154 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/chap.py
--rw-r--r--   0 yxu        (502) staff       (20)     5364 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/connection.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/connection_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4664 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/connection_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/connection_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4219 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/controller.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/controller_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4223 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/controllers.py
--rw-r--r--   0 yxu        (502) staff       (20)     3534 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/destroyed_patch_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     5851 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service.py
--rw-r--r--   0 yxu        (502) staff       (20)     4847 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3987 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_management.py
--rw-r--r--   0 yxu        (502) staff       (20)     3172 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3779 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_role.py
--rw-r--r--   0 yxu        (502) staff       (20)     4875 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_role_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3200 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_role_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3376 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/dns.py
--rw-r--r--   0 yxu        (502) staff       (20)     4756 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/dns_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3396 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/dns_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/dns_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3323 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/eula.py
--rw-r--r--   0 yxu        (502) staff       (20)     4763 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/eula_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3088 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/eula_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3828 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/eula_signature.py
--rw-r--r--   0 yxu        (502) staff       (20)     3167 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/fixed_name_resource_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     3349 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/fixed_reference.py
--rw-r--r--   0 yxu        (502) staff       (20)     3153 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/fixed_reference_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     5924 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/hardware.py
--rw-r--r--   0 yxu        (502) staff       (20)     4791 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/hardware_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3700 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/hardware_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3116 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/hardware_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7232 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host.py
--rw-r--r--   0 yxu        (502) staff       (20)     4866 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4261 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     4901 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3092 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19335 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19612 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     3226 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3522 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     7782 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19315 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19592 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     3549 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_port_connectivity.py
--rw-r--r--   0 yxu        (502) staff       (20)     5382 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3191 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3502 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/inline_response400.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/inline_response401.py
--rw-r--r--   0 yxu        (502) staff       (20)     4147 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip.py
--rw-r--r--   0 yxu        (502) staff       (20)     4763 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3936 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3932 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3088 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5046 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_test_result.py
--rw-r--r--   0 yxu        (502) staff       (20)     4833 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_test_result_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3680 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/maintenance_window.py
--rw-r--r--   0 yxu        (502) staff       (20)     3495 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/maintenance_window_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     4858 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/maintenance_windows_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3183 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/maintenance_windows_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3262 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member.py
--rw-r--r--   0 yxu        (502) staff       (20)     4934 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3430 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all.py
--rw-r--r--   0 yxu        (502) staff       (20)     4929 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3254 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_no_id_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     3259 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3064 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/new_name.py
--rw-r--r--   0 yxu        (502) staff       (20)     4342 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/oauth_token_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5133 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload.py
--rw-r--r--   0 yxu        (502) staff       (20)     4175 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_azure.py
--rw-r--r--   0 yxu        (502) staff       (20)     5165 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4559 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_google_cloud.py
--rw-r--r--   0 yxu        (502) staff       (20)     4257 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_nfs.py
--rw-r--r--   0 yxu        (502) staff       (20)     3816 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3109 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6121 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_s3.py
--rw-r--r--   0 yxu        (502) staff       (20)     4933 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/override_check.py
--rw-r--r--   0 yxu        (502) staff       (20)     4539 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/page_info.py
--rw-r--r--   0 yxu        (502) staff       (20)    18814 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     9871 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod.py
--rw-r--r--   0 yxu        (502) staff       (20)     7481 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_array_status.py
--rw-r--r--   0 yxu        (502) staff       (20)     5112 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6509 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19311 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19588 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     5842 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication.py
--rw-r--r--   0 yxu        (502) staff       (20)     6089 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     5469 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3794 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5380 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3705 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4466 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     5620 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link.py
--rw-r--r--   0 yxu        (502) staff       (20)     4870 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5452 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag.py
--rw-r--r--   0 yxu        (502) staff       (20)     4895 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3220 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3312 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     6196 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     6240 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication.py
--rw-r--r--   0 yxu        (502) staff       (20)     5504 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3829 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3195 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     9277 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     4267 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/port.py
--rw-r--r--   0 yxu        (502) staff       (20)     3767 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/port_common.py
--rw-r--r--   0 yxu        (502) staff       (20)     4763 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/port_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/port_initiator.py
--rw-r--r--   0 yxu        (502) staff       (20)     4830 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/port_initiators_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7747 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     5402 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3955 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     4425 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4986 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_array_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4433 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4954 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3322 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5991 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     5428 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5624 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     5798 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3324 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5387 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5508 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3380 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3546 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3861 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_target.py
--rw-r--r--   0 yxu        (502) staff       (20)     4985 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_target_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_target_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4245 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/qos.py
--rw-r--r--   0 yxu        (502) staff       (20)     3329 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/reference.py
--rw-r--r--   0 yxu        (502) staff       (20)     3133 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/reference_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     3581 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_pod.py
--rw-r--r--   0 yxu        (502) staff       (20)     4893 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_pods_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5722 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     4985 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5472 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     5041 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3366 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5411 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5465 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3319 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6402 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     4875 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3200 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5624 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5375 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3256 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3756 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/replica_link_lag.py
--rw-r--r--   0 yxu        (502) staff       (20)     6024 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/replica_link_performance_replication.py
--rw-r--r--   0 yxu        (502) staff       (20)     4911 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/replication_performance_with_total.py
--rw-r--r--   0 yxu        (502) staff       (20)     4175 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/replication_schedule.py
--rw-r--r--   0 yxu        (502) staff       (20)     3361 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource.py
--rw-r--r--   0 yxu        (502) staff       (20)     3372 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_fixed_non_unique_name.py
--rw-r--r--   0 yxu        (502) staff       (20)     3128 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)    19331 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19608 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     5450 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_by_array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5358 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    19098 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)    19375 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     5490 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_by_array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5398 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3878 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_pod_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     5400 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_pod_space_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3857 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     5382 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_space_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3534 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_space_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     4854 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_space_no_id_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3707 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/retention_policy.py
--rw-r--r--   0 yxu        (502) staff       (20)     3531 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/smis.py
--rw-r--r--   0 yxu        (502) staff       (20)     4763 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/smis_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3088 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/smis_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5869 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     3834 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/snapshot_schedule.py
--rw-r--r--   0 yxu        (502) staff       (20)     6252 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software.py
--rw-r--r--   0 yxu        (502) staff       (20)     4791 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6323 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation.py
--rw-r--r--   0 yxu        (502) staff       (20)     3346 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3948 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     5629 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_step.py
--rw-r--r--   0 yxu        (502) staff       (20)     5633 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps.py
--rw-r--r--   0 yxu        (502) staff       (20)     4212 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_checks.py
--rw-r--r--   0 yxu        (502) staff       (20)     4907 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3232 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6327 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installations.py
--rw-r--r--   0 yxu        (502) staff       (20)     4879 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installations_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3204 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installations_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3116 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     8620 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3390 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/start_end_time.py
--rw-r--r--   0 yxu        (502) staff       (20)     5425 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/subnet.py
--rw-r--r--   0 yxu        (502) staff       (20)     4777 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/subnet_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4820 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/subnet_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     4580 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/subnet_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/subnet_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5569 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/support.py
--rw-r--r--   0 yxu        (502) staff       (20)     4784 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/support_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4052 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/support_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3579 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/support_remote_assist_paths.py
--rw-r--r--   0 yxu        (502) staff       (20)     3109 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/support_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4418 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/tag.py
--rw-r--r--   0 yxu        (502) staff       (20)     4756 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/tag_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/tag_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3773 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/target_protection_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     3951 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/target_protection_group_post_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     5549 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/test_result.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/test_result_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/test_result_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5882 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/test_result_with_resource.py
--rw-r--r--   0 yxu        (502) staff       (20)     4877 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/test_result_with_resource_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3494 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/time_window.py
--rw-r--r--   0 yxu        (502) staff       (20)     5059 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/username.py
--rw-r--r--   0 yxu        (502) staff       (20)     3116 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/username_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     8928 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume.py
--rw-r--r--   0 yxu        (502) staff       (20)     6702 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_common.py
--rw-r--r--   0 yxu        (502) staff       (20)     5297 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5114 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     5205 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    19343 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     4850 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3137 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3869 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     5500 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19323 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19600 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4667 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3257 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7257 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     5392 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3730 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     4009 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3315 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5600 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5472 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3371 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3849 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_space.py
--rw-r--r--   0 yxu        (502) staff       (20)    13088 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/rest.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:01.542027 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/
--rw-r--r--   0 yxu        (502) staff       (20)    16195 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/__init__.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:02.024057 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/
--rw-r--r--   0 yxu        (502) staff       (20)     1834 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)    16246 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/active_directory_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    58610 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/administrators_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    20753 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/alerts_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    20392 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/api_clients_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    18819 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/apps_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    42836 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/arrays_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     8049 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/audits_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    14706 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/authorization_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    22035 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/connections_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7737 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/controllers_api.py
--rw-r--r--   0 yxu        (502) staff       (20)   117857 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/directories_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    21387 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/directory_exports_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    31766 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/directory_services_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    24127 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/directory_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    10127 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/dns_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    21311 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/file_systems_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    11156 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/hardware_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    75510 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/host_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    75642 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/hosts_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    22891 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/kmip_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    15865 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/maintenance_windows_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    15864 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/offloads_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    63516 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/pod_replica_links_api.py
--rw-r--r--   0 yxu        (502) staff       (20)   100471 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/pods_api.py
--rw-r--r--   0 yxu        (502) staff       (20)   196023 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/policies_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    14048 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/ports_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    30174 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/protection_group_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)   126965 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/protection_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7987 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/remote_pods_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    26280 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/remote_protection_group_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    18457 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/remote_protection_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    18899 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/remote_volume_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    10154 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/smi_s_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    32959 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/software_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    19422 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/subnets_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    17289 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/support_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    55148 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/volume_groups_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    51428 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/volume_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)   102940 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/volumes_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    24491 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api_client.py
--rw-r--r--   0 yxu        (502) staff       (20)  1022486 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/client.py
--rw-r--r--   0 yxu        (502) staff       (20)     7679 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/configuration.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:05.658642 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/
--rw-r--r--   0 yxu        (502) staff       (20)    20328 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     4876 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/active_directory.py
--rw-r--r--   0 yxu        (502) staff       (20)     4908 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/active_directory_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5442 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/active_directory_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3233 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/active_directory_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5100 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin.py
--rw-r--r--   0 yxu        (502) staff       (20)     3357 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_api_token.py
--rw-r--r--   0 yxu        (502) staff       (20)     4826 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_api_token_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3151 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_api_token_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3591 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_cache.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_cache_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_cache_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4770 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5367 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3296 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3117 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_role.py
--rw-r--r--   0 yxu        (502) staff       (20)     5080 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_settings.py
--rw-r--r--   0 yxu        (502) staff       (20)     3151 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_settings_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3483 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/aggregate_replication_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     7730 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert.py
--rw-r--r--   0 yxu        (502) staff       (20)     6208 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert_event.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert_event_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert_event_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4770 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6448 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_client.py
--rw-r--r--   0 yxu        (502) staff       (20)     4901 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_client_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3223 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_client_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     5443 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_client_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3226 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_client_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3568 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_token.py
--rw-r--r--   0 yxu        (502) staff       (20)     3153 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_version_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4864 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app.py
--rw-r--r--   0 yxu        (502) staff       (20)     4756 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4051 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app_node.py
--rw-r--r--   0 yxu        (502) staff       (20)     4784 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app_node_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3109 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app_node_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5865 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4773 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    21752 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     4847 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_performance_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3098 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4242 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_space_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5869 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/arrays.py
--rw-r--r--   0 yxu        (502) staff       (20)     5197 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/audit.py
--rw-r--r--   0 yxu        (502) staff       (20)     4770 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/audit_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/audit_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3352 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/built_in.py
--rw-r--r--   0 yxu        (502) staff       (20)     3124 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/built_in_relationship.py
--rw-r--r--   0 yxu        (502) staff       (20)     3151 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/built_in_resource_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     4154 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/chap.py
--rw-r--r--   0 yxu        (502) staff       (20)     5364 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/connection.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/connection_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4664 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/connection_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/connection_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4219 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/controller.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/controller_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4223 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/controllers.py
--rw-r--r--   0 yxu        (502) staff       (20)     3534 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/destroyed_patch_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     5767 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory.py
--rw-r--r--   0 yxu        (502) staff       (20)     4674 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_export.py
--rw-r--r--   0 yxu        (502) staff       (20)     4941 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_export_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3225 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_export_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3266 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_export_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5273 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3092 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     9599 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     5359 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_performance_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3401 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_policy_export_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3349 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_policy_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3703 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3224 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5851 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service.py
--rw-r--r--   0 yxu        (502) staff       (20)     4847 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3987 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_management.py
--rw-r--r--   0 yxu        (502) staff       (20)     3172 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3779 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_role.py
--rw-r--r--   0 yxu        (502) staff       (20)     4875 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_role_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3200 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_role_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6848 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     5353 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4222 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3696 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3280 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3861 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3536 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directorypolicyexportpost_policies.py
--rw-r--r--   0 yxu        (502) staff       (20)     3204 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directorypolicypost_policies.py
--rw-r--r--   0 yxu        (502) staff       (20)     3376 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/dns.py
--rw-r--r--   0 yxu        (502) staff       (20)     4756 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/dns_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3396 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/dns_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/dns_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3323 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/eula.py
--rw-r--r--   0 yxu        (502) staff       (20)     4763 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/eula_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3088 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/eula_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3828 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/eula_signature.py
--rw-r--r--   0 yxu        (502) staff       (20)     4759 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/file_system.py
--rw-r--r--   0 yxu        (502) staff       (20)     4906 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/file_system_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3714 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/file_system_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3231 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/file_system_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3167 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/fixed_name_resource_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     3349 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/fixed_reference.py
--rw-r--r--   0 yxu        (502) staff       (20)     3153 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/fixed_reference_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     3894 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/fixed_reference_with_type.py
--rw-r--r--   0 yxu        (502) staff       (20)     5924 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/hardware.py
--rw-r--r--   0 yxu        (502) staff       (20)     4791 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/hardware_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3700 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/hardware_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3116 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/hardware_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7232 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host.py
--rw-r--r--   0 yxu        (502) staff       (20)     4866 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4261 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     4901 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3092 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19335 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19612 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     3226 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3522 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     7782 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19315 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19592 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     3549 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_port_connectivity.py
--rw-r--r--   0 yxu        (502) staff       (20)     5382 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3191 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3502 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/inline_response400.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/inline_response401.py
--rw-r--r--   0 yxu        (502) staff       (20)     4147 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip.py
--rw-r--r--   0 yxu        (502) staff       (20)     4763 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3936 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3932 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3088 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5046 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_test_result.py
--rw-r--r--   0 yxu        (502) staff       (20)     4833 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_test_result_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3680 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/maintenance_window.py
--rw-r--r--   0 yxu        (502) staff       (20)     3495 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/maintenance_window_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     4858 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/maintenance_windows_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3183 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/maintenance_windows_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3262 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member.py
--rw-r--r--   0 yxu        (502) staff       (20)     4934 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3430 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all.py
--rw-r--r--   0 yxu        (502) staff       (20)     4929 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3254 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_no_id_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     3259 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3064 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/new_name.py
--rw-r--r--   0 yxu        (502) staff       (20)     4342 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/oauth_token_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5133 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload.py
--rw-r--r--   0 yxu        (502) staff       (20)     4175 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_azure.py
--rw-r--r--   0 yxu        (502) staff       (20)     5165 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4559 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_google_cloud.py
--rw-r--r--   0 yxu        (502) staff       (20)     4257 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_nfs.py
--rw-r--r--   0 yxu        (502) staff       (20)     3816 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3109 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6121 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_s3.py
--rw-r--r--   0 yxu        (502) staff       (20)     4933 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/override_check.py
--rw-r--r--   0 yxu        (502) staff       (20)     4539 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/page_info.py
--rw-r--r--   0 yxu        (502) staff       (20)    18814 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    10133 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod.py
--rw-r--r--   0 yxu        (502) staff       (20)     7481 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_array_status.py
--rw-r--r--   0 yxu        (502) staff       (20)     5112 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6509 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19311 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19588 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     5842 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication.py
--rw-r--r--   0 yxu        (502) staff       (20)     6089 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     5469 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3794 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5380 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3705 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4466 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     5620 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link.py
--rw-r--r--   0 yxu        (502) staff       (20)     4870 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5452 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag.py
--rw-r--r--   0 yxu        (502) staff       (20)     4895 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3220 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3312 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     6196 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     6240 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication.py
--rw-r--r--   0 yxu        (502) staff       (20)     5504 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3829 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3195 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     9277 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3877 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy.py
--rw-r--r--   0 yxu        (502) staff       (20)     4878 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3954 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member.py
--rw-r--r--   0 yxu        (502) staff       (20)     4238 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_export.py
--rw-r--r--   0 yxu        (502) staff       (20)     4962 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3285 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3287 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4920 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3234 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3245 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3346 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3150 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3203 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4443 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client.py
--rw-r--r--   0 yxu        (502) staff       (20)     4969 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3243 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3294 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4621 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client.py
--rw-r--r--   0 yxu        (502) staff       (20)     4971 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3243 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3296 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5426 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     4964 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3241 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3289 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3692 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policymemberexportpost_members.py
--rw-r--r--   0 yxu        (502) staff       (20)     3360 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policymemberpost_members.py
--rw-r--r--   0 yxu        (502) staff       (20)     3943 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policyrulenfsclientpost_rules.py
--rw-r--r--   0 yxu        (502) staff       (20)     4118 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policyrulesmbclientpost_rules.py
--rw-r--r--   0 yxu        (502) staff       (20)     4951 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policyrulesnapshotpost_rules.py
--rw-r--r--   0 yxu        (502) staff       (20)     4267 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/port.py
--rw-r--r--   0 yxu        (502) staff       (20)     3767 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/port_common.py
--rw-r--r--   0 yxu        (502) staff       (20)     4763 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/port_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/port_initiator.py
--rw-r--r--   0 yxu        (502) staff       (20)     4830 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/port_initiators_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7747 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     5402 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3955 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     4425 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4986 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_array_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4433 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4954 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3322 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5991 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     5428 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5624 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     5798 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3324 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5387 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5508 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3380 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3546 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3861 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_target.py
--rw-r--r--   0 yxu        (502) staff       (20)     4985 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_target_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_target_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4245 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/qos.py
--rw-r--r--   0 yxu        (502) staff       (20)     3329 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/reference.py
--rw-r--r--   0 yxu        (502) staff       (20)     3133 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/reference_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     3874 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/reference_with_type.py
--rw-r--r--   0 yxu        (502) staff       (20)     3581 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_pod.py
--rw-r--r--   0 yxu        (502) staff       (20)     4893 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_pods_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5722 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     4985 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3310 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5472 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     5041 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3366 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5411 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5465 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3319 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6402 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     4875 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3200 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5624 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5375 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3256 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3756 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/replica_link_lag.py
--rw-r--r--   0 yxu        (502) staff       (20)     6024 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/replica_link_performance_replication.py
--rw-r--r--   0 yxu        (502) staff       (20)     4911 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/replication_performance_with_total.py
--rw-r--r--   0 yxu        (502) staff       (20)     4175 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/replication_schedule.py
--rw-r--r--   0 yxu        (502) staff       (20)     3361 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource.py
--rw-r--r--   0 yxu        (502) staff       (20)     3372 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_fixed_non_unique_name.py
--rw-r--r--   0 yxu        (502) staff       (20)     3128 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)    19331 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19608 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     5450 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_by_array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5358 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    19098 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)    19375 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     5490 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_by_array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5398 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3878 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_pod_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     5400 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_pod_space_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3857 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     5382 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_space_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3534 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_space_no_id.py
--rw-r--r--   0 yxu        (502) staff       (20)     4854 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_space_no_id_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3707 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/retention_policy.py
--rw-r--r--   0 yxu        (502) staff       (20)     3531 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/smis.py
--rw-r--r--   0 yxu        (502) staff       (20)     4763 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/smis_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3088 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/smis_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5869 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     3834 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/snapshot_schedule.py
--rw-r--r--   0 yxu        (502) staff       (20)     6252 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software.py
--rw-r--r--   0 yxu        (502) staff       (20)     4791 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6323 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation.py
--rw-r--r--   0 yxu        (502) staff       (20)     3346 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3948 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     5629 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_step.py
--rw-r--r--   0 yxu        (502) staff       (20)     5633 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps.py
--rw-r--r--   0 yxu        (502) staff       (20)     4212 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_checks.py
--rw-r--r--   0 yxu        (502) staff       (20)     4907 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3232 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6327 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installations.py
--rw-r--r--   0 yxu        (502) staff       (20)     4879 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installations_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3204 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installations_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3116 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     8620 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/space.py
--rw-r--r--   0 yxu        (502) staff       (20)     3390 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/start_end_time.py
--rw-r--r--   0 yxu        (502) staff       (20)     5425 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/subnet.py
--rw-r--r--   0 yxu        (502) staff       (20)     4777 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/subnet_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4820 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/subnet_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     4580 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/subnet_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/subnet_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5569 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/support.py
--rw-r--r--   0 yxu        (502) staff       (20)     4784 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/support_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4052 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/support_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     3579 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/support_remote_assist_paths.py
--rw-r--r--   0 yxu        (502) staff       (20)     3109 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/support_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4418 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/tag.py
--rw-r--r--   0 yxu        (502) staff       (20)     4756 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/tag_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/tag_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3773 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/target_protection_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     3951 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/target_protection_group_post_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     5549 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/test_result.py
--rw-r--r--   0 yxu        (502) staff       (20)     4805 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/test_result_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/test_result_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5882 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/test_result_with_resource.py
--rw-r--r--   0 yxu        (502) staff       (20)     4877 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/test_result_with_resource_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3494 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/time_window.py
--rw-r--r--   0 yxu        (502) staff       (20)     5059 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/username.py
--rw-r--r--   0 yxu        (502) staff       (20)     3116 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/username_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     8928 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume.py
--rw-r--r--   0 yxu        (502) staff       (20)     6702 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_common.py
--rw-r--r--   0 yxu        (502) staff       (20)     5297 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5114 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group.py
--rw-r--r--   0 yxu        (502) staff       (20)     5205 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    19343 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)     4850 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3137 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3869 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group_space.py
--rw-r--r--   0 yxu        (502) staff       (20)     5500 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)    19323 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_performance.py
--rw-r--r--   0 yxu        (502) staff       (20)    19600 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_performance_by_array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4667 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3257 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     7257 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     5392 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3730 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_patch.py
--rw-r--r--   0 yxu        (502) staff       (20)     4009 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_post.py
--rw-r--r--   0 yxu        (502) staff       (20)     3315 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5600 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer.py
--rw-r--r--   0 yxu        (502) staff       (20)     5472 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3371 2020-09-24 18:20:28.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3849 2020-09-24 18:20:27.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_space.py
--rw-r--r--   0 yxu        (502) staff       (20)    13088 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/rest.py
--rw-r--r--   0 yxu        (502) staff       (20)       49 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     3015 2020-09-24 18:20:29.000000 py-pure-client-1.8.0/pypureclient/flasharray/client.py
--rw-r--r--   0 yxu        (502) staff       (20)      830 2020-09-24 18:20:30.000000 py-pure-client-1.8.0/pypureclient/keywords.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:05.668885 py-pure-client-1.8.0/pypureclient/mordac/
--rw-r--r--   0 yxu        (502) staff       (20)        0 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/mordac/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)    18592 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/properties.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:05.685283 py-pure-client-1.8.0/pypureclient/pure1/
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:05.743286 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/
--rw-r--r--   0 yxu        (502) staff       (20)     3235 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/__init__.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:06.033935 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/
--rw-r--r--   0 yxu        (502) staff       (20)     1137 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     7031 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/alerts_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    32055 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/arrays_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6980 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/audits_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6378 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/authorization_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6998 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/blades_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    11997 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/bucket_replica_links_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6980 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/buckets_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7038 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/controllers_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6998 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/drives_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    20127 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/file_system_replica_links_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    16441 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/file_system_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    15046 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/file_systems_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7022 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/hardware_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7124 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/hardware_connectors_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    15461 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/metrics_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7132 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/network_interfaces_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7112 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/object_store_accounts_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    11967 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/pod_replica_links_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6975 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/pods_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    39114 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/policies_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6988 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/ports_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6998 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/targets_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     8364 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/volume_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7005 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/volumes_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    24493 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api_client.py
--rw-r--r--   0 yxu        (502) staff       (20)   164930 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/client.py
--rw-r--r--   0 yxu        (502) staff       (20)     7969 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/configuration.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:07.332063 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/
--rw-r--r--   0 yxu        (502) staff       (20)     5864 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     7945 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/alert.py
--rw-r--r--   0 yxu        (502) staff       (20)     4178 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/alerts_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3099 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/alerts_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4110 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4174 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/array_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3260 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/arrays.py
--rw-r--r--   0 yxu        (502) staff       (20)     3944 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/arrays_built_in.py
--rw-r--r--   0 yxu        (502) staff       (20)     3942 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/arrays_resource.py
--rw-r--r--   0 yxu        (502) staff       (20)     5258 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/audit.py
--rw-r--r--   0 yxu        (502) staff       (20)     4178 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/audits_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3099 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/audits_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4674 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/blade.py
--rw-r--r--   0 yxu        (502) staff       (20)     4238 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/blade_array_status.py
--rw-r--r--   0 yxu        (502) staff       (20)     4174 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/blade_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/blade_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5254 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket.py
--rw-r--r--   0 yxu        (502) staff       (20)     4181 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5704 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link.py
--rw-r--r--   0 yxu        (502) staff       (20)     4258 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3179 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3544 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/built_in_as_of.py
--rw-r--r--   0 yxu        (502) staff       (20)     5102 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/controller.py
--rw-r--r--   0 yxu        (502) staff       (20)     4209 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/controller_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/controller_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5198 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/drive.py
--rw-r--r--   0 yxu        (502) staff       (20)     4250 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/drive_array_status.py
--rw-r--r--   0 yxu        (502) staff       (20)     4174 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/drive_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/drive_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3122 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/error.py
--rw-r--r--   0 yxu        (502) staff       (20)     3256 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/error_errors.py
--rw-r--r--   0 yxu        (502) staff       (20)     3084 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/error_no_context.py
--rw-r--r--   0 yxu        (502) staff       (20)     6336 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system.py
--rw-r--r--   0 yxu        (502) staff       (20)     4209 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5758 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link.py
--rw-r--r--   0 yxu        (502) staff       (20)     4286 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3207 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5212 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     4265 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3186 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3707 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/fixed_reference.py
--rw-r--r--   0 yxu        (502) staff       (20)     6631 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware.py
--rw-r--r--   0 yxu        (502) staff       (20)     5358 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector.py
--rw-r--r--   0 yxu        (502) staff       (20)     4258 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3179 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4195 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3116 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3073 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/http.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/inline_response400.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/inline_response401.py
--rw-r--r--   0 yxu        (502) staff       (20)     4828 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric.py
--rw-r--r--   0 yxu        (502) staff       (20)     3764 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_availability.py
--rw-r--r--   0 yxu        (502) staff       (20)     4181 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5365 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_history.py
--rw-r--r--   0 yxu        (502) staff       (20)     4230 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_history_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3151 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_history_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5824 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/network_interface.py
--rw-r--r--   0 yxu        (502) staff       (20)     4289 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/network_interface_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3210 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/network_interface_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3249 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/nfs.py
--rw-r--r--   0 yxu        (502) staff       (20)     4342 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/oauth_token_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4478 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/object_store_account.py
--rw-r--r--   0 yxu        (502) staff       (20)     4299 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/object_store_account_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3220 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/object_store_account_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3943 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/page_info.py
--rw-r--r--   0 yxu        (502) staff       (20)     4370 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod.py
--rw-r--r--   0 yxu        (502) staff       (20)     6031 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_array_status.py
--rw-r--r--   0 yxu        (502) staff       (20)     4160 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5495 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link.py
--rw-r--r--   0 yxu        (502) staff       (20)     4237 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3158 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4360 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy.py
--rw-r--r--   0 yxu        (502) staff       (20)     4181 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3555 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_member.py
--rw-r--r--   0 yxu        (502) staff       (20)     4227 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_members_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3148 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_members_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3868 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_rule.py
--rw-r--r--   0 yxu        (502) staff       (20)     5124 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/port.py
--rw-r--r--   0 yxu        (502) staff       (20)     4167 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/port_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3088 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/port_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4445 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/replica_link.py
--rw-r--r--   0 yxu        (502) staff       (20)     3526 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/resource.py
--rw-r--r--   0 yxu        (502) staff       (20)     3335 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/resource_no_name.py
--rw-r--r--   0 yxu        (502) staff       (20)     3963 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/resource_with_location.py
--rw-r--r--   0 yxu        (502) staff       (20)     3993 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/resource_with_locations.py
--rw-r--r--   0 yxu        (502) staff       (20)     3069 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/smb.py
--rw-r--r--   0 yxu        (502) staff       (20)     3798 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/support_contract.py
--rw-r--r--   0 yxu        (502) staff       (20)     4244 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/support_contract_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3165 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/support_contract_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4013 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/tag.py
--rw-r--r--   0 yxu        (502) staff       (20)     4160 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/tag_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3224 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/tag_put.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/tag_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4747 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/target.py
--rw-r--r--   0 yxu        (502) staff       (20)     4181 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/target_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/target_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3111 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/time_aware.py
--rw-r--r--   0 yxu        (502) staff       (20)     6066 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume.py
--rw-r--r--   0 yxu        (502) staff       (20)     4181 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6399 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     4237 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3158 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    13090 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/rest.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:07.397131 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/
--rw-r--r--   0 yxu        (502) staff       (20)     3393 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/__init__.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:07.713881 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/
--rw-r--r--   0 yxu        (502) staff       (20)     1137 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     7031 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/alerts_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    33254 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/arrays_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6980 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/audits_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6378 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/authorization_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6998 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/blades_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    11997 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/bucket_replica_links_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6980 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/buckets_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7038 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/controllers_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6998 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/drives_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    20127 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/file_system_replica_links_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    16441 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/file_system_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    15057 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/file_systems_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7022 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/hardware_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7124 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/hardware_connectors_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    15461 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/metrics_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7132 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/network_interfaces_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7112 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/object_store_accounts_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    11967 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/pod_replica_links_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6975 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/pods_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    39114 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/policies_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6988 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/ports_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     6998 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/targets_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     8364 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/volume_snapshots_api.py
--rw-r--r--   0 yxu        (502) staff       (20)     7016 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/volumes_api.py
--rw-r--r--   0 yxu        (502) staff       (20)    24493 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api_client.py
--rw-r--r--   0 yxu        (502) staff       (20)   165511 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/client.py
--rw-r--r--   0 yxu        (502) staff       (20)     7969 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/configuration.py
-drwxr-xr-x   0 yxu        (502) staff       (20)        0 2020-09-28 18:31:09.103134 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/
--rw-r--r--   0 yxu        (502) staff       (20)     5963 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     7957 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/alert.py
--rw-r--r--   0 yxu        (502) staff       (20)     4178 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/alerts_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3099 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/alerts_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4317 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/array.py
--rw-r--r--   0 yxu        (502) staff       (20)     4174 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/array_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/array_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3272 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/arrays.py
--rw-r--r--   0 yxu        (502) staff       (20)     3267 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/arrays2.py
--rw-r--r--   0 yxu        (502) staff       (20)     3947 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/arrays_built_in.py
--rw-r--r--   0 yxu        (502) staff       (20)     3954 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/arrays_resource.py
--rw-r--r--   0 yxu        (502) staff       (20)     5270 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/audit.py
--rw-r--r--   0 yxu        (502) staff       (20)     4178 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/audits_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3099 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/audits_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4674 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/blade.py
--rw-r--r--   0 yxu        (502) staff       (20)     4500 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/blade_array_status.py
--rw-r--r--   0 yxu        (502) staff       (20)     4174 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/blade_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/blade_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5254 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket.py
--rw-r--r--   0 yxu        (502) staff       (20)     4181 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5704 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link.py
--rw-r--r--   0 yxu        (502) staff       (20)     4258 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3179 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3544 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/built_in_as_of.py
--rw-r--r--   0 yxu        (502) staff       (20)     5114 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/controller.py
--rw-r--r--   0 yxu        (502) staff       (20)     4209 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/controller_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/controller_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5198 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/drive.py
--rw-r--r--   0 yxu        (502) staff       (20)     4512 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/drive_array_status.py
--rw-r--r--   0 yxu        (502) staff       (20)     4174 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/drive_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3095 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/drive_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3122 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/error.py
--rw-r--r--   0 yxu        (502) staff       (20)     3256 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/error_errors.py
--rw-r--r--   0 yxu        (502) staff       (20)     3084 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/error_no_context.py
--rw-r--r--   0 yxu        (502) staff       (20)     6348 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system.py
--rw-r--r--   0 yxu        (502) staff       (20)     4209 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5758 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link.py
--rw-r--r--   0 yxu        (502) staff       (20)     4286 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3207 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3130 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5180 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     4265 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3186 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3707 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/fixed_reference.py
--rw-r--r--   0 yxu        (502) staff       (20)     3711 2020-09-24 18:31:00.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/fixed_reference2.py
--rw-r--r--   0 yxu        (502) staff       (20)     3985 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/fixed_reference_fqdn.py
--rw-r--r--   0 yxu        (502) staff       (20)     6643 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware.py
--rw-r--r--   0 yxu        (502) staff       (20)     5370 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector.py
--rw-r--r--   0 yxu        (502) staff       (20)     4258 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3179 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4195 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3116 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3073 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/http.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/inline_response400.py
--rw-r--r--   0 yxu        (502) staff       (20)     3344 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/inline_response401.py
--rw-r--r--   0 yxu        (502) staff       (20)     4828 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric.py
--rw-r--r--   0 yxu        (502) staff       (20)     3764 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_availability.py
--rw-r--r--   0 yxu        (502) staff       (20)     4181 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5050 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_history.py
--rw-r--r--   0 yxu        (502) staff       (20)     4230 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_history_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3151 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_history_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5836 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/network_interface.py
--rw-r--r--   0 yxu        (502) staff       (20)     4289 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/network_interface_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3210 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/network_interface_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3249 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/nfs.py
--rw-r--r--   0 yxu        (502) staff       (20)     4342 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/oauth_token_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4478 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/object_store_account.py
--rw-r--r--   0 yxu        (502) staff       (20)     4299 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/object_store_account_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3220 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/object_store_account_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3943 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/page_info.py
--rw-r--r--   0 yxu        (502) staff       (20)     4404 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod.py
--rw-r--r--   0 yxu        (502) staff       (20)     6031 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_array_status.py
--rw-r--r--   0 yxu        (502) staff       (20)     4160 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     5495 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link.py
--rw-r--r--   0 yxu        (502) staff       (20)     4237 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3158 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4372 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy.py
--rw-r--r--   0 yxu        (502) staff       (20)     4181 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3555 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_member.py
--rw-r--r--   0 yxu        (502) staff       (20)     4227 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_members_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3148 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_members_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3868 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_rule.py
--rw-r--r--   0 yxu        (502) staff       (20)     5136 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/port.py
--rw-r--r--   0 yxu        (502) staff       (20)     4167 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/port_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3088 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/port_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4445 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/replica_link.py
--rw-r--r--   0 yxu        (502) staff       (20)     3526 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/resource.py
--rw-r--r--   0 yxu        (502) staff       (20)     3335 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/resource_no_name.py
--rw-r--r--   0 yxu        (502) staff       (20)     3975 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/resource_with_location.py
--rw-r--r--   0 yxu        (502) staff       (20)     4005 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/resource_with_locations.py
--rw-r--r--   0 yxu        (502) staff       (20)     3069 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/smb.py
--rw-r--r--   0 yxu        (502) staff       (20)     3810 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/support_contract.py
--rw-r--r--   0 yxu        (502) staff       (20)     4244 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/support_contract_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3165 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/support_contract_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4013 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/tag.py
--rw-r--r--   0 yxu        (502) staff       (20)     4160 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/tag_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3224 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/tag_put.py
--rw-r--r--   0 yxu        (502) staff       (20)     3081 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/tag_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     4759 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/target.py
--rw-r--r--   0 yxu        (502) staff       (20)     4181 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/target_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/target_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3111 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/time_aware.py
--rw-r--r--   0 yxu        (502) staff       (20)     6078 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume.py
--rw-r--r--   0 yxu        (502) staff       (20)     4181 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3102 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     6352 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot.py
--rw-r--r--   0 yxu        (502) staff       (20)     4237 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot_get_response.py
--rw-r--r--   0 yxu        (502) staff       (20)     3158 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot_response.py
--rw-r--r--   0 yxu        (502) staff       (20)    13090 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/rest.py
--rw-r--r--   0 yxu        (502) staff       (20)       52 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/__init__.py
--rw-r--r--   0 yxu        (502) staff       (20)     1895 2020-09-24 18:20:25.000000 py-pure-client-1.8.0/pypureclient/pure1/client.py
--rw-r--r--   0 yxu        (502) staff       (20)    11340 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/responses.py
--rw-r--r--   0 yxu        (502) staff       (20)     7296 2020-09-24 18:20:26.000000 py-pure-client-1.8.0/pypureclient/token_manager.py
--rw-r--r--   0 yxu        (502) staff       (20)       38 2020-09-28 18:31:09.125702 py-pure-client-1.8.0/setup.cfg
--rw-r--r--   0 yxu        (502) staff       (20)     1166 2020-09-28 18:29:56.000000 py-pure-client-1.8.0/setup.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:21.932465 py-pure-client-1.9.0/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     1871 2020-10-22 23:31:21.925340 py-pure-client-1.9.0/PKG-INFO
+-rw-r--r--   0 tvilcu     (502) staff       (20)     1032 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/README.md
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:10.291283 py-pure-client-1.9.0/py_pure_client.egg-info/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     1871 2020-10-22 23:31:09.000000 py-pure-client-1.9.0/py_pure_client.egg-info/PKG-INFO
+-rw-r--r--   0 tvilcu     (502) staff       (20)    76825 2020-10-22 23:31:10.000000 py-pure-client-1.9.0/py_pure_client.egg-info/SOURCES.txt
+-rw-r--r--   0 tvilcu     (502) staff       (20)        1 2020-10-22 23:31:09.000000 py-pure-client-1.9.0/py_pure_client.egg-info/dependency_links.txt
+-rw-r--r--   0 tvilcu     (502) staff       (20)      111 2020-10-22 23:31:09.000000 py-pure-client-1.9.0/py_pure_client.egg-info/requires.txt
+-rw-r--r--   0 tvilcu     (502) staff       (20)       13 2020-10-22 23:31:09.000000 py-pure-client-1.9.0/py_pure_client.egg-info/top_level.txt
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:10.358251 py-pure-client-1.9.0/pypureclient/
+-rw-r--r--   0 tvilcu     (502) staff       (20)      200 2020-10-22 23:16:14.000000 py-pure-client-1.9.0/pypureclient/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     2073 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/api_token_manager.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)      276 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/exceptions.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:10.375198 py-pure-client-1.9.0/pypureclient/flasharray/
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:10.423002 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3768 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/__init__.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:10.483816 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/
+-rw-r--r--   0 tvilcu     (502) staff       (20)      328 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    14706 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/authorization_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    21406 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/connections_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    40358 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/host_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    40650 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/hosts_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    32502 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/volume_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    57311 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/volumes_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    24491 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   141512 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7677 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/configuration.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:11.135118 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4537 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3153 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/api_version_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3352 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/built_in.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4154 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/chap.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5563 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/connection.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4202 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/connection_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4664 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/connection_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3287 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/connection_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3534 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/destroyed_patch_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3349 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/fixed_reference.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3153 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/fixed_reference_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6860 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4160 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4261 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4141 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3092 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19335 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19612 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3226 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7782 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19315 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19592 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3549 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_port_connectivity.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5382 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3245 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/inline_response400.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/inline_response401.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3262 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/member.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3430 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4169 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3254 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3064 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/new_name.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4342 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/oauth_token_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3779 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/page_info.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18814 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4245 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/qos.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3329 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/reference.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3133 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/reference_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3361 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3128 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19331 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19608 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4690 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_by_array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4598 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19098 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19375 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4730 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_by_array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4638 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3857 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4622 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_space_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5869 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8620 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4703 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/username.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3116 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/username_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7705 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6702 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_common.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4552 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4887 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19323 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19600 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4667 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3259 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7257 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4632 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3730 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4009 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3315 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5244 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4712 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3371 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3849 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    13088 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/rest.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:11.179916 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7691 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/__init__.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:11.338979 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/
+-rw-r--r--   0 tvilcu     (502) staff       (20)      875 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    20392 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/api_clients_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    14706 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/authorization_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    22009 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/connections_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    75517 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/host_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    75649 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/hosts_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    15870 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/offloads_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    76932 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/pods_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    30197 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/protection_group_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   126965 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/protection_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7987 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/remote_pods_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    26280 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/remote_protection_group_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18457 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/remote_protection_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18899 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/remote_volume_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    54326 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/volume_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    33102 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/volume_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    84705 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/volumes_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    24491 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   474676 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7679 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/configuration.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:12.723740 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     9408 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3483 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/aggregate_replication_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6448 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4901 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_client_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3223 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_client_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5443 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_client_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3226 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_client_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3153 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_version_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3352 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/built_in.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3151 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/built_in_resource_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4154 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/chap.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5364 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/connection.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/connection_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4664 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/connection_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/connection_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3534 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/destroyed_patch_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3349 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/fixed_reference.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3153 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/fixed_reference_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7232 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4866 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4261 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4901 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3092 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19335 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19612 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3226 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3522 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7782 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19315 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19592 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3549 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_port_connectivity.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5382 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3191 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3502 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/inline_response400.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/inline_response401.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3262 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4934 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3430 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4929 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3254 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_no_id_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3259 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3064 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/new_name.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4342 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/oauth_token_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5861 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4175 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_azure.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5268 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4257 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_nfs.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3543 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3212 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6121 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_s3.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4539 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/page_info.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18814 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7362 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7481 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_array_status.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5228 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5355 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19311 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19588 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4466 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3184 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8632 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7747 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5402 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3955 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4425 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4986 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_array_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4433 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4954 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3322 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5991 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5428 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5624 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5798 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3324 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5387 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5508 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3380 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3546 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3861 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_target.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4985 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_target_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_target_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4245 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/qos.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3329 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/reference.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3133 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/reference_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3581 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_pod.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4893 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_pods_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5722 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4985 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5472 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5041 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3366 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5411 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5465 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3319 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6402 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4875 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3200 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5624 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5375 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3256 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4175 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/replication_schedule.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3361 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3128 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19331 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19608 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5450 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_by_array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5358 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19098 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19375 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5490 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_by_array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5398 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3857 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5382 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_space_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3534 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_space_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4854 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_space_no_id_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3707 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/retention_policy.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5869 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3834 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/snapshot_schedule.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8620 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3773 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/target_protection_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3951 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/target_protection_group_post_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3494 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/time_window.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5059 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/username.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3116 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/username_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7705 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6702 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_common.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5312 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5114 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5205 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19343 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4850 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3137 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3869 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4887 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19323 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19600 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4667 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3259 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7257 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5392 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3730 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4009 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3315 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5600 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5472 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3371 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3849 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    13088 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/rest.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:12.775475 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/
+-rw-r--r--   0 tvilcu     (502) staff       (20)    12907 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/__init__.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:13.097872 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     1540 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    58610 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/administrators_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    20753 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/alerts_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    20392 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/api_clients_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18819 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/apps_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    42836 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/arrays_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8049 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/audits_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    14706 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/authorization_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    22035 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/connections_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7737 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/controllers_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    31766 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/directory_services_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    10127 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/dns_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    11156 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/hardware_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    75510 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/host_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    75642 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/hosts_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    22891 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/kmip_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    15865 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/maintenance_windows_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    15864 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/offloads_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    63516 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/pod_replica_links_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   101781 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/pods_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    14048 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/ports_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    30174 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/protection_group_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   126965 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/protection_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7987 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/remote_pods_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    26280 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/remote_protection_group_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18457 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/remote_protection_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18899 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/remote_volume_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    10154 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/smi_s_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    32959 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/software_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19422 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/subnets_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    17289 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/support_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    54326 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/volume_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    50371 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/volume_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   101901 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/volumes_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    24491 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   763246 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7679 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/configuration.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:15.705018 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/
+-rw-r--r--   0 tvilcu     (502) staff       (20)    16731 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5100 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3357 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_api_token.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4826 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_api_token_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3151 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_api_token_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3591 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_cache.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_cache_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_cache_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4770 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5367 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3296 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3117 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_role.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5080 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_settings.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3151 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_settings_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3483 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/aggregate_replication_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7730 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6208 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert_event.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert_event_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert_event_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4770 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6448 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4901 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_client_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3223 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_client_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5443 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_client_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3226 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_client_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3568 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_token.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3153 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_version_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4864 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4756 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4051 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app_node.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4784 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app_node_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3109 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app_node_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5865 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4773 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    21752 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4847 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_performance_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3098 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4242 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_space_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5869 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/arrays.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5197 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/audit.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4770 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/audit_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/audit_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3352 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/built_in.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3124 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/built_in_relationship.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3151 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/built_in_resource_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4154 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/chap.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5364 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/connection.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/connection_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4664 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/connection_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/connection_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4219 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/controller.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/controller_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4223 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/controllers.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3534 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/destroyed_patch_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5851 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4847 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3987 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_management.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3172 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3779 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_role.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4875 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_role_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3200 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_role_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3376 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/dns.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4756 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/dns_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3396 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/dns_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/dns_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3323 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/eula.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4763 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/eula_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3088 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/eula_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3828 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/eula_signature.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3167 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/fixed_name_resource_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3349 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/fixed_reference.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3153 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/fixed_reference_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5924 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/hardware.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4791 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/hardware_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3700 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/hardware_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3116 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/hardware_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7232 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4866 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4261 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4901 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3092 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19335 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19612 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3226 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3522 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7782 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19315 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19592 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3549 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_port_connectivity.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5382 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3191 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3502 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/inline_response400.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/inline_response401.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4147 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4763 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3936 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3932 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3088 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5046 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_test_result.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4833 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_test_result_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3680 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/maintenance_window.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3495 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/maintenance_window_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4858 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/maintenance_windows_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3183 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/maintenance_windows_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3262 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4934 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3430 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4929 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3254 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_no_id_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3259 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3064 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/new_name.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4342 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/oauth_token_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5133 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4175 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_azure.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5165 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4559 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_google_cloud.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4257 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_nfs.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3816 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3109 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6121 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_s3.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4933 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/override_check.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4539 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/page_info.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18814 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     9871 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7481 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_array_status.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5112 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6509 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19311 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19588 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5842 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6089 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5469 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3794 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5380 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3705 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4466 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5620 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4870 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5452 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4895 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3220 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3312 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6196 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6240 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5504 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3829 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3195 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     9277 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4267 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/port.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3767 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/port_common.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4763 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/port_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/port_initiator.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4830 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/port_initiators_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7747 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5402 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3955 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4425 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4986 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_array_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4433 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4954 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3322 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5991 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5428 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5624 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5798 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3324 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5387 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5508 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3380 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3546 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3861 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_target.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4985 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_target_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_target_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4245 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/qos.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3329 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/reference.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3133 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/reference_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3581 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_pod.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4893 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_pods_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5722 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4985 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5472 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5041 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3366 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5411 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5465 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3319 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6402 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4875 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3200 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5624 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5375 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3256 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3756 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/replica_link_lag.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6024 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/replica_link_performance_replication.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4911 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/replication_performance_with_total.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4175 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/replication_schedule.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3361 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3372 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_fixed_non_unique_name.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3128 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19331 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19608 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5450 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_by_array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5358 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19098 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19375 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5490 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_by_array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5398 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3878 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_pod_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5400 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_pod_space_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3857 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5382 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_space_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3534 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_space_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4854 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_space_no_id_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3707 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/retention_policy.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3531 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/smis.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4763 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/smis_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3088 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/smis_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5869 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3834 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/snapshot_schedule.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6252 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4791 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6323 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3346 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3948 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5629 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_step.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5633 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4212 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_checks.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4907 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3232 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6327 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installations.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4879 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installations_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3204 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installations_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3116 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8620 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3390 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/start_end_time.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5425 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/subnet.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4777 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/subnet_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4820 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/subnet_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4580 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/subnet_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/subnet_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5569 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/support.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4784 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/support_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4052 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/support_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3579 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/support_remote_assist_paths.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3109 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/support_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4418 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/tag.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4756 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/tag_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/tag_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3773 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/target_protection_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3951 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/target_protection_group_post_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5549 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/test_result.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/test_result_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/test_result_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5882 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/test_result_with_resource.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4877 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/test_result_with_resource_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3494 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/time_window.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5059 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/username.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3116 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/username_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8928 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6702 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_common.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5297 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5114 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5205 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19343 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4850 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3137 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3869 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5500 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19323 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19600 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4667 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3257 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7257 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5392 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3730 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4009 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3315 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5600 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5472 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3371 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3849 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    13088 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/rest.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:15.763574 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/
+-rw-r--r--   0 tvilcu     (502) staff       (20)    16195 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/__init__.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:16.152133 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     1834 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    16246 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/active_directory_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    58610 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/administrators_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    20753 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/alerts_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    20392 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/api_clients_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18819 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/apps_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    42836 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/arrays_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8049 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/audits_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    14706 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/authorization_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    22035 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/connections_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7737 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/controllers_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   117857 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/directories_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    21387 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/directory_exports_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    31766 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/directory_services_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    24127 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/directory_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    10127 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/dns_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    21311 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/file_systems_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    11156 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/hardware_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    75510 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/host_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    75642 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/hosts_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    22891 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/kmip_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    15865 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/maintenance_windows_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    15864 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/offloads_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    63516 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/pod_replica_links_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   100471 2020-10-22 23:15:07.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/pods_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   196023 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/policies_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    14048 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/ports_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    30174 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/protection_group_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   126965 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/protection_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7987 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/remote_pods_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    26280 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/remote_protection_group_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18457 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/remote_protection_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18899 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/remote_volume_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    10154 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/smi_s_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    32959 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/software_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19422 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/subnets_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    17289 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/support_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    55148 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/volume_groups_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    51428 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/volume_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   102940 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/volumes_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    24491 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)  1022486 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7679 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/configuration.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:19.383971 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/
+-rw-r--r--   0 tvilcu     (502) staff       (20)    20328 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4876 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/active_directory.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4908 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/active_directory_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5442 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/active_directory_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3233 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/active_directory_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5100 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3357 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_api_token.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4826 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_api_token_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3151 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_api_token_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3591 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_cache.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_cache_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_cache_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4770 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5367 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3296 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3117 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_role.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5080 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_settings.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3151 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_settings_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3483 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/aggregate_replication_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7730 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6208 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert_event.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert_event_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert_event_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4770 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6448 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4901 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_client_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3223 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_client_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5443 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_client_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3226 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_client_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3568 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_token.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3153 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_version_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4864 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4756 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4051 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app_node.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4784 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app_node_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3109 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app_node_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5865 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4773 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    21752 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4847 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_performance_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3098 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4242 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_space_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5869 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/arrays.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5197 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/audit.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4770 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/audit_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/audit_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3352 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/built_in.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3124 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/built_in_relationship.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3151 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/built_in_resource_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4154 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/chap.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5364 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/connection.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/connection_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4664 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/connection_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/connection_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4219 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/controller.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/controller_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4223 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/controllers.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3534 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/destroyed_patch_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5767 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4674 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_export.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4941 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_export_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3225 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_export_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3266 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_export_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5273 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3092 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     9599 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5359 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_performance_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3401 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_policy_export_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3349 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_policy_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3703 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3224 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5851 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4847 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3987 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_management.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3172 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3779 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_role.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4875 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_role_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3200 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_role_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6848 2020-10-22 23:15:08.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5353 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4222 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3696 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3280 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3861 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3536 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directorypolicyexportpost_policies.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3204 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directorypolicypost_policies.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3376 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/dns.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4756 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/dns_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3396 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/dns_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/dns_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3323 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/eula.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4763 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/eula_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3088 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/eula_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3828 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/eula_signature.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4759 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/file_system.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4906 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/file_system_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3714 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/file_system_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3231 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/file_system_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3167 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/fixed_name_resource_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3349 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/fixed_reference.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3153 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/fixed_reference_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3894 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/fixed_reference_with_type.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5924 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/hardware.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4791 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/hardware_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3700 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/hardware_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3116 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/hardware_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7232 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4866 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4261 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4901 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3092 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19335 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19612 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3226 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3522 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7782 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19315 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19592 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3549 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_port_connectivity.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5382 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3191 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3502 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/inline_response400.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/inline_response401.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4147 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4763 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3936 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3932 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3088 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5046 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_test_result.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4833 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_test_result_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3680 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/maintenance_window.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3495 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/maintenance_window_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4858 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/maintenance_windows_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3183 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/maintenance_windows_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3262 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4934 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3430 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4929 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3254 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_no_id_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3259 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3064 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/new_name.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4342 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/oauth_token_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5133 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4175 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_azure.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5165 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4559 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_google_cloud.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4257 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_nfs.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3816 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3109 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6121 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_s3.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4933 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/override_check.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4539 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/page_info.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18814 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    10133 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7481 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_array_status.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5112 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6509 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19311 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19588 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5842 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6089 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5469 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3794 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5380 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3705 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4466 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5620 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4870 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5452 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4895 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3220 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3312 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6196 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6240 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5504 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3829 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3195 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     9277 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3877 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4878 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3954 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4238 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_export.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4962 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3285 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3287 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4920 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3234 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3245 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3346 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3150 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3203 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4443 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4969 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3243 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3294 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4621 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4971 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3243 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3296 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5426 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4964 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3241 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3289 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3692 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policymemberexportpost_members.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3360 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policymemberpost_members.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3943 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policyrulenfsclientpost_rules.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4118 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policyrulesmbclientpost_rules.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4951 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policyrulesnapshotpost_rules.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4267 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/port.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3767 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/port_common.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4763 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/port_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/port_initiator.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4830 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/port_initiators_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7747 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5402 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3955 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4425 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4986 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_array_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4433 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4954 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3322 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5991 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5428 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5624 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5798 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3324 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5387 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5508 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3380 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3546 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3861 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_target.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4985 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_target_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_target_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4245 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/qos.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3329 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/reference.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3133 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/reference_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3874 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/reference_with_type.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3581 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_pod.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4893 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_pods_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5722 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4985 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3310 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5472 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5041 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3366 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5411 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5465 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3319 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6402 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4875 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3200 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5624 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5375 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3256 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3756 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/replica_link_lag.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6024 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/replica_link_performance_replication.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4911 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/replication_performance_with_total.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4175 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/replication_schedule.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3361 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3372 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_fixed_non_unique_name.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3128 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19331 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19608 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5450 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_by_array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5358 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19098 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19375 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5490 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_by_array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5398 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3878 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_pod_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5400 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_pod_space_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3857 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5382 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_space_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3534 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_space_no_id.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4854 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_space_no_id_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3707 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/retention_policy.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3531 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/smis.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4763 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/smis_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3088 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/smis_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5869 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3834 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/snapshot_schedule.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6252 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4791 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6323 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3346 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3948 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5629 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_step.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5633 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4212 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_checks.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4907 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3232 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6327 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installations.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4879 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installations_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3204 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installations_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3116 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8620 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3390 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/start_end_time.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5425 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/subnet.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4777 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/subnet_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4820 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/subnet_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4580 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/subnet_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/subnet_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5569 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/support.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4784 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/support_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4052 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/support_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3579 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/support_remote_assist_paths.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3109 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/support_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4418 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/tag.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4756 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/tag_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/tag_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3773 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/target_protection_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3951 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/target_protection_group_post_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5549 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/test_result.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4805 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/test_result_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/test_result_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5882 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/test_result_with_resource.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4877 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/test_result_with_resource_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3494 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/time_window.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5059 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/username.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3116 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/username_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8928 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6702 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_common.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5297 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5114 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5205 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19343 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4850 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3137 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3869 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5500 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19323 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_performance.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    19600 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_performance_by_array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4667 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3257 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7257 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5392 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3730 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_patch.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4009 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_post.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3315 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5600 2020-10-22 23:12:32.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5472 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3371 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3849 2020-10-22 23:12:31.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_space.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    13088 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/rest.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)       49 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3015 2020-10-22 23:12:33.000000 py-pure-client-1.9.0/pypureclient/flasharray/client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)      830 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/pypureclient/keywords.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    18592 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/properties.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:19.400151 py-pure-client-1.9.0/pypureclient/pure1/
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:19.443828 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3290 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/__init__.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:19.671816 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     1181 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7031 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/alerts_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    32055 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/arrays_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6980 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/audits_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6378 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/authorization_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6998 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/blades_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    11997 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/bucket_replica_links_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6980 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/buckets_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7038 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/controllers_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8455 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/directories_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6998 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/drives_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    20160 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/file_system_replica_links_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    16485 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/file_system_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    15120 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/file_systems_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7022 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/hardware_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7124 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/hardware_connectors_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    15461 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/metrics_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7132 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/network_interfaces_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7112 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/object_store_accounts_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    11967 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/pod_replica_links_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6975 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/pods_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    39180 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/policies_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6988 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/ports_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6998 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/targets_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8364 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/volume_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7005 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/volumes_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    24493 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   169990 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7969 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/configuration.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:20.641270 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6004 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7945 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/alert.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4178 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/alerts_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3099 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/alerts_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4110 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4174 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/array_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3260 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/arrays.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3944 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/arrays_built_in.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3942 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/arrays_resource.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5258 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/audit.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4178 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/audits_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3099 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/audits_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4674 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/blade.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4238 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/blade_array_status.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4174 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/blade_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/blade_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5254 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4181 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5704 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4258 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3179 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3544 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/built_in_as_of.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5102 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/controller.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4209 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/controller_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/controller_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5460 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/directory.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4202 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/directory_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3123 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/directory_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5198 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/drive.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4250 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/drive_array_status.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4174 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/drive_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/drive_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3122 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/error.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3256 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/error_errors.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3084 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/error_no_context.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6990 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4209 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5758 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4286 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3207 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5212 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4265 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3186 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3707 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/fixed_reference.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6631 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5358 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4258 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3179 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4195 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3116 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3073 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/http.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/inline_response400.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/inline_response401.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4828 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3764 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_availability.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4181 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5365 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_history.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4230 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_history_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3151 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_history_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5824 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/network_interface.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4289 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/network_interface_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3210 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/network_interface_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3249 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/nfs.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4342 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/oauth_token_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4478 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/object_store_account.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4299 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/object_store_account_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3220 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/object_store_account_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3943 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/page_info.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4370 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6031 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_array_status.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4160 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5495 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4237 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3158 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4360 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4181 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3555 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_member.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4227 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_members_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3148 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_members_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3868 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_rule.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5124 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/port.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4167 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/port_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3088 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/port_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4445 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/replica_link.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3526 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/resource.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3335 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/resource_no_name.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3963 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/resource_with_location.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3993 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/resource_with_locations.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3069 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/smb.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3798 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/support_contract.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4244 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/support_contract_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3165 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/support_contract_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4013 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/tag.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4160 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/tag_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3224 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/tag_put.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/tag_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4747 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/target.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4181 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/target_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/target_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3111 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/time_aware.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6066 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4181 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6399 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4237 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3158 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    13090 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/rest.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:20.687127 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3374 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/__init__.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:20.925793 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     1181 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7031 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/alerts_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    33254 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/arrays_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6980 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/audits_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6378 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/authorization_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6998 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/blades_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    11997 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/bucket_replica_links_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6980 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/buckets_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7038 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/controllers_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8455 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/directories_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6998 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/drives_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    20160 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/file_system_replica_links_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    16485 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/file_system_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    15120 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/file_systems_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7022 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/hardware_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7124 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/hardware_connectors_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    15461 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/metrics_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7132 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/network_interfaces_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7112 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/object_store_accounts_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    11967 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/pod_replica_links_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6975 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/pods_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    39180 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/policies_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6988 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/ports_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6998 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/targets_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     8364 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/volume_snapshots_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7016 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/volumes_api.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    24493 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api_client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)   170560 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7969 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/configuration.py
+drwxr-xr-x   0 tvilcu     (502) staff       (20)        0 2020-10-22 23:31:21.915807 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6057 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7957 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/alert.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4178 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/alerts_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3099 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/alerts_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4317 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/array.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4174 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/array_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/array_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3272 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/arrays.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3954 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/arrays_resource.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5270 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/audit.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4178 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/audits_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3099 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/audits_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4674 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/blade.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4500 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/blade_array_status.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4174 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/blade_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/blade_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5254 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4181 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5704 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4258 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3179 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3544 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/built_in_as_of.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5114 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/controller.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4209 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/controller_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/controller_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3284 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/directory.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4202 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/directory_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3123 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/directory_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5198 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/drive.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4512 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/drive_array_status.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4174 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/drive_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3095 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/drive_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3122 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/error.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3256 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/error_errors.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3084 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/error_no_context.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7002 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4209 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5758 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4286 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3207 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3130 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5180 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4265 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3186 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3707 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/fixed_reference.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3985 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/fixed_reference_fqdn.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6643 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5370 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4258 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3179 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4195 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3116 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3073 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/http.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/inline_response400.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3344 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/inline_response401.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4828 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3764 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_availability.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4181 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5050 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_history.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4230 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_history_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3151 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_history_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5836 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/network_interface.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4289 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/network_interface_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3210 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/network_interface_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3249 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/nfs.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4342 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/oauth_token_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4478 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/object_store_account.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4299 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/object_store_account_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3220 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/object_store_account_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3943 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/page_info.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4404 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6031 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_array_status.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4160 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5495 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4237 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3158 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4372 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4181 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3555 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_member.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4227 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_members_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3148 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_members_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3868 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_rule.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     5136 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/port.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4167 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/port_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3088 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/port_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4445 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/replica_link.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3526 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/resource.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3335 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/resource_no_name.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3975 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/resource_with_location.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4005 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/resource_with_locations.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3069 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/smb.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3810 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/support_contract.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4244 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/support_contract_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3165 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/support_contract_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4013 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/tag.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4160 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/tag_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3224 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/tag_put.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3081 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/tag_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4759 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/target.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4181 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/target_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/target_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3111 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/time_aware.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6078 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4181 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3102 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     6352 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     4237 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot_get_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     3158 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot_response.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    13090 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/rest.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)       52 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/__init__.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     1895 2020-10-22 23:12:29.000000 py-pure-client-1.9.0/pypureclient/pure1/client.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)    11340 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/responses.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)     7296 2020-10-22 23:12:30.000000 py-pure-client-1.9.0/pypureclient/token_manager.py
+-rw-r--r--   0 tvilcu     (502) staff       (20)       38 2020-10-22 23:31:21.932584 py-pure-client-1.9.0/setup.cfg
+-rw-r--r--   0 tvilcu     (502) staff       (20)     1166 2020-10-22 23:12:34.000000 py-pure-client-1.9.0/setup.py
```

### Comparing `py-pure-client-1.8.0/PKG-INFO` & `py-pure-client-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: py-pure-client
-Version: 1.8.0
+Version: 1.9.0
 Summary: Pure Storage Python clients for FlashArray, FlashBlade, and Pure1 APIs
 Home-page: https://github.com/PureStorage-OpenConnect/py-pure-client
 Author: Pure Storage
 Author-email: tvilcu@purestorage.com
 License: BSD 2-Clause
-Download-URL: https://github.com/PureStorage-OpenConnect/py-pure-client/archive/1.8.0.tar.gz
+Download-URL: https://github.com/PureStorage-OpenConnect/py-pure-client/archive/1.9.0.tar.gz
 Description: # Pure Storage Unified Python SDK
         
         ## Overview
         
         The `py-pure-client` Python package provides clients that use the Pure1 1.x REST API
         and the FlashArray REST 2.x API.
```

### Comparing `py-pure-client-1.8.0/README.md` & `py-pure-client-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/py_pure_client.egg-info/PKG-INFO` & `py-pure-client-1.9.0/py_pure_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: py-pure-client
-Version: 1.8.0
+Version: 1.9.0
 Summary: Pure Storage Python clients for FlashArray, FlashBlade, and Pure1 APIs
 Home-page: https://github.com/PureStorage-OpenConnect/py-pure-client
 Author: Pure Storage
 Author-email: tvilcu@purestorage.com
 License: BSD 2-Clause
-Download-URL: https://github.com/PureStorage-OpenConnect/py-pure-client/archive/1.8.0.tar.gz
+Download-URL: https://github.com/PureStorage-OpenConnect/py-pure-client/archive/1.9.0.tar.gz
 Description: # Pure Storage Unified Python SDK
         
         ## Overview
         
         The `py-pure-client` Python package provides clients that use the Pure1 1.x REST API
         and the FlashArray REST 2.x API.
```

### Comparing `py-pure-client-1.8.0/py_pure_client.egg-info/SOURCES.txt` & `py-pure-client-1.9.0/py_pure_client.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -992,15 +992,14 @@
 pypureclient/flasharray/FA_2_3/models/volume_snapshot_patch.py
 pypureclient/flasharray/FA_2_3/models/volume_snapshot_post.py
 pypureclient/flasharray/FA_2_3/models/volume_snapshot_response.py
 pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer.py
 pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer_get_response.py
 pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer_response.py
 pypureclient/flasharray/FA_2_3/models/volume_space.py
-pypureclient/mordac/__init__.py
 pypureclient/pure1/__init__.py
 pypureclient/pure1/client.py
 pypureclient/pure1/Pure1_1_0/__init__.py
 pypureclient/pure1/Pure1_1_0/api_client.py
 pypureclient/pure1/Pure1_1_0/client.py
 pypureclient/pure1/Pure1_1_0/configuration.py
 pypureclient/pure1/Pure1_1_0/rest.py
@@ -1009,14 +1008,15 @@
 pypureclient/pure1/Pure1_1_0/api/arrays_api.py
 pypureclient/pure1/Pure1_1_0/api/audits_api.py
 pypureclient/pure1/Pure1_1_0/api/authorization_api.py
 pypureclient/pure1/Pure1_1_0/api/blades_api.py
 pypureclient/pure1/Pure1_1_0/api/bucket_replica_links_api.py
 pypureclient/pure1/Pure1_1_0/api/buckets_api.py
 pypureclient/pure1/Pure1_1_0/api/controllers_api.py
+pypureclient/pure1/Pure1_1_0/api/directories_api.py
 pypureclient/pure1/Pure1_1_0/api/drives_api.py
 pypureclient/pure1/Pure1_1_0/api/file_system_replica_links_api.py
 pypureclient/pure1/Pure1_1_0/api/file_system_snapshots_api.py
 pypureclient/pure1/Pure1_1_0/api/file_systems_api.py
 pypureclient/pure1/Pure1_1_0/api/hardware_api.py
 pypureclient/pure1/Pure1_1_0/api/hardware_connectors_api.py
 pypureclient/pure1/Pure1_1_0/api/metrics_api.py
@@ -1052,14 +1052,17 @@
 pypureclient/pure1/Pure1_1_0/models/bucket_replica_link_get_response.py
 pypureclient/pure1/Pure1_1_0/models/bucket_replica_link_response.py
 pypureclient/pure1/Pure1_1_0/models/bucket_response.py
 pypureclient/pure1/Pure1_1_0/models/built_in_as_of.py
 pypureclient/pure1/Pure1_1_0/models/controller.py
 pypureclient/pure1/Pure1_1_0/models/controller_get_response.py
 pypureclient/pure1/Pure1_1_0/models/controller_response.py
+pypureclient/pure1/Pure1_1_0/models/directory.py
+pypureclient/pure1/Pure1_1_0/models/directory_get_response.py
+pypureclient/pure1/Pure1_1_0/models/directory_response.py
 pypureclient/pure1/Pure1_1_0/models/drive.py
 pypureclient/pure1/Pure1_1_0/models/drive_array_status.py
 pypureclient/pure1/Pure1_1_0/models/drive_get_response.py
 pypureclient/pure1/Pure1_1_0/models/drive_response.py
 pypureclient/pure1/Pure1_1_0/models/error.py
 pypureclient/pure1/Pure1_1_0/models/error_errors.py
 pypureclient/pure1/Pure1_1_0/models/error_no_context.py
@@ -1148,14 +1151,15 @@
 pypureclient/pure1/Pure1_1_1/api/arrays_api.py
 pypureclient/pure1/Pure1_1_1/api/audits_api.py
 pypureclient/pure1/Pure1_1_1/api/authorization_api.py
 pypureclient/pure1/Pure1_1_1/api/blades_api.py
 pypureclient/pure1/Pure1_1_1/api/bucket_replica_links_api.py
 pypureclient/pure1/Pure1_1_1/api/buckets_api.py
 pypureclient/pure1/Pure1_1_1/api/controllers_api.py
+pypureclient/pure1/Pure1_1_1/api/directories_api.py
 pypureclient/pure1/Pure1_1_1/api/drives_api.py
 pypureclient/pure1/Pure1_1_1/api/file_system_replica_links_api.py
 pypureclient/pure1/Pure1_1_1/api/file_system_snapshots_api.py
 pypureclient/pure1/Pure1_1_1/api/file_systems_api.py
 pypureclient/pure1/Pure1_1_1/api/hardware_api.py
 pypureclient/pure1/Pure1_1_1/api/hardware_connectors_api.py
 pypureclient/pure1/Pure1_1_1/api/metrics_api.py
@@ -1172,16 +1176,14 @@
 pypureclient/pure1/Pure1_1_1/models/alert.py
 pypureclient/pure1/Pure1_1_1/models/alerts_get_response.py
 pypureclient/pure1/Pure1_1_1/models/alerts_response.py
 pypureclient/pure1/Pure1_1_1/models/array.py
 pypureclient/pure1/Pure1_1_1/models/array_get_response.py
 pypureclient/pure1/Pure1_1_1/models/array_response.py
 pypureclient/pure1/Pure1_1_1/models/arrays.py
-pypureclient/pure1/Pure1_1_1/models/arrays2.py
-pypureclient/pure1/Pure1_1_1/models/arrays_built_in.py
 pypureclient/pure1/Pure1_1_1/models/arrays_resource.py
 pypureclient/pure1/Pure1_1_1/models/audit.py
 pypureclient/pure1/Pure1_1_1/models/audits_get_response.py
 pypureclient/pure1/Pure1_1_1/models/audits_response.py
 pypureclient/pure1/Pure1_1_1/models/blade.py
 pypureclient/pure1/Pure1_1_1/models/blade_array_status.py
 pypureclient/pure1/Pure1_1_1/models/blade_get_response.py
@@ -1192,14 +1194,17 @@
 pypureclient/pure1/Pure1_1_1/models/bucket_replica_link_get_response.py
 pypureclient/pure1/Pure1_1_1/models/bucket_replica_link_response.py
 pypureclient/pure1/Pure1_1_1/models/bucket_response.py
 pypureclient/pure1/Pure1_1_1/models/built_in_as_of.py
 pypureclient/pure1/Pure1_1_1/models/controller.py
 pypureclient/pure1/Pure1_1_1/models/controller_get_response.py
 pypureclient/pure1/Pure1_1_1/models/controller_response.py
+pypureclient/pure1/Pure1_1_1/models/directory.py
+pypureclient/pure1/Pure1_1_1/models/directory_get_response.py
+pypureclient/pure1/Pure1_1_1/models/directory_response.py
 pypureclient/pure1/Pure1_1_1/models/drive.py
 pypureclient/pure1/Pure1_1_1/models/drive_array_status.py
 pypureclient/pure1/Pure1_1_1/models/drive_get_response.py
 pypureclient/pure1/Pure1_1_1/models/drive_response.py
 pypureclient/pure1/Pure1_1_1/models/error.py
 pypureclient/pure1/Pure1_1_1/models/error_errors.py
 pypureclient/pure1/Pure1_1_1/models/error_no_context.py
@@ -1209,15 +1214,14 @@
 pypureclient/pure1/Pure1_1_1/models/file_system_replica_link_get_response.py
 pypureclient/pure1/Pure1_1_1/models/file_system_replica_link_response.py
 pypureclient/pure1/Pure1_1_1/models/file_system_response.py
 pypureclient/pure1/Pure1_1_1/models/file_system_snapshot.py
 pypureclient/pure1/Pure1_1_1/models/file_system_snapshot_get_response.py
 pypureclient/pure1/Pure1_1_1/models/file_system_snapshot_response.py
 pypureclient/pure1/Pure1_1_1/models/fixed_reference.py
-pypureclient/pure1/Pure1_1_1/models/fixed_reference2.py
 pypureclient/pure1/Pure1_1_1/models/fixed_reference_fqdn.py
 pypureclient/pure1/Pure1_1_1/models/hardware.py
 pypureclient/pure1/Pure1_1_1/models/hardware_connector.py
 pypureclient/pure1/Pure1_1_1/models/hardware_connector_get_response.py
 pypureclient/pure1/Pure1_1_1/models/hardware_connector_response.py
 pypureclient/pure1/Pure1_1_1/models/hardware_get_response.py
 pypureclient/pure1/Pure1_1_1/models/hardware_response.py
```

### Comparing `py-pure-client-1.8.0/pypureclient/api_token_manager.py` & `py-pure-client-1.9.0/pypureclient/api_token_manager.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/authorization_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/authorization_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/connections_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/connections_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/host_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/host_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/hosts_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/hosts_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/volume_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/volume_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api/volumes_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api/volumes_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/api_client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/api_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/configuration.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/configuration.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/api_version_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/api_version_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/built_in.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/built_in.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/chap.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/chap.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/connection.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/connection.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/connection_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/connection_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/connection_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/connection_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/connection_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/connection_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/destroyed_patch_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/destroyed_patch_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/fixed_reference.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/fixed_reference.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/fixed_reference_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/fixed_reference_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_port_connectivity.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_port_connectivity.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/host_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/host_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/inline_response400.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/inline_response401.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/inline_response401.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/member.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/member.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/member_no_id_all_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/new_name.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/new_name.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/oauth_token_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/oauth_token_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/page_info.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/page_info.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/qos.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/qos.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/reference.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/reference.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/reference_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/reference_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_by_array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_by_array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_by_array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_by_array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_performance_no_id_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/resource_space_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/resource_space_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/username.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/username.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/username_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/username_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_common.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_common.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/models/volume_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/models/volume_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_0/rest.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_0/rest.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/api_clients_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/api_clients_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/authorization_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/authorization_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/connections_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/connections_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/host_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/host_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/hosts_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/hosts_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/offloads_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/offloads_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/pods_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/pods_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/protection_group_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/protection_group_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/protection_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/protection_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/remote_pods_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/remote_pods_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/remote_protection_group_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/remote_protection_group_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/remote_protection_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/remote_protection_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/remote_volume_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/remote_volume_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/volume_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/volume_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/volume_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/volume_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api/volumes_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api/volumes_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/api_client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/api_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/configuration.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/configuration.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/aggregate_replication_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/aggregate_replication_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_client_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_client_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_client_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_client_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_client_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_client_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_client_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_client_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/api_version_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/api_version_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/built_in.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/built_in.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/built_in_resource_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/built_in_resource_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/chap.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/chap.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/connection.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/connection.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/connection_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/connection_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/connection_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/connection_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/connection_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/connection_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/destroyed_patch_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/destroyed_patch_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/fixed_reference.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/fixed_reference.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/fixed_reference_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/fixed_reference_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_group_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_group_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_port_connectivity.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_port_connectivity.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/host_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/host_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/inline_response400.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/inline_response401.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/inline_response401.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_no_id_all_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_no_id_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_no_id_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/member_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/member_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/new_name.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/new_name.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/oauth_token_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/oauth_token_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_azure.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_azure.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_nfs.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_nfs.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/offload_s3.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/offload_s3.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/page_info.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/page_info.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_array_status.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_array_status.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/pod_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/pod_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_array_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_array_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_performance_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_target.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_target.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_target_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_target_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/protection_group_target_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/protection_group_target_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/qos.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/qos.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/reference.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/reference.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/reference_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/reference_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_pod.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_pod.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_pods_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_pods_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_protection_group_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/remote_volume_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/replication_schedule.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/replication_schedule.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_by_array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_by_array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_by_array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_by_array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_performance_no_id_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_space_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_space_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_space_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_space_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/resource_space_no_id_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/resource_space_no_id_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/retention_policy.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/retention_policy.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/snapshot_schedule.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/target_protection_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/target_protection_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/target_protection_group_post_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/target_protection_group_post_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/time_window.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/time_window.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/username.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/username.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/username_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/username_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_common.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_common.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_group_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_group_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/models/volume_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/models/volume_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_1/rest.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_1/rest.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/administrators_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/administrators_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/alerts_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/alerts_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/api_clients_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/api_clients_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/apps_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/apps_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/arrays_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/arrays_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/audits_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/audits_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/authorization_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/authorization_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/connections_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/connections_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/controllers_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/controllers_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/directory_services_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/directory_services_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/dns_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/dns_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/hardware_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/hardware_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/host_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/host_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/hosts_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/hosts_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/kmip_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/kmip_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/maintenance_windows_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/maintenance_windows_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/offloads_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/offloads_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/pod_replica_links_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/pod_replica_links_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/pods_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/pods_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/ports_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/ports_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/protection_group_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/protection_group_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/protection_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/protection_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/remote_pods_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/remote_pods_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/remote_protection_group_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/remote_protection_group_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/remote_protection_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/remote_protection_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/remote_volume_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/remote_volume_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/smi_s_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/smi_s_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/software_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/software_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/subnets_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/subnets_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/support_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/support_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/volume_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/volume_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/volume_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/volume_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api/volumes_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api/volumes_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/api_client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/api_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/configuration.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/configuration.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_api_token.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_api_token.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_api_token_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_api_token_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_api_token_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_api_token_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_cache.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_cache.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_cache_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_cache_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_cache_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_cache_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_role.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_role.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_settings.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_settings.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/admin_settings_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/admin_settings_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/aggregate_replication_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/aggregate_replication_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert_event.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert_event.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert_event_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert_event_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert_event_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert_event_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/alert_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/alert_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_client_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_client_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_client_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_client_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_client_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_client_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_client_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_client_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_token.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_token.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/api_version_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/api_version_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app_node.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app_node.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app_node_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app_node_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app_node_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app_node_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/app_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/app_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_performance_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_performance_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/array_space_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/array_space_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/arrays.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/arrays.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/audit.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/audit.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/audit_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/audit_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/audit_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/audit_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/built_in.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/built_in.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/built_in_relationship.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/built_in_relationship.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/built_in_resource_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/built_in_resource_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/chap.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/chap.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/connection.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/connection.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/connection_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/connection_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/connection_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/connection_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/connection_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/connection_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/controller.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/controller.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/controller_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/controller_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/controllers.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/controllers.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/destroyed_patch_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/destroyed_patch_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_management.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_management.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_role.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_role.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_role_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_role_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/directory_service_role_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/directory_service_role_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/dns.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/dns.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/dns_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/dns_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/dns_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/dns_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/dns_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/dns_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/eula.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/eula.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/eula_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/eula_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/eula_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/eula_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/eula_signature.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/eula_signature.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/fixed_name_resource_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/fixed_name_resource_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/fixed_reference.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/fixed_reference.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/fixed_reference_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/fixed_reference_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/hardware.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/hardware.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/hardware_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/hardware_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/hardware_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/hardware_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/hardware_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/hardware_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_group_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_group_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_port_connectivity.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_port_connectivity.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/host_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/host_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/inline_response400.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/inline_response401.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/inline_response401.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_test_result.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_test_result.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/kmip_test_result_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/kmip_test_result_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/maintenance_window.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/maintenance_window_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/maintenance_window_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/maintenance_windows_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/maintenance_windows_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/maintenance_windows_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/maintenance_windows_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_no_id_all_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_no_id_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_no_id_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/member_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/member_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/new_name.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/new_name.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/oauth_token_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/oauth_token_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_azure.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_azure.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_google_cloud.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_google_cloud.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_nfs.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_nfs.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/offload_s3.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/offload_s3.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/override_check.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/override_check.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/page_info.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/page_info.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_array_status.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_array_status.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_by_array_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_performance_replication_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_lag_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_performance_replication_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_replica_link_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/pod_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/pod_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/port.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/port.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/port_common.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/port_common.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/port_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/port_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/port_initiator.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/port_initiator.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/port_initiators_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/port_initiators_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_array_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_array_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_performance_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_target.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_target.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_target_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_target_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/protection_group_target_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/protection_group_target_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/qos.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/qos.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/reference.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/reference.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/reference_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/reference_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_pod.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_pod.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_pods_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_pods_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_protection_group_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/remote_volume_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/replica_link_lag.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/replica_link_lag.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/replica_link_performance_replication.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/replica_link_performance_replication.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/replication_performance_with_total.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/replication_performance_with_total.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/replication_schedule.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/replication_schedule.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_fixed_non_unique_name.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_fixed_non_unique_name.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_by_array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_by_array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_by_array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_by_array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_performance_no_id_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_pod_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_pod_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_pod_space_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_pod_space_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_space_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_space_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_space_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_space_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/resource_space_no_id_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/resource_space_no_id_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/retention_policy.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/retention_policy.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/smis.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/smis.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/smis_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/smis_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/smis_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/smis_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/snapshot_schedule.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_step.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_step.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_checks.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_checks.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installation_steps_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installations.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installations.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installations_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installations_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_installations_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_installations_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/software_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/software_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/start_end_time.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/start_end_time.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/subnet.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/subnet.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/subnet_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/subnet_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/subnet_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/subnet_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/subnet_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/subnet_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/subnet_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/subnet_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/support.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/support.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/support_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/support_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/support_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/support_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/support_remote_assist_paths.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/support_remote_assist_paths.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/support_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/support_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/tag.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/tag.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/tag_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/tag_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/tag_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/tag_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/target_protection_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/target_protection_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/target_protection_group_post_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/target_protection_group_post_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/test_result.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/test_result.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/test_result_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/test_result_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/test_result_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/test_result_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/test_result_with_resource.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/test_result_with_resource.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/test_result_with_resource_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/test_result_with_resource_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/time_window.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/time_window.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/username.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/username.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/username_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/username_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_common.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_common.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_group_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_group_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/models/volume_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/models/volume_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_2/rest.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_2/rest.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/active_directory_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/active_directory_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/administrators_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/administrators_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/alerts_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/alerts_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/api_clients_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/api_clients_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/apps_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/apps_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/arrays_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/arrays_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/audits_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/audits_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/authorization_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/authorization_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/connections_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/connections_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/controllers_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/controllers_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/directories_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/directories_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/directory_exports_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/directory_exports_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/directory_services_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/directory_services_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/directory_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/directory_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/dns_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/dns_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/file_systems_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/file_systems_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/hardware_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/hardware_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/host_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/host_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/hosts_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/hosts_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/kmip_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/kmip_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/maintenance_windows_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/maintenance_windows_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/offloads_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/offloads_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/pod_replica_links_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/pod_replica_links_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/pods_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/pods_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/policies_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/policies_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/ports_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/ports_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/protection_group_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/protection_group_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/protection_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/protection_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/remote_pods_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/remote_pods_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/remote_protection_group_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/remote_protection_group_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/remote_protection_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/remote_protection_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/remote_volume_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/remote_volume_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/smi_s_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/smi_s_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/software_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/software_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/subnets_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/subnets_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/support_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/support_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/volume_groups_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/volume_groups_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/volume_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/volume_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api/volumes_api.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api/volumes_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/api_client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/api_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/configuration.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/configuration.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/__init__.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/active_directory.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/active_directory.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/active_directory_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/active_directory_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/active_directory_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/active_directory_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/active_directory_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/active_directory_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_api_token.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_api_token.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_api_token_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_api_token_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_api_token_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_api_token_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_cache.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_cache.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_cache_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_cache_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_cache_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_cache_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_role.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_role.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_settings.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_settings.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/admin_settings_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/admin_settings_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/aggregate_replication_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/aggregate_replication_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert_event.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert_event.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert_event_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert_event_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert_event_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert_event_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/alert_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/alert_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_client_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_client_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_client_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_client_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_client_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_client_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_client_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_client_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_token.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_token.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/api_version_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/api_version_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app_node.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app_node.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app_node_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app_node_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app_node_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app_node_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/app_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/app_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_performance_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_performance_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/array_space_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/array_space_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/arrays.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/arrays.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/audit.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/audit.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/audit_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/audit_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/audit_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/audit_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/built_in.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/built_in.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/built_in_relationship.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/built_in_relationship.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/built_in_resource_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/built_in_resource_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/chap.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/chap.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/connection.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/connection.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/connection_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/connection_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/connection_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/connection_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/connection_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/connection_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/controller.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/controller.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/controller_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/controller_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/controllers.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/controllers.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/destroyed_patch_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/destroyed_patch_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_export.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_export.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_export_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_export_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_export_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_export_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_export_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_export_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_performance_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_performance_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_policy_export_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_policy_export_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_policy_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_policy_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_management.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_management.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_role.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_role.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_role_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_role_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_service_role_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_service_role_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directory_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directory_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directorypolicyexportpost_policies.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directorypolicyexportpost_policies.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/directorypolicypost_policies.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/directorypolicypost_policies.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/dns.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/dns.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/dns_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/dns_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/dns_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/dns_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/dns_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/dns_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/eula.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/eula.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/eula_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/eula_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/eula_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/eula_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/eula_signature.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/eula_signature.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/file_system.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/file_system.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/file_system_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/file_system_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/file_system_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/file_system_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/file_system_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/file_system_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/fixed_name_resource_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/fixed_name_resource_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/fixed_reference.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/fixed_reference.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/fixed_reference_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/fixed_reference_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/fixed_reference_with_type.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/fixed_reference_with_type.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/hardware.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/hardware.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/hardware_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/hardware_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/hardware_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/hardware_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/hardware_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/hardware_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_group_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_group_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_port_connectivity.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_port_connectivity.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/host_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/host_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/inline_response400.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/inline_response401.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/inline_response401.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_test_result.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_test_result.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/kmip_test_result_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/kmip_test_result_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/maintenance_window.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/maintenance_window.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/maintenance_window_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/maintenance_window_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/maintenance_windows_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/maintenance_windows_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/maintenance_windows_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/maintenance_windows_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_no_id_all_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_no_id_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_no_id_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/member_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/member_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/new_name.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/new_name.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/oauth_token_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/oauth_token_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_azure.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_azure.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_google_cloud.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_google_cloud.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_nfs.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_nfs.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/offload_s3.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/offload_s3.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/override_check.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/override_check.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/page_info.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/page_info.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_array_status.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_array_status.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_by_array_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_performance_replication_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_lag_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_performance_replication_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_replica_link_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/pod_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/pod_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_export.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_export.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_export_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_member_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_member_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_nfs_client_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_smb_client_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policy_rule_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policymemberexportpost_members.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policymemberexportpost_members.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policymemberpost_members.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policymemberpost_members.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policyrulenfsclientpost_rules.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policyrulenfsclientpost_rules.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policyrulesmbclientpost_rules.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policyrulesmbclientpost_rules.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/policyrulesnapshotpost_rules.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/policyrulesnapshotpost_rules.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/port.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/port.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/port_common.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/port_common.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/port_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/port_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/port_initiator.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/port_initiator.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/port_initiators_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/port_initiators_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_array_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_array_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_performance_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_target.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_target.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_target_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_target_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/protection_group_target_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/protection_group_target_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/qos.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/qos.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/reference.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/reference.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/reference_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/reference_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/reference_with_type.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/reference_with_type.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_pod.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_pod.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_pods_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_pods_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_protection_group_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/remote_volume_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/replica_link_lag.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/replica_link_lag.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/replica_link_performance_replication.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/replica_link_performance_replication.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/replication_performance_with_total.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/replication_performance_with_total.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/replication_schedule.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/replication_schedule.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_fixed_non_unique_name.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_fixed_non_unique_name.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_by_array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_by_array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_by_array_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_by_array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_performance_no_id_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_pod_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_pod_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_pod_space_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_pod_space_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_space_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_space_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_space_no_id.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_space_no_id.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/resource_space_no_id_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/resource_space_no_id_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/retention_policy.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/retention_policy.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/smis.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/smis.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/smis_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/smis_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/smis_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/smis_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/snapshot_schedule.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/snapshot_schedule.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_step.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_step.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_checks.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_checks.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installation_steps_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installations.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installations.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installations_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installations_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_installations_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_installations_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/software_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/software_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/start_end_time.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/start_end_time.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/subnet.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/subnet.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/subnet_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/subnet_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/subnet_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/subnet_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/subnet_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/subnet_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/subnet_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/subnet_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/support.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/support.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/support_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/support_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/support_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/support_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/support_remote_assist_paths.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/support_remote_assist_paths.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/support_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/support_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/tag.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/tag.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/tag_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/tag_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/tag_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/tag_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/target_protection_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/target_protection_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/target_protection_group_post_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/target_protection_group_post_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/test_result.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/test_result.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/test_result_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/test_result_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/test_result_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/test_result_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/test_result_with_resource.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/test_result_with_resource.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/test_result_with_resource_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/test_result_with_resource_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/time_window.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/time_window.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/username.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/username.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/username_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/username_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_common.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_common.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_group_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_group_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_performance.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_performance.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_performance_by_array.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_performance_by_array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_patch.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_patch.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_post.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_post.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer_get_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer_response.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_snapshot_transfer_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/models/volume_space.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/models/volume_space.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/FA_2_3/rest.py` & `py-pure-client-1.9.0/pypureclient/flasharray/FA_2_3/rest.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/flasharray/client.py` & `py-pure-client-1.9.0/pypureclient/flasharray/client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/keywords.py` & `py-pure-client-1.9.0/pypureclient/keywords.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/properties.py` & `py-pure-client-1.9.0/pypureclient/properties.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/__init__.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .models.array import Array
 from .models.audit import Audit
 from .models.blade import Blade
 from .models.blade_array_status import BladeArrayStatus
 from .models.bucket import Bucket
 from .models.bucket_replica_link import BucketReplicaLink
 from .models.controller import Controller
+from .models.directory import Directory
 from .models.drive import Drive
 from .models.drive_array_status import DriveArrayStatus
 from .models.error import Error
 from .models.error_errors import ErrorErrors
 from .models.error_no_context import ErrorNoContext
 from .models.file_system import FileSystem
 from .models.file_system_replica_link import FileSystemReplicaLink
@@ -63,14 +64,15 @@
     Array,
     Audit,
     Blade,
     BladeArrayStatus,
     Bucket,
     BucketReplicaLink,
     Controller,
+    Directory,
     Drive,
     DriveArrayStatus,
     Error,
     ErrorErrors,
     ErrorNoContext,
     FileSystem,
     FileSystemReplicaLink,
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/__init__.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .arrays_api import ArraysApi
 from .audits_api import AuditsApi
 from .authorization_api import AuthorizationApi
 from .blades_api import BladesApi
 from .bucket_replica_links_api import BucketReplicaLinksApi
 from .buckets_api import BucketsApi
 from .controllers_api import ControllersApi
+from .directories_api import DirectoriesApi
 from .drives_api import DrivesApi
 from .file_system_replica_links_api import FileSystemReplicaLinksApi
 from .file_system_snapshots_api import FileSystemSnapshotsApi
 from .file_systems_api import FileSystemsApi
 from .hardware_api import HardwareApi
 from .hardware_connectors_api import HardwareConnectorsApi
 from .metrics_api import MetricsApi
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/alerts_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/alerts_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/arrays_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/arrays_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/audits_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/audits_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/authorization_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/authorization_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/blades_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/blades_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/bucket_replica_links_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/bucket_replica_links_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/buckets_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/buckets_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/controllers_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/controllers_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/drives_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/drives_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/file_system_replica_links_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/file_system_replica_links_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         target_names=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.FileSystemReplicaLinkGetResponse
-        """Get file system replica links
+        """Get FlashBlade file system replica links
 
         Retrieves information about FlashBlade file system replica links. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api10_file_system_replica_links_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
@@ -211,17 +211,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get file system replica link / policy pairs
+        """Get FlashBlade file system replica link / policy pairs
 
-        Retrieves pairs of file system replica link members and their policies. 
+        Retrieves pairs of FlashBlade file system replica link members and their policies. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api10_file_system_replica_links_policies_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/file_system_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/file_system_snapshots_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Pure1 Public REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: 1.0
+    OpenAPI spec version: 1.1
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -22,15 +22,15 @@
 from .. import models
 
 class FileSystemSnapshotsApi(object):
 
     def __init__(self, api_client):
         self.api_client = api_client
 
-    def api10_file_system_snapshots_get_with_http_info(
+    def api11_file_system_snapshots_get_with_http_info(
         self,
         authorization=None,  # type: str
         x_request_id=None,  # type: str
         continuation_token=None,  # type: str
         filter=None,  # type: str
         ids=None,  # type: List[str]
         limit=None,  # type: int
@@ -41,20 +41,20 @@
         source_names=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.FileSystemSnapshotGetResponse
-        """Get file system snapshots
+        """Get FlashBlade file system snapshots
 
-        Retrieves snapshots of file systems. 
+        Retrieves snapshots of FlashBlade file systems. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.api10_file_system_snapshots_get_with_http_info(async_req=True)
+        >>> thread = api.api11_file_system_snapshots_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
         :param str continuation_token: An opaque token used to iterate over a collection. The token to use on the next request is returned in the `continuation_token` field of the result. Single quotes are required around all strings.
         :param str filter: Exclude resources that don't match the specified criteria. Single quotes are required around all strings inside the filters.
         :param list[str] ids: A comma-separated list of resource IDs. If there is not at least one resource that matches each `id` element, an error is returned. Single quotes are required around all strings.
@@ -98,15 +98,15 @@
         # Convert the filter into a string
         if params.get('filter'):
             params['filter'] = str(params['filter'])
         if params.get('sort'):
             params['sort'] = [str(_x) for _x in params['sort']]
 
         if 'offset' in params and params['offset'] < 0:
-            raise ValueError("Invalid value for parameter `offset` when calling `api10_file_system_snapshots_get`, must be a value greater than or equal to `0`")
+            raise ValueError("Invalid value for parameter `offset` when calling `api11_file_system_snapshots_get`, must be a value greater than or equal to `0`")
         collection_formats = {}
         path_params = {}
 
         query_params = []
         if 'continuation_token' in params:
             query_params.append(('continuation_token', params['continuation_token']))
         if 'filter' in params:
@@ -149,15 +149,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(
             ['application/json'])
 
         # Authentication setting
         auth_settings = ['AuthorizationHeader']
 
         return self.api_client.call_api(
-            '/api/1.0/file-system-snapshots', 'GET',
+            '/api/1.1/file-system-snapshots', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='FileSystemSnapshotGetResponse',
@@ -165,15 +165,15 @@
             async_req=async_req,
             _return_http_data_only=_return_http_data_only,
             _preload_content=_preload_content,
             _request_timeout=_request_timeout,
             collection_formats=collection_formats,
         )
 
-    def api10_file_system_snapshots_policies_get_with_http_info(
+    def api11_file_system_snapshots_policies_get_with_http_info(
         self,
         authorization=None,  # type: str
         x_request_id=None,  # type: str
         continuation_token=None,  # type: str
         filter=None,  # type: str
         limit=None,  # type: int
         member_ids=None,  # type: List[str]
@@ -184,20 +184,20 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get file system snapshot / policy pairs
+        """Get FlashBlade file system snapshot / policy pairs
 
-        Retrieves pairs of file system snapshot members and their policies. 
+        Retrieves pairs of FlashBlade file system snapshot members and their policies. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.api10_file_system_snapshots_policies_get_with_http_info(async_req=True)
+        >>> thread = api.api11_file_system_snapshots_policies_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
         :param str continuation_token: An opaque token used to iterate over a collection. The token to use on the next request is returned in the `continuation_token` field of the result. Single quotes are required around all strings.
         :param str filter: Exclude resources that don't match the specified criteria. Single quotes are required around all strings inside the filters.
         :param int limit: Limit the size of the response to the specified number of resources. A limit of 0 can be used to get the number of resources without getting all of the resources. It will be returned in the total_item_count field. If a client asks for a page size larger than the maximum number, the request is still valid. In that case the server just returns the maximum number of items, disregarding the client's page size request. If not specified, defaults to 1000.
@@ -241,15 +241,15 @@
         # Convert the filter into a string
         if params.get('filter'):
             params['filter'] = str(params['filter'])
         if params.get('sort'):
             params['sort'] = [str(_x) for _x in params['sort']]
 
         if 'offset' in params and params['offset'] < 0:
-            raise ValueError("Invalid value for parameter `offset` when calling `api10_file_system_snapshots_policies_get`, must be a value greater than or equal to `0`")
+            raise ValueError("Invalid value for parameter `offset` when calling `api11_file_system_snapshots_policies_get`, must be a value greater than or equal to `0`")
         collection_formats = {}
         path_params = {}
 
         query_params = []
         if 'continuation_token' in params:
             query_params.append(('continuation_token', params['continuation_token']))
         if 'filter' in params:
@@ -292,15 +292,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(
             ['application/json'])
 
         # Authentication setting
         auth_settings = ['AuthorizationHeader']
 
         return self.api_client.call_api(
-            '/api/1.0/file-system-snapshots/policies', 'GET',
+            '/api/1.1/file-system-snapshots/policies', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='PolicyMembersGetResponse',
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/file_systems_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/file_systems_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.FileSystemGetResponse
-        """Get file systems
+        """Get FlashArray and FlashBlade file systems
 
-        Retrieves information about file system objects. 
+        Retrieves information about FlashArray and FlashBlade file system objects. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api10_file_systems_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
@@ -166,17 +166,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get file system / policy pairs
+        """Get FlashBlade file system / policy pairs
 
-        Retrieves pairs of file system members and their policies. 
+        Retrieves pairs of FlashBlade file system members and their policies. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api10_file_systems_policies_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/hardware_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/hardware_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/hardware_connectors_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/hardware_connectors_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/metrics_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/network_interfaces_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/network_interfaces_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/object_store_accounts_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/object_store_accounts_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/pod_replica_links_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/pod_replica_links_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/pods_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/pods_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/policies_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/policies_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get policy / file system replica link pairs
+        """Get policy / FlashBlade file system replica link pairs
 
-        Retrieves pairs of policy references and their file system replica link members. 
+        Retrieves pairs of policy references and their FlashBlade file system replica link members. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api10_policies_file_system_replica_links_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
@@ -184,17 +184,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get policy / file system snapshot pairs
+        """Get policy / FlashBlade file system snapshot pairs
 
-        Retrieves pairs of policy references and their file system snapshot members. 
+        Retrieves pairs of policy references and their FlashBlade file system snapshot members. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api10_policies_file_system_snapshots_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
@@ -327,17 +327,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get policy / file system pairs
+        """Get policy / FlashBlade file system pairs
 
-        Retrieves pairs of policy references and their file system members. 
+        Retrieves pairs of policy references and their FlashBlade file system members. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api10_policies_file_systems_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/ports_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/ports_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/targets_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/targets_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/volume_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/volume_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api/volumes_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/volumes_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/api_client.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/client.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     PRIVATE_KEY_PASSWORD_ENV = 'PURE1_PRIVATE_KEY_PASSWORD'
     RETRIES_KEY = 'retries'
     RETRIES_DEFAULT = 5
     TOKEN_ENDPOINT = 'https://api.pure1.purestorage.com/oauth2/1.0/token'
     TIMEOUT_KEY = 'timeout'
     TIMEOUT_DEFAULT = 15.0
     # Format: client/client_version/endpoint/endpoint_version/system/release
-    USER_AGENT = ('pypureclient/1.7.0/Pure1/1.0/{sys}/{rel}'
+    USER_AGENT = ('pypureclient/1.9.0/Pure1/1.0/{sys}/{rel}'
                   .format(sys=platform.system(), rel=platform.release()))
 
     def __init__(self, **kwargs):
         """
         Initialize a Pure1 Client.
 
         Keyword args:
@@ -94,14 +94,15 @@
         self._alerts_api = api.AlertsApi(self._api_client)
         self._arrays_api = api.ArraysApi(self._api_client)
         self._audits_api = api.AuditsApi(self._api_client)
         self._blades_api = api.BladesApi(self._api_client)
         self._bucket_replica_links_api = api.BucketReplicaLinksApi(self._api_client)
         self._buckets_api = api.BucketsApi(self._api_client)
         self._controllers_api = api.ControllersApi(self._api_client)
+        self._directories_api = api.DirectoriesApi(self._api_client)
         self._drives_api = api.DrivesApi(self._api_client)
         self._file_system_replica_links_api = api.FileSystemReplicaLinksApi(self._api_client)
         self._file_system_snapshots_api = api.FileSystemSnapshotsApi(self._api_client)
         self._file_systems_api = api.FileSystemsApi(self._api_client)
         self._hardware_api = api.HardwareApi(self._api_client)
         self._hardware_connectors_api = api.HardwareConnectorsApi(self._api_client)
         self._metrics_api = api.MetricsApi(self._api_client)
@@ -1094,14 +1095,115 @@
             _request_timeout=_request_timeout,
         )
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         endpoint = self._controllers_api.api10_controllers_get_with_http_info
         _process_references(references, ['ids', 'names'], kwargs)
         return self._call_api(endpoint, kwargs)
 
+    def get_directories(
+        self,
+        file_systems=None,  # type: List[models.ReferenceType]
+        references=None,  # type: List[models.ReferenceType]
+        authorization=None,  # type: str
+        x_request_id=None,  # type: str
+        continuation_token=None,  # type: str
+        file_system_ids=None,  # type: List[str]
+        file_system_names=None,  # type: List[str]
+        filter=None,  # type: str
+        ids=None,  # type: List[str]
+        limit=None,  # type: int
+        names=None,  # type: List[str]
+        offset=None,  # type: int
+        sort=None,  # type: List[str]
+        async_req=False,  # type: bool
+        _return_http_data_only=False,  # type: bool
+        _preload_content=True,  # type: bool
+        _request_timeout=None,  # type: Optional[int]
+    ):
+        # type: (...) -> models.DirectoryGetResponse
+        """
+        Retrieves information about FlashArray managed directory objects.
+
+        Args:
+            file_systems (list[FixedReference], optional):
+                A list of file_systems to query for. Overrides file_system_ids and file_system_names keyword arguments.
+            references (list[FixedReference], optional):
+                A list of references to query for. Overrides ids and names keyword arguments.
+
+            x_request_id (str, optional):
+                A header to provide to track the API call. Generated by the server if not
+                provided.
+            continuation_token (str, optional):
+                An opaque token to iterate over a collection of resources.
+            file_system_ids (list[str], optional):
+                Performs the operation on the file system ID specified. Enter multiple file
+                system IDs in comma-separated format. The `file_system_ids` and
+                `file_system_names` parameters cannot be provided together.
+            file_system_names (list[str], optional):
+                Performs the operation on the file system name specified. Enter multiple file
+                system names in comma-separated format. For example, `filesystem1,filesystem2`.
+                The `file_system_ids` and `file_system_names` parameters cannot be provided
+                together.
+            filter (Filter, optional):
+                A filter to include only resources that match the specified criteria.
+            ids (list[str], optional):
+                A list of resource IDs. If there is not at least one resource that matches each
+                `id` element, an error is returned.
+            limit (int, optional):
+                Limit the number of resources in the response. If not specified, defaults to
+                1000.
+            names (list[str], optional):
+                A list of resource names. If there is not at least one resource that matches
+                each `name` element, an error is returned.
+            offset (int, optional):
+                The offset of the first resource to return from a collection.
+            sort (list[Property], optional):
+                Sort the response by the specified Properties. Can also be a single element.
+            async_req (bool, optional):
+                Request runs in separate thread and method returns
+                multiprocessing.pool.ApplyResult.
+            _return_http_data_only (bool, optional):
+                Returns only data field.
+            _preload_content (bool, optional):
+                Response is converted into objects.
+            _request_timeout (int, optional):
+                Total request timeout in seconds.
+
+        Returns:
+            ValidResponse: If the call was successful.
+            ErrorResponse: If the call was not successful.
+
+        Raises:
+            PureError: If calling the API fails.
+            ValueError: If a parameter is of an invalid type.
+            TypeError: If invalid or missing parameters are used.
+        """
+        kwargs = dict(
+            authorization=authorization,
+            x_request_id=x_request_id,
+            continuation_token=continuation_token,
+            file_system_ids=file_system_ids,
+            file_system_names=file_system_names,
+            filter=filter,
+            ids=ids,
+            limit=limit,
+            names=names,
+            offset=offset,
+            sort=sort,
+            async_req=async_req,
+            _return_http_data_only=_return_http_data_only,
+            _preload_content=_preload_content,
+            _request_timeout=_request_timeout,
+        )
+        kwargs = {k: v for k, v in kwargs.items() if v is not None}
+        endpoint = self._directories_api.api10_directories_get_with_http_info
+        _process_references(file_systems, ['file_system_ids', 'file_system_names'], kwargs)
+        _process_references(references, ['ids', 'names'], kwargs)
+        return self._call_api(endpoint, kwargs)
+
     def get_drives(
         self,
         references=None,  # type: List[models.ReferenceType]
         authorization=None,  # type: str
         x_request_id=None,  # type: str
         continuation_token=None,  # type: str
         filter=None,  # type: str
@@ -1345,15 +1447,16 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of file system replica link members and their policies.
+        Retrieves pairs of FlashBlade file system replica link members and their
+        policies.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
 
@@ -1443,15 +1546,15 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.FileSystemSnapshotGetResponse
         """
-        Retrieves snapshots of file systems.
+        Retrieves snapshots of FlashBlade file systems.
 
         Args:
             references (list[FixedReference], optional):
                 A list of references to query for. Overrides ids and names keyword arguments.
             sources (list[FixedReference], optional):
                 A list of sources to query for. Overrides source_ids and source_names keyword arguments.
 
@@ -1541,15 +1644,15 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of file system snapshot members and their policies.
+        Retrieves pairs of FlashBlade file system snapshot members and their policies.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
 
@@ -1636,15 +1739,15 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.FileSystemGetResponse
         """
-        Retrieves information about file system objects.
+        Retrieves information about FlashArray and FlashBlade file system objects.
 
         Args:
             references (list[FixedReference], optional):
                 A list of references to query for. Overrides ids and names keyword arguments.
 
             x_request_id (str, optional):
                 A header to provide to track the API call. Generated by the server if not
@@ -1723,15 +1826,15 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of file system members and their policies.
+        Retrieves pairs of FlashBlade file system members and their policies.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
 
@@ -2571,15 +2674,16 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of policy references and their file system replica link members.
+        Retrieves pairs of policy references and their FlashBlade file system replica
+        link members.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
 
@@ -2669,15 +2773,16 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of policy references and their file system snapshot members.
+        Retrieves pairs of policy references and their FlashBlade file system snapshot
+        members.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
 
@@ -2767,15 +2872,15 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of policy references and their file system members.
+        Retrieves pairs of policy references and their FlashBlade file system members.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/configuration.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/configuration.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/__init__.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 from .bucket_replica_link import BucketReplicaLink
 from .bucket_replica_link_get_response import BucketReplicaLinkGetResponse
 from .bucket_replica_link_response import BucketReplicaLinkResponse
 from .bucket_response import BucketResponse
 from .controller import Controller
 from .controller_get_response import ControllerGetResponse
 from .controller_response import ControllerResponse
+from .directory import Directory
+from .directory_get_response import DirectoryGetResponse
+from .directory_response import DirectoryResponse
 from .drive import Drive
 from .drive_array_status import DriveArrayStatus
 from .drive_get_response import DriveGetResponse
 from .drive_response import DriveResponse
 from .error import Error
 from .error_errors import ErrorErrors
 from .error_no_context import ErrorNoContext
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/alert.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/alert.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/alerts_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/alerts_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/alerts_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/alerts_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/array.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/array_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/array_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/array_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/arrays.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/arrays.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/arrays_built_in.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/arrays_built_in.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/arrays_resource.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/arrays_resource.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/audit.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/audit.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/audits_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/audits_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/audits_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/audits_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/blade.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/blade.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/blade_array_status.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/blade_array_status.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/blade_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/blade_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/blade_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/blade_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket_replica_link_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/bucket_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/bucket_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/built_in_as_of.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/built_in_as_of.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/controller.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/controller.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/controller_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/controller_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/controller_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/controller_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/drive.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/drive.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/drive_array_status.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/drive_array_status.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/drive_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/drive_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/drive_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/drive_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/error.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/error.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/error_errors.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/error_errors.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/error_no_context.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/error_no_context.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,21 +84,21 @@
         Keyword args:
             as_of (int): The freshness of the data (timestamp in millis since epoch).
             id (str): A non-modifiable, globally unique ID chosen by the system.
             name (str): A non-modifiable, locally unique name chosen by the system.
             arrays (list[FixedReference]): The list of arrays where this resource exists. Many resources are on a single array, but some resources, such as pods, can be shared across multiple arrays.
             created (int): Creation time in milliseconds since UNIX epoch.
             destroyed (bool): Is the file system destroyed?
-            fast_remove_directory_enabled (bool): Is fast remove directory enabled?
-            hard_limit_enabled (bool): Is the file system's size a hard limit quota?
-            http (Http): HTTP configuration.
-            nfs (Nfs): NFS configuration.
-            provisioned (int): The provisioned size of the file system in bytes. A value of 0 means unlimited.
-            smb (Smb): SMB configuration.
-            snapshot_directory_enabled (bool): Is snapshot directory enabled?
+            fast_remove_directory_enabled (bool): On a FlashBlade file system, returns the value of `true` if fast remove directory is enabled and `false` if it is not. On a FlashArray file system, the value is always `null`.
+            hard_limit_enabled (bool): On a FlashBlade file system, returns the value of `true` if the file system's size is a hard limit quota and `false` if it is not. On a FlashArray file system, the value is always `null`.
+            http (Http): HTTP configuration. On a FlashArray file system, the value is always `null`.
+            nfs (Nfs): NFS configuration. On a FlashArray file system, the value is always `null`.
+            provisioned (int): The provisioned size of the file system in bytes. A value of 0 means unlimited. On a FlashArray file system, the value is always `null`.
+            smb (Smb): SMB configuration. On a FlashArray file system, the value is always `null`.
+            snapshot_directory_enabled (bool): On a FlashBlade file system, returns the value of `true` if snapshot directory is enabled and `false` if it is not. On a FlashArray file system, the value is always `null`.
         """
         if as_of is not None:
             self.as_of = as_of
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_replica_link_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/file_system_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/fixed_reference.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/fixed_reference.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware_connector_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/hardware_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/hardware_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/http.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/http.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/inline_response400.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/inline_response401.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/inline_response401.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_availability.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_availability.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_history.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_history.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_history_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_history_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_history_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_history_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/metric_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/metric_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/network_interface.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/network_interface.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/network_interface_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/network_interface_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/network_interface_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/network_interface_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/nfs.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/nfs.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/oauth_token_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/oauth_token_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/object_store_account.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/object_store_account.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/object_store_account_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/object_store_account_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/object_store_account_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/object_store_account_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/page_info.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/page_info.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_array_status.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_array_status.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_replica_link_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/pod_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/pod_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_member.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_member.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_members_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_members_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_members_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_members_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/policy_rule.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/policy_rule.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/port.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/port.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/port_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/port_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/port_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/port_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/replica_link.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/replica_link.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/resource.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/resource.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/resource_no_name.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/resource_no_name.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/resource_with_location.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/resource_with_location.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/resource_with_locations.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/resource_with_locations.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/smb.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/smb.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/support_contract.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/support_contract.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/support_contract_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/support_contract_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/support_contract_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/support_contract_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/tag.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/tag.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/tag_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/tag_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/tag_put.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/tag_put.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/tag_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/tag_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/target.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/target.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/target_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/target_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/target_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/target_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/time_aware.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/time_aware.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/volume_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_0/rest.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/rest.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/__init__.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 from .models.array import Array
 from .models.audit import Audit
 from .models.blade import Blade
 from .models.blade_array_status import BladeArrayStatus
 from .models.bucket import Bucket
 from .models.bucket_replica_link import BucketReplicaLink
 from .models.controller import Controller
+from .models.directory import Directory
 from .models.drive import Drive
 from .models.drive_array_status import DriveArrayStatus
 from .models.error import Error
 from .models.error_errors import ErrorErrors
 from .models.error_no_context import ErrorNoContext
 from .models.file_system import FileSystem
 from .models.file_system_replica_link import FileSystemReplicaLink
 from .models.file_system_snapshot import FileSystemSnapshot
 from .models.fixed_reference import FixedReference
-from .models.fixed_reference2 import FixedReference2
 from .models.fixed_reference_fqdn import FixedReferenceFqdn
 from .models.hardware import Hardware
 from .models.hardware_connector import HardwareConnector
 from .models.http import Http
 from .models.metric import Metric
 from .models.metric_availability import MetricAvailability
 from .models.metric_history import MetricHistory
@@ -65,24 +65,24 @@
     Array,
     Audit,
     Blade,
     BladeArrayStatus,
     Bucket,
     BucketReplicaLink,
     Controller,
+    Directory,
     Drive,
     DriveArrayStatus,
     Error,
     ErrorErrors,
     ErrorNoContext,
     FileSystem,
     FileSystemReplicaLink,
     FileSystemSnapshot,
     FixedReference,
-    FixedReference2,
     FixedReferenceFqdn,
     Hardware,
     HardwareConnector,
     Http,
     Metric,
     MetricAvailability,
     MetricHistory,
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/__init__.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from .arrays_api import ArraysApi
 from .audits_api import AuditsApi
 from .authorization_api import AuthorizationApi
 from .blades_api import BladesApi
 from .bucket_replica_links_api import BucketReplicaLinksApi
 from .buckets_api import BucketsApi
 from .controllers_api import ControllersApi
+from .directories_api import DirectoriesApi
 from .drives_api import DrivesApi
 from .file_system_replica_links_api import FileSystemReplicaLinksApi
 from .file_system_snapshots_api import FileSystemSnapshotsApi
 from .file_systems_api import FileSystemsApi
 from .hardware_api import HardwareApi
 from .hardware_connectors_api import HardwareConnectorsApi
 from .metrics_api import MetricsApi
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/alerts_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/alerts_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/arrays_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/arrays_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/audits_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/audits_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/authorization_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/authorization_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/blades_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/blades_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/bucket_replica_links_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/bucket_replica_links_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/buckets_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/buckets_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/controllers_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/controllers_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/drives_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/drives_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/file_system_replica_links_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/file_system_replica_links_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         target_names=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.FileSystemReplicaLinkGetResponse
-        """Get file system replica links
+        """Get FlashBlade file system replica links
 
         Retrieves information about FlashBlade file system replica links. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api11_file_system_replica_links_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
@@ -211,17 +211,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get file system replica link / policy pairs
+        """Get FlashBlade file system replica link / policy pairs
 
-        Retrieves pairs of file system replica link members and their policies. 
+        Retrieves pairs of FlashBlade file system replica link members and their policies. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api11_file_system_replica_links_policies_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/file_system_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/api/file_system_snapshots_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Pure1 Public REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: 1.1
+    OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 from __future__ import absolute_import
 
@@ -22,15 +22,15 @@
 from .. import models
 
 class FileSystemSnapshotsApi(object):
 
     def __init__(self, api_client):
         self.api_client = api_client
 
-    def api11_file_system_snapshots_get_with_http_info(
+    def api10_file_system_snapshots_get_with_http_info(
         self,
         authorization=None,  # type: str
         x_request_id=None,  # type: str
         continuation_token=None,  # type: str
         filter=None,  # type: str
         ids=None,  # type: List[str]
         limit=None,  # type: int
@@ -41,20 +41,20 @@
         source_names=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.FileSystemSnapshotGetResponse
-        """Get file system snapshots
+        """Get FlashBlade file system snapshots
 
-        Retrieves snapshots of file systems. 
+        Retrieves snapshots of FlashBlade file systems. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.api11_file_system_snapshots_get_with_http_info(async_req=True)
+        >>> thread = api.api10_file_system_snapshots_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
         :param str continuation_token: An opaque token used to iterate over a collection. The token to use on the next request is returned in the `continuation_token` field of the result. Single quotes are required around all strings.
         :param str filter: Exclude resources that don't match the specified criteria. Single quotes are required around all strings inside the filters.
         :param list[str] ids: A comma-separated list of resource IDs. If there is not at least one resource that matches each `id` element, an error is returned. Single quotes are required around all strings.
@@ -98,15 +98,15 @@
         # Convert the filter into a string
         if params.get('filter'):
             params['filter'] = str(params['filter'])
         if params.get('sort'):
             params['sort'] = [str(_x) for _x in params['sort']]
 
         if 'offset' in params and params['offset'] < 0:
-            raise ValueError("Invalid value for parameter `offset` when calling `api11_file_system_snapshots_get`, must be a value greater than or equal to `0`")
+            raise ValueError("Invalid value for parameter `offset` when calling `api10_file_system_snapshots_get`, must be a value greater than or equal to `0`")
         collection_formats = {}
         path_params = {}
 
         query_params = []
         if 'continuation_token' in params:
             query_params.append(('continuation_token', params['continuation_token']))
         if 'filter' in params:
@@ -149,15 +149,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(
             ['application/json'])
 
         # Authentication setting
         auth_settings = ['AuthorizationHeader']
 
         return self.api_client.call_api(
-            '/api/1.1/file-system-snapshots', 'GET',
+            '/api/1.0/file-system-snapshots', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='FileSystemSnapshotGetResponse',
@@ -165,15 +165,15 @@
             async_req=async_req,
             _return_http_data_only=_return_http_data_only,
             _preload_content=_preload_content,
             _request_timeout=_request_timeout,
             collection_formats=collection_formats,
         )
 
-    def api11_file_system_snapshots_policies_get_with_http_info(
+    def api10_file_system_snapshots_policies_get_with_http_info(
         self,
         authorization=None,  # type: str
         x_request_id=None,  # type: str
         continuation_token=None,  # type: str
         filter=None,  # type: str
         limit=None,  # type: int
         member_ids=None,  # type: List[str]
@@ -184,20 +184,20 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get file system snapshot / policy pairs
+        """Get FlashBlade file system snapshot / policy pairs
 
-        Retrieves pairs of file system snapshot members and their policies. 
+        Retrieves pairs of FlashBlade file system snapshot members and their policies. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
-        >>> thread = api.api11_file_system_snapshots_policies_get_with_http_info(async_req=True)
+        >>> thread = api.api10_file_system_snapshots_policies_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
         :param str continuation_token: An opaque token used to iterate over a collection. The token to use on the next request is returned in the `continuation_token` field of the result. Single quotes are required around all strings.
         :param str filter: Exclude resources that don't match the specified criteria. Single quotes are required around all strings inside the filters.
         :param int limit: Limit the size of the response to the specified number of resources. A limit of 0 can be used to get the number of resources without getting all of the resources. It will be returned in the total_item_count field. If a client asks for a page size larger than the maximum number, the request is still valid. In that case the server just returns the maximum number of items, disregarding the client's page size request. If not specified, defaults to 1000.
@@ -241,15 +241,15 @@
         # Convert the filter into a string
         if params.get('filter'):
             params['filter'] = str(params['filter'])
         if params.get('sort'):
             params['sort'] = [str(_x) for _x in params['sort']]
 
         if 'offset' in params and params['offset'] < 0:
-            raise ValueError("Invalid value for parameter `offset` when calling `api11_file_system_snapshots_policies_get`, must be a value greater than or equal to `0`")
+            raise ValueError("Invalid value for parameter `offset` when calling `api10_file_system_snapshots_policies_get`, must be a value greater than or equal to `0`")
         collection_formats = {}
         path_params = {}
 
         query_params = []
         if 'continuation_token' in params:
             query_params.append(('continuation_token', params['continuation_token']))
         if 'filter' in params:
@@ -292,15 +292,15 @@
         header_params['Content-Type'] = self.api_client.select_header_content_type(
             ['application/json'])
 
         # Authentication setting
         auth_settings = ['AuthorizationHeader']
 
         return self.api_client.call_api(
-            '/api/1.1/file-system-snapshots/policies', 'GET',
+            '/api/1.0/file-system-snapshots/policies', 'GET',
             path_params,
             query_params,
             header_params,
             body=body_params,
             post_params=form_params,
             files=local_var_files,
             response_type='PolicyMembersGetResponse',
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/file_systems_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/file_systems_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.FileSystemGetResponse
-        """Get file systems
+        """Get FlashArray and FlashBlade file systems
 
-        Retrieves information about FlashBlade file system objects. 
+        Retrieves information about FlashArray and FlashBlade file system objects. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api11_file_systems_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
@@ -166,17 +166,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get file system / policy pairs
+        """Get FlashBlade file system / policy pairs
 
-        Retrieves pairs of file system members and their policies. 
+        Retrieves pairs of FlashBlade file system members and their policies. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api11_file_systems_policies_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/hardware_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/hardware_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/hardware_connectors_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/hardware_connectors_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/metrics_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/metrics_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/network_interfaces_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/network_interfaces_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/object_store_accounts_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/object_store_accounts_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/pod_replica_links_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/pod_replica_links_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/pods_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/pods_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/policies_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/policies_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,17 +41,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get policy / file system replica link pairs
+        """Get policy / FlashBlade file system replica link pairs
 
-        Retrieves pairs of policy references and their file system replica link members. 
+        Retrieves pairs of policy references and their FlashBlade file system replica link members. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api11_policies_file_system_replica_links_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
@@ -184,17 +184,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get policy / file system snapshot pairs
+        """Get policy / FlashBlade file system snapshot pairs
 
-        Retrieves pairs of policy references and their file system snapshot members. 
+        Retrieves pairs of policy references and their FlashBlade file system snapshot members. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api11_policies_file_system_snapshots_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
@@ -327,17 +327,17 @@
         sort=None,  # type: List[str]
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
-        """Get policy / file system pairs
+        """Get policy / FlashBlade file system pairs
 
-        Retrieves pairs of policy references and their file system members. 
+        Retrieves pairs of policy references and their FlashBlade file system members. 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.api11_policies_file_systems_get_with_http_info(async_req=True)
         >>> result = thread.get()
 
         :param str authorization: Access token (in JWT format) required to use any API endpoint (except `/oauth2`)
         :param str x_request_id: Supplied by client during request or generated by server.
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/ports_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/ports_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/targets_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/targets_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/volume_snapshots_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/volume_snapshots_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api/volumes_api.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api/volumes_api.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/api_client.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/api_client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/client.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     PRIVATE_KEY_PASSWORD_ENV = 'PURE1_PRIVATE_KEY_PASSWORD'
     RETRIES_KEY = 'retries'
     RETRIES_DEFAULT = 5
     TOKEN_ENDPOINT = 'https://api.pure1.purestorage.com/oauth2/1.0/token'
     TIMEOUT_KEY = 'timeout'
     TIMEOUT_DEFAULT = 15.0
     # Format: client/client_version/endpoint/endpoint_version/system/release
-    USER_AGENT = ('pypureclient/1.7.0/Pure1/1.1/{sys}/{rel}'
+    USER_AGENT = ('pypureclient/1.9.0/Pure1/1.1/{sys}/{rel}'
                   .format(sys=platform.system(), rel=platform.release()))
 
     def __init__(self, **kwargs):
         """
         Initialize a Pure1 Client.
 
         Keyword args:
@@ -94,14 +94,15 @@
         self._alerts_api = api.AlertsApi(self._api_client)
         self._arrays_api = api.ArraysApi(self._api_client)
         self._audits_api = api.AuditsApi(self._api_client)
         self._blades_api = api.BladesApi(self._api_client)
         self._bucket_replica_links_api = api.BucketReplicaLinksApi(self._api_client)
         self._buckets_api = api.BucketsApi(self._api_client)
         self._controllers_api = api.ControllersApi(self._api_client)
+        self._directories_api = api.DirectoriesApi(self._api_client)
         self._drives_api = api.DrivesApi(self._api_client)
         self._file_system_replica_links_api = api.FileSystemReplicaLinksApi(self._api_client)
         self._file_system_snapshots_api = api.FileSystemSnapshotsApi(self._api_client)
         self._file_systems_api = api.FileSystemsApi(self._api_client)
         self._hardware_api = api.HardwareApi(self._api_client)
         self._hardware_connectors_api = api.HardwareConnectorsApi(self._api_client)
         self._metrics_api = api.MetricsApi(self._api_client)
@@ -1104,14 +1105,115 @@
             _request_timeout=_request_timeout,
         )
         kwargs = {k: v for k, v in kwargs.items() if v is not None}
         endpoint = self._controllers_api.api11_controllers_get_with_http_info
         _process_references(references, ['ids', 'names'], kwargs)
         return self._call_api(endpoint, kwargs)
 
+    def get_directories(
+        self,
+        file_systems=None,  # type: List[models.ReferenceType]
+        references=None,  # type: List[models.ReferenceType]
+        authorization=None,  # type: str
+        x_request_id=None,  # type: str
+        continuation_token=None,  # type: str
+        file_system_ids=None,  # type: List[str]
+        file_system_names=None,  # type: List[str]
+        filter=None,  # type: str
+        ids=None,  # type: List[str]
+        limit=None,  # type: int
+        names=None,  # type: List[str]
+        offset=None,  # type: int
+        sort=None,  # type: List[str]
+        async_req=False,  # type: bool
+        _return_http_data_only=False,  # type: bool
+        _preload_content=True,  # type: bool
+        _request_timeout=None,  # type: Optional[int]
+    ):
+        # type: (...) -> models.DirectoryGetResponse
+        """
+        Retrieves information about FlashArray managed directory objects.
+
+        Args:
+            file_systems (list[FixedReference], optional):
+                A list of file_systems to query for. Overrides file_system_ids and file_system_names keyword arguments.
+            references (list[FixedReference], optional):
+                A list of references to query for. Overrides ids and names keyword arguments.
+
+            x_request_id (str, optional):
+                A header to provide to track the API call. Generated by the server if not
+                provided.
+            continuation_token (str, optional):
+                An opaque token to iterate over a collection of resources.
+            file_system_ids (list[str], optional):
+                Performs the operation on the file system ID specified. Enter multiple file
+                system IDs in comma-separated format. The `file_system_ids` and
+                `file_system_names` parameters cannot be provided together.
+            file_system_names (list[str], optional):
+                Performs the operation on the file system name specified. Enter multiple file
+                system names in comma-separated format. For example, `filesystem1,filesystem2`.
+                The `file_system_ids` and `file_system_names` parameters cannot be provided
+                together.
+            filter (Filter, optional):
+                A filter to include only resources that match the specified criteria.
+            ids (list[str], optional):
+                A list of resource IDs. If there is not at least one resource that matches each
+                `id` element, an error is returned.
+            limit (int, optional):
+                Limit the number of resources in the response. If not specified, defaults to
+                1000.
+            names (list[str], optional):
+                A list of resource names. If there is not at least one resource that matches
+                each `name` element, an error is returned.
+            offset (int, optional):
+                The offset of the first resource to return from a collection.
+            sort (list[Property], optional):
+                Sort the response by the specified Properties. Can also be a single element.
+            async_req (bool, optional):
+                Request runs in separate thread and method returns
+                multiprocessing.pool.ApplyResult.
+            _return_http_data_only (bool, optional):
+                Returns only data field.
+            _preload_content (bool, optional):
+                Response is converted into objects.
+            _request_timeout (int, optional):
+                Total request timeout in seconds.
+
+        Returns:
+            ValidResponse: If the call was successful.
+            ErrorResponse: If the call was not successful.
+
+        Raises:
+            PureError: If calling the API fails.
+            ValueError: If a parameter is of an invalid type.
+            TypeError: If invalid or missing parameters are used.
+        """
+        kwargs = dict(
+            authorization=authorization,
+            x_request_id=x_request_id,
+            continuation_token=continuation_token,
+            file_system_ids=file_system_ids,
+            file_system_names=file_system_names,
+            filter=filter,
+            ids=ids,
+            limit=limit,
+            names=names,
+            offset=offset,
+            sort=sort,
+            async_req=async_req,
+            _return_http_data_only=_return_http_data_only,
+            _preload_content=_preload_content,
+            _request_timeout=_request_timeout,
+        )
+        kwargs = {k: v for k, v in kwargs.items() if v is not None}
+        endpoint = self._directories_api.api11_directories_get_with_http_info
+        _process_references(file_systems, ['file_system_ids', 'file_system_names'], kwargs)
+        _process_references(references, ['ids', 'names'], kwargs)
+        return self._call_api(endpoint, kwargs)
+
     def get_drives(
         self,
         references=None,  # type: List[models.ReferenceType]
         authorization=None,  # type: str
         x_request_id=None,  # type: str
         continuation_token=None,  # type: str
         filter=None,  # type: str
@@ -1355,15 +1457,16 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of file system replica link members and their policies.
+        Retrieves pairs of FlashBlade file system replica link members and their
+        policies.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
 
@@ -1453,15 +1556,15 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.FileSystemSnapshotGetResponse
         """
-        Retrieves snapshots of file systems.
+        Retrieves snapshots of FlashBlade file systems.
 
         Args:
             references (list[FixedReference], optional):
                 A list of references to query for. Overrides ids and names keyword arguments.
             sources (list[FixedReference], optional):
                 A list of sources to query for. Overrides source_ids and source_names keyword arguments.
 
@@ -1551,15 +1654,15 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of file system snapshot members and their policies.
+        Retrieves pairs of FlashBlade file system snapshot members and their policies.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
 
@@ -1646,15 +1749,15 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.FileSystemGetResponse
         """
-        Retrieves information about FlashBlade file system objects.
+        Retrieves information about FlashArray and FlashBlade file system objects.
 
         Args:
             references (list[FixedReference], optional):
                 A list of references to query for. Overrides ids and names keyword arguments.
 
             x_request_id (str, optional):
                 A header to provide to track the API call. Generated by the server if not
@@ -1733,15 +1836,15 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of file system members and their policies.
+        Retrieves pairs of FlashBlade file system members and their policies.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
 
@@ -2581,15 +2684,16 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of policy references and their file system replica link members.
+        Retrieves pairs of policy references and their FlashBlade file system replica
+        link members.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
 
@@ -2679,15 +2783,16 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of policy references and their file system snapshot members.
+        Retrieves pairs of policy references and their FlashBlade file system snapshot
+        members.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
 
@@ -2777,15 +2882,15 @@
         async_req=False,  # type: bool
         _return_http_data_only=False,  # type: bool
         _preload_content=True,  # type: bool
         _request_timeout=None,  # type: Optional[int]
     ):
         # type: (...) -> models.PolicyMembersGetResponse
         """
-        Retrieves pairs of policy references and their file system members.
+        Retrieves pairs of policy references and their FlashBlade file system members.
 
         Args:
             members (list[FixedReference], optional):
                 A list of members to query for. Overrides member_ids and member_names keyword arguments.
             policies (list[FixedReference], optional):
                 A list of policies to query for. Overrides policy_ids and policy_names keyword arguments.
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/configuration.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/configuration.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/__init__.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,14 +62,17 @@
 from .bucket_replica_link import BucketReplicaLink
 from .bucket_replica_link_get_response import BucketReplicaLinkGetResponse
 from .bucket_replica_link_response import BucketReplicaLinkResponse
 from .bucket_response import BucketResponse
 from .controller import Controller
 from .controller_get_response import ControllerGetResponse
 from .controller_response import ControllerResponse
+from .directory import Directory
+from .directory_get_response import DirectoryGetResponse
+from .directory_response import DirectoryResponse
 from .drive import Drive
 from .drive_array_status import DriveArrayStatus
 from .drive_get_response import DriveGetResponse
 from .drive_response import DriveResponse
 from .error import Error
 from .error_errors import ErrorErrors
 from .error_no_context import ErrorNoContext
@@ -79,15 +82,14 @@
 from .file_system_replica_link_get_response import FileSystemReplicaLinkGetResponse
 from .file_system_replica_link_response import FileSystemReplicaLinkResponse
 from .file_system_response import FileSystemResponse
 from .file_system_snapshot import FileSystemSnapshot
 from .file_system_snapshot_get_response import FileSystemSnapshotGetResponse
 from .file_system_snapshot_response import FileSystemSnapshotResponse
 from .fixed_reference import FixedReference
-from .fixed_reference2 import FixedReference2
 from .fixed_reference_fqdn import FixedReferenceFqdn
 from .hardware import Hardware
 from .hardware_connector import HardwareConnector
 from .hardware_connector_get_response import HardwareConnectorGetResponse
 from .hardware_connector_response import HardwareConnectorResponse
 from .hardware_get_response import HardwareGetResponse
 from .hardware_response import HardwareResponse
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/alert.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/alert.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/alerts_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/alerts_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/alerts_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/alerts_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/array.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/array.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/array_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/array_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/array_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/array_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/arrays.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/arrays.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/arrays2.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/error_no_context.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,47 +17,47 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class Arrays2(object):
+class ErrorNoContext(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'arrays': 'list[FixedReference2]'
+        'message': 'str'
     }
 
     attribute_map = {
-        'arrays': 'arrays'
+        'message': 'message'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        arrays=None,  # type: List[models.FixedReference2]
+        message=None,  # type: str
     ):
         """
         Keyword args:
-            arrays (list[FixedReference2]): The list of arrays where this resource exists. Many resources are on a single array, but some resources, such as pods, can be shared across multiple arrays.
+            message (str)
         """
-        if arrays is not None:
-            self.arrays = arrays
+        if message is not None:
+            self.message = message
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `Arrays2`".format(key))
+            raise KeyError("Invalid key `{}` for `ErrorNoContext`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -81,15 +81,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(Arrays2, dict):
+        if issubclass(ErrorNoContext, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -97,15 +97,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Arrays2):
+        if not isinstance(other, ErrorNoContext):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/arrays_built_in.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/arrays_resource.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,27 +17,27 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class ArraysBuiltIn(object):
+class ArraysResource(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'as_of': 'int',
         'id': 'str',
         'name': 'str',
-        'arrays': 'list[FixedReference2]'
+        'arrays': 'list[FixedReferenceFqdn]'
     }
 
     attribute_map = {
         'as_of': '_as_of',
         'id': 'id',
         'name': 'name',
         'arrays': 'arrays'
@@ -47,35 +47,35 @@
     }
 
     def __init__(
         self,
         as_of=None,  # type: int
         id=None,  # type: str
         name=None,  # type: str
-        arrays=None,  # type: List[models.FixedReference2]
+        arrays=None,  # type: List[models.FixedReferenceFqdn]
     ):
         """
         Keyword args:
             as_of (int): The freshness of the data (timestamp in millis since epoch).
             id (str): A non-modifiable, globally unique ID chosen by the system.
-            name (str): A non-modifiable, locally unique name chosen by the system.
-            arrays (list[FixedReference2]): The list of arrays where this resource exists. Many resources are on a single array, but some resources, such as pods, can be shared across multiple arrays.
+            name (str): A modifiable, locally unique name chosen by the user.
+            arrays (list[FixedReferenceFqdn]): The list of arrays where this resource exists. Many resources are on a single array, but some resources, such as pods, can be shared across multiple arrays.
         """
         if as_of is not None:
             self.as_of = as_of
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
         if arrays is not None:
             self.arrays = arrays
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `ArraysBuiltIn`".format(key))
+            raise KeyError("Invalid key `{}` for `ArraysResource`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -99,15 +99,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(ArraysBuiltIn, dict):
+        if issubclass(ArraysResource, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -115,15 +115,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ArraysBuiltIn):
+        if not isinstance(other, ArraysResource):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/arrays_resource.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/resource.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,65 +17,59 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class ArraysResource(object):
+class Resource(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'as_of': 'int',
         'id': 'str',
-        'name': 'str',
-        'arrays': 'list[FixedReferenceFqdn]'
+        'name': 'str'
     }
 
     attribute_map = {
         'as_of': '_as_of',
         'id': 'id',
-        'name': 'name',
-        'arrays': 'arrays'
+        'name': 'name'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
         as_of=None,  # type: int
         id=None,  # type: str
         name=None,  # type: str
-        arrays=None,  # type: List[models.FixedReferenceFqdn]
     ):
         """
         Keyword args:
             as_of (int): The freshness of the data (timestamp in millis since epoch).
             id (str): A non-modifiable, globally unique ID chosen by the system.
             name (str): A modifiable, locally unique name chosen by the user.
-            arrays (list[FixedReferenceFqdn]): The list of arrays where this resource exists. Many resources are on a single array, but some resources, such as pods, can be shared across multiple arrays.
         """
         if as_of is not None:
             self.as_of = as_of
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
-        if arrays is not None:
-            self.arrays = arrays
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `ArraysResource`".format(key))
+            raise KeyError("Invalid key `{}` for `Resource`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -99,15 +93,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(ArraysResource, dict):
+        if issubclass(Resource, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -115,15 +109,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ArraysResource):
+        if not isinstance(other, Resource):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/audit.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/audit.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/audits_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/audits_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/audits_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/audits_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/blade.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/blade.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/blade_array_status.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/blade_array_status.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/blade_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/blade_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/blade_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/blade_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket_replica_link_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/bucket_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/bucket_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/built_in_as_of.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/built_in_as_of.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/controller.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/controller.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/controller_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/controller_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/controller_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/controller_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/drive.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/drive.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/drive_array_status.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/drive_array_status.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/drive_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/drive_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/drive_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/drive_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/error.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/error.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/error_errors.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/error_errors.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/error_no_context.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/resource_no_name.py`

 * *Files 7% similar despite different names*

```diff
@@ -17,47 +17,53 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class ErrorNoContext(object):
+class ResourceNoName(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'message': 'str'
+        'as_of': 'int',
+        'id': 'str'
     }
 
     attribute_map = {
-        'message': 'message'
+        'as_of': '_as_of',
+        'id': 'id'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        message=None,  # type: str
+        as_of=None,  # type: int
+        id=None,  # type: str
     ):
         """
         Keyword args:
-            message (str)
+            as_of (int): The freshness of the data (timestamp in millis since epoch).
+            id (str): A non-modifiable, globally unique ID chosen by the system.
         """
-        if message is not None:
-            self.message = message
+        if as_of is not None:
+            self.as_of = as_of
+        if id is not None:
+            self.id = id
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `ErrorNoContext`".format(key))
+            raise KeyError("Invalid key `{}` for `ResourceNoName`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -81,15 +87,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(ErrorNoContext, dict):
+        if issubclass(ResourceNoName, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -97,15 +103,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ErrorNoContext):
+        if not isinstance(other, ResourceNoName):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system.py`

 * *Files 7% similar despite different names*

```diff
@@ -84,21 +84,21 @@
         Keyword args:
             as_of (int): The freshness of the data (timestamp in millis since epoch).
             id (str): A non-modifiable, globally unique ID chosen by the system.
             name (str): A non-modifiable, locally unique name chosen by the system.
             arrays (list[FixedReferenceFqdn]): The list of arrays where this resource exists. Many resources are on a single array, but some resources, such as pods, can be shared across multiple arrays.
             created (int): Creation time in milliseconds since UNIX epoch.
             destroyed (bool): Is the file system destroyed?
-            fast_remove_directory_enabled (bool): Is fast remove directory enabled?
-            hard_limit_enabled (bool): Is the file system's size a hard limit quota?
-            http (Http): HTTP configuration.
-            nfs (Nfs): NFS configuration.
-            provisioned (int): The provisioned size of the file system in bytes. A value of 0 means unlimited.
-            smb (Smb): SMB configuration.
-            snapshot_directory_enabled (bool): Is snapshot directory enabled?
+            fast_remove_directory_enabled (bool): On a FlashBlade file system, returns the value of `true` if fast remove directory is enabled and `false` if it is not. On a FlashArray file system, the value is always `null`.
+            hard_limit_enabled (bool): On a FlashBlade file system, returns the value of `true` if the file system's size is a hard limit quota and `false` if it is not. On a FlashArray file system, the value is always `null`.
+            http (Http): HTTP configuration. On a FlashArray file system, the value is always `null`.
+            nfs (Nfs): NFS configuration. On a FlashArray file system, the value is always `null`.
+            provisioned (int): The provisioned size of the file system in bytes. A value of 0 means unlimited. On a FlashArray file system, the value is always `null`.
+            smb (Smb): SMB configuration. On a FlashArray file system, the value is always `null`.
+            snapshot_directory_enabled (bool): On a FlashBlade file system, returns the value of `true` if snapshot directory is enabled and `false` if it is not. On a FlashArray file system, the value is always `null`.
         """
         if as_of is not None:
             self.as_of = as_of
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_replica_link_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/file_system_snapshot_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/fixed_reference.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/fixed_reference.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/fixed_reference2.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/resource_with_location.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,59 +17,65 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class FixedReference2(object):
+class ResourceWithLocation(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'str',
         'name': 'str',
-        'resource_type': 'str'
+        'resource_type': 'str',
+        'location': 'FixedReferenceFqdn'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
-        'resource_type': 'resource_type'
+        'resource_type': 'resource_type',
+        'location': 'location'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
         id=None,  # type: str
         name=None,  # type: str
         resource_type=None,  # type: str
+        location=None,  # type: models.FixedReferenceFqdn
     ):
         """
         Keyword args:
             id (str): The opaque and unique id of this resource.
             name (str): The name of this resource.
             resource_type (str): The type of this resource represented by the name of its REST endpoint. For example, \"arrays\", \"network-interfaces\", and \"metrics\". The value may be `null` if the resource is not represented.
+            location (FixedReferenceFqdn)
         """
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
         if resource_type is not None:
             self.resource_type = resource_type
+        if location is not None:
+            self.location = location
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `FixedReference2`".format(key))
+            raise KeyError("Invalid key `{}` for `ResourceWithLocation`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -93,15 +99,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(FixedReference2, dict):
+        if issubclass(ResourceWithLocation, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -109,15 +115,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, FixedReference2):
+        if not isinstance(other, ResourceWithLocation):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/fixed_reference_fqdn.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/fixed_reference_fqdn.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware_connector_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/hardware_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/hardware_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/http.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/http.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/inline_response400.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/inline_response400.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/inline_response401.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/inline_response401.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_availability.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_availability.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_history.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_history.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_history_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_history_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_history_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_history_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/metric_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/metric_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/network_interface.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/network_interface.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/network_interface_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/network_interface_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/network_interface_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/network_interface_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/nfs.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/nfs.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/oauth_token_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/oauth_token_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/object_store_account.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/object_store_account.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/object_store_account_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/object_store_account_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/object_store_account_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/object_store_account_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/page_info.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/page_info.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_array_status.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_array_status.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_replica_link_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/pod_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/pod_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_member.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_member.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_members_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_members_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_members_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_members_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/policy_rule.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/policy_rule.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/port.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/port.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/port_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/port_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/port_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/port_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/replica_link.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/replica_link.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/resource.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/support_contract.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,59 +17,59 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class Resource(object):
+class SupportContract(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'as_of': 'int',
-        'id': 'str',
-        'name': 'str'
+        'start_date': 'int',
+        'end_date': 'int',
+        'resource': 'FixedReferenceFqdn'
     }
 
     attribute_map = {
-        'as_of': '_as_of',
-        'id': 'id',
-        'name': 'name'
+        'start_date': 'start_date',
+        'end_date': 'end_date',
+        'resource': 'resource'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        as_of=None,  # type: int
-        id=None,  # type: str
-        name=None,  # type: str
+        start_date=None,  # type: int
+        end_date=None,  # type: int
+        resource=None,  # type: models.FixedReferenceFqdn
     ):
         """
         Keyword args:
-            as_of (int): The freshness of the data (timestamp in millis since epoch).
-            id (str): A non-modifiable, globally unique ID chosen by the system.
-            name (str): A modifiable, locally unique name chosen by the user.
+            start_date (int): Date when the support contract started. Represented as a timestamp of 00:00 on that date in UTC, in milliseconds since UNIX epoch.
+            end_date (int): Date when the support contract ended. Represented as a timestamp of 00:00 on that date in UTC, in milliseconds since UNIX epoch.
+            resource (FixedReferenceFqdn)
         """
-        if as_of is not None:
-            self.as_of = as_of
-        if id is not None:
-            self.id = id
-        if name is not None:
-            self.name = name
+        if start_date is not None:
+            self.start_date = start_date
+        if end_date is not None:
+            self.end_date = end_date
+        if resource is not None:
+            self.resource = resource
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `Resource`".format(key))
+            raise KeyError("Invalid key `{}` for `SupportContract`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -93,15 +93,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(Resource, dict):
+        if issubclass(SupportContract, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -109,15 +109,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Resource):
+        if not isinstance(other, SupportContract):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/resource_no_name.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/time_aware.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,53 +17,47 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class ResourceNoName(object):
+class TimeAware(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'as_of': 'int',
-        'id': 'str'
+        'as_of': 'int'
     }
 
     attribute_map = {
-        'as_of': '_as_of',
-        'id': 'id'
+        'as_of': '_as_of'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
         as_of=None,  # type: int
-        id=None,  # type: str
     ):
         """
         Keyword args:
             as_of (int): The freshness of the data (timestamp in millis since epoch).
-            id (str): A non-modifiable, globally unique ID chosen by the system.
         """
         if as_of is not None:
             self.as_of = as_of
-        if id is not None:
-            self.id = id
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `ResourceNoName`".format(key))
+            raise KeyError("Invalid key `{}` for `TimeAware`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -87,15 +81,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(ResourceNoName, dict):
+        if issubclass(TimeAware, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -103,15 +97,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResourceNoName):
+        if not isinstance(other, TimeAware):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/resource_with_location.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/resource_with_locations.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,65 +17,65 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class ResourceWithLocation(object):
+class ResourceWithLocations(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'id': 'str',
         'name': 'str',
         'resource_type': 'str',
-        'location': 'FixedReferenceFqdn'
+        'locations': 'list[FixedReferenceFqdn]'
     }
 
     attribute_map = {
         'id': 'id',
         'name': 'name',
         'resource_type': 'resource_type',
-        'location': 'location'
+        'locations': 'locations'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
         id=None,  # type: str
         name=None,  # type: str
         resource_type=None,  # type: str
-        location=None,  # type: models.FixedReferenceFqdn
+        locations=None,  # type: List[models.FixedReferenceFqdn]
     ):
         """
         Keyword args:
             id (str): The opaque and unique id of this resource.
             name (str): The name of this resource.
             resource_type (str): The type of this resource represented by the name of its REST endpoint. For example, \"arrays\", \"network-interfaces\", and \"metrics\". The value may be `null` if the resource is not represented.
-            location (FixedReferenceFqdn)
+            locations (list[FixedReferenceFqdn])
         """
         if id is not None:
             self.id = id
         if name is not None:
             self.name = name
         if resource_type is not None:
             self.resource_type = resource_type
-        if location is not None:
-            self.location = location
+        if locations is not None:
+            self.locations = locations
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `ResourceWithLocation`".format(key))
+            raise KeyError("Invalid key `{}` for `ResourceWithLocations`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -99,15 +99,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(ResourceWithLocation, dict):
+        if issubclass(ResourceWithLocations, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -115,15 +115,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResourceWithLocation):
+        if not isinstance(other, ResourceWithLocations):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/resource_with_locations.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/directory_get_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,65 +17,59 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class ResourceWithLocations(object):
+class DirectoryGetResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'id': 'str',
-        'name': 'str',
-        'resource_type': 'str',
-        'locations': 'list[FixedReferenceFqdn]'
+        'continuation_token': 'str',
+        'total_item_count': 'int',
+        'items': 'list[Directory]'
     }
 
     attribute_map = {
-        'id': 'id',
-        'name': 'name',
-        'resource_type': 'resource_type',
-        'locations': 'locations'
+        'continuation_token': 'continuation_token',
+        'total_item_count': 'total_item_count',
+        'items': 'items'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        id=None,  # type: str
-        name=None,  # type: str
-        resource_type=None,  # type: str
-        locations=None,  # type: List[models.FixedReferenceFqdn]
+        continuation_token=None,  # type: str
+        total_item_count=None,  # type: int
+        items=None,  # type: List[models.Directory]
     ):
         """
         Keyword args:
-            id (str): The opaque and unique id of this resource.
-            name (str): The name of this resource.
-            resource_type (str): The type of this resource represented by the name of its REST endpoint. For example, \"arrays\", \"network-interfaces\", and \"metrics\". The value may be `null` if the resource is not represented.
-            locations (list[FixedReferenceFqdn])
+            continuation_token (str): Continuation token that can be provided in the continuation_token query param to get the next page of data. If you use the continuation token to page through data you are guaranteed to get all items exactly once regardless of how items are modified. If an item is added or deleted during the pagination then it may or may not be returned. The continuation token is generated if the limit is less than the remaining number of items, and the default sort is used (no sort is specified).
+            total_item_count (int): Total number of items after applying filter params.
+            items (list[Directory])
         """
-        if id is not None:
-            self.id = id
-        if name is not None:
-            self.name = name
-        if resource_type is not None:
-            self.resource_type = resource_type
-        if locations is not None:
-            self.locations = locations
+        if continuation_token is not None:
+            self.continuation_token = continuation_token
+        if total_item_count is not None:
+            self.total_item_count = total_item_count
+        if items is not None:
+            self.items = items
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `ResourceWithLocations`".format(key))
+            raise KeyError("Invalid key `{}` for `DirectoryGetResponse`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -99,15 +93,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(ResourceWithLocations, dict):
+        if issubclass(DirectoryGetResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -115,15 +109,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ResourceWithLocations):
+        if not isinstance(other, DirectoryGetResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/smb.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/smb.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/support_contract.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/tag_put.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,59 +17,53 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class SupportContract(object):
+class TagPut(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'start_date': 'int',
-        'end_date': 'int',
-        'resource': 'FixedReferenceFqdn'
+        'key': 'str',
+        'value': 'str'
     }
 
     attribute_map = {
-        'start_date': 'start_date',
-        'end_date': 'end_date',
-        'resource': 'resource'
+        'key': 'key',
+        'value': 'value'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        start_date=None,  # type: int
-        end_date=None,  # type: int
-        resource=None,  # type: models.FixedReferenceFqdn
+        key=None,  # type: str
+        value=None,  # type: str
     ):
         """
         Keyword args:
-            start_date (int): Date when the support contract started. Represented as a timestamp of 00:00 on that date in UTC, in milliseconds since UNIX epoch.
-            end_date (int): Date when the support contract ended. Represented as a timestamp of 00:00 on that date in UTC, in milliseconds since UNIX epoch.
-            resource (FixedReferenceFqdn)
+            key (str): Key of the tag.
+            value (str): Value of the tag.
         """
-        if start_date is not None:
-            self.start_date = start_date
-        if end_date is not None:
-            self.end_date = end_date
-        if resource is not None:
-            self.resource = resource
+        if key is not None:
+            self.key = key
+        if value is not None:
+            self.value = value
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `SupportContract`".format(key))
+            raise KeyError("Invalid key `{}` for `TagPut`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -93,15 +87,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(SupportContract, dict):
+        if issubclass(TagPut, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -109,15 +103,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, SupportContract):
+        if not isinstance(other, TagPut):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/support_contract_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/support_contract_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/support_contract_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/support_contract_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/tag.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/tag.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/tag_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/tag_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/tag_put.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/tag_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,53 +17,47 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class TagPut(object):
+class TagResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'key': 'str',
-        'value': 'str'
+        'items': 'list[Tag]'
     }
 
     attribute_map = {
-        'key': 'key',
-        'value': 'value'
+        'items': 'items'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        key=None,  # type: str
-        value=None,  # type: str
+        items=None,  # type: List[models.Tag]
     ):
         """
         Keyword args:
-            key (str): Key of the tag.
-            value (str): Value of the tag.
+            items (list[Tag])
         """
-        if key is not None:
-            self.key = key
-        if value is not None:
-            self.value = value
+        if items is not None:
+            self.items = items
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `TagPut`".format(key))
+            raise KeyError("Invalid key `{}` for `TagResponse`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -87,15 +81,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(TagPut, dict):
+        if issubclass(TagResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -103,15 +97,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TagPut):
+        if not isinstance(other, TagResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/tag_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/target_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,47 +17,47 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class TagResponse(object):
+class TargetResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'items': 'list[Tag]'
+        'items': 'list[Target]'
     }
 
     attribute_map = {
         'items': 'items'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        items=None,  # type: List[models.Tag]
+        items=None,  # type: List[models.Target]
     ):
         """
         Keyword args:
-            items (list[Tag])
+            items (list[Target])
         """
         if items is not None:
             self.items = items
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `TagResponse`".format(key))
+            raise KeyError("Invalid key `{}` for `TargetResponse`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -81,15 +81,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(TagResponse, dict):
+        if issubclass(TargetResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -97,15 +97,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TagResponse):
+        if not isinstance(other, TargetResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/target.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/target.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/target_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/target_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/target_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,47 +17,47 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class TargetResponse(object):
+class VolumeResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'items': 'list[Target]'
+        'items': 'list[Volume]'
     }
 
     attribute_map = {
         'items': 'items'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        items=None,  # type: List[models.Target]
+        items=None,  # type: List[models.Volume]
     ):
         """
         Keyword args:
-            items (list[Target])
+            items (list[Volume])
         """
         if items is not None:
             self.items = items
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `TargetResponse`".format(key))
+            raise KeyError("Invalid key `{}` for `VolumeResponse`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -81,15 +81,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(TargetResponse, dict):
+        if issubclass(VolumeResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -97,15 +97,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TargetResponse):
+        if not isinstance(other, VolumeResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/time_aware.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -17,47 +17,47 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class TimeAware(object):
+class VolumeSnapshotResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'as_of': 'int'
+        'items': 'list[VolumeSnapshot]'
     }
 
     attribute_map = {
-        'as_of': '_as_of'
+        'items': 'items'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        as_of=None,  # type: int
+        items=None,  # type: List[models.VolumeSnapshot]
     ):
         """
         Keyword args:
-            as_of (int): The freshness of the data (timestamp in millis since epoch).
+            items (list[VolumeSnapshot])
         """
-        if as_of is not None:
-            self.as_of = as_of
+        if items is not None:
+            self.items = items
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `TimeAware`".format(key))
+            raise KeyError("Invalid key `{}` for `VolumeSnapshotResponse`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -81,15 +81,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(TimeAware, dict):
+        if issubclass(VolumeSnapshotResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -97,15 +97,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TimeAware):
+        if not isinstance(other, VolumeSnapshotResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/directory_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,47 +17,47 @@
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
     from pypureclient.pure1.Pure1_1_1 import models
 
-class VolumeResponse(object):
+class DirectoryResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'items': 'list[Volume]'
+        'items': 'list[Directory]'
     }
 
     attribute_map = {
         'items': 'items'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        items=None,  # type: List[models.Volume]
+        items=None,  # type: List[models.Directory]
     ):
         """
         Keyword args:
-            items (list[Volume])
+            items (list[Directory])
         """
         if items is not None:
             self.items = items
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `VolumeResponse`".format(key))
+            raise KeyError("Invalid key `{}` for `DirectoryResponse`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -81,15 +81,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(VolumeResponse, dict):
+        if issubclass(DirectoryResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -97,15 +97,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, VolumeResponse):
+        if not isinstance(other, DirectoryResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot_get_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot_get_response.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/models/volume_snapshot_response.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_0/models/directory_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 # coding: utf-8
 
 """
     Pure1 Public REST API
 
     No description provided (generated by Swagger Codegen https://github.com/swagger-api/swagger-codegen)
 
-    OpenAPI spec version: 1.1
+    OpenAPI spec version: 1.0
     
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 
 import pprint
 import re
 
 import six
 import typing
 
 from ....properties import Property
 if typing.TYPE_CHECKING:
-    from pypureclient.pure1.Pure1_1_1 import models
+    from pypureclient.pure1.Pure1_1_0 import models
 
-class VolumeSnapshotResponse(object):
+class DirectoryResponse(object):
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'items': 'list[VolumeSnapshot]'
+        'items': 'list[Directory]'
     }
 
     attribute_map = {
         'items': 'items'
     }
 
     required_args = {
     }
 
     def __init__(
         self,
-        items=None,  # type: List[models.VolumeSnapshot]
+        items=None,  # type: List[models.Directory]
     ):
         """
         Keyword args:
-            items (list[VolumeSnapshot])
+            items (list[Directory])
         """
         if items is not None:
             self.items = items
 
     def __setattr__(self, key, value):
         if key not in self.attribute_map:
-            raise KeyError("Invalid key `{}` for `VolumeSnapshotResponse`".format(key))
+            raise KeyError("Invalid key `{}` for `DirectoryResponse`".format(key))
         self.__dict__[key] = value
 
     def __getattribute__(self, item):
         value = object.__getattribute__(self, item)
         if isinstance(value, Property):
             raise AttributeError
         else:
@@ -81,15 +81,15 @@
                     result[attr] = dict(map(
                         lambda item: (item[0], item[1].to_dict())
                         if hasattr(item[1], "to_dict") else item,
                         value.items()
                     ))
                 else:
                     result[attr] = value
-        if issubclass(VolumeSnapshotResponse, dict):
+        if issubclass(DirectoryResponse, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -97,15 +97,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, VolumeSnapshotResponse):
+        if not isinstance(other, DirectoryResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/Pure1_1_1/rest.py` & `py-pure-client-1.9.0/pypureclient/pure1/Pure1_1_1/rest.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/pure1/client.py` & `py-pure-client-1.9.0/pypureclient/pure1/client.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/responses.py` & `py-pure-client-1.9.0/pypureclient/responses.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/pypureclient/token_manager.py` & `py-pure-client-1.9.0/pypureclient/token_manager.py`

 * *Files identical despite different names*

### Comparing `py-pure-client-1.8.0/setup.py` & `py-pure-client-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 Pure Storage Python clients for FlashArray, FlashBlade, and Pure1 APIs
 '''
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = 'py-pure-client'
-VERSION = '1.8.0'
+VERSION = '1.9.0'
 
 REQUIRES = ['urllib3 >= 1.15', 'six >= 1.10', 'certifi >= 14.05.14',
             'python-dateutil >= 2.5.3', 'paramiko == 2.7.1',
             'PyJWT >= 1.7.1', 'requests >= 2.20.1']
 
 readme = open('README.md', 'r')
 README_TEXT = readme.read()
@@ -22,15 +22,15 @@
 setup(
     name=NAME,
     version=VERSION,
     description='Pure Storage Python clients for FlashArray, FlashBlade, and Pure1 APIs',
     author='Pure Storage',
     author_email='tvilcu@purestorage.com',
     url='https://github.com/PureStorage-OpenConnect/py-pure-client',
-    download_url='https://github.com/PureStorage-OpenConnect/py-pure-client/archive/1.8.0.tar.gz',
+    download_url='https://github.com/PureStorage-OpenConnect/py-pure-client/archive/1.9.0.tar.gz',
     keywords=['Swagger', 'Pure Storage', 'Python', 'clients', 'REST', 'API', 'FlashArray', 'FlashBlade', 'Pure1'],
     license='BSD 2-Clause',
     install_requires=REQUIRES,
     packages=find_packages(),
     include_package_data=True,
     long_description=README_TEXT,
     long_description_content_type='text/markdown'
```

