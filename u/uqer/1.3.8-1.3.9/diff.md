# Comparing `tmp/uqer-1.3.8.tar.gz` & `tmp/uqer-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/uqer-1.3.8.tar", last modified: Wed Dec 25 04:26:50 2019, max compression
+gzip compressed data, was "dist/uqer-1.3.9.tar", last modified: Mon Mar 30 07:32:20 2020, max compression
```

## Comparing `uqer-1.3.8.tar` & `uqer-1.3.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-25 04:26:50.000000 uqer-1.3.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-25 04:26:50.000000 uqer-1.3.8/docs/
--rw-rw-r--   0 root         (0) root         (0)        0 2019-12-09 08:15:16.000000 uqer-1.3.8/docs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-25 04:26:50.000000 uqer-1.3.8/uqer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-25 04:26:50.000000 uqer-1.3.8/uqer/DataAPI/
--rw-rw-r--   0 root         (0) root         (0)  1489511 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/ACMR.py
--rw-rw-r--   0 root         (0) root         (0)   561807 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/CCXE.py
--rw-rw-r--   0 root         (0) root         (0)    15486 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/CHINABOND.py
--rw-rw-r--   0 root         (0) root         (0)      359 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/CSI.py
--rw-rw-r--   0 root         (0) root         (0)  6219510 2019-12-23 01:18:54.000000 uqer-1.3.8/uqer/DataAPI/DATAYES.py
--rw-rw-r--   0 root         (0) root         (0)    12199 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/DYZH.py
--rw-rw-r--   0 root         (0) root         (0)    14797 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/DataCube.py
--rw-rw-r--   0 root         (0) root         (0)      371 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/FDC.py
--rw-rw-r--   0 root         (0) root         (0)    19990 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/FH.py
--rw-rw-r--   0 root         (0) root         (0)    95350 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/GG.py
--rw-rw-r--   0 root         (0) root         (0)      359 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/IT.py
--rw-rw-r--   0 root         (0) root         (0)    31679 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/IVOLATILITY.py
--rw-rw-r--   0 root         (0) root         (0)      356 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/JDW.py
--rw-rw-r--   0 root         (0) root         (0)   482353 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/JL.py
--rw-rw-r--   0 root         (0) root         (0)  1309902 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/JY.py
--rw-rw-r--   0 root         (0) root         (0)      359 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/JYDB.py
--rw-rw-r--   0 root         (0) root         (0)    20015 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/NH.py
--rw-rw-r--   0 root         (0) root         (0)     6212 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/OTHER.py
--rw-rw-r--   0 root         (0) root         (0)      359 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/QAI.py
--rw-rw-r--   0 root         (0) root         (0)      365 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/QGW.py
--rw-rw-r--   0 root         (0) root         (0)     4267 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/SILKRIVER.py
--rw-rw-r--   0 root         (0) root         (0)     4275 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/SW.py
--rw-rw-r--   0 root         (0) root         (0)   150770 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/TEJ.py
--rw-rw-r--   0 root         (0) root         (0)      929 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     9018 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/api_base.py
--rw-rw-r--   0 root         (0) root         (0)      484 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/DataAPI/settings.py
--rw-rw-r--   0 root         (0) root         (0)     1199 2019-12-25 11:25:10.000000 uqer-1.3.8/uqer/DataAPI/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-25 04:26:50.000000 uqer-1.3.8/uqer/mfclient/
--rw-rw-r--   0 root         (0) root         (0)      143 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/mfclient/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     7507 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/mfclient/portfolio_construct.py
--rw-rw-r--   0 root         (0) root         (0)     8285 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/mfclient/signal_process.py
--rw-rw-r--   0 root         (0) root         (0)     4708 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/mfclient/signal_process_check.py
--rw-rw-r--   0 root         (0) root         (0)      691 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     4869 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/authorize.py
--rw-rw-r--   0 root         (0) root         (0)     3489 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/config.py
--rw-rw-r--   0 root         (0) root         (0)     8284 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/data.py
--rw-rw-r--   0 root         (0) root         (0)     3876 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/factor.py
--rw-rw-r--   0 root         (0) root         (0)     4838 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/notebook.py
--rw-rw-r--   0 root         (0) root         (0)     1484 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/trading.py
--rw-rw-r--   0 root         (0) root         (0)     1345 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/uqer.py
--rw-rw-r--   0 root         (0) root         (0)    14019 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/user_factor.py
--rw-rw-r--   0 root         (0) root         (0)      452 2019-12-09 08:15:16.000000 uqer-1.3.8/uqer/utils.py
--rw-rw-r--   0 root         (0) root         (0)       23 2019-12-25 11:25:10.000000 uqer-1.3.8/uqer/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2019-12-25 04:26:50.000000 uqer-1.3.8/uqer.egg-info/
--rw-rw-r--   0 root         (0) root         (0)      220 2019-12-25 04:26:50.000000 uqer-1.3.8/uqer.egg-info/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1063 2019-12-25 04:26:50.000000 uqer-1.3.8/uqer.egg-info/SOURCES.txt
--rw-rw-r--   0 root         (0) root         (0)        1 2019-12-25 04:26:50.000000 uqer-1.3.8/uqer.egg-info/dependency_links.txt
--rw-rw-r--   0 root         (0) root         (0)       10 2019-12-25 04:26:50.000000 uqer-1.3.8/uqer.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       22 2019-12-09 08:15:16.000000 uqer-1.3.8/MANIFEST.in
--rw-rw-r--   0 root         (0) root         (0)        0 2019-12-09 08:15:16.000000 uqer-1.3.8/README.md
--rw-rw-r--   0 root         (0) root         (0)      826 2019-12-09 08:15:16.000000 uqer-1.3.8/setup.py
--rw-r--r--   0 root         (0) root         (0)      220 2019-12-25 04:26:50.000000 uqer-1.3.8/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      100 2019-12-25 04:26:50.000000 uqer-1.3.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-30 07:32:20.000000 uqer-1.3.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-30 07:32:20.000000 uqer-1.3.9/docs/
+-rw-rw-r--   0 root         (0) root         (0)        0 2020-03-30 07:09:26.000000 uqer-1.3.9/docs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-30 07:32:20.000000 uqer-1.3.9/uqer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-30 07:32:20.000000 uqer-1.3.9/uqer/DataAPI/
+-rw-rw-r--   0 root         (0) root         (0)  1489511 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/ACMR.py
+-rw-rw-r--   0 root         (0) root         (0)   561807 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/CCXE.py
+-rw-rw-r--   0 root         (0) root         (0)    15486 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/CHINABOND.py
+-rw-rw-r--   0 root         (0) root         (0)      359 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/CSI.py
+-rw-rw-r--   0 root         (0) root         (0)  6224271 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/DATAYES.py
+-rw-rw-r--   0 root         (0) root         (0)    12199 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/DYZH.py
+-rw-rw-r--   0 root         (0) root         (0)    14797 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/DataCube.py
+-rw-rw-r--   0 root         (0) root         (0)      371 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/FDC.py
+-rw-rw-r--   0 root         (0) root         (0)    19990 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/FH.py
+-rw-rw-r--   0 root         (0) root         (0)    95350 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/GG.py
+-rw-rw-r--   0 root         (0) root         (0)      359 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/IT.py
+-rw-rw-r--   0 root         (0) root         (0)    31679 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/IVOLATILITY.py
+-rw-rw-r--   0 root         (0) root         (0)      356 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/JDW.py
+-rw-rw-r--   0 root         (0) root         (0)   482353 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/JL.py
+-rw-rw-r--   0 root         (0) root         (0)  1309902 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/JY.py
+-rw-rw-r--   0 root         (0) root         (0)      359 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/JYDB.py
+-rw-rw-r--   0 root         (0) root         (0)    20015 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/NH.py
+-rw-rw-r--   0 root         (0) root         (0)     6212 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/OTHER.py
+-rw-rw-r--   0 root         (0) root         (0)      359 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/QAI.py
+-rw-rw-r--   0 root         (0) root         (0)      365 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/QGW.py
+-rw-rw-r--   0 root         (0) root         (0)     4267 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/SILKRIVER.py
+-rw-rw-r--   0 root         (0) root         (0)     4275 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/SW.py
+-rw-rw-r--   0 root         (0) root         (0)   150770 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/TEJ.py
+-rw-rw-r--   0 root         (0) root         (0)      929 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     9018 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/api_base.py
+-rw-rw-r--   0 root         (0) root         (0)      484 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/settings.py
+-rw-rw-r--   0 root         (0) root         (0)     1199 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/DataAPI/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-30 07:32:20.000000 uqer-1.3.9/uqer/mfclient/
+-rw-rw-r--   0 root         (0) root         (0)      143 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/mfclient/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     7507 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/mfclient/portfolio_construct.py
+-rw-rw-r--   0 root         (0) root         (0)     8285 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/mfclient/signal_process.py
+-rw-rw-r--   0 root         (0) root         (0)     4708 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/mfclient/signal_process_check.py
+-rw-rw-r--   0 root         (0) root         (0)      691 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     4869 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/authorize.py
+-rw-rw-r--   0 root         (0) root         (0)     3489 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/config.py
+-rw-rw-r--   0 root         (0) root         (0)     8284 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/data.py
+-rw-rw-r--   0 root         (0) root         (0)     3876 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/factor.py
+-rw-rw-r--   0 root         (0) root         (0)     4838 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/notebook.py
+-rw-rw-r--   0 root         (0) root         (0)     1484 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/trading.py
+-rw-rw-r--   0 root         (0) root         (0)     1345 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/uqer.py
+-rw-rw-r--   0 root         (0) root         (0)    14019 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/user_factor.py
+-rw-rw-r--   0 root         (0) root         (0)      452 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/utils.py
+-rw-rw-r--   0 root         (0) root         (0)       23 2020-03-30 07:09:26.000000 uqer-1.3.9/uqer/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-03-30 07:32:20.000000 uqer-1.3.9/uqer.egg-info/
+-rw-rw-r--   0 root         (0) root         (0)      220 2020-03-30 07:32:20.000000 uqer-1.3.9/uqer.egg-info/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     1063 2020-03-30 07:32:20.000000 uqer-1.3.9/uqer.egg-info/SOURCES.txt
+-rw-rw-r--   0 root         (0) root         (0)        1 2020-03-30 07:32:20.000000 uqer-1.3.9/uqer.egg-info/dependency_links.txt
+-rw-rw-r--   0 root         (0) root         (0)       10 2020-03-30 07:32:20.000000 uqer-1.3.9/uqer.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       22 2020-03-30 07:09:26.000000 uqer-1.3.9/MANIFEST.in
+-rw-rw-r--   0 root         (0) root         (0)        0 2020-03-30 07:09:26.000000 uqer-1.3.9/README.md
+-rw-rw-r--   0 root         (0) root         (0)      826 2020-03-30 07:09:26.000000 uqer-1.3.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)      220 2020-03-30 07:32:20.000000 uqer-1.3.9/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      100 2020-03-30 07:32:20.000000 uqer-1.3.9/setup.cfg
```

### Comparing `uqer-1.3.8/uqer/DataAPI/ACMR.py` & `uqer-1.3.9/uqer/DataAPI/ACMR.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/CCXE.py` & `uqer-1.3.9/uqer/DataAPI/CCXE.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/CHINABOND.py` & `uqer-1.3.9/uqer/DataAPI/CHINABOND.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/DATAYES.py` & `uqer-1.3.9/uqer/DataAPI/DATAYES.py`

 * *Files 0% similar despite different names*

```diff
@@ -120534,7 +120534,95 @@
         put_data_in_cache(func_name, cache_key, pdFrame)
         return pdFrame
     except Exception as e:
         raise e
     finally:
         myIO.close()
 
+def Dy1dFacRetCNE6Get(beginDate = "", endDate = "", tradeDate = "", field = "", pandas = "1"):
+    """
+    获取Trading Model的风格因子和行业因子对应的收益率，各因子计算查看getDy1dExposureCNE6接口。
+
+    :param beginDate: 交易日的起始日期，输入格式“YYYYMMDD”。,beginDate、endDate至少选择一个
+    :param endDate: 交易日的截止日期，输入格式“YYYYMMDD”。,beginDate、endDate至少选择一个
+    :param tradeDate: 交易日期，输入格式“YYYYMMDD”。,可以是列表,可空
+    :param field: 所需字段,可以是列表,可空
+    :param pandas: 1表示返回 pandas data frame，0表示返回csv,可空
+    :return: :raise e: API查询的结果，是CSV或者被转成pandas data frame；若查询API失败，返回空data frame； 若解析失败，则抛出异常
+    """
+
+    pretty_traceback()
+    frame = inspect.currentframe()
+    func_name, cache_key = get_cache_key(frame)
+    cache_result = get_data_from_cache(func_name, cache_key)
+    if cache_result is not None:
+        return cache_result
+    split_index = None
+    split_param = None
+    httpClient = api_base.__getConn__()
+    requestString = []
+    requestString.append('/api/equity/getDy1dFacRetCNE6.csv?ispandas=1&')
+    if not isinstance(beginDate, str) and not isinstance(beginDate, unicode):
+        beginDate = str(beginDate)
+
+    requestString.append("beginDate=%s"%(beginDate))
+    if not isinstance(endDate, str) and not isinstance(endDate, unicode):
+        endDate = str(endDate)
+
+    requestString.append("&endDate=%s"%(endDate))
+    requestString.append("&tradeDate=")
+    if hasattr(tradeDate,'__iter__') and not isinstance(tradeDate, str):
+        if len(tradeDate) > 100 and split_param is None:
+            split_index = len(requestString)
+            split_param = tradeDate
+            requestString.append(None)
+        else:
+            requestString.append(','.join(tradeDate))
+    else:
+        requestString.append(tradeDate)
+    requestString.append("&field=")
+    if hasattr(field,'__iter__') and not isinstance(field, str):
+        if len(field) > 100 and split_param is None:
+            split_index = len(requestString)
+            split_param = field
+            requestString.append(None)
+        else:
+            requestString.append(','.join(field))
+    else:
+        requestString.append(field)
+    if split_param is None:
+        csvString = api_base.__getCSV__(''.join(requestString), httpClient, gw=True)
+        if csvString is None or len(csvString) == 0 or (csvString[0] == '-' and not api_base.is_no_data_warn(csvString, False)) or csvString[0] == '{':
+            api_base.handle_error(csvString, 'Dy1dFacRetCNE6Get')
+        elif csvString[:2] == '-1':
+            csvString = ''
+    else:
+        p_list = api_base.splist(split_param, 100)
+        csvString = []
+        for index, item in enumerate(p_list):
+            requestString[split_index] = ','.join(item)
+            temp_result = api_base.__getCSV__(''.join(requestString), httpClient, gw=True)
+            if temp_result is None or len(temp_result) == 0 or temp_result[0] == '{' or (temp_result[0] == '-' and not api_base.is_no_data_warn(temp_result, False)):
+                api_base.handle_error(temp_result, 'Dy1dFacRetCNE6Get')
+            if temp_result[:2] != '-1':
+                csvString.append(temp_result if len(csvString) == 0 else temp_result[temp_result.find('\n')+1:])
+        csvString = ''.join(csvString)
+
+    if len(csvString) == 0:
+        if 'field' not in locals() or len(field) == 0:
+            field = [u'tradeDate', u'BETA', u'MOMENTUM', u'SIZE', u'EARNYILD', u'RESVOL', u'GROWTH', u'BTOP', u'LEVERAGE', u'LIQUIDTY', u'MIDCAP', u'DIVYILD', u'EARNQLTY', u'EARNVAR', u'INVSQLTY', u'LTREVRSL', u'PROFIT', u'ANALSENTI', u'INDMOM', u'SEASON', u'STREVRSL', u'Bank', u'RealEstate', u'Health', u'Transportation', u'Mining', u'NonFerMetal', u'HouseApp', u'LeiService', u'MachiEquip', u'BuildDeco', u'CommeTrade', u'CONMAT', u'Auto', u'Textile', u'FoodBever', u'Electronics', u'Computer', u'LightIndus', u'Utilities', u'Telecom', u'AgriForest', u'CHEM', u'Media', u'IronSteel', u'NonBankFinan', u'ELECEQP', u'AERODEF', u'Conglomerates', u'COUNTRY']
+        if hasattr(field, '__iter__') and not isinstance(field, str):
+            csvString = ','.join(field) + '\n'
+        else:
+            csvString = field + '\n'
+    if pandas != "1":
+        put_data_in_cache(func_name, cache_key, csvString)
+        return csvString
+    try:
+        myIO = StringIO(csvString)
+        pdFrame = pd.read_csv(myIO, dtype = {'tradeDate': 'str'},  )
+        put_data_in_cache(func_name, cache_key, pdFrame)
+        return pdFrame
+    except Exception as e:
+        raise e
+    finally:
+        myIO.close()
```

### Comparing `uqer-1.3.8/uqer/DataAPI/DYZH.py` & `uqer-1.3.9/uqer/DataAPI/DYZH.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/DataCube.py` & `uqer-1.3.9/uqer/DataAPI/DataCube.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/FH.py` & `uqer-1.3.9/uqer/DataAPI/FH.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/GG.py` & `uqer-1.3.9/uqer/DataAPI/GG.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/IVOLATILITY.py` & `uqer-1.3.9/uqer/DataAPI/IVOLATILITY.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/JL.py` & `uqer-1.3.9/uqer/DataAPI/JL.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/JY.py` & `uqer-1.3.9/uqer/DataAPI/JY.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/NH.py` & `uqer-1.3.9/uqer/DataAPI/NH.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/OTHER.py` & `uqer-1.3.9/uqer/DataAPI/OTHER.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/SILKRIVER.py` & `uqer-1.3.9/uqer/DataAPI/SILKRIVER.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/SW.py` & `uqer-1.3.9/uqer/DataAPI/SW.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/TEJ.py` & `uqer-1.3.9/uqer/DataAPI/TEJ.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/__init__.py` & `uqer-1.3.9/uqer/DataAPI/__init__.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/api_base.py` & `uqer-1.3.9/uqer/DataAPI/api_base.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/DataAPI/version.py` & `uqer-1.3.9/uqer/DataAPI/version.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/mfclient/portfolio_construct.py` & `uqer-1.3.9/uqer/mfclient/portfolio_construct.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/mfclient/signal_process.py` & `uqer-1.3.9/uqer/mfclient/signal_process.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/mfclient/signal_process_check.py` & `uqer-1.3.9/uqer/mfclient/signal_process_check.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/__init__.py` & `uqer-1.3.9/uqer/__init__.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/authorize.py` & `uqer-1.3.9/uqer/authorize.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/config.py` & `uqer-1.3.9/uqer/config.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/data.py` & `uqer-1.3.9/uqer/data.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/factor.py` & `uqer-1.3.9/uqer/factor.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/notebook.py` & `uqer-1.3.9/uqer/notebook.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/trading.py` & `uqer-1.3.9/uqer/trading.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/uqer.py` & `uqer-1.3.9/uqer/uqer.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer/user_factor.py` & `uqer-1.3.9/uqer/user_factor.py`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/uqer.egg-info/SOURCES.txt` & `uqer-1.3.9/uqer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `uqer-1.3.8/setup.py` & `uqer-1.3.9/setup.py`

 * *Files identical despite different names*

