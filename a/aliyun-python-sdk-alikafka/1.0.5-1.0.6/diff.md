# Comparing `tmp/aliyun-python-sdk-alikafka-1.0.5.tar.gz` & `tmp/aliyun-python-sdk-alikafka-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-alikafka-1.0.5.tar", last modified: Tue Apr 25 11:50:10 2023, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-alikafka-1.0.6.tar", last modified: Wed Apr  3 08:43:34 2024, max compression
```

## Comparing `aliyun-python-sdk-alikafka-1.0.5.tar` & `aliyun-python-sdk-alikafka-1.0.6.tar`

### file list

```diff
@@ -1,57 +1,64 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/
--rw-r--r--   0 root         (0) root         (0)      575 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1562 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      537 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1562 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2764 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/
--rw-r--r--   0 root         (0) root         (0)       21 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1088 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/endpoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/
--rw-r--r--   0 root         (0) root         (0)     1714 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ChangeResourceGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1656 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ConvertPostPayOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateConsumerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     3569 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreatePostPayOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     3567 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreatePrePayOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     1978 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateSaslUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     3432 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateTopicRequest.py
--rw-r--r--   0 root         (0) root         (0)     2566 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteAclRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteConsumerGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1465 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteSaslUserRequest.py
--rw-r--r--   0 root         (0) root         (0)     1620 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteTopicRequest.py
--rw-r--r--   0 root         (0) root         (0)     2345 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DescribeAclsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DescribeSaslUsersRequest.py
--rw-r--r--   0 root         (0) root         (0)     1286 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetAllInstanceIdListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1469 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetAllowedIpListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1658 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetConsumerListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetConsumerProgressRequest.py
--rw-r--r--   0 root         (0) root         (0)     2359 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetInstanceListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1459 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetQuotaTipRequest.py
--rw-r--r--   0 root         (0) root         (0)     1998 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetTopicListRequest.py
--rw-r--r--   0 root         (0) root         (0)     1626 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetTopicStatusRequest.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ListTagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1676 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyInstanceNameRequest.py
--rw-r--r--   0 root         (0) root         (0)     1857 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyPartitionNumRequest.py
--rw-r--r--   0 root         (0) root         (0)     1799 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyTopicRemarkRequest.py
--rw-r--r--   0 root         (0) root         (0)     1714 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ReleaseInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     4752 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/StartInstanceRequest.py
--rw-r--r--   0 root         (0) root         (0)     2353 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/TagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2140 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UntagResourcesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2470 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateAllowedIpRequest.py
--rw-r--r--   0 root         (0) root         (0)     2364 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateConsumerOffsetRequest.py
--rw-r--r--   0 root         (0) root         (0)     1644 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateInstanceConfigRequest.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradeInstanceVersionRequest.py
--rw-r--r--   0 root         (0) root         (0)     2931 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradePostPayOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)     2929 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradePrePayOrderRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2477 2023-04-25 11:50:10.000000 aliyun-python-sdk-alikafka-1.0.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/
+-rw-r--r--   0 root         (0) root         (0)      575 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1562 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      537 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyun_python_sdk_alikafka.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1562 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyun_python_sdk_alikafka.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3217 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyun_python_sdk_alikafka.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyun_python_sdk_alikafka.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyun_python_sdk_alikafka.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyun_python_sdk_alikafka.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/
+-rw-r--r--   0 root         (0) root         (0)     1725 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ChangeResourceGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ConvertPostPayOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/CreateAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2263 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/CreateConsumerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3580 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/CreatePostPayOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4185 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/CreatePrePayOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2174 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/CreateSaslUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3443 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/CreateTopicRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3198 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DeleteAclRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DeleteConsumerGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DeleteInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1995 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DeleteSaslUserRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1631 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DeleteTopicRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2971 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DescribeAclsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1482 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DescribeSaslUsersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/EnableAutoGroupCreationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/EnableAutoTopicCreationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetAllInstanceIdListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1480 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetAllowedIpListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2049 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetConsumerListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetConsumerProgressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2370 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetInstanceListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1470 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetQuotaTipRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2009 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetTopicListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetTopicStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetTopicSubscribeStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2366 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ModifyInstanceNameRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1868 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ModifyPartitionNumRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ModifyTopicRemarkRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2350 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/QueryMessageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1725 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ReleaseInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ReopenInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     5220 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/StartInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1472 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/StopInstanceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2364 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2481 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpdateAllowedIpRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2375 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpdateConsumerOffsetRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1655 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpdateInstanceConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1971 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpdateTopicConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpgradeInstanceVersionRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3193 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpgradePostPayOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3366 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpgradePrePayOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2477 2024-04-03 08:43:34.000000 aliyun-python-sdk-alikafka-1.0.6/setup.py
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/LICENSE` & `aliyun-python-sdk-alikafka-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alikafka-1.0.5/PKG-INFO` & `aliyun-python-sdk-alikafka-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alikafka
-Version: 1.0.5
+Version: 1.0.6
 Summary: The alikafka module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alikafka
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/README.rst` & `aliyun-python-sdk-alikafka-1.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/PKG-INFO` & `aliyun-python-sdk-alikafka-1.0.6/aliyun_python_sdk_alikafka.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-alikafka
-Version: 1.0.5
+Version: 1.0.6
 Summary: The alikafka module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-alikafka
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyun_python_sdk_alikafka.egg-info/SOURCES.txt` & `aliyun-python-sdk-alikafka-1.0.6/aliyun_python_sdk_alikafka.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -22,30 +22,37 @@
 aliyunsdkalikafka/request/v20190916/DeleteAclRequest.py
 aliyunsdkalikafka/request/v20190916/DeleteConsumerGroupRequest.py
 aliyunsdkalikafka/request/v20190916/DeleteInstanceRequest.py
 aliyunsdkalikafka/request/v20190916/DeleteSaslUserRequest.py
 aliyunsdkalikafka/request/v20190916/DeleteTopicRequest.py
 aliyunsdkalikafka/request/v20190916/DescribeAclsRequest.py
 aliyunsdkalikafka/request/v20190916/DescribeSaslUsersRequest.py
+aliyunsdkalikafka/request/v20190916/EnableAutoGroupCreationRequest.py
+aliyunsdkalikafka/request/v20190916/EnableAutoTopicCreationRequest.py
 aliyunsdkalikafka/request/v20190916/GetAllInstanceIdListRequest.py
 aliyunsdkalikafka/request/v20190916/GetAllowedIpListRequest.py
 aliyunsdkalikafka/request/v20190916/GetConsumerListRequest.py
 aliyunsdkalikafka/request/v20190916/GetConsumerProgressRequest.py
 aliyunsdkalikafka/request/v20190916/GetInstanceListRequest.py
 aliyunsdkalikafka/request/v20190916/GetQuotaTipRequest.py
 aliyunsdkalikafka/request/v20190916/GetTopicListRequest.py
 aliyunsdkalikafka/request/v20190916/GetTopicStatusRequest.py
+aliyunsdkalikafka/request/v20190916/GetTopicSubscribeStatusRequest.py
 aliyunsdkalikafka/request/v20190916/ListTagResourcesRequest.py
 aliyunsdkalikafka/request/v20190916/ModifyInstanceNameRequest.py
 aliyunsdkalikafka/request/v20190916/ModifyPartitionNumRequest.py
 aliyunsdkalikafka/request/v20190916/ModifyTopicRemarkRequest.py
+aliyunsdkalikafka/request/v20190916/QueryMessageRequest.py
 aliyunsdkalikafka/request/v20190916/ReleaseInstanceRequest.py
+aliyunsdkalikafka/request/v20190916/ReopenInstanceRequest.py
 aliyunsdkalikafka/request/v20190916/StartInstanceRequest.py
+aliyunsdkalikafka/request/v20190916/StopInstanceRequest.py
 aliyunsdkalikafka/request/v20190916/TagResourcesRequest.py
 aliyunsdkalikafka/request/v20190916/UntagResourcesRequest.py
 aliyunsdkalikafka/request/v20190916/UpdateAllowedIpRequest.py
 aliyunsdkalikafka/request/v20190916/UpdateConsumerOffsetRequest.py
 aliyunsdkalikafka/request/v20190916/UpdateInstanceConfigRequest.py
+aliyunsdkalikafka/request/v20190916/UpdateTopicConfigRequest.py
 aliyunsdkalikafka/request/v20190916/UpgradeInstanceVersionRequest.py
 aliyunsdkalikafka/request/v20190916/UpgradePostPayOrderRequest.py
 aliyunsdkalikafka/request/v20190916/UpgradePrePayOrderRequest.py
 aliyunsdkalikafka/request/v20190916/__init__.py
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/endpoint.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ChangeResourceGroupRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ChangeResourceGroupRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ChangeResourceGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ChangeResourceGroup')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ChangeResourceGroup','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ConvertPostPayOrderRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ConvertPostPayOrderRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ConvertPostPayOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ConvertPostPayOrder')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ConvertPostPayOrder','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateAclRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DeleteSaslUserRequest.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,48 +16,38 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class CreateAclRequest(RpcRequest):
+class DeleteSaslUserRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateAcl')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteSaslUser','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_AclResourcePatternType(self): # String
-		return self.get_query_params().get('AclResourcePatternType')
+	def get_Type(self): # String
+		return self.get_query_params().get('Type')
 
-	def set_AclResourcePatternType(self, AclResourcePatternType):  # String
-		self.add_query_param('AclResourcePatternType', AclResourcePatternType)
-	def get_AclResourceType(self): # String
-		return self.get_query_params().get('AclResourceType')
-
-	def set_AclResourceType(self, AclResourceType):  # String
-		self.add_query_param('AclResourceType', AclResourceType)
-	def get_AclOperationType(self): # String
-		return self.get_query_params().get('AclOperationType')
-
-	def set_AclOperationType(self, AclOperationType):  # String
-		self.add_query_param('AclOperationType', AclOperationType)
-	def get_AclResourceName(self): # String
-		return self.get_query_params().get('AclResourceName')
-
-	def set_AclResourceName(self, AclResourceName):  # String
-		self.add_query_param('AclResourceName', AclResourceName)
+	def set_Type(self, Type):  # String
+		self.add_query_param('Type', Type)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
+	def get_Mechanism(self): # String
+		return self.get_query_params().get('Mechanism')
+
+	def set_Mechanism(self, Mechanism):  # String
+		self.add_query_param('Mechanism', Mechanism)
 	def get_Username(self): # String
 		return self.get_query_params().get('Username')
 
 	def set_Username(self, Username):  # String
 		self.add_query_param('Username', Username)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateConsumerGroupRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/CreateConsumerGroupRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class CreateConsumerGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateConsumerGroup')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateConsumerGroup','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreatePostPayOrderRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/CreatePostPayOrderRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class CreatePostPayOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreatePostPayOrder')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreatePostPayOrder','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreatePrePayOrderRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/CreatePrePayOrderRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,19 +15,20 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
+import json
 
 class CreatePrePayOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreatePrePayOrder')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreatePrePayOrder','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,38 +38,53 @@
 	def set_IoMax(self, IoMax):  # Integer
 		self.add_query_param('IoMax', IoMax)
 	def get_EipMax(self): # Integer
 		return self.get_query_params().get('EipMax')
 
 	def set_EipMax(self, EipMax):  # Integer
 		self.add_query_param('EipMax', EipMax)
+	def get_Duration(self): # Integer
+		return self.get_query_params().get('Duration')
+
+	def set_Duration(self, Duration):  # Integer
+		self.add_query_param('Duration', Duration)
 	def get_SpecType(self): # String
 		return self.get_query_params().get('SpecType')
 
 	def set_SpecType(self, SpecType):  # String
 		self.add_query_param('SpecType', SpecType)
 	def get_ResourceGroupId(self): # String
 		return self.get_query_params().get('ResourceGroupId')
 
 	def set_ResourceGroupId(self, ResourceGroupId):  # String
 		self.add_query_param('ResourceGroupId', ResourceGroupId)
+	def get_ConfluentConfig(self): # Struct
+		return self.get_query_params().get('ConfluentConfig')
+
+	def set_ConfluentConfig(self, ConfluentConfig):  # Struct
+		self.add_query_param("ConfluentConfig", json.dumps(ConfluentConfig))
 	def get_Tags(self): # RepeatList
 		return self.get_query_params().get('Tag')
 
 	def set_Tags(self, Tag):  # RepeatList
 		for depth1 in range(len(Tag)):
 			if Tag[depth1].get('Value') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Value', Tag[depth1].get('Value'))
 			if Tag[depth1].get('Key') is not None:
 				self.add_query_param('Tag.' + str(depth1 + 1) + '.Key', Tag[depth1].get('Key'))
 	def get_PartitionNum(self): # Integer
 		return self.get_query_params().get('PartitionNum')
 
 	def set_PartitionNum(self, PartitionNum):  # Integer
 		self.add_query_param('PartitionNum', PartitionNum)
+	def get_PaidType(self): # Integer
+		return self.get_query_params().get('PaidType')
+
+	def set_PaidType(self, PaidType):  # Integer
+		self.add_query_param('PaidType', PaidType)
 	def get_DiskSize(self): # Integer
 		return self.get_query_params().get('DiskSize')
 
 	def set_DiskSize(self, DiskSize):  # Integer
 		self.add_query_param('DiskSize', DiskSize)
 	def get_IoMaxSpec(self): # String
 		return self.get_query_params().get('IoMaxSpec')
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateSaslUserRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/EnableAutoTopicCreationRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,38 +16,33 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class CreateSaslUserRequest(RpcRequest):
+class EnableAutoTopicCreationRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateSaslUser')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'EnableAutoTopicCreation','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Type(self): # String
-		return self.get_query_params().get('Type')
-
-	def set_Type(self, Type):  # String
-		self.add_query_param('Type', Type)
-	def get_Password(self): # String
-		return self.get_query_params().get('Password')
-
-	def set_Password(self, Password):  # String
-		self.add_query_param('Password', Password)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
-	def get_Username(self): # String
-		return self.get_query_params().get('Username')
+	def get_Operate(self): # String
+		return self.get_query_params().get('Operate')
+
+	def set_Operate(self, Operate):  # String
+		self.add_query_param('Operate', Operate)
+	def get_PartitionNum(self): # Long
+		return self.get_query_params().get('PartitionNum')
 
-	def set_Username(self, Username):  # String
-		self.add_query_param('Username', Username)
+	def set_PartitionNum(self, PartitionNum):  # Long
+		self.add_query_param('PartitionNum', PartitionNum)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/CreateTopicRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/CreateTopicRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class CreateTopicRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateTopic')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'CreateTopic','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteAclRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DeleteAclRequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class DeleteAclRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteAcl')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteAcl','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,14 +37,19 @@
 	def set_AclResourcePatternType(self, AclResourcePatternType):  # String
 		self.add_query_param('AclResourcePatternType', AclResourcePatternType)
 	def get_AclResourceType(self): # String
 		return self.get_query_params().get('AclResourceType')
 
 	def set_AclResourceType(self, AclResourceType):  # String
 		self.add_query_param('AclResourceType', AclResourceType)
+	def get_AclOperationTypes(self): # String
+		return self.get_query_params().get('AclOperationTypes')
+
+	def set_AclOperationTypes(self, AclOperationTypes):  # String
+		self.add_query_param('AclOperationTypes', AclOperationTypes)
 	def get_AclOperationType(self): # String
 		return self.get_query_params().get('AclOperationType')
 
 	def set_AclOperationType(self, AclOperationType):  # String
 		self.add_query_param('AclOperationType', AclOperationType)
 	def get_AclResourceName(self): # String
 		return self.get_query_params().get('AclResourceName')
@@ -52,12 +57,22 @@
 	def set_AclResourceName(self, AclResourceName):  # String
 		self.add_query_param('AclResourceName', AclResourceName)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
+	def get_Host(self): # String
+		return self.get_query_params().get('Host')
+
+	def set_Host(self, Host):  # String
+		self.add_query_param('Host', Host)
+	def get_AclPermissionType(self): # String
+		return self.get_query_params().get('AclPermissionType')
+
+	def set_AclPermissionType(self, AclPermissionType):  # String
+		self.add_query_param('AclPermissionType', AclPermissionType)
 	def get_Username(self): # String
 		return self.get_query_params().get('Username')
 
 	def set_Username(self, Username):  # String
 		self.add_query_param('Username', Username)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteConsumerGroupRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DeleteConsumerGroupRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class DeleteConsumerGroupRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteConsumerGroup')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteConsumerGroup','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteInstanceRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ReopenInstanceRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class DeleteInstanceRequest(RpcRequest):
+class ReopenInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteInstance')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ReopenInstance','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteSaslUserRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetTopicSubscribeStatusRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,33 +16,28 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class DeleteSaslUserRequest(RpcRequest):
+class GetTopicSubscribeStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteSaslUser')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetTopicSubscribeStatus','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_Type(self): # String
-		return self.get_query_params().get('Type')
-
-	def set_Type(self, Type):  # String
-		self.add_query_param('Type', Type)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
-	def get_Username(self): # String
-		return self.get_query_params().get('Username')
+	def get_Topic(self): # String
+		return self.get_query_params().get('Topic')
 
-	def set_Username(self, Username):  # String
-		self.add_query_param('Username', Username)
+	def set_Topic(self, Topic):  # String
+		self.add_query_param('Topic', Topic)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DeleteTopicRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DeleteTopicRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class DeleteTopicRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteTopic')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DeleteTopic','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DescribeAclsRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DescribeAclsRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class DescribeAclsRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DescribeAcls')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DescribeAcls','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -37,22 +37,37 @@
 	def set_AclResourcePatternType(self, AclResourcePatternType):  # String
 		self.add_query_param('AclResourcePatternType', AclResourcePatternType)
 	def get_AclResourceType(self): # String
 		return self.get_query_params().get('AclResourceType')
 
 	def set_AclResourceType(self, AclResourceType):  # String
 		self.add_query_param('AclResourceType', AclResourceType)
+	def get_AclOperationType(self): # String
+		return self.get_query_params().get('AclOperationType')
+
+	def set_AclOperationType(self, AclOperationType):  # String
+		self.add_query_param('AclOperationType', AclOperationType)
 	def get_AclResourceName(self): # String
 		return self.get_query_params().get('AclResourceName')
 
 	def set_AclResourceName(self, AclResourceName):  # String
 		self.add_query_param('AclResourceName', AclResourceName)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
+	def get_Host(self): # String
+		return self.get_query_params().get('Host')
+
+	def set_Host(self, Host):  # String
+		self.add_query_param('Host', Host)
+	def get_AclPermissionType(self): # String
+		return self.get_query_params().get('AclPermissionType')
+
+	def set_AclPermissionType(self, AclPermissionType):  # String
+		self.add_query_param('AclPermissionType', AclPermissionType)
 	def get_Username(self): # String
 		return self.get_query_params().get('Username')
 
 	def set_Username(self, Username):  # String
 		self.add_query_param('Username', Username)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/DescribeSaslUsersRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/DescribeSaslUsersRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class DescribeSaslUsersRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DescribeSaslUsers')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'DescribeSaslUsers','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetAllInstanceIdListRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetAllInstanceIdListRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetAllInstanceIdListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetAllInstanceIdList')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetAllInstanceIdList','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetAllowedIpListRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetAllowedIpListRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetAllowedIpListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetAllowedIpList')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetAllowedIpList','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetConsumerListRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetConsumerProgressRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,18 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class GetConsumerListRequest(RpcRequest):
+class GetConsumerProgressRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetConsumerList')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetConsumerProgress','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetConsumerProgressRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/StopInstanceRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,28 +16,23 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
-class GetConsumerProgressRequest(RpcRequest):
+class StopInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetConsumerProgress')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'StopInstance','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_ConsumerId(self): # String
-		return self.get_query_params().get('ConsumerId')
-
-	def set_ConsumerId(self, ConsumerId):  # String
-		self.add_query_param('ConsumerId', ConsumerId)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetInstanceListRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetInstanceListRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetInstanceListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetInstanceList')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetInstanceList','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetQuotaTipRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetQuotaTipRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetQuotaTipRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetQuotaTip')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetQuotaTip','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetTopicListRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetTopicListRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetTopicListRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetTopicList')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetTopicList','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/GetTopicStatusRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/GetTopicStatusRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class GetTopicStatusRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetTopicStatus')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'GetTopicStatus','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ListTagResourcesRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ListTagResourcesRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ListTagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ListTagResources')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ListTagResources','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyInstanceNameRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ModifyInstanceNameRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ModifyInstanceNameRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyInstanceName')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyInstanceName','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyPartitionNumRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ModifyPartitionNumRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ModifyPartitionNumRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyPartitionNum')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyPartitionNum','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ModifyTopicRemarkRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ModifyTopicRemarkRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ModifyTopicRemarkRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyTopicRemark')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ModifyTopicRemark','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_Remark(self): # String
+		return self.get_query_params().get('Remark')
+
+	def set_Remark(self, Remark):  # String
+		self.add_query_param('Remark', Remark)
 	def get_InstanceId(self): # String
 		return self.get_query_params().get('InstanceId')
 
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
 	def get_Topic(self): # String
 		return self.get_query_params().get('Topic')
 
 	def set_Topic(self, Topic):  # String
 		self.add_query_param('Topic', Topic)
-	def get_Remark(self): # String
-		return self.get_query_params().get('Remark')
-
-	def set_Remark(self, Remark):  # String
-		self.add_query_param('Remark', Remark)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/ReleaseInstanceRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/ReleaseInstanceRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class ReleaseInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ReleaseInstance')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'ReleaseInstance','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/StartInstanceRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/StartInstanceRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,22 +19,28 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class StartInstanceRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'StartInstance')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'StartInstance','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_VSwitchIdss(self): # RepeatList
+		return self.get_query_params().get('VSwitchIds')
+
+	def set_VSwitchIdss(self, VSwitchIds):  # RepeatList
+		for depth1 in range(len(VSwitchIds)):
+			self.add_query_param('VSwitchIds.' + str(depth1 + 1), VSwitchIds[depth1])
 	def get_SelectedZones(self): # String
 		return self.get_query_params().get('SelectedZones')
 
 	def set_SelectedZones(self, SelectedZones):  # String
 		self.add_query_param('SelectedZones', SelectedZones)
 	def get_IsEipInner(self): # Boolean
 		return self.get_query_params().get('IsEipInner')
@@ -87,14 +93,19 @@
 	def set_InstanceId(self, InstanceId):  # String
 		self.add_query_param('InstanceId', InstanceId)
 	def get_VpcId(self): # String
 		return self.get_query_params().get('VpcId')
 
 	def set_VpcId(self, VpcId):  # String
 		self.add_query_param('VpcId', VpcId)
+	def get_CrossZone(self): # Boolean
+		return self.get_query_params().get('CrossZone')
+
+	def set_CrossZone(self, CrossZone):  # Boolean
+		self.add_query_param('CrossZone', CrossZone)
 	def get_Name(self): # String
 		return self.get_query_params().get('Name')
 
 	def set_Name(self, Name):  # String
 		self.add_query_param('Name', Name)
 	def get_ServiceVersion(self): # String
 		return self.get_query_params().get('ServiceVersion')
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/TagResourcesRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/TagResourcesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class TagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'TagResources')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'TagResources','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UntagResourcesRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UntagResourcesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class UntagResourcesRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UntagResources')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UntagResources','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateAllowedIpRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpdateAllowedIpRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class UpdateAllowedIpRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpdateAllowedIp')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpdateAllowedIp','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateConsumerOffsetRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpdateConsumerOffsetRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 import json
 
 class UpdateConsumerOffsetRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpdateConsumerOffset')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpdateConsumerOffset','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpdateInstanceConfigRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpdateInstanceConfigRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class UpdateInstanceConfigRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpdateInstanceConfig')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpdateInstanceConfig','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradeInstanceVersionRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpgradeInstanceVersionRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
 
 class UpgradeInstanceVersionRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradeInstanceVersion')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradeInstanceVersion','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradePostPayOrderRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpgradePostPayOrderRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,26 +15,32 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
+import json
 
 class UpgradePostPayOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradePostPayOrder')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradePostPayOrder','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
+	def get_ServerlessConfig(self): # Struct
+		return self.get_query_params().get('ServerlessConfig')
+
+	def set_ServerlessConfig(self, ServerlessConfig):  # Struct
+		self.add_query_param("ServerlessConfig", json.dumps(ServerlessConfig))
 	def get_DiskSize(self): # Integer
 		return self.get_query_params().get('DiskSize')
 
 	def set_DiskSize(self, DiskSize):  # Integer
 		self.add_query_param('DiskSize', DiskSize)
 	def get_IoMax(self): # Integer
 		return self.get_query_params().get('IoMax')
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/aliyunsdkalikafka/request/v20190916/UpgradePrePayOrderRequest.py` & `aliyun-python-sdk-alikafka-1.0.6/aliyunsdkalikafka/request/v20190916/UpgradePrePayOrderRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,64 +15,75 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkalikafka.endpoint import endpoint_data
+import json
 
 class UpgradePrePayOrderRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradePrePayOrder')
+		RpcRequest.__init__(self, 'alikafka', '2019-09-16', 'UpgradePrePayOrder','alikafka')
 		self.set_method('POST')
 
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
-	def get_DiskSize(self): # Integer
-		return self.get_query_params().get('DiskSize')
-
-	def set_DiskSize(self, DiskSize):  # Integer
-		self.add_query_param('DiskSize', DiskSize)
 	def get_IoMax(self): # Integer
 		return self.get_query_params().get('IoMax')
 
 	def set_IoMax(self, IoMax):  # Integer
 		self.add_query_param('IoMax', IoMax)
 	def get_EipModel(self): # Boolean
 		return self.get_query_params().get('EipModel')
 
 	def set_EipModel(self, EipModel):  # Boolean
 		self.add_query_param('EipModel', EipModel)
-	def get_IoMaxSpec(self): # String
-		return self.get_query_params().get('IoMaxSpec')
-
-	def set_IoMaxSpec(self, IoMaxSpec):  # String
-		self.add_query_param('IoMaxSpec', IoMaxSpec)
-	def get_TopicQuota(self): # Integer
-		return self.get_query_params().get('TopicQuota')
-
-	def set_TopicQuota(self, TopicQuota):  # Integer
-		self.add_query_param('TopicQuota', TopicQuota)
 	def get_EipMax(self): # Integer
 		return self.get_query_params().get('EipMax')
 
 	def set_EipMax(self, EipMax):  # Integer
 		self.add_query_param('EipMax', EipMax)
 	def get_SpecType(self): # String
 		return self.get_query_params().get('SpecType')
 
 	def set_SpecType(self, SpecType):  # String
 		self.add_query_param('SpecType', SpecType)
-	def get_InstanceId(self): # String
-		return self.get_query_params().get('InstanceId')
+	def get_ConfluentConfig(self): # Struct
+		return self.get_query_params().get('ConfluentConfig')
 
-	def set_InstanceId(self, InstanceId):  # String
-		self.add_query_param('InstanceId', InstanceId)
+	def set_ConfluentConfig(self, ConfluentConfig):  # Struct
+		self.add_query_param("ConfluentConfig", json.dumps(ConfluentConfig))
 	def get_PartitionNum(self): # Integer
 		return self.get_query_params().get('PartitionNum')
 
 	def set_PartitionNum(self, PartitionNum):  # Integer
 		self.add_query_param('PartitionNum', PartitionNum)
+	def get_PaidType(self): # Integer
+		return self.get_query_params().get('PaidType')
+
+	def set_PaidType(self, PaidType):  # Integer
+		self.add_query_param('PaidType', PaidType)
+	def get_DiskSize(self): # Integer
+		return self.get_query_params().get('DiskSize')
+
+	def set_DiskSize(self, DiskSize):  # Integer
+		self.add_query_param('DiskSize', DiskSize)
+	def get_IoMaxSpec(self): # String
+		return self.get_query_params().get('IoMaxSpec')
+
+	def set_IoMaxSpec(self, IoMaxSpec):  # String
+		self.add_query_param('IoMaxSpec', IoMaxSpec)
+	def get_TopicQuota(self): # Integer
+		return self.get_query_params().get('TopicQuota')
+
+	def set_TopicQuota(self, TopicQuota):  # Integer
+		self.add_query_param('TopicQuota', TopicQuota)
+	def get_InstanceId(self): # String
+		return self.get_query_params().get('InstanceId')
+
+	def set_InstanceId(self, InstanceId):  # String
+		self.add_query_param('InstanceId', InstanceId)
```

### Comparing `aliyun-python-sdk-alikafka-1.0.5/setup.py` & `aliyun-python-sdk-alikafka-1.0.6/setup.py`

 * *Files identical despite different names*

