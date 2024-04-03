# Comparing `tmp/speakeasy-client-sdk-python-5.6.1.tar.gz` & `tmp/speakeasy-client-sdk-python-5.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "speakeasy-client-sdk-python-5.6.1.tar", last modified: Wed Apr  3 09:00:36 2024, max compression
+gzip compressed data, was "speakeasy-client-sdk-python-5.6.2.tar", last modified: Wed Apr  3 11:05:06 2024, max compression
```

## Comparing `speakeasy-client-sdk-python-5.6.1.tar` & `speakeasy-client-sdk-python-5.6.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:00:36.118274 speakeasy-client-sdk-python-5.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-04-03 09:00:36.118274 speakeasy-client-sdk-python-5.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 09:00:36.118274 speakeasy-client-sdk-python-5.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1644 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:00:36.102274 speakeasy-client-sdk-python-5.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:00:36.102274 speakeasy-client-sdk-python-5.6.1/src/speakeasy/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:00:36.106274 speakeasy-client-sdk-python-5.6.1/src/speakeasy/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    29322 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/apiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    22126 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/apis.py
--rw-r--r--   0 runner    (1001) docker     (127)    13891 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/embeds.py
--rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/events.py
--rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:00:36.106274 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:00:36.106274 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/errors/error.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:00:36.110274 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/deleteapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/deleteapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/deleteschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/deleteversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/downloadschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/downloadschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/findapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/generateopenapispec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/generatepostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/generaterequestpostmancollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getallapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getallapiversions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getallforversionapiendpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getapis.py
--rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getrequestfromeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getschema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getschemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getschemarevision.py
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getschemas.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getuser.py
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getvalidembedaccesstokens.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getworkspaceaccess.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getworkspacetargets.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/insertversionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/postworkspaceevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/queryeventlog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/registerschema.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/revokeembedaccesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/upsertapi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/upsertapiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/validateapikey.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:00:36.114274 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/accessdetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/accesstoken.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/api_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/apiendpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/apiendpoint_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/apikeydetails.py
--rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/boundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/clievent.py
--rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/embedaccesstokenresponse.py
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/embedtoken.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/filter_.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/generateopenapispecdiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/interactiontype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/requestmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/schemadiff.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/targetsdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/unboundedrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/versionmetadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/versionmetadata_input.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28778 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/sdkconfiguration.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:00:36.114274 speakeasy-client-sdk-python-5.6.1/src/speakeasy/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30022 2024-04-03 09:00:27.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 09:00:36.118274 speakeasy-client-sdk-python-5.6.1/src/speakeasy_client_sdk_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20667 2024-04-03 09:00:35.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-03 09:00:36.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 09:00:35.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 09:00:35.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy_client_sdk_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 09:00:35.000000 speakeasy-client-sdk-python-5.6.1/src/speakeasy_client_sdk_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:06.499003 speakeasy-client-sdk-python-5.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    20475 2024-04-03 11:05:06.499003 speakeasy-client-sdk-python-5.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13565 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 11:05:06.499003 speakeasy-client-sdk-python-5.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:06.483003 speakeasy-client-sdk-python-5.6.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:06.487003 speakeasy-client-sdk-python-5.6.2/src/speakeasy/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:06.487003 speakeasy-client-sdk-python-5.6.2/src/speakeasy/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      625 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29322 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/apiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22126 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/apis.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13891 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10492 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/embeds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12124 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10832 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:06.487003 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:06.487003 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/errors/error.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:06.495003 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/deleteapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/deleteapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/deleteschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/deleteversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/downloadschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/downloadschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/findapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/generateopenapispec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/generatepostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/generaterequestpostmancollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getallapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getallapiversions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getallforversionapiendpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1543 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getapis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getrequestfromeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1306 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getschemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1513 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getschemarevision.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getschemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getuser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getvalidembedaccesstokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getworkspaceaccess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getworkspacetargets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/insertversionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/postworkspaceevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/queryeventlog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/registerschema.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/revokeembedaccesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/upsertapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/upsertapiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/validateapikey.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:06.495003 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/accessdetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2414 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/accesstoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2330 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/api_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/apiendpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/apiendpoint_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/apikeydetails.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3288 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/boundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13210 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/clievent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      556 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/embedaccesstokenresponse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/embedtoken.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/filter_.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/generateopenapispecdiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/interactiontype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1641 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/requestmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/schemadiff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/targetsdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/unboundedrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/versionmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/versionmetadata_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11565 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28778 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4509 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1563 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/sdkconfiguration.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:06.499003 speakeasy-client-sdk-python-5.6.2/src/speakeasy/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30022 2024-04-03 11:04:57.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 11:05:06.499003 speakeasy-client-sdk-python-5.6.2/src/speakeasy_client_sdk_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20475 2024-04-03 11:05:06.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy_client_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-03 11:05:06.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 11:05:06.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy_client_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 11:05:06.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy_client_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-03 11:05:06.000000 speakeasy-client-sdk-python-5.6.2/src/speakeasy_client_sdk_python.egg-info/top_level.txt
```

### Comparing `speakeasy-client-sdk-python-5.6.1/PKG-INFO` & `speakeasy-client-sdk-python-5.6.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.6.1
+Version: 5.6.2
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -41,79 +41,79 @@
         
         ```
         <!-- End SDK Example Usage [usage] -->
         
         <!-- Start Available Resources and Operations [operations] -->
         ## Available Resources and Operations
         
-        ### [apis](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md)
+        ### [apis](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md)
         
-        * [delete_api](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#delete_api) - Delete an Api.
-        * [generate_open_api_spec](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#generate_open_api_spec) - Generate an OpenAPI specification for a particular Api.
-        * [generate_postman_collection](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#generate_postman_collection) - Generate a Postman collection for a particular Api.
-        * [get_all_api_versions](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#get_all_api_versions) - Get all Api versions for a particular ApiEndpoint.
-        * [get_apis](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#get_apis) - Get a list of Apis for a given workspace
-        * [upsert_api](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#upsert_api) - Upsert an Api
+        * [delete_api](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#delete_api) - Delete an Api.
+        * [generate_open_api_spec](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#generate_open_api_spec) - Generate an OpenAPI specification for a particular Api.
+        * [generate_postman_collection](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#generate_postman_collection) - Generate a Postman collection for a particular Api.
+        * [get_all_api_versions](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#get_all_api_versions) - Get all Api versions for a particular ApiEndpoint.
+        * [get_apis](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#get_apis) - Get a list of Apis for a given workspace
+        * [upsert_api](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#upsert_api) - Upsert an Api
         
-        ### [api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md)
+        ### [api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md)
         
-        * [delete_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#delete_api_endpoint) - Delete an ApiEndpoint.
-        * [find_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#find_api_endpoint) - Find an ApiEndpoint via its displayName.
-        * [generate_open_api_spec_for_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#generate_open_api_spec_for_api_endpoint) - Generate an OpenAPI specification for a particular ApiEndpoint.
-        * [generate_postman_collection_for_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#generate_postman_collection_for_api_endpoint) - Generate a Postman collection for a particular ApiEndpoint.
-        * [get_all_api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#get_all_api_endpoints) - Get all Api endpoints for a particular apiID.
-        * [get_all_for_version_api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#get_all_for_version_api_endpoints) - Get all ApiEndpoints for a particular apiID and versionID.
-        * [get_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#get_api_endpoint) - Get an ApiEndpoint.
-        * [upsert_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#upsert_api_endpoint) - Upsert an ApiEndpoint.
+        * [delete_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#delete_api_endpoint) - Delete an ApiEndpoint.
+        * [find_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#find_api_endpoint) - Find an ApiEndpoint via its displayName.
+        * [generate_open_api_spec_for_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#generate_open_api_spec_for_api_endpoint) - Generate an OpenAPI specification for a particular ApiEndpoint.
+        * [generate_postman_collection_for_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#generate_postman_collection_for_api_endpoint) - Generate a Postman collection for a particular ApiEndpoint.
+        * [get_all_api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#get_all_api_endpoints) - Get all Api endpoints for a particular apiID.
+        * [get_all_for_version_api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#get_all_for_version_api_endpoints) - Get all ApiEndpoints for a particular apiID and versionID.
+        * [get_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#get_api_endpoint) - Get an ApiEndpoint.
+        * [upsert_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#upsert_api_endpoint) - Upsert an ApiEndpoint.
         
-        ### [metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/metadata/README.md)
+        ### [metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/metadata/README.md)
         
-        * [delete_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/metadata/README.md#delete_version_metadata) - Delete metadata for a particular apiID and versionID.
-        * [get_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/metadata/README.md#get_version_metadata) - Get all metadata for a particular apiID and versionID.
-        * [insert_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/metadata/README.md#insert_version_metadata) - Insert metadata for a particular apiID and versionID.
+        * [delete_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/metadata/README.md#delete_version_metadata) - Delete metadata for a particular apiID and versionID.
+        * [get_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/metadata/README.md#get_version_metadata) - Get all metadata for a particular apiID and versionID.
+        * [insert_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/metadata/README.md#insert_version_metadata) - Insert metadata for a particular apiID and versionID.
         
-        ### [schemas](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md)
+        ### [schemas](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md)
         
-        * [delete_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#delete_schema) - Delete a particular schema revision for an Api.
-        * [download_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#download_schema) - Download the latest schema for a particular apiID.
-        * [download_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#download_schema_revision) - Download a particular schema revision for an Api.
-        * [get_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#get_schema) - Get information about the latest schema.
-        * [get_schema_diff](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#get_schema_diff) - Get a diff of two schema revisions for an Api.
-        * [get_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#get_schema_revision) - Get information about a particular schema revision for an Api.
-        * [get_schemas](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#get_schemas) - Get information about all schemas associated with a particular apiID.
-        * [register_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#register_schema) - Register a schema.
+        * [delete_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#delete_schema) - Delete a particular schema revision for an Api.
+        * [download_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#download_schema) - Download the latest schema for a particular apiID.
+        * [download_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#download_schema_revision) - Download a particular schema revision for an Api.
+        * [get_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema) - Get information about the latest schema.
+        * [get_schema_diff](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema_diff) - Get a diff of two schema revisions for an Api.
+        * [get_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema_revision) - Get information about a particular schema revision for an Api.
+        * [get_schemas](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schemas) - Get information about all schemas associated with a particular apiID.
+        * [register_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#register_schema) - Register a schema.
         
-        ### [auth](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/auth/README.md)
+        ### [auth](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md)
         
-        * [get_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/auth/README.md#get_access_token) - Get or refresh an access token for the current workspace.
-        * [get_user](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/auth/README.md#get_user) - Get information about the current user.
-        * [get_workspace_access](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/auth/README.md#get_workspace_access) - Get access allowances for a particular workspace
-        * [validate_api_key](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/auth/README.md#validate_api_key) - Validate the current api key.
+        * [get_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_access_token) - Get or refresh an access token for the current workspace.
+        * [get_user](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_user) - Get information about the current user.
+        * [get_workspace_access](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_workspace_access) - Get access allowances for a particular workspace
+        * [validate_api_key](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#validate_api_key) - Validate the current api key.
         
-        ### [requests](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/requests/README.md)
+        ### [requests](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md)
         
-        * [generate_request_postman_collection](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/requests/README.md#generate_request_postman_collection) - Generate a Postman collection for a particular request.
-        * [get_request_from_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/requests/README.md#get_request_from_event_log) - Get information about a particular request.
-        * [query_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/requests/README.md#query_event_log) - Query the event log to retrieve a list of requests.
+        * [generate_request_postman_collection](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#generate_request_postman_collection) - Generate a Postman collection for a particular request.
+        * [get_request_from_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#get_request_from_event_log) - Get information about a particular request.
+        * [query_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#query_event_log) - Query the event log to retrieve a list of requests.
         
-        ### [organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/organizations/README.md)
+        ### [organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md)
         
-        * [get_organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/organizations/README.md#get_organizations) - Get organizations for a user
+        * [get_organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md#get_organizations) - Get organizations for a user
         
-        ### [embeds](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/embeds/README.md)
+        ### [embeds](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md)
         
-        * [get_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/embeds/README.md#get_embed_access_token) - Get an embed access token for the current workspace.
-        * [get_valid_embed_access_tokens](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/embeds/README.md#get_valid_embed_access_tokens) - Get all valid embed access tokens for the current workspace.
-        * [revoke_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/embeds/README.md#revoke_embed_access_token) - Revoke an embed access EmbedToken.
+        * [get_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_embed_access_token) - Get an embed access token for the current workspace.
+        * [get_valid_embed_access_tokens](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_valid_embed_access_tokens) - Get all valid embed access tokens for the current workspace.
+        * [revoke_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#revoke_embed_access_token) - Revoke an embed access EmbedToken.
         
-        ### [events](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/events/README.md)
+        ### [events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md)
         
-        * [get_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/events/README.md#get_workspace_events) - Load recent events for a particular workspace
-        * [get_workspace_targets](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/events/README.md#get_workspace_targets) - Load targets for a particular workspace
-        * [post_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/events/README.md#post_workspace_events) - Post events for a specific workspace
+        * [get_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#get_workspace_events) - Load recent events for a particular workspace
+        * [get_workspace_targets](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#get_workspace_targets) - Load targets for a particular workspace
+        * [post_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#post_workspace_events) - Post events for a specific workspace
         <!-- End Available Resources and Operations [operations] -->
```

### Comparing `speakeasy-client-sdk-python-5.6.1/README.md` & `speakeasy-client-sdk-python-5.6.2/README.md`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/setup.py` & `speakeasy-client-sdk-python-5.6.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,26 +3,27 @@
 import setuptools
 import re
 
 try:
     with open('README.md', 'r') as fh:
         long_description = fh.read()
         GITHUB_URL = 'https://github.com/speakeasy-api/speakeasy-client-sdk-python.git'
+        GITHUB_URL = GITHUB_URL[: -len('.git')] if GITHUB_URL.endswith('.git') else GITHUB_URL
         # links on PyPI should have absolute URLs
         long_description = re.sub(
             r'(\[[^\]]+\]\()((?!https?:)[^\)]+)(\))',
             lambda m: m.group(1) + GITHUB_URL + '/blob/master/' + m.group(2) + m.group(3),
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='speakeasy-client-sdk-python',
-    version='5.6.1',
+    version='5.6.2',
     author='Speakeasy',
     description='Speakeasy API Client SDK for Python',
     url='https://github.com/speakeasy-api/speakeasy-client-sdk-python.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/_hooks/registration.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/_hooks/registration.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/_hooks/sdkhooks.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/_hooks/types.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/apiendpoints.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/apiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/apis.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/apis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/auth.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/auth.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/embeds.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/embeds.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/events.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/events.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/metadata.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/metadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/errors/error.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/errors/sdkerror.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/__init__.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/deleteapi.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/deleteapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/deleteapiendpoint.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/deleteapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/deleteschema.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/deleteschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/deleteversionmetadata.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/deleteversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/downloadschema.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/downloadschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/downloadschemarevision.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/downloadschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/findapiendpoint.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/findapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/generateopenapispec.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/generateopenapispec.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/generateopenapispecforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/generatepostmancollection.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/generatepostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/generatepostmancollectionforapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/generaterequestpostmancollection.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/generaterequestpostmancollection.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getaccesstoken.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getallapiendpoints.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getallapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getallapiversions.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getallapiversions.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getallforversionapiendpoints.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getallforversionapiendpoints.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getapiendpoint.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getapis.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getapis.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getembedaccesstoken.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getorganizations.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getorganizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getrequestfromeventlog.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getrequestfromeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getschema.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getschemadiff.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getschemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getschemarevision.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getschemarevision.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getschemas.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getschemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getuser.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getuser.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getvalidembedaccesstokens.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getvalidembedaccesstokens.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getversionmetadata.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getworkspaceaccess.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getworkspaceaccess.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getworkspaceevents.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/getworkspacetargets.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/getworkspacetargets.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/insertversionmetadata.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/insertversionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/postworkspaceevents.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/postworkspaceevents.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/queryeventlog.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/queryeventlog.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/registerschema.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/registerschema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/revokeembedaccesstoken.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/revokeembedaccesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/upsertapi.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/upsertapi.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/upsertapiendpoint.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/upsertapiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/operations/validateapikey.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/operations/validateapikey.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/__init__.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/accessdetails.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/accessdetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/accesstoken.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/accesstoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/api.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/api.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/api_input.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/api_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/apiendpoint.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/apiendpoint.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/apiendpoint_input.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/apiendpoint_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/apikeydetails.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/apikeydetails.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/boundedrequest.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/boundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/clievent.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/clievent.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/embedaccesstokenresponse.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/embedaccesstokenresponse.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/embedtoken.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/embedtoken.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/filter_.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/filter_.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/filters.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/filters.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/generateopenapispecdiff.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/generateopenapispecdiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/organization.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/organization.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/requestmetadata.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/requestmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/schema.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/schema.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/schemadiff.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/schemadiff.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/security.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/security.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/targetsdk.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/targetsdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/unboundedrequest.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/unboundedrequest.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/user.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/user.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/versionmetadata.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/versionmetadata.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/models/shared/versionmetadata_input.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/models/shared/versionmetadata_input.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/organizations.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/organizations.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/requests.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/requests.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/schemas.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/schemas.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/sdk.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/sdk.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/sdkconfiguration.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/sdkconfiguration.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,17 +22,17 @@
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server: Optional[str] = ''
     globals: Dict[str, Dict[str, Dict[str, Any]]] = field(default_factory=Dict)
     language: str = 'python'
     openapi_doc_version: str = '0.4.0'
-    sdk_version: str = '5.6.1'
-    gen_version: str = '2.298.1'
-    user_agent: str = 'speakeasy-sdk/python 5.6.1 2.298.1 0.4.0 speakeasy-client-sdk-python'
+    sdk_version: str = '5.6.2'
+    gen_version: str = '2.298.2'
+    user_agent: str = 'speakeasy-sdk/python 5.6.2 2.298.2 0.4.0 speakeasy-client-sdk-python'
     retry_config: Optional[RetryConfig] = None
     _hooks: Optional[SDKHooks] = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if not self.server:
```

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/utils/retries.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/utils/retries.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy/utils/utils.py` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy/utils/utils.py`

 * *Files identical despite different names*

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy_client_sdk_python.egg-info/PKG-INFO` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy_client_sdk_python.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: speakeasy-client-sdk-python
-Version: 5.6.1
+Version: 5.6.2
 Summary: Speakeasy API Client SDK for Python
 Home-page: https://github.com/speakeasy-api/speakeasy-client-sdk-python.git
 Author: Speakeasy
 License: UNKNOWN
 Description: # speakeasy-client-sdk-python
         
         <!-- Start SDK Installation [installation] -->
@@ -41,79 +41,79 @@
         
         ```
         <!-- End SDK Example Usage [usage] -->
         
         <!-- Start Available Resources and Operations [operations] -->
         ## Available Resources and Operations
         
-        ### [apis](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md)
+        ### [apis](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md)
         
-        * [delete_api](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#delete_api) - Delete an Api.
-        * [generate_open_api_spec](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#generate_open_api_spec) - Generate an OpenAPI specification for a particular Api.
-        * [generate_postman_collection](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#generate_postman_collection) - Generate a Postman collection for a particular Api.
-        * [get_all_api_versions](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#get_all_api_versions) - Get all Api versions for a particular ApiEndpoint.
-        * [get_apis](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#get_apis) - Get a list of Apis for a given workspace
-        * [upsert_api](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apis/README.md#upsert_api) - Upsert an Api
+        * [delete_api](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#delete_api) - Delete an Api.
+        * [generate_open_api_spec](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#generate_open_api_spec) - Generate an OpenAPI specification for a particular Api.
+        * [generate_postman_collection](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#generate_postman_collection) - Generate a Postman collection for a particular Api.
+        * [get_all_api_versions](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#get_all_api_versions) - Get all Api versions for a particular ApiEndpoint.
+        * [get_apis](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#get_apis) - Get a list of Apis for a given workspace
+        * [upsert_api](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apis/README.md#upsert_api) - Upsert an Api
         
-        ### [api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md)
+        ### [api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md)
         
-        * [delete_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#delete_api_endpoint) - Delete an ApiEndpoint.
-        * [find_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#find_api_endpoint) - Find an ApiEndpoint via its displayName.
-        * [generate_open_api_spec_for_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#generate_open_api_spec_for_api_endpoint) - Generate an OpenAPI specification for a particular ApiEndpoint.
-        * [generate_postman_collection_for_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#generate_postman_collection_for_api_endpoint) - Generate a Postman collection for a particular ApiEndpoint.
-        * [get_all_api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#get_all_api_endpoints) - Get all Api endpoints for a particular apiID.
-        * [get_all_for_version_api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#get_all_for_version_api_endpoints) - Get all ApiEndpoints for a particular apiID and versionID.
-        * [get_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#get_api_endpoint) - Get an ApiEndpoint.
-        * [upsert_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/apiendpoints/README.md#upsert_api_endpoint) - Upsert an ApiEndpoint.
+        * [delete_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#delete_api_endpoint) - Delete an ApiEndpoint.
+        * [find_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#find_api_endpoint) - Find an ApiEndpoint via its displayName.
+        * [generate_open_api_spec_for_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#generate_open_api_spec_for_api_endpoint) - Generate an OpenAPI specification for a particular ApiEndpoint.
+        * [generate_postman_collection_for_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#generate_postman_collection_for_api_endpoint) - Generate a Postman collection for a particular ApiEndpoint.
+        * [get_all_api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#get_all_api_endpoints) - Get all Api endpoints for a particular apiID.
+        * [get_all_for_version_api_endpoints](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#get_all_for_version_api_endpoints) - Get all ApiEndpoints for a particular apiID and versionID.
+        * [get_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#get_api_endpoint) - Get an ApiEndpoint.
+        * [upsert_api_endpoint](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/apiendpoints/README.md#upsert_api_endpoint) - Upsert an ApiEndpoint.
         
-        ### [metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/metadata/README.md)
+        ### [metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/metadata/README.md)
         
-        * [delete_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/metadata/README.md#delete_version_metadata) - Delete metadata for a particular apiID and versionID.
-        * [get_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/metadata/README.md#get_version_metadata) - Get all metadata for a particular apiID and versionID.
-        * [insert_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/metadata/README.md#insert_version_metadata) - Insert metadata for a particular apiID and versionID.
+        * [delete_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/metadata/README.md#delete_version_metadata) - Delete metadata for a particular apiID and versionID.
+        * [get_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/metadata/README.md#get_version_metadata) - Get all metadata for a particular apiID and versionID.
+        * [insert_version_metadata](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/metadata/README.md#insert_version_metadata) - Insert metadata for a particular apiID and versionID.
         
-        ### [schemas](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md)
+        ### [schemas](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md)
         
-        * [delete_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#delete_schema) - Delete a particular schema revision for an Api.
-        * [download_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#download_schema) - Download the latest schema for a particular apiID.
-        * [download_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#download_schema_revision) - Download a particular schema revision for an Api.
-        * [get_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#get_schema) - Get information about the latest schema.
-        * [get_schema_diff](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#get_schema_diff) - Get a diff of two schema revisions for an Api.
-        * [get_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#get_schema_revision) - Get information about a particular schema revision for an Api.
-        * [get_schemas](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#get_schemas) - Get information about all schemas associated with a particular apiID.
-        * [register_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/schemas/README.md#register_schema) - Register a schema.
+        * [delete_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#delete_schema) - Delete a particular schema revision for an Api.
+        * [download_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#download_schema) - Download the latest schema for a particular apiID.
+        * [download_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#download_schema_revision) - Download a particular schema revision for an Api.
+        * [get_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema) - Get information about the latest schema.
+        * [get_schema_diff](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema_diff) - Get a diff of two schema revisions for an Api.
+        * [get_schema_revision](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schema_revision) - Get information about a particular schema revision for an Api.
+        * [get_schemas](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#get_schemas) - Get information about all schemas associated with a particular apiID.
+        * [register_schema](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/schemas/README.md#register_schema) - Register a schema.
         
-        ### [auth](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/auth/README.md)
+        ### [auth](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md)
         
-        * [get_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/auth/README.md#get_access_token) - Get or refresh an access token for the current workspace.
-        * [get_user](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/auth/README.md#get_user) - Get information about the current user.
-        * [get_workspace_access](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/auth/README.md#get_workspace_access) - Get access allowances for a particular workspace
-        * [validate_api_key](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/auth/README.md#validate_api_key) - Validate the current api key.
+        * [get_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_access_token) - Get or refresh an access token for the current workspace.
+        * [get_user](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_user) - Get information about the current user.
+        * [get_workspace_access](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#get_workspace_access) - Get access allowances for a particular workspace
+        * [validate_api_key](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/auth/README.md#validate_api_key) - Validate the current api key.
         
-        ### [requests](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/requests/README.md)
+        ### [requests](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md)
         
-        * [generate_request_postman_collection](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/requests/README.md#generate_request_postman_collection) - Generate a Postman collection for a particular request.
-        * [get_request_from_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/requests/README.md#get_request_from_event_log) - Get information about a particular request.
-        * [query_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/requests/README.md#query_event_log) - Query the event log to retrieve a list of requests.
+        * [generate_request_postman_collection](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#generate_request_postman_collection) - Generate a Postman collection for a particular request.
+        * [get_request_from_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#get_request_from_event_log) - Get information about a particular request.
+        * [query_event_log](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/requests/README.md#query_event_log) - Query the event log to retrieve a list of requests.
         
-        ### [organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/organizations/README.md)
+        ### [organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md)
         
-        * [get_organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/organizations/README.md#get_organizations) - Get organizations for a user
+        * [get_organizations](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/organizations/README.md#get_organizations) - Get organizations for a user
         
-        ### [embeds](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/embeds/README.md)
+        ### [embeds](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md)
         
-        * [get_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/embeds/README.md#get_embed_access_token) - Get an embed access token for the current workspace.
-        * [get_valid_embed_access_tokens](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/embeds/README.md#get_valid_embed_access_tokens) - Get all valid embed access tokens for the current workspace.
-        * [revoke_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/embeds/README.md#revoke_embed_access_token) - Revoke an embed access EmbedToken.
+        * [get_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_embed_access_token) - Get an embed access token for the current workspace.
+        * [get_valid_embed_access_tokens](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#get_valid_embed_access_tokens) - Get all valid embed access tokens for the current workspace.
+        * [revoke_embed_access_token](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/embeds/README.md#revoke_embed_access_token) - Revoke an embed access EmbedToken.
         
-        ### [events](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/events/README.md)
+        ### [events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md)
         
-        * [get_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/events/README.md#get_workspace_events) - Load recent events for a particular workspace
-        * [get_workspace_targets](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/events/README.md#get_workspace_targets) - Load targets for a particular workspace
-        * [post_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python.git/blob/master/docs/sdks/events/README.md#post_workspace_events) - Post events for a specific workspace
+        * [get_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#get_workspace_events) - Load recent events for a particular workspace
+        * [get_workspace_targets](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#get_workspace_targets) - Load targets for a particular workspace
+        * [post_workspace_events](https://github.com/speakeasy-api/speakeasy-client-sdk-python/blob/master/docs/sdks/events/README.md#post_workspace_events) - Post events for a specific workspace
         <!-- End Available Resources and Operations [operations] -->
```

### Comparing `speakeasy-client-sdk-python-5.6.1/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt` & `speakeasy-client-sdk-python-5.6.2/src/speakeasy_client_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

