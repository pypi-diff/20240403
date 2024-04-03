# Comparing `tmp/aliyun-python-sdk-cloudauth-2.0.8.tar.gz` & `tmp/aliyun-python-sdk-cloudauth-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-cloudauth-2.0.8.tar", last modified: Wed Apr  8 13:41:05 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-cloudauth-2.0.9.tar", last modified: Mon Apr 20 06:54:53 2020, max compression
```

## Comparing `aliyun-python-sdk-cloudauth-2.0.8.tar` & `aliyun-python-sdk-cloudauth-2.0.9.tar`

### file list

```diff
@@ -1,45 +1,49 @@
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/
--rw-rw-r--   0 admin      (531) admin      (531)       38 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/setup.cfg
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyun_python_sdk_cloudauth.egg-info/
--rw-rw-r--   0 admin      (531) admin      (531)        1 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyun_python_sdk_cloudauth.egg-info/dependency_links.txt
--rw-rw-r--   0 admin      (531) admin      (531)       31 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyun_python_sdk_cloudauth.egg-info/requires.txt
--rw-rw-r--   0 admin      (531) admin      (531)     2117 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyun_python_sdk_cloudauth.egg-info/SOURCES.txt
--rw-rw-r--   0 admin      (531) admin      (531)       19 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyun_python_sdk_cloudauth.egg-info/top_level.txt
--rw-rw-r--   0 admin      (531) admin      (531)     1567 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyun_python_sdk_cloudauth.egg-info/PKG-INFO
--rw-rw-r--   0 admin      (531) admin      (531)     2482 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/setup.py
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/
--rw-rw-r--   0 admin      (531) admin      (531)       21 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/__init__.py
--rw-rw-r--   0 admin      (531) admin      (531)     1087 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/endpoint.py
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/
--rw-rw-r--   0 admin      (531) admin      (531)        0 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/__init__.py
-drwxrwxr-x   0 admin      (531) admin      (531)        0 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/
--rw-rw-r--   0 admin      (531) admin      (531)        0 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/__init__.py
--rw-rw-r--   0 admin      (531) admin      (531)     2251 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/UpdateVerifySettingRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1565 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifyResultRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2493 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeDeviceInfoRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2833 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DetectFaceAttributesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1273 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeOssUploadTokenRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1583 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeFaceUsageRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     4045 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifyTokenRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1567 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/CreateVerifySDKRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1585 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeFaceVerifyRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1411 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifySDKRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2251 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/CreateVerifySettingRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1769 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/VerifyDeviceRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2337 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/CompareFacesRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     3141 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/InitDeviceRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     3863 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/ContrastFaceVerifyRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2091 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/ModifyDeviceInfoRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     4003 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/InitFaceVerifyRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1895 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/CreateAuthKeyRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1855 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/CreateRPSDKRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1271 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifySettingRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1265 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeUserStatusRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2889 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifyRecordsRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1265 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeUploadInfoRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1699 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeRPSDKRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     2651 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/VerifyMaterialRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)     1741 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifyUsageRequest.py
--rw-rw-r--   0 admin      (531) admin      (531)        0 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/MANIFEST.in
--rw-rw-r--   0 admin      (531) admin      (531)      539 2020-04-08 13:41:04.000000 aliyun-python-sdk-cloudauth-2.0.8/README.rst
--rw-rw-r--   0 admin      (531) admin      (531)     1567 2020-04-08 13:41:05.000000 aliyun-python-sdk-cloudauth-2.0.8/PKG-INFO
+drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/
+-rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/MANIFEST.in
+drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyun_python_sdk_cloudauth.egg-info/
+-rw-rw-r--   0 admin     (1017) admin     (1017)        1 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyun_python_sdk_cloudauth.egg-info/dependency_links.txt
+-rw-rw-r--   0 admin     (1017) admin     (1017)       19 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyun_python_sdk_cloudauth.egg-info/top_level.txt
+-rw-rw-r--   0 admin     (1017) admin     (1017)       31 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyun_python_sdk_cloudauth.egg-info/requires.txt
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2381 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyun_python_sdk_cloudauth.egg-info/SOURCES.txt
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1567 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyun_python_sdk_cloudauth.egg-info/PKG-INFO
+drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/
+-rw-rw-r--   0 admin     (1017) admin     (1017)       21 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/__init__.py
+drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/
+-rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/__init__.py
+drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2091 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/ModifyDeviceInfoRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1273 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeOssUploadTokenRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2337 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/CompareFacesRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1741 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifyUsageRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2493 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeDeviceInfoRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2251 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/UpdateVerifySettingRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     4003 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/InitFaceVerifyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1757 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeAppInfoRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     4045 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifyTokenRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2651 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/VerifyMaterialRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/__init__.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1585 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeFaceVerifyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1567 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/CreateVerifySDKRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1395 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeUploadInfoRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1431 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeUpdatePackageResultRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2889 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifyRecordsRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1895 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/CreateAuthKeyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     3863 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/ContrastFaceVerifyRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1411 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifySDKRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1265 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeUserStatusRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     3141 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/InitDeviceRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1523 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeSdkUrlRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1699 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeRPSDKRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1859 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/UpdateAppPackageRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1565 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifyResultRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1583 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeFaceUsageRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2251 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/CreateVerifySettingRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1769 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/VerifyDeviceRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2833 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DetectFaceAttributesRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1855 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/CreateRPSDKRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1271 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifySettingRequest.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1087 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/endpoint.py
+-rw-rw-r--   0 admin     (1017) admin     (1017)       38 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/setup.cfg
+-rw-rw-r--   0 admin     (1017) admin     (1017)      539 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/README.rst
+-rw-rw-r--   0 admin     (1017) admin     (1017)     1567 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/PKG-INFO
+-rw-rw-r--   0 admin     (1017) admin     (1017)     2482 2020-04-20 06:54:53.000000 aliyun-python-sdk-cloudauth-2.0.9/setup.py
```

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyun_python_sdk_cloudauth.egg-info/SOURCES.txt` & `aliyun-python-sdk-cloudauth-2.0.9/aliyun_python_sdk_cloudauth.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,28 +11,32 @@
 aliyunsdkcloudauth/request/__init__.py
 aliyunsdkcloudauth/request/v20190307/CompareFacesRequest.py
 aliyunsdkcloudauth/request/v20190307/ContrastFaceVerifyRequest.py
 aliyunsdkcloudauth/request/v20190307/CreateAuthKeyRequest.py
 aliyunsdkcloudauth/request/v20190307/CreateRPSDKRequest.py
 aliyunsdkcloudauth/request/v20190307/CreateVerifySDKRequest.py
 aliyunsdkcloudauth/request/v20190307/CreateVerifySettingRequest.py
+aliyunsdkcloudauth/request/v20190307/DescribeAppInfoRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeDeviceInfoRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeFaceUsageRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeFaceVerifyRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeOssUploadTokenRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeRPSDKRequest.py
+aliyunsdkcloudauth/request/v20190307/DescribeSdkUrlRequest.py
+aliyunsdkcloudauth/request/v20190307/DescribeUpdatePackageResultRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeUploadInfoRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeUserStatusRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeVerifyRecordsRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeVerifyResultRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeVerifySDKRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeVerifySettingRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeVerifyTokenRequest.py
 aliyunsdkcloudauth/request/v20190307/DescribeVerifyUsageRequest.py
 aliyunsdkcloudauth/request/v20190307/DetectFaceAttributesRequest.py
 aliyunsdkcloudauth/request/v20190307/InitDeviceRequest.py
 aliyunsdkcloudauth/request/v20190307/InitFaceVerifyRequest.py
 aliyunsdkcloudauth/request/v20190307/ModifyDeviceInfoRequest.py
+aliyunsdkcloudauth/request/v20190307/UpdateAppPackageRequest.py
 aliyunsdkcloudauth/request/v20190307/UpdateVerifySettingRequest.py
 aliyunsdkcloudauth/request/v20190307/VerifyDeviceRequest.py
 aliyunsdkcloudauth/request/v20190307/VerifyMaterialRequest.py
 aliyunsdkcloudauth/request/v20190307/__init__.py
```

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyun_python_sdk_cloudauth.egg-info/PKG-INFO` & `aliyun-python-sdk-cloudauth-2.0.9/aliyun_python_sdk_cloudauth.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cloudauth
-Version: 2.0.8
+Version: 2.0.9
 Summary: The cloudauth module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cloudauth
```

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/setup.py` & `aliyun-python-sdk-cloudauth-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/endpoint.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/endpoint.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/UpdateVerifySettingRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/UpdateVerifySettingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifyResultRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifyResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeDeviceInfoRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeDeviceInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DetectFaceAttributesRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DetectFaceAttributesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeOssUploadTokenRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeOssUploadTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeFaceUsageRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeFaceUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifyTokenRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifyTokenRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/CreateVerifySDKRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/CreateVerifySDKRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeFaceVerifyRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeFaceVerifyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifySDKRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifySDKRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/CreateVerifySettingRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/CreateVerifySettingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/VerifyDeviceRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/VerifyDeviceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/CompareFacesRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/CompareFacesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/InitDeviceRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/InitDeviceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/ContrastFaceVerifyRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/InitFaceVerifyRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,65 +16,35 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcloudauth.endpoint import endpoint_data
 
-class ContrastFaceVerifyRequest(RpcRequest):
+class InitFaceVerifyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cloudauth', '2019-03-07', 'ContrastFaceVerify','cloudauth')
+		RpcRequest.__init__(self, 'Cloudauth', '2019-03-07', 'InitFaceVerify','cloudauth')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ProductCode(self):
 		return self.get_query_params().get('ProductCode')
 
 	def set_ProductCode(self,ProductCode):
 		self.add_query_param('ProductCode',ProductCode)
 
-	def get_OssObjectName(self):
-		return self.get_query_params().get('OssObjectName')
-
-	def set_OssObjectName(self,OssObjectName):
-		self.add_query_param('OssObjectName',OssObjectName)
-
 	def get_FaceContrastPicture(self):
-		return self.get_query_params().get('FaceContrastPicture')
+		return self.get_body_params().get('FaceContrastPicture')
 
 	def set_FaceContrastPicture(self,FaceContrastPicture):
-		self.add_query_param('FaceContrastPicture',FaceContrastPicture)
-
-	def get_CertName(self):
-		return self.get_query_params().get('CertName')
-
-	def set_CertName(self,CertName):
-		self.add_query_param('CertName',CertName)
-
-	def get_Ip(self):
-		return self.get_query_params().get('Ip')
-
-	def set_Ip(self,Ip):
-		self.add_query_param('Ip',Ip)
-
-	def get_Mobile(self):
-		return self.get_query_params().get('Mobile')
-
-	def set_Mobile(self,Mobile):
-		self.add_query_param('Mobile',Mobile)
-
-	def get_DeviceToken(self):
-		return self.get_query_params().get('DeviceToken')
-
-	def set_DeviceToken(self,DeviceToken):
-		self.add_query_param('DeviceToken',DeviceToken)
+		self.add_body_params('FaceContrastPicture', FaceContrastPicture)
 
 	def get_UserId(self):
 		return self.get_query_params().get('UserId')
 
 	def set_UserId(self,UserId):
 		self.add_query_param('UserId',UserId)
 
@@ -104,18 +74,54 @@
 
 	def get_FaceContrastPictureUrl(self):
 		return self.get_query_params().get('FaceContrastPictureUrl')
 
 	def set_FaceContrastPictureUrl(self,FaceContrastPictureUrl):
 		self.add_query_param('FaceContrastPictureUrl',FaceContrastPictureUrl)
 
+	def get_MetaInfo(self):
+		return self.get_query_params().get('MetaInfo')
+
+	def set_MetaInfo(self,MetaInfo):
+		self.add_query_param('MetaInfo',MetaInfo)
+
+	def get_OssObjectName(self):
+		return self.get_query_params().get('OssObjectName')
+
+	def set_OssObjectName(self,OssObjectName):
+		self.add_query_param('OssObjectName',OssObjectName)
+
+	def get_CertName(self):
+		return self.get_query_params().get('CertName')
+
+	def set_CertName(self,CertName):
+		self.add_query_param('CertName',CertName)
+
+	def get_Ip(self):
+		return self.get_query_params().get('Ip')
+
+	def set_Ip(self,Ip):
+		self.add_query_param('Ip',Ip)
+
+	def get_Mobile(self):
+		return self.get_query_params().get('Mobile')
+
+	def set_Mobile(self,Mobile):
+		self.add_query_param('Mobile',Mobile)
+
 	def get_SceneId(self):
 		return self.get_query_params().get('SceneId')
 
 	def set_SceneId(self,SceneId):
 		self.add_query_param('SceneId',SceneId)
 
 	def get_OssBucketName(self):
 		return self.get_query_params().get('OssBucketName')
 
 	def set_OssBucketName(self,OssBucketName):
-		self.add_query_param('OssBucketName',OssBucketName)
+		self.add_query_param('OssBucketName',OssBucketName)
+
+	def get_ReturnUrl(self):
+		return self.get_query_params().get('ReturnUrl')
+
+	def set_ReturnUrl(self,ReturnUrl):
+		self.add_query_param('ReturnUrl',ReturnUrl)
```

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/ModifyDeviceInfoRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/ModifyDeviceInfoRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/InitFaceVerifyRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/ContrastFaceVerifyRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,112 +16,106 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 from aliyunsdkcloudauth.endpoint import endpoint_data
 
-class InitFaceVerifyRequest(RpcRequest):
+class ContrastFaceVerifyRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'Cloudauth', '2019-03-07', 'InitFaceVerify','cloudauth')
+		RpcRequest.__init__(self, 'Cloudauth', '2019-03-07', 'ContrastFaceVerify','cloudauth')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ProductCode(self):
-		return self.get_query_params().get('ProductCode')
+		return self.get_body_params().get('ProductCode')
 
 	def set_ProductCode(self,ProductCode):
-		self.add_query_param('ProductCode',ProductCode)
+		self.add_body_params('ProductCode', ProductCode)
+
+	def get_OssObjectName(self):
+		return self.get_body_params().get('OssObjectName')
+
+	def set_OssObjectName(self,OssObjectName):
+		self.add_body_params('OssObjectName', OssObjectName)
 
 	def get_FaceContrastPicture(self):
-		return self.get_query_params().get('FaceContrastPicture')
+		return self.get_body_params().get('FaceContrastPicture')
 
 	def set_FaceContrastPicture(self,FaceContrastPicture):
-		self.add_query_param('FaceContrastPicture',FaceContrastPicture)
+		self.add_body_params('FaceContrastPicture', FaceContrastPicture)
+
+	def get_CertName(self):
+		return self.get_body_params().get('CertName')
+
+	def set_CertName(self,CertName):
+		self.add_body_params('CertName', CertName)
+
+	def get_Ip(self):
+		return self.get_body_params().get('Ip')
+
+	def set_Ip(self,Ip):
+		self.add_body_params('Ip', Ip)
+
+	def get_Mobile(self):
+		return self.get_body_params().get('Mobile')
+
+	def set_Mobile(self,Mobile):
+		self.add_body_params('Mobile', Mobile)
+
+	def get_DeviceToken(self):
+		return self.get_body_params().get('DeviceToken')
+
+	def set_DeviceToken(self,DeviceToken):
+		self.add_body_params('DeviceToken', DeviceToken)
 
 	def get_UserId(self):
-		return self.get_query_params().get('UserId')
+		return self.get_body_params().get('UserId')
 
 	def set_UserId(self,UserId):
-		self.add_query_param('UserId',UserId)
+		self.add_body_params('UserId', UserId)
 
 	def get_CertifyId(self):
-		return self.get_query_params().get('CertifyId')
+		return self.get_body_params().get('CertifyId')
 
 	def set_CertifyId(self,CertifyId):
-		self.add_query_param('CertifyId',CertifyId)
+		self.add_body_params('CertifyId', CertifyId)
 
 	def get_CertNo(self):
-		return self.get_query_params().get('CertNo')
+		return self.get_body_params().get('CertNo')
 
 	def set_CertNo(self,CertNo):
-		self.add_query_param('CertNo',CertNo)
+		self.add_body_params('CertNo', CertNo)
 
 	def get_OuterOrderNo(self):
-		return self.get_query_params().get('OuterOrderNo')
+		return self.get_body_params().get('OuterOrderNo')
 
 	def set_OuterOrderNo(self,OuterOrderNo):
-		self.add_query_param('OuterOrderNo',OuterOrderNo)
+		self.add_body_params('OuterOrderNo', OuterOrderNo)
 
 	def get_CertType(self):
-		return self.get_query_params().get('CertType')
+		return self.get_body_params().get('CertType')
 
 	def set_CertType(self,CertType):
-		self.add_query_param('CertType',CertType)
+		self.add_body_params('CertType', CertType)
 
 	def get_FaceContrastPictureUrl(self):
-		return self.get_query_params().get('FaceContrastPictureUrl')
+		return self.get_body_params().get('FaceContrastPictureUrl')
 
 	def set_FaceContrastPictureUrl(self,FaceContrastPictureUrl):
-		self.add_query_param('FaceContrastPictureUrl',FaceContrastPictureUrl)
-
-	def get_MetaInfo(self):
-		return self.get_query_params().get('MetaInfo')
-
-	def set_MetaInfo(self,MetaInfo):
-		self.add_query_param('MetaInfo',MetaInfo)
-
-	def get_OssObjectName(self):
-		return self.get_query_params().get('OssObjectName')
-
-	def set_OssObjectName(self,OssObjectName):
-		self.add_query_param('OssObjectName',OssObjectName)
-
-	def get_CertName(self):
-		return self.get_query_params().get('CertName')
-
-	def set_CertName(self,CertName):
-		self.add_query_param('CertName',CertName)
-
-	def get_Ip(self):
-		return self.get_query_params().get('Ip')
-
-	def set_Ip(self,Ip):
-		self.add_query_param('Ip',Ip)
-
-	def get_Mobile(self):
-		return self.get_query_params().get('Mobile')
-
-	def set_Mobile(self,Mobile):
-		self.add_query_param('Mobile',Mobile)
+		self.add_body_params('FaceContrastPictureUrl', FaceContrastPictureUrl)
 
 	def get_SceneId(self):
-		return self.get_query_params().get('SceneId')
+		return self.get_body_params().get('SceneId')
 
 	def set_SceneId(self,SceneId):
-		self.add_query_param('SceneId',SceneId)
+		self.add_body_params('SceneId', SceneId)
 
 	def get_OssBucketName(self):
-		return self.get_query_params().get('OssBucketName')
+		return self.get_body_params().get('OssBucketName')
 
 	def set_OssBucketName(self,OssBucketName):
-		self.add_query_param('OssBucketName',OssBucketName)
-
-	def get_ReturnUrl(self):
-		return self.get_query_params().get('ReturnUrl')
-
-	def set_ReturnUrl(self,ReturnUrl):
-		self.add_query_param('ReturnUrl',ReturnUrl)
+		self.add_body_params('OssBucketName', OssBucketName)
```

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/CreateAuthKeyRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/CreateAuthKeyRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/CreateRPSDKRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/CreateRPSDKRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifySettingRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifySettingRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeUserStatusRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeUserStatusRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifyRecordsRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifyRecordsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeUploadInfoRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeUploadInfoRequest.py`

 * *Files 22% similar despite different names*

```diff
@@ -24,7 +24,14 @@
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'Cloudauth', '2019-03-07', 'DescribeUploadInfo','cloudauth')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
+
+
+	def get_Biz(self):
+		return self.get_query_params().get('Biz')
+
+	def set_Biz(self,Biz):
+		self.add_query_param('Biz',Biz)
```

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeRPSDKRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeRPSDKRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/VerifyMaterialRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/VerifyMaterialRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/aliyunsdkcloudauth/request/v20190307/DescribeVerifyUsageRequest.py` & `aliyun-python-sdk-cloudauth-2.0.9/aliyunsdkcloudauth/request/v20190307/DescribeVerifyUsageRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/README.rst` & `aliyun-python-sdk-cloudauth-2.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-cloudauth-2.0.8/PKG-INFO` & `aliyun-python-sdk-cloudauth-2.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-cloudauth
-Version: 2.0.8
+Version: 2.0.9
 Summary: The cloudauth module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-cloudauth
```

