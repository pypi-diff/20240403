# Comparing `tmp/Leonardo-Ai-SDK-5.2.6.tar.gz` & `tmp/Leonardo-Ai-SDK-5.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-5.2.6.tar", last modified: Wed Mar 27 22:57:04 2024, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-5.3.0.tar", last modified: Wed Apr  3 00:02:52 2024, max compression
```

## Comparing `Leonardo-Ai-SDK-5.2.6.tar` & `Leonardo-Ai-SDK-5.3.0.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:57:04.903673 Leonardo-Ai-SDK-5.2.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-03-27 22:57:04.903673 Leonardo-Ai-SDK-5.2.6/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     9598 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 22:57:04.903673 Leonardo-Ai-SDK-5.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:57:04.891673 Leonardo-Ai-SDK-5.2.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:57:04.895673 Leonardo-Ai-SDK-5.2.6/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12043 2024-03-27 22:57:04.000000 Leonardo-Ai-SDK-5.2.6/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-03-27 22:57:04.000000 Leonardo-Ai-SDK-5.2.6/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 22:57:04.000000 Leonardo-Ai-SDK-5.2.6/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-03-27 22:57:04.000000 Leonardo-Ai-SDK-5.2.6/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-27 22:57:04.000000 Leonardo-Ai-SDK-5.2.6/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:57:04.895673 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:57:04.895673 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    16886 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    43766 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     9719 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/initimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    26418 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:57:04.895673 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:57:04.895673 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:57:04.903673 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/creategeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createlcmgeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createtexturegeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createvariationnobg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createvariationunzoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createvariationupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/get3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getuserself.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getvariationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/listelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/listplatformmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/performinpaintinglcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/performinstantrefine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/uploadinitimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/uploadmodelasset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:57:04.903673 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/controlnet_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/custom_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/lcm_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/model_asset_texture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/sd_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/sd_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/strength.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/variation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1281 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3413 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 22:57:04.903673 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3778 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30022 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13304 2024-03-27 22:56:56.000000 Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:52.481411 Leonardo-Ai-SDK-5.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-04-03 00:02:52.481411 Leonardo-Ai-SDK-5.3.0/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9597 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 00:02:52.481411 Leonardo-Ai-SDK-5.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:52.469411 Leonardo-Ai-SDK-5.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:52.473410 Leonardo-Ai-SDK-5.3.0/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12098 2024-04-03 00:02:52.000000 Leonardo-Ai-SDK-5.3.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-03 00:02:52.000000 Leonardo-Ai-SDK-5.3.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 00:02:52.000000 Leonardo-Ai-SDK-5.3.0/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-03 00:02:52.000000 Leonardo-Ai-SDK-5.3.0/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-03 00:02:52.000000 Leonardo-Ai-SDK-5.3.0/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:52.473410 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:52.473410 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17468 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45180 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10093 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/initimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27312 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:52.473410 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:52.473410 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:52.481411 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14776 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/creategeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4960 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createlcmgeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4497 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createtexturegeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createvariationnobg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createvariationunzoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/get3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14832 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getuserself.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/listelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/listplatformmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6200 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5351 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/performinpaintinglcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5038 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/performinstantrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/uploadinitimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/uploadmodelasset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:52.481411 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/controlnet_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/custom_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/lcm_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/model_asset_texture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/sd_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/strength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/variation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 00:02:52.481411 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30022 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13782 2024-04-03 00:02:42.000000 Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-5.2.6/LICENSE.md` & `Leonardo-Ai-SDK-5.3.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/PKG-INFO` & `Leonardo-Ai-SDK-5.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.2.6
+Version: 5.3.0
 Summary: Leonardo AI Python Client SDK
-Home-page: UNKNOWN
+Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
         
         <!-- Start SDK Installation [installation] -->
@@ -112,15 +112,15 @@
         <!-- Start Error Handling [errors] -->
         ## Error Handling
         
         Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
         
         | Error Object    | Status Code     | Content Type    |
         | --------------- | --------------- | --------------- |
-        | errors.SDKError | 4x-5xx          | */*             |
+        | errors.SDKError | 4xx-5xx         | */*             |
         
         ### Example
         
         ```python
         import leonardoaisdk
         from leonardoaisdk.models import errors, operations
         
@@ -156,15 +156,15 @@
         For example, you could specify a header for every request that this sdk makes as follows:
         ```python
         import leonardoaisdk
         import requests
         
         http_client = requests.Session()
         http_client.headers.update({'x-custom-header': 'someValue'})
-        s = leonardoaisdk.LeonardoAiSDK(client: http_client)
+        s = leonardoaisdk.LeonardoAiSDK(client=http_client)
         ```
         <!-- End Custom HTTP Client [http-client] -->
         
         
         
         <!-- Start Server Selection [server] -->
         ## Server Selection
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.2.6 Summary: Leonardo AI
-Python Client SDK Home-page: UNKNOWN Author: Leonardo-Ai License: UNKNOWN
-Description: # Leonardo-Ai-SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK
-Installation ```bash pip install Leonardo-Ai-SDK ``` ## SDK Example Usage ###
-Example ```python import leonardoaisdk from leonardoaisdk.models import
-operations s = leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.0 Summary: Leonardo AI
+Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
+python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
+SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
+install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
+leonardoaisdk from leonardoaisdk.models import operations s =
+leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
 (req) if res.object is not None: # handle response pass ``` ## Available
 Resources and Operations ### [dataset](docs/sdks/dataset/README.md) *
 [create_dataset](docs/sdks/dataset/README.md#create_dataset) - Create a Dataset
 * [delete_dataset_by_id](docs/sdks/dataset/README.md#delete_dataset_by_id) -
 Delete a Single Dataset by ID * [get_dataset_by_id](docs/sdks/dataset/
 README.md#get_dataset_by_id) - Get a Single Dataset by ID *
@@ -63,29 +64,29 @@
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (docs/sdks/variation/README.md#create_variation_upscale) - Create upscale *
 [get_variation_by_id](docs/sdks/variation/README.md#get_variation_by_id) - Get
 variation by ID ## Error Handling Handling errors in this SDK should largely
 match your expectations. All operations return a response object or raise an
 error. If Error objects are specified in your OpenAPI Spec, the SDK will raise
 the appropriate Error type. | Error Object | Status Code | Content Type | | ---
------------- | --------------- | --------------- | | errors.SDKError | 4x-5xx |
-*/* | ### Example ```python import leonardoaisdk from leonardoaisdk.models
+------------ | --------------- | --------------- | | errors.SDKError | 4xx-5xx
+| */* | ### Example ```python import leonardoaisdk from leonardoaisdk.models
 import errors, operations s = leonardoaisdk.LeonardoAiSDK( bearer_auth="", )
 req = operations.CreateDatasetRequestBody( name='', ) res = None try: res =
 s.dataset.create_dataset(req) except errors.SDKError as e: # handle exception
 raise(e) if res.object is not None: # handle response pass ``` ## Custom HTTP
 Client The Python SDK makes API calls using the [requests](https://pypi.org/
 project/requests/) HTTP library. In order to provide a convenient way to
 configure timeouts, cookies, proxies, custom headers, and other low-level
 configuration, you can initialize the SDK client with a custom
 `requests.Session` object. For example, you could specify a header for every
 request that this sdk makes as follows: ```python import leonardoaisdk import
 requests http_client = requests.Session() http_client.headers.update({'x-
-custom-header': 'someValue'}) s = leonardoaisdk.LeonardoAiSDK(client:
-http_client) ``` ## Server Selection ### Select Server by Index You can
+custom-header': 'someValue'}) s = leonardoaisdk.LeonardoAiSDK
+(client=http_client) ``` ## Server Selection ### Select Server by Index You can
 override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
 The selected server will then be used as the default on the operations that use
 it. This table lists the indexes associated with the available servers: | # |
 Server | Variables | | - | ------ | --------- | | 0 | `https://
 cloud.leonardo.ai/api/rest/v1` | None | #### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
```

### Comparing `Leonardo-Ai-SDK-5.2.6/README.md` & `Leonardo-Ai-SDK-5.3.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
 <!-- Start Error Handling [errors] -->
 ## Error Handling
 
 Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
 
 | Error Object    | Status Code     | Content Type    |
 | --------------- | --------------- | --------------- |
-| errors.SDKError | 4x-5xx          | */*             |
+| errors.SDKError | 4xx-5xx         | */*             |
 
 ### Example
 
 ```python
 import leonardoaisdk
 from leonardoaisdk.models import errors, operations
 
@@ -149,15 +149,15 @@
 For example, you could specify a header for every request that this sdk makes as follows:
 ```python
 import leonardoaisdk
 import requests
 
 http_client = requests.Session()
 http_client.headers.update({'x-custom-header': 'someValue'})
-s = leonardoaisdk.LeonardoAiSDK(client: http_client)
+s = leonardoaisdk.LeonardoAiSDK(client=http_client)
 ```
 <!-- End Custom HTTP Client [http-client] -->
 
 
 
 <!-- Start Server Selection [server] -->
 ## Server Selection
```

#### html2text {}

```diff
@@ -61,29 +61,29 @@
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (docs/sdks/variation/README.md#create_variation_upscale) - Create upscale *
 [get_variation_by_id](docs/sdks/variation/README.md#get_variation_by_id) - Get
 variation by ID ## Error Handling Handling errors in this SDK should largely
 match your expectations. All operations return a response object or raise an
 error. If Error objects are specified in your OpenAPI Spec, the SDK will raise
 the appropriate Error type. | Error Object | Status Code | Content Type | | ---
------------- | --------------- | --------------- | | errors.SDKError | 4x-5xx |
-*/* | ### Example ```python import leonardoaisdk from leonardoaisdk.models
+------------ | --------------- | --------------- | | errors.SDKError | 4xx-5xx
+| */* | ### Example ```python import leonardoaisdk from leonardoaisdk.models
 import errors, operations s = leonardoaisdk.LeonardoAiSDK( bearer_auth="", )
 req = operations.CreateDatasetRequestBody( name='', ) res = None try: res =
 s.dataset.create_dataset(req) except errors.SDKError as e: # handle exception
 raise(e) if res.object is not None: # handle response pass ``` ## Custom HTTP
 Client The Python SDK makes API calls using the [requests](https://pypi.org/
 project/requests/) HTTP library. In order to provide a convenient way to
 configure timeouts, cookies, proxies, custom headers, and other low-level
 configuration, you can initialize the SDK client with a custom
 `requests.Session` object. For example, you could specify a header for every
 request that this sdk makes as follows: ```python import leonardoaisdk import
 requests http_client = requests.Session() http_client.headers.update({'x-
-custom-header': 'someValue'}) s = leonardoaisdk.LeonardoAiSDK(client:
-http_client) ``` ## Server Selection ### Select Server by Index You can
+custom-header': 'someValue'}) s = leonardoaisdk.LeonardoAiSDK
+(client=http_client) ``` ## Server Selection ### Select Server by Index You can
 override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
 The selected server will then be used as the default on the operations that use
 it. This table lists the indexes associated with the available servers: | # |
 Server | Variables | | - | ------ | --------- | | 0 | `https://
 cloud.leonardo.ai/api/rest/v1` | None | #### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
```

### Comparing `Leonardo-Ai-SDK-5.2.6/setup.py` & `Leonardo-Ai-SDK-5.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,17 +6,18 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="Leonardo-Ai-SDK",
-    version="5.2.6",
+    version="5.3.0",
     author="Leonardo-Ai",
     description="Leonardo AI Python Client SDK",
+    url="https://github.com/Leonardo-Interactive/leonardo-python-sdk.git",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(where="src"),
     install_requires=[
         "certifi>=2023.7.22",
         "charset-normalizer>=3.2.0",
         "dataclasses-json>=0.6.4",
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-5.3.0/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.2.6
+Version: 5.3.0
 Summary: Leonardo AI Python Client SDK
-Home-page: UNKNOWN
+Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
         
         <!-- Start SDK Installation [installation] -->
@@ -112,15 +112,15 @@
         <!-- Start Error Handling [errors] -->
         ## Error Handling
         
         Handling errors in this SDK should largely match your expectations.  All operations return a response object or raise an error.  If Error objects are specified in your OpenAPI Spec, the SDK will raise the appropriate Error type.
         
         | Error Object    | Status Code     | Content Type    |
         | --------------- | --------------- | --------------- |
-        | errors.SDKError | 4x-5xx          | */*             |
+        | errors.SDKError | 4xx-5xx         | */*             |
         
         ### Example
         
         ```python
         import leonardoaisdk
         from leonardoaisdk.models import errors, operations
         
@@ -156,15 +156,15 @@
         For example, you could specify a header for every request that this sdk makes as follows:
         ```python
         import leonardoaisdk
         import requests
         
         http_client = requests.Session()
         http_client.headers.update({'x-custom-header': 'someValue'})
-        s = leonardoaisdk.LeonardoAiSDK(client: http_client)
+        s = leonardoaisdk.LeonardoAiSDK(client=http_client)
         ```
         <!-- End Custom HTTP Client [http-client] -->
         
         
         
         <!-- Start Server Selection [server] -->
         ## Server Selection
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.2.6 Summary: Leonardo AI
-Python Client SDK Home-page: UNKNOWN Author: Leonardo-Ai License: UNKNOWN
-Description: # Leonardo-Ai-SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK
-Installation ```bash pip install Leonardo-Ai-SDK ``` ## SDK Example Usage ###
-Example ```python import leonardoaisdk from leonardoaisdk.models import
-operations s = leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.0 Summary: Leonardo AI
+Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
+python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
+SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
+install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
+leonardoaisdk from leonardoaisdk.models import operations s =
+leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
 (req) if res.object is not None: # handle response pass ``` ## Available
 Resources and Operations ### [dataset](docs/sdks/dataset/README.md) *
 [create_dataset](docs/sdks/dataset/README.md#create_dataset) - Create a Dataset
 * [delete_dataset_by_id](docs/sdks/dataset/README.md#delete_dataset_by_id) -
 Delete a Single Dataset by ID * [get_dataset_by_id](docs/sdks/dataset/
 README.md#get_dataset_by_id) - Get a Single Dataset by ID *
@@ -63,29 +64,29 @@
 README.md#create_variation_unzoom) - Create unzoom * [create_variation_upscale]
 (docs/sdks/variation/README.md#create_variation_upscale) - Create upscale *
 [get_variation_by_id](docs/sdks/variation/README.md#get_variation_by_id) - Get
 variation by ID ## Error Handling Handling errors in this SDK should largely
 match your expectations. All operations return a response object or raise an
 error. If Error objects are specified in your OpenAPI Spec, the SDK will raise
 the appropriate Error type. | Error Object | Status Code | Content Type | | ---
------------- | --------------- | --------------- | | errors.SDKError | 4x-5xx |
-*/* | ### Example ```python import leonardoaisdk from leonardoaisdk.models
+------------ | --------------- | --------------- | | errors.SDKError | 4xx-5xx
+| */* | ### Example ```python import leonardoaisdk from leonardoaisdk.models
 import errors, operations s = leonardoaisdk.LeonardoAiSDK( bearer_auth="", )
 req = operations.CreateDatasetRequestBody( name='', ) res = None try: res =
 s.dataset.create_dataset(req) except errors.SDKError as e: # handle exception
 raise(e) if res.object is not None: # handle response pass ``` ## Custom HTTP
 Client The Python SDK makes API calls using the [requests](https://pypi.org/
 project/requests/) HTTP library. In order to provide a convenient way to
 configure timeouts, cookies, proxies, custom headers, and other low-level
 configuration, you can initialize the SDK client with a custom
 `requests.Session` object. For example, you could specify a header for every
 request that this sdk makes as follows: ```python import leonardoaisdk import
 requests http_client = requests.Session() http_client.headers.update({'x-
-custom-header': 'someValue'}) s = leonardoaisdk.LeonardoAiSDK(client:
-http_client) ``` ## Server Selection ### Select Server by Index You can
+custom-header': 'someValue'}) s = leonardoaisdk.LeonardoAiSDK
+(client=http_client) ``` ## Server Selection ### Select Server by Index You can
 override the default server globally by passing a server index to the
 `server_idx: int` optional parameter when initializing the SDK client instance.
 The selected server will then be used as the default on the operations that use
 it. This table lists the indexes associated with the available servers: | # |
 Server | Variables | | - | ------ | --------- | | 0 | `https://
 cloud.leonardo.ai/api/rest/v1` | None | #### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-5.3.0/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/_hooks/sdkhooks.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/_hooks/sdkhooks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests
 from .types import SDKInitHook, BeforeRequestContext, BeforeRequestHook, AfterSuccessContext, AfterSuccessHook, AfterErrorContext, AfterErrorHook, Hooks
-from typing import List, Optional, Tuple, Union
+from typing import List, Optional, Tuple
 
 
 class SDKHooks(Hooks):
     def __init__(self):
         self.sdk_init_hooks: List[SDKInitHook] = []
         self.before_request_hooks: List[BeforeRequestHook] = []
         self.after_success_hooks: List[AfterSuccessHook] = []
@@ -25,27 +25,29 @@
         self.after_error_hooks.append(hook)
 
     def sdk_init(self, base_url: str, client: requests.Session) -> Tuple[str, requests.Session]:
         for hook in self.sdk_init_hooks:
             base_url, client = hook.sdk_init(base_url, client)
         return base_url, client
 
-    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> Union[requests.PreparedRequest, Exception]:
+    def before_request(self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest) -> requests.PreparedRequest:
         for hook in self.before_request_hooks:
-            request = hook.before_request(hook_ctx, request)
-            if isinstance(request, Exception):
-                raise request
+            out = hook.before_request(hook_ctx, request)
+            if isinstance(out, Exception):
+                raise out
+            request = out
 
         return request
 
     def after_success(self, hook_ctx: AfterSuccessContext, response: requests.Response) -> requests.Response:
         for hook in self.after_success_hooks:
-            response = hook.after_success(hook_ctx, response)
-            if isinstance(response, Exception):
-                raise response
+            out = hook.after_success(hook_ctx, response)
+            if isinstance(out, Exception):
+                raise out
+            response = out
         return response
 
     def after_error(self, hook_ctx: AfterErrorContext, response: Optional[requests.Response], error: Optional[Exception]) -> Tuple[Optional[requests.Response], Optional[Exception]]:
         for hook in self.after_error_hooks:
             result = hook.after_error(hook_ctx, response, error)
             if isinstance(result, Exception):
                 raise result
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/_hooks/types.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/_hooks/types.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,23 +13,27 @@
     def __init__(self, operation_id: str, oauth2_scopes: Optional[List[str]], security_source: Optional[Union[Any, Callable[[], Any]]]):
         self.operation_id = operation_id
         self.oauth2_scopes = oauth2_scopes
         self.security_source = security_source
 
 
 class BeforeRequestContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class AfterSuccessContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
+    
 
 
 class AfterErrorContext(HookContext):
-    pass
+    def __init__(self, hook_ctx: HookContext):
+        super().__init__(hook_ctx.operation_id, hook_ctx.oauth2_scopes, hook_ctx.security_source)
 
 
 class SDKInitHook(ABC):
     @abstractmethod
     def sdk_init(self, base_url: str, client: requests_http.Session) -> Tuple[str, requests_http.Session]:
         pass
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/dataset.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk._hooks import HookContext
+from leonardoaisdk._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class Dataset:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -35,38 +35,37 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreateDatasetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateDatasetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateDatasetResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -96,38 +95,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.DeleteDatasetByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.DeleteDatasetByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteDatasetByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -157,38 +155,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetDatasetByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetDatasetByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetDatasetByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -224,38 +221,37 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.UploadDatasetImageResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UploadDatasetImageResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UploadDatasetImageResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -291,38 +287,37 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.UploadDatasetImageFromGenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UploadDatasetImageFromGenResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UploadDatasetImageFromGenResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/element.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/element.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk._hooks import HookContext
+from leonardoaisdk._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class Element:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -30,38 +30,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.ListElementsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ListElementsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.ListElementsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/generation.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/generation.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk._hooks import HookContext
+from leonardoaisdk._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class Generation:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -35,38 +35,37 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreateGenerationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateGenerationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateGenerationResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -95,38 +94,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreateLCMGenerationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateLCMGenerationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateLCMGenerationResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -155,38 +153,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreateSVDMotionGenerationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateSVDMotionGenerationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateSVDMotionGenerationResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -215,38 +212,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreateTextureGenerationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateTextureGenerationResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateTextureGenerationResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -276,38 +272,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.DeleteGenerationByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.DeleteGenerationByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteGenerationByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -341,38 +336,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.DeleteTextureGenerationByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.DeleteTextureGenerationByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteTextureGenerationByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -402,38 +396,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetGenerationByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetGenerationByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetGenerationByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -466,38 +459,37 @@
         
         query_params = { **utils.get_query_params(operations.GetGenerationsByUserIDRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetGenerationsByUserIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetGenerationsByUserIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetGenerationsByUserIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -534,38 +526,37 @@
             headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(operations.GetTextureGenerationByIDRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetTextureGenerationByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetTextureGenerationByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetTextureGenerationByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -602,38 +593,37 @@
             headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(operations.GetTextureGenerationsByModelIDRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetTextureGenerationsByModelIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetTextureGenerationsByModelIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetTextureGenerationsByModelIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -662,38 +652,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.PerformAlchemyUpscaleLCMResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.PerformAlchemyUpscaleLCMResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PerformAlchemyUpscaleLCMResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -722,38 +711,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.PerformInpaintingLCMResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.PerformInpaintingLCMResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PerformInpaintingLCMResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -782,38 +770,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.PerformInstantRefineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.PerformInstantRefineResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.PerformInstantRefineResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/initimage.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk._hooks import HookContext
+from leonardoaisdk._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class InitImage:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -34,38 +34,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.DeleteInitImageByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.DeleteInitImageByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteInitImageByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -95,38 +94,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetInitImageByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetInitImageByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetInitImageByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -157,38 +155,37 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.UploadInitImageResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UploadInitImageResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UploadInitImageResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk._hooks import HookContext
+from leonardoaisdk._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class Model:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -35,38 +35,37 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreateModelResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateModelResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateModelResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -100,38 +99,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.Delete3DModelByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.Delete3DModelByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.Delete3DModelByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -161,38 +159,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('DELETE', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.DeleteModelByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.DeleteModelByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.DeleteModelByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -229,38 +226,37 @@
             headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(operations.Get3DModelByIDRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.Get3DModelByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.Get3DModelByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.Get3DModelByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -297,38 +293,37 @@
             headers['content-type'] = req_content_type
         query_params = { **utils.get_query_params(operations.Get3DModelsByUserIDRequest, request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.Get3DModelsByUserIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.Get3DModelsByUserIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.Get3DModelsByUserIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -358,38 +353,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetModelByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetModelByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetModelByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -415,38 +409,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.ListPlatformModelsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.ListPlatformModelsResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.ListPlatformModelsResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -475,38 +468,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.UploadModelAssetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.UploadModelAssetResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.UploadModelAssetResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/errors/sdkerror.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createlcmgeneration.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createlcmgeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createtexturegeneration.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createtexturegeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createvariationnobg.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createvariationnobg.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createvariationunzoom.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createvariationunzoom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/delete3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/delete3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/get3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/get3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/listelements.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/listelements.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/listplatformmodels.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/listplatformmodels.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/performinpaintinglcm.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/performinpaintinglcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/performinstantrefine.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/performinstantrefine.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/operations/uploadmodelasset.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/operations/uploadmodelasset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/__init__.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/element_input.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/element_input.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/lcm_generation_style.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/lcm_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/models/shared/sd_generation_style.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/models/shared/sd_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/sdk.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .dataset import Dataset
 from .element import Element
 from .generation import Generation
 from .initimage import InitImage
 from .model import Model
 from .sdkconfiguration import SDKConfiguration
 from .user import User
+from .utils.retries import RetryConfig
 from .variation import Variation
 from leonardoaisdk import utils
 from leonardoaisdk._hooks import SDKHooks
 from leonardoaisdk.models import shared
 from typing import Callable, Dict, Optional, Union
 
 class LeonardoAiSDK:
@@ -28,30 +29,30 @@
 
     def __init__(self,
                  bearer_auth: Union[str, Callable[[], str]],
                  server_idx: Optional[int] = None,
                  server_url: Optional[str] = None,
                  url_params: Optional[Dict[str, str]] = None,
                  client: Optional[requests_http.Session] = None,
-                 retry_config: Optional[utils.RetryConfig] = None
+                 retry_config: Optional[RetryConfig] = None
                  ) -> None:
         """Instantiates the SDK configuring it with the provided parameters.
 
         :param bearer_auth: The bearer_auth required for authentication
         :type bearer_auth: Union[str, Callable[[], str]]
         :param server_idx: The index of the server to use for all operations
         :type server_idx: int
         :param server_url: The server URL to use for all operations
         :type server_url: str
         :param url_params: Parameters to optionally template the server URL with
         :type url_params: Dict[str, str]
         :param client: The requests.Session HTTP client to use for all operations
         :type client: requests_http.Session
         :param retry_config: The utils.RetryConfig to use globally
-        :type retry_config: utils.RetryConfig
+        :type retry_config: RetryConfig
         """
         if client is None:
             client = requests_http.Session()
 
         if callable(bearer_auth):
             def security():
                 return shared.Security(bearer_auth = bearer_auth())
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,39 +3,39 @@
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
 from dataclasses import dataclass
 from leonardoaisdk.models import shared
-from typing import Callable, Dict, Tuple, Union
+from typing import Callable, Dict, Optional, Tuple, Union
 
 
 SERVERS = [
     'https://cloud.leonardo.ai/api/rest/v1',
     # Leonardo.Ai API server
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
-    server_url: str = ''
-    server_idx: int = 0
+    server_url: Optional[str] = ''
+    server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '5.2.6'
-    gen_version: str = '2.292.0'
-    user_agent: str = 'speakeasy-sdk/python 5.2.6 2.292.0 v1.0.0 Leonardo-Ai-SDK'
-    retry_config: RetryConfig = None
-    _hooks: SDKHooks = None
+    sdk_version: str = '5.3.0'
+    gen_version: str = '2.298.0'
+    user_agent: str = 'speakeasy-sdk/python 5.3.0 2.298.0 v1.0.0 Leonardo-Ai-SDK'
+    retry_config: Optional[RetryConfig] = None
+    _hooks: Optional[SDKHooks] = None
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
-        if self.server_url:
+        if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
 
         return SERVERS[self.server_idx], {}
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/user.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk._hooks import HookContext
+from leonardoaisdk._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class User:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -30,38 +30,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetUserSelfResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetUserSelfResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetUserSelfResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/utils/retries.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,20 +71,20 @@
                             raise TemporaryError(res)
                     else:
                         parsed_code = int(code)
 
                         if res.status_code == parsed_code:
                             raise TemporaryError(res)
             except requests.exceptions.ConnectionError as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except requests.exceptions.Timeout as exception:
-                if retries.config.config.retry_connection_errors:
+                if retries.config.retry_connection_errors:
                     raise
 
                 raise PermanentError(exception) from exception
             except TemporaryError:
                 raise
             except Exception as exception:
                 raise PermanentError(exception) from exception
```

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.2.6/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-5.3.0/src/leonardoaisdk/variation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from leonardoaisdk import utils
-from leonardoaisdk._hooks import HookContext
+from leonardoaisdk._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from leonardoaisdk.models import errors, operations
 from typing import Optional
 
 class Variation:
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
@@ -35,38 +35,37 @@
         if data is None and form is None:
             raise Exception('request body is required')
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreateVariationNoBGResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateVariationNoBGResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateVariationNoBGResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -95,38 +94,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreateVariationUnzoomResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateVariationUnzoomResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateVariationUnzoomResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -155,38 +153,37 @@
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.CreateVariationUpscaleResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.CreateVariationUpscaleResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.CreateVariationUpscaleResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
@@ -216,38 +213,37 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = self.sdk_configuration.get_hooks().before_request(
-                hook_ctx, 
-                requests_http.Request('GET', url, params=query_params, headers=headers).prepare(),
-            )
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, None, e)
-            raise e
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
 
         if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            http_res, e = self.sdk_configuration.get_hooks().after_error(hook_ctx, http_res, None)
-            if e:
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
                 raise e
+            if result is not None:
+                http_res = result
         else:
-            result = self.sdk_configuration.get_hooks().after_success(hook_ctx, http_res)
-            if isinstance(result, Exception):
-                raise result
-            http_res = result
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
         
         
-        res = operations.GetVariationByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type'), raw_response=http_res)
+        res = operations.GetVariationByIDResponse(status_code=http_res.status_code, content_type=http_res.headers.get('Content-Type') or '', raw_response=http_res)
         
         if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type'), 'application/json'):                
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
                 out = utils.unmarshal_json(http_res.text, Optional[operations.GetVariationByIDResponseBody])
                 res.object = out
             else:
                 content_type = http_res.headers.get('Content-Type')
                 raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
```

