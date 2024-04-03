# Comparing `tmp/snbpy-1.0.2.tar.gz` & `tmp/snbpy-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/snbpy-1.0.2.tar", last modified: Tue Dec 15 09:54:53 2020, max compression
+gzip compressed data, was "snbpy-1.0.6.tar", last modified: Wed Apr  3 07:25:35 2024, max compression
```

## Comparing `snbpy-1.0.2.tar` & `snbpy-1.0.6.tar`

### file list

```diff
@@ -1,34 +1,36 @@
-drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2020-12-15 09:54:53.000000 snbpy-1.0.2/
--rw-r--r--   0 yangjie    (501) staff       (20)    11615 2020-12-15 09:54:53.000000 snbpy-1.0.2/PKG-INFO
-drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2020-12-15 09:54:53.000000 snbpy-1.0.2/snbpy.egg-info/
--rw-r--r--   0 yangjie    (501) staff       (20)    11615 2020-12-15 09:54:52.000000 snbpy-1.0.2/snbpy.egg-info/PKG-INFO
--rw-r--r--   0 yangjie    (501) staff       (20)      735 2020-12-15 09:54:53.000000 snbpy-1.0.2/snbpy.egg-info/SOURCES.txt
--rw-r--r--   0 yangjie    (501) staff       (20)        9 2020-12-15 09:54:52.000000 snbpy-1.0.2/snbpy.egg-info/requires.txt
--rw-r--r--   0 yangjie    (501) staff       (20)        6 2020-12-15 09:54:52.000000 snbpy-1.0.2/snbpy.egg-info/top_level.txt
--rw-r--r--   0 yangjie    (501) staff       (20)        1 2020-12-15 09:54:52.000000 snbpy-1.0.2/snbpy.egg-info/dependency_links.txt
--rw-r--r--   0 yangjie    (501) staff       (20)     8536 2020-12-14 03:54:55.000000 snbpy-1.0.2/README.md
--rw-r--r--   0 yangjie    (501) staff       (20)     1557 2020-12-15 09:48:39.000000 snbpy-1.0.2/setup.py
--rw-r--r--   0 yangjie    (501) staff       (20)       38 2020-12-15 09:54:53.000000 snbpy-1.0.2/setup.cfg
-drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2020-12-15 09:54:53.000000 snbpy-1.0.2/src/
-drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2020-12-15 09:54:53.000000 snbpy-1.0.2/src/snbpy/
--rw-r--r--   0 yangjie    (501) staff       (20)        0 2020-05-06 07:14:58.000000 snbpy-1.0.2/src/snbpy/__init__.py
-drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2020-12-15 09:54:53.000000 snbpy-1.0.2/src/snbpy/common/
-drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2020-12-15 09:54:53.000000 snbpy-1.0.2/src/snbpy/common/util/
--rw-r--r--   0 yangjie    (501) staff       (20)      155 2020-10-19 09:18:28.000000 snbpy-1.0.2/src/snbpy/common/util/array_utils.py
--rw-r--r--   0 yangjie    (501) staff       (20)     1491 2020-06-24 10:46:05.000000 snbpy-1.0.2/src/snbpy/common/util/config_reader.py
--rw-r--r--   0 yangjie    (501) staff       (20)        0 2020-05-08 08:43:21.000000 snbpy-1.0.2/src/snbpy/common/util/__init__.py
--rw-r--r--   0 yangjie    (501) staff       (20)     4927 2020-10-19 09:18:28.000000 snbpy-1.0.2/src/snbpy/common/util/string_utils.py
--rw-r--r--   0 yangjie    (501) staff       (20)        0 2020-05-08 08:43:11.000000 snbpy-1.0.2/src/snbpy/common/__init__.py
-drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2020-12-15 09:54:53.000000 snbpy-1.0.2/src/snbpy/common/component/
--rw-r--r--   0 yangjie    (501) staff       (20)       35 2020-05-15 07:40:21.000000 snbpy-1.0.2/src/snbpy/common/component/local_cache.py
--rw-r--r--   0 yangjie    (501) staff       (20)        0 2020-05-15 07:39:01.000000 snbpy-1.0.2/src/snbpy/common/component/__init__.py
-drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2020-12-15 09:54:53.000000 snbpy-1.0.2/src/snbpy/common/constant/
--rw-r--r--   0 yangjie    (501) staff       (20)        0 2020-05-06 07:15:34.000000 snbpy-1.0.2/src/snbpy/common/constant/__init__.py
--rw-r--r--   0 yangjie    (501) staff       (20)      517 2020-11-24 07:23:56.000000 snbpy-1.0.2/src/snbpy/common/constant/exceptions.py
--rw-r--r--   0 yangjie    (501) staff       (20)     1911 2020-05-26 03:17:02.000000 snbpy-1.0.2/src/snbpy/common/constant/snb_constant.py
-drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2020-12-15 09:54:53.000000 snbpy-1.0.2/src/snbpy/common/domain/
--rw-r--r--   0 yangjie    (501) staff       (20)     3114 2020-11-19 06:41:40.000000 snbpy-1.0.2/src/snbpy/common/domain/snb_config.py
--rw-r--r--   0 yangjie    (501) staff       (20)    12193 2020-11-24 07:26:12.000000 snbpy-1.0.2/src/snbpy/common/domain/request.py
--rw-r--r--   0 yangjie    (501) staff       (20)        0 2020-05-08 08:49:07.000000 snbpy-1.0.2/src/snbpy/common/domain/__init__.py
--rw-r--r--   0 yangjie    (501) staff       (20)      902 2020-05-18 07:07:22.000000 snbpy-1.0.2/src/snbpy/common/domain/response.py
--rw-r--r--   0 yangjie    (501) staff       (20)    12471 2020-12-15 09:44:55.000000 snbpy-1.0.2/src/snbpy/snb_api_client.py
+drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2024-04-03 07:25:35.134796 snbpy-1.0.6/
+-rw-r--r--   0 yangjie    (501) staff       (20)     1067 2023-12-28 02:06:03.000000 snbpy-1.0.6/LICENSE
+-rw-r--r--   0 yangjie    (501) staff       (20)     1095 2023-12-28 02:06:03.000000 snbpy-1.0.6/LICENSES
+-rw-r--r--   0 yangjie    (501) staff       (20)     9585 2024-04-03 07:25:35.134128 snbpy-1.0.6/PKG-INFO
+-rw-r--r--   0 yangjie    (501) staff       (20)     8541 2023-12-28 03:02:36.000000 snbpy-1.0.6/README.md
+-rw-r--r--   0 yangjie    (501) staff       (20)       38 2024-04-03 07:25:35.134977 snbpy-1.0.6/setup.cfg
+-rw-r--r--   0 yangjie    (501) staff       (20)     1557 2024-04-03 07:25:08.000000 snbpy-1.0.6/setup.py
+drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2024-04-03 07:25:35.125340 snbpy-1.0.6/snbpy.egg-info/
+-rw-r--r--   0 yangjie    (501) staff       (20)     9585 2024-04-03 07:25:35.000000 snbpy-1.0.6/snbpy.egg-info/PKG-INFO
+-rw-r--r--   0 yangjie    (501) staff       (20)      752 2024-04-03 07:25:35.000000 snbpy-1.0.6/snbpy.egg-info/SOURCES.txt
+-rw-r--r--   0 yangjie    (501) staff       (20)        1 2024-04-03 07:25:35.000000 snbpy-1.0.6/snbpy.egg-info/dependency_links.txt
+-rw-r--r--   0 yangjie    (501) staff       (20)        9 2024-04-03 07:25:35.000000 snbpy-1.0.6/snbpy.egg-info/requires.txt
+-rw-r--r--   0 yangjie    (501) staff       (20)        6 2024-04-03 07:25:35.000000 snbpy-1.0.6/snbpy.egg-info/top_level.txt
+drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2024-04-03 07:25:35.121278 snbpy-1.0.6/src/
+drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2024-04-03 07:25:35.126130 snbpy-1.0.6/src/snbpy/
+-rw-r--r--   0 yangjie    (501) staff       (20)        0 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/__init__.py
+drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2024-04-03 07:25:35.126753 snbpy-1.0.6/src/snbpy/common/
+-rw-r--r--   0 yangjie    (501) staff       (20)        0 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/__init__.py
+drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2024-04-03 07:25:35.127561 snbpy-1.0.6/src/snbpy/common/component/
+-rw-r--r--   0 yangjie    (501) staff       (20)        0 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/component/__init__.py
+-rw-r--r--   0 yangjie    (501) staff       (20)       35 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/component/local_cache.py
+drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2024-04-03 07:25:35.128996 snbpy-1.0.6/src/snbpy/common/constant/
+-rw-r--r--   0 yangjie    (501) staff       (20)        0 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/constant/__init__.py
+-rw-r--r--   0 yangjie    (501) staff       (20)      517 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/constant/exceptions.py
+-rw-r--r--   0 yangjie    (501) staff       (20)     2069 2023-12-28 03:26:07.000000 snbpy-1.0.6/src/snbpy/common/constant/snb_constant.py
+drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2024-04-03 07:25:35.131006 snbpy-1.0.6/src/snbpy/common/domain/
+-rw-r--r--   0 yangjie    (501) staff       (20)        0 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/domain/__init__.py
+-rw-r--r--   0 yangjie    (501) staff       (20)    12712 2023-12-28 08:34:31.000000 snbpy-1.0.6/src/snbpy/common/domain/request.py
+-rw-r--r--   0 yangjie    (501) staff       (20)      902 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/domain/response.py
+-rw-r--r--   0 yangjie    (501) staff       (20)     3114 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/domain/snb_config.py
+drwxr-xr-x   0 yangjie    (501) staff       (20)        0 2024-04-03 07:25:35.133040 snbpy-1.0.6/src/snbpy/common/util/
+-rw-r--r--   0 yangjie    (501) staff       (20)        0 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/util/__init__.py
+-rw-r--r--   0 yangjie    (501) staff       (20)      155 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/util/array_utils.py
+-rw-r--r--   0 yangjie    (501) staff       (20)     1491 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/util/config_reader.py
+-rw-r--r--   0 yangjie    (501) staff       (20)     4927 2023-12-28 02:06:03.000000 snbpy-1.0.6/src/snbpy/common/util/string_utils.py
+-rw-r--r--   0 yangjie    (501) staff       (20)    23860 2024-04-03 05:57:39.000000 snbpy-1.0.6/src/snbpy/snb_api_client.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `snbpy-1.0.2/PKG-INFO` & `snbpy-1.0.6/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,281 +1,254 @@
-Metadata-Version: 2.1
-Name: snbpy
-Version: 1.0.2
-Summary: snbpy
-Home-page: https://www.snowballsecurities.com
-Author: SNB
-Author-email: service@xueqiu.com
-License: UNKNOWN
-Project-URL: Bug Reports, https://github.com/snowballsecurities/snbpy/issues
-Project-URL: Funding, https://www.snowballsecurities.com
-Project-URL: Say Thanks!, https://www.snowballsecurities.com
-Project-URL: Source, https://github.com/snowballsecurities/snbpy
-Description: # 雪盈证券 Open API Python SDK 接入说明书
-        
-        ## 接入准备
-        
-        ### 开户入金
-        
-        开发者在接入雪盈证券开发平台之前，需要提前开通雪盈账号。账号开通后，您可以自己的账号ID（以后统称为：account id）作为您账号的唯一标识。
-        
-        #### 开户地址
-        
-        [开户链接](https://www.snowballsecurities.com/xy-account-open/phone-verify)
-        
-        > `https://www.snowballsecurities.com/xy-account-open/phone-verify`
-        
-        #### 查看账户 ID
-        
-        登录雪盈证券APP，查找“我的-设置-账号与安全”，即可看到雪盈账号 ID。
-        
-        ### 申请密钥
-        
-        获取自己的 accountId 后可以在雪盈官网-申请 API，来注册开发者信息，注册后将获得您自己的专属密钥（以后统称为：secret key）作为您登录雪盈开发平台的唯一凭证，请妥善保存。
-        
-        [注册地址](https://www.snowballsecurities.com)
-        
-        > `https://www.snowballsecurities.com`
-        
-        ### 引入代码
-        
-        获取 secret key 后即可进行 Python SDK 接入，有以下几种获取 SDK 的方式：
-        
-        #### pip 安装
-        
-        ##### 测试仓库
-        
-        `pip install -i https://test.pypi.org/simple/ snbpy==1.0.0`
-        
-        ##### 正式仓库(暂未发布)
-        
-        `pip install snbpy`
-        
-        #### 源码安装
-        
-        [源码仓库](https://github.com/snowballsecurities/snbpy)
-        
-        > `https://github.com/snowballsecurities/snbpy`
-        
-        `python3 setup.py install`
-        
-        > 请与客户经理联系获取源码或者访问项目 GitHub 首页获取
-        
-        ### 环境说明
-        
-        雪盈证券为 API 开发者提供两套环境，分别是 sit 测试环境和 prod 生产环境，现对这两套环境做分别说明。
-        
-        | **环境** | **环境名称** | **链接方式**                             | **账号获取**     |
-        | -------- | ------------ | ---------------------------------------- | ---------------- |
-        | sit      | 测试环境     | `https://sandbox.snbsecurities.com` | 联系雪盈客服获得 |
-        | prod     | 正式环境     | `https:// openapi.snbsecurities.com` | 参考1.1和1.2     |
-        
-        >  **PORD**  环境中用户账号、资金均为真实账号、资金，所做操作全部真实有效，请**勿**做测试操作。
-        
-        > SIT 环境的用户账户为模拟账号，资金是虚拟的用于测试验证，测试账号的申请联系雪盈证券 API 服务群的群主。
-        
-        ## 快速开始
-        
-        ### 代码概要
-        
-        SDK 主要有以下几个类 
-        
-        * SnbConfig SDK 的 Client 的基础配置
-          > `from snbpy.common.domain.snb_config import SnbConfig`
-        * TradeInterface API 的 接口类,包含 10 个抽象方法,对应 10 种 API.
-        * SnbApiClient SDK 的基础框架.
-          > `from snbpy.snb_api_client import SnbHttpClient, TradeInterface`
-        
-        ### 配置项
-        
-        | **key**    | **含义**        | **备注** |
-        | ---------- | --------------- | -------- |
-        | account    | U 账户          |          |
-        | key        | API access Key  |          |
-        | sign_type  | 加密方式        | 暂不支持 |
-        | snb_server | API 服务器地址  |          |
-        | snb_port   | API 服务器端口  |          |
-        | timeout    | Http 超时时间   |          |
-        | cache_path | 缓存路径        | 暂不支持 |
-        | schema     | API Http Schema |          |
-        | auto_login | 是否自动登陆    | 暂不支持 |
-        
-        ### 调用示例
-        
-        SDK 提供了Http API 的 requests 实现 `SnbHttpClient(SnbApiClient)`, 如想替换其他 httpClient 可以重写 `_do_execute` 方法, 下面是登陆并查询订单的示例代码. 
-        
-        ```python
-        from snbpy.common.domain.snb_config import SnbConfig
-        from snbpy.snb_api_client import SnbHttpClient
-        if __name__ == '__main__':
-            config = SnbConfig()
-            config.account = "DU876752"
-            config.key = '123456'
-            config.sign_type = 'None'
-            config.snb_server ='sandbox.snbsecurities.com'
-            config.snb_port = '443'
-            config.timeout = 1000
-            config.schema = 'https'
-        
-            client = SnbHttpClient(config)
-            client.login()
-            order_list_response = client.get_order_list()
-        ```
-        
-        
-        
-        ### 管理
-        
-        token是一串无序加密的字符串，形如: `pwQxtqj3Bl1q3ThX3I5rRJyUyQxffWX9`，在访问 API 时，用户需携带该 token 作为身份凭证。用户获取 token 的个数没有限制，但服务器仅为每个用户保存 10 个有效 token ，再用户连续申请第 11 个 token 时，第一个 token 开始失效，以此类推。
-        
-        `SnbHttpClient` 中封装了token相关的方法，login 方法会直接访问API获取一个Auth对象，包含了token和过期时间.
-        
-        ### 方法描述
-        
-        更多详情请使用 `help(TradeInterface)` 方法获取文档
-        
-        ```python
-        >>> from snbpy.snb_api_client import TradeInterface
-        >>> help(TradeInterface)
-        ```
-        
-        以下是方法列表
-        
-        | 方法名               | 描述                                   |
-        | -------------------- | -------------------------------------- |
-        | login                | 访问API生成一个新token，不会使用缓存   |
-        | get_token_status     | 查询token，一般用于查询token的过期时间 |
-        | place_order          | 下单                                   |
-        | get_order_by_id      | 订单查询，单条                         |
-        | get_order_list       | 订单查询，批量                         |
-        | cancel_order         | 撤销订单                               |
-        | get_position_list    | 持仓查询                               |
-        | get_balance          | 资产查询                               |
-        | get_security_detail  | 证券信息查询                           |
-        | get_transaction_list | 成交查询                               |
-        
-        ## 数据字典
-        
-        ### Currency
-        
-        | 名称 | 描述         |
-        | ---- | ------------ |
-        | BASE | 基础货币     |
-        | USX  |              |
-        | CNY  | 人民币       |
-        | USD  | 美元         |
-        | SEK  | 瑞典克朗     |
-        | SGD  | 新加坡币     |
-        | TRY  | 土耳其里拉   |
-        | ZAR  | 南非兰特     |
-        | JPY  | 日元         |
-        | AUD  | 澳元         |
-        | CAD  | 加币         |
-        | CHF  | 瑞士法郎     |
-        | CNH  | 人民币       |
-        | HKD  | 港币         |
-        | NZD  | 新西兰币     |
-        | CZK  | 捷克克朗     |
-        | DKK  | 丹麦克朗     |
-        | HUF  | 匈牙利福林   |
-        | NOK  | 挪威克朗     |
-        | PLN  | 波兰兹罗提   |
-        | EUR  | 欧元         |
-        | GBP  | 英镑         |
-        | ILS  | 以色列谢克尔 |
-        | MXN  | 墨西哥比索   |
-        | RUB  | 卢布         |
-        | KRW  | 韩元         |
-        
-        ### SecurityType
-        
-        | 名称  | 描述               |
-        | ----- | ------------------ |
-        | STK   | 股票               |
-        | FUT   | 期货               |
-        | OPT   | 期权               |
-        | FOP   | 期货期权           |
-        | WAR   | 涡轮               |
-        | MLEG  | 不支持             |
-        | CASH  | 外汇               |
-        | CFD   | 差价合约           |
-        | CMDTY | 大宗商品           |
-        | FUND  | 基金               |
-        | IOPT  | 牛熊证             |
-        | BOND  | 债券               |
-        | ALL   | 全部类型(查询条件) |
-        
-        ### OderType
-        
-        | 名称              | 描述       |
-        | ----------------- | ---------- |
-        | LIMIT             | 限价单     |
-        | MARKET            | 市价单     |
-        | AT                | 不支持     |
-        | ATL               | 不支持     |
-        | SSL               | 不支持     |
-        | SEL               | 不支持     |
-        | STOP              | 止损单     |
-        | STOP_LIMIT        | 限价止损单 |
-        | TRAIL             | 追踪单     |
-        | TRAIL_LIMIT       | 限价追踪单 |
-        | LIMIT_ON_OPENING  | 开市限价单 |
-        | MARKET_ON_OPENING | 开市市价单 |
-        | LIMIT_ON_CLOSE    | 闭市限价单 |
-        | MARKET_ON_CLOSE   | 闭市市价单 |
-        
-        ### OrderSide
-        
-        | 名称 | 描述 |
-        | ---- | ---- |
-        | BUY  | 买入 |
-        | SELL | 卖出 |
-        
-        ### OrderStatus
-        
-        | 名称               | 描述     |
-        | ------------------ | -------- |
-        | NO_REPORT          | 未报     |
-        | WAIT_REPORT        | 待报     |
-        | REPORTED           | 已报     |
-        | WAIT_WITHDRAW      | 已报待撤 |
-        | PART_WAIT_WITHDRAW | 部成待撤 |
-        | PART_WITHDRAW      | 部撤     |
-        | WITHDRAWED         | 已撤     |
-        | PART_CONCLUDED     | 部成     |
-        | CONCLUDED          | 已成     |
-        | INVALID            | 废单     |
-        
-        ### TimeInForce
-        
-        | 名称 | 描述       |
-        | ---- | ---------- |
-        | DAY  | 当日有效   |
-        | GTC  | 撤单前有效 |
-        
-        ## 更新日志
-        
-        | 更新日期   | 更新内容                         |version|
-        | ---------- | -------------------------------- |---|
-        | 2020-11-24 | 增加更多日志, 增加 OrderID 的非空验证 |1.0.1|
-        | 2020-07-08 | 更新至当前最新安装方式与连接方式 | 1.0.0|
-        | 2020-06-08 | 初始化更新                       |--|
-        
-        ##  **联系我们**
-        
-        如果您在使用过程中遇到任何问题，可以通过以下方式联系我们获取帮助，雪盈证券客服电话：400-118-8886。
-        
-        
-Keywords: snbpy
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6, <4
-Description-Content-Type: text/markdown
+# 雪盈证券 Open API Python SDK 接入说明书
+
+## 接入准备
+
+### 开户入金
+
+开发者在接入雪盈证券开发平台之前，需要提前开通雪盈账号。账号开通后，您可以自己的账号ID（以后统称为：account id）作为您账号的唯一标识。
+
+#### 开户地址
+
+[开户链接](https://www.snowballsecurities.com/xy-account-open/phone-verify)
+
+> `https://www.snowballsecurities.com/xy-account-open/phone-verify`
+
+#### 查看账户 ID
+
+登录雪盈证券APP，查找“我的-设置-账号与安全”，即可看到雪盈账号 ID。
+
+### 申请密钥
+
+获取自己的 accountId 后可以在雪盈官网-申请 API，来注册开发者信息，注册后将获得您自己的专属密钥（以后统称为：secret key）作为您登录雪盈开发平台的唯一凭证，请妥善保存。
+
+[注册地址](https://www.snowballsecurities.com)
+
+> `https://www.snowballsecurities.com`
+
+### 引入代码
+
+获取 secret key 后即可进行 Python SDK 接入，有以下几种获取 SDK 的方式：
+
+#### pip 安装
+
+##### 测试仓库
+
+`pip install -i https://test.pypi.org/simple/ snbpy==1.0.3`
+
+##### 正式仓库(最新版本1.0.3)
+
+`pip install snbpy`
+
+#### 源码安装
+
+[源码仓库](https://github.com/snowballsecurities/snbpy)
+
+> `https://github.com/snowballsecurities/snbpy`
+
+`python3 setup.py install`
+
+> 请与客户经理联系获取源码或者访问项目 GitHub 首页获取
+
+### 环境说明
+
+雪盈证券为 API 开发者提供两套环境，分别是 sit 测试环境和 prod 生产环境，现对这两套环境做分别说明。
+
+| **环境** | **环境名称** | **链接方式**                             | **账号获取**     |
+| -------- | ------------ | ---------------------------------------- | ---------------- |
+| sit      | 测试环境     | `https://sandbox.snbsecurities.com` | 联系雪盈客服获得 |
+| prod     | 正式环境     | `https:// openapi.snbsecurities.com` | 参考1.1和1.2     |
+
+>  **PORD**  环境中用户账号、资金均为真实账号、资金，所做操作全部真实有效，请**勿**做测试操作。
+
+> SIT 环境的用户账户为模拟账号，资金是虚拟的用于测试验证，测试账号的申请联系雪盈证券 API 服务群的群主。
+
+## 快速开始
+
+### 代码概要
+
+SDK 主要有以下几个类 
+
+* SnbConfig SDK 的 Client 的基础配置
+  > `from snbpy.common.domain.snb_config import SnbConfig`
+* TradeInterface API 的 接口类,包含 10 个抽象方法,对应 10 种 API.
+* SnbApiClient SDK 的基础框架.
+  > `from snbpy.snb_api_client import SnbHttpClient, TradeInterface`
+
+### 配置项
+
+| **key**    | **含义**        | **备注** |
+| ---------- | --------------- | -------- |
+| account    | U 账户          |          |
+| key        | API access Key  |          |
+| sign_type  | 加密方式        | 暂不支持 |
+| snb_server | API 服务器地址  |          |
+| snb_port   | API 服务器端口  |          |
+| timeout    | Http 超时时间   |          |
+| cache_path | 缓存路径        | 暂不支持 |
+| schema     | API Http Schema |          |
+| auto_login | 是否自动登陆    | 暂不支持 |
+
+### 调用示例
+
+SDK 提供了Http API 的 requests 实现 `SnbHttpClient(SnbApiClient)`, 如想替换其他 httpClient 可以重写 `_do_execute` 方法, 下面是登陆并查询订单的示例代码. 
+
+```python
+from snbpy.common.domain.snb_config import SnbConfig
+from snbpy.snb_api_client import SnbHttpClient
+if __name__ == '__main__':
+    config = SnbConfig()
+    config.account = "DU876752"
+    config.key = '123456'
+    config.sign_type = 'None'
+    config.snb_server ='sandbox.snbsecurities.com'
+    config.snb_port = '443'
+    config.timeout = 1000
+    config.schema = 'https'
+
+    client = SnbHttpClient(config)
+    client.login()
+    order_list_response = client.get_order_list()
+```
+
+
+
+### 管理
+
+token是一串无序加密的字符串，形如: `pwQxtqj3Bl1q3ThX3I5rRJyUyQxffWX9`，在访问 API 时，用户需携带该 token 作为身份凭证。用户获取 token 的个数没有限制，但服务器仅为每个用户保存 10 个有效 token ，再用户连续申请第 11 个 token 时，第一个 token 开始失效，以此类推。
+
+`SnbHttpClient` 中封装了token相关的方法，login 方法会直接访问API获取一个Auth对象，包含了token和过期时间.
+
+### 方法描述
+
+更多详情请使用 `help(TradeInterface)` 方法获取文档
+
+```python
+>>> from snbpy.snb_api_client import TradeInterface
+>>> help(TradeInterface)
+```
+
+以下是方法列表
+
+| 方法名               | 描述                                   |
+| -------------------- | -------------------------------------- |
+| login                | 访问API生成一个新token，不会使用缓存   |
+| get_token_status     | 查询token，一般用于查询token的过期时间 |
+| place_order          | 下单                                   |
+| get_order_by_id      | 订单查询，单条                         |
+| get_order_list       | 订单查询，批量                         |
+| cancel_order         | 撤销订单                               |
+| get_position_list    | 持仓查询                               |
+| get_balance          | 资产查询                               |
+| get_security_detail  | 证券信息查询                           |
+| get_transaction_list | 成交查询                               |
+
+## 数据字典
+
+### Currency
+
+| 名称 | 描述         |
+| ---- | ------------ |
+| BASE | 基础货币     |
+| USX  |              |
+| CNY  | 人民币       |
+| USD  | 美元         |
+| SEK  | 瑞典克朗     |
+| SGD  | 新加坡币     |
+| TRY  | 土耳其里拉   |
+| ZAR  | 南非兰特     |
+| JPY  | 日元         |
+| AUD  | 澳元         |
+| CAD  | 加币         |
+| CHF  | 瑞士法郎     |
+| CNH  | 人民币       |
+| HKD  | 港币         |
+| NZD  | 新西兰币     |
+| CZK  | 捷克克朗     |
+| DKK  | 丹麦克朗     |
+| HUF  | 匈牙利福林   |
+| NOK  | 挪威克朗     |
+| PLN  | 波兰兹罗提   |
+| EUR  | 欧元         |
+| GBP  | 英镑         |
+| ILS  | 以色列谢克尔 |
+| MXN  | 墨西哥比索   |
+| RUB  | 卢布         |
+| KRW  | 韩元         |
+
+### SecurityType
+
+| 名称  | 描述               |
+| ----- | ------------------ |
+| STK   | 股票               |
+| FUT   | 期货               |
+| OPT   | 期权               |
+| FOP   | 期货期权           |
+| WAR   | 涡轮               |
+| MLEG  | 不支持             |
+| CASH  | 外汇               |
+| CFD   | 差价合约           |
+| CMDTY | 大宗商品           |
+| FUND  | 基金               |
+| IOPT  | 牛熊证             |
+| BOND  | 债券               |
+| ALL   | 全部类型(查询条件) |
+
+### OderType
+
+| 名称              | 描述       |
+| ----------------- | ---------- |
+| LIMIT             | 限价单     |
+| MARKET            | 市价单     |
+| AT                | 不支持     |
+| ATL               | 不支持     |
+| SSL               | 不支持     |
+| SEL               | 不支持     |
+| STOP              | 止损单     |
+| STOP_LIMIT        | 限价止损单 |
+| TRAIL             | 追踪单     |
+| TRAIL_LIMIT       | 限价追踪单 |
+| LIMIT_ON_OPENING  | 开市限价单 |
+| MARKET_ON_OPENING | 开市市价单 |
+| LIMIT_ON_CLOSE    | 闭市限价单 |
+| MARKET_ON_CLOSE   | 闭市市价单 |
+
+### OrderSide
+
+| 名称 | 描述 |
+| ---- | ---- |
+| BUY  | 买入 |
+| SELL | 卖出 |
+
+### OrderStatus
+
+| 名称               | 描述     |
+| ------------------ | -------- |
+| NO_REPORT          | 未报     |
+| WAIT_REPORT        | 待报     |
+| REPORTED           | 已报     |
+| WAIT_WITHDRAW      | 已报待撤 |
+| PART_WAIT_WITHDRAW | 部成待撤 |
+| PART_WITHDRAW      | 部撤     |
+| WITHDRAWED         | 已撤     |
+| PART_CONCLUDED     | 部成     |
+| CONCLUDED          | 已成     |
+| INVALID            | 废单     |
+
+### TimeInForce
+
+| 名称 | 描述       |
+| ---- | ---------- |
+| DAY  | 当日有效   |
+| GTC  | 撤单前有效 |
+
+## 更新日志
+
+| 更新日期   | 更新内容                         |version|
+| ---------- | -------------------------------- |---|
+| 2020-11-24 | 增加更多日志, 增加 OrderID 的非空验证 |1.0.1|
+| 2020-07-08 | 更新至当前最新安装方式与连接方式 | 1.0.0|
+| 2020-06-08 | 初始化更新                       |--|
+
+##  **联系我们**
+
+如果您在使用过程中遇到任何问题，可以通过以下方式联系我们获取帮助，雪盈证券客服电话：400-118-8886。
+
```

### Comparing `snbpy-1.0.2/snbpy.egg-info/SOURCES.txt` & `snbpy-1.0.6/snbpy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+LICENSE
+LICENSES
 README.md
 setup.py
 snbpy.egg-info/PKG-INFO
 snbpy.egg-info/SOURCES.txt
 snbpy.egg-info/dependency_links.txt
 snbpy.egg-info/requires.txt
 snbpy.egg-info/top_level.txt
```

### Comparing `snbpy-1.0.2/README.md` & `snbpy-1.0.6/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,34 @@
+Metadata-Version: 2.1
+Name: snbpy
+Version: 1.0.6
+Summary: snbpy
+Home-page: https://www.snowballsecurities.com
+Author: SNB
+Author-email: service@xueqiu.com
+Project-URL: Bug Reports, https://github.com/snowballsecurities/snbpy/issues
+Project-URL: Funding, https://www.snowballsecurities.com
+Project-URL: Say Thanks!, https://www.snowballsecurities.com
+Project-URL: Source, https://github.com/snowballsecurities/snbpy
+Keywords: snbpy
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.6, <4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: LICENSES
+
 # 雪盈证券 Open API Python SDK 接入说明书
 
 ## 接入准备
 
 ### 开户入金
 
 开发者在接入雪盈证券开发平台之前，需要提前开通雪盈账号。账号开通后，您可以自己的账号ID（以后统称为：account id）作为您账号的唯一标识。
@@ -28,17 +55,17 @@
 
 获取 secret key 后即可进行 Python SDK 接入，有以下几种获取 SDK 的方式：
 
 #### pip 安装
 
 ##### 测试仓库
 
-`pip install -i https://test.pypi.org/simple/ snbpy==1.0.0`
+`pip install -i https://test.pypi.org/simple/ snbpy==1.0.3`
 
-##### 正式仓库(暂未发布)
+##### 正式仓库(最新版本1.0.3)
 
 `pip install snbpy`
 
 #### 源码安装
 
 [源码仓库](https://github.com/snowballsecurities/snbpy)
```

### Comparing `snbpy-1.0.2/setup.py` & `snbpy-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='snbpy',
 
-    version='1.0.2',
+    version='1.0.6',
 
     description='snbpy',
 
     long_description=long_description,
 
     long_description_content_type='text/markdown',
```

### Comparing `snbpy-1.0.2/src/snbpy/common/util/config_reader.py` & `snbpy-1.0.6/src/snbpy/common/util/config_reader.py`

 * *Files identical despite different names*

### Comparing `snbpy-1.0.2/src/snbpy/common/util/string_utils.py` & `snbpy-1.0.6/src/snbpy/common/util/string_utils.py`

 * *Files identical despite different names*

### Comparing `snbpy-1.0.2/src/snbpy/common/constant/exceptions.py` & `snbpy-1.0.6/src/snbpy/common/constant/exceptions.py`

 * *Files identical despite different names*

### Comparing `snbpy-1.0.2/src/snbpy/common/constant/snb_constant.py` & `snbpy-1.0.6/src/snbpy/common/constant/snb_constant.py`

 * *Files 10% similar despite different names*

```diff
@@ -46,14 +46,16 @@
     STOP_LIMIT = 'STOP_LIMIT'
     TRAIL = 'TRAIL'
     TRAIL_LIMIT = 'TRAIL_LIMIT'
     LIMIT_ON_OPENING = 'LIMIT_ON_OPENING'
     MARKET_ON_OPENING = 'MARKET_ON_OPENING'
     LIMIT_ON_CLOSE = 'LIMIT_ON_CLOSE'
     MARKET_ON_CLOSE = 'MARKET_ON_CLOSE'
+    LIMIT_IF_TOUCHED = 'LIMIT_IF_TOUCHED'
+    MARKET_IF_TOUCHED = 'MARKET_IF_TOUCHED'
 
 
 @unique
 class SecurityType(Enum):
     ALL = 'ALL'
     STK = 'STK'
     FUT = 'FUT'
@@ -70,14 +72,19 @@
 
 
 @unique
 class OrderSide(Enum):
     BUY = 'BUY'
     SELL = 'SELL'
 
+@unique
+class OrderIdType(Enum):
+    CLIENT = 'CLIENT'
+    SNB = 'SNB'
+
 
 @unique
 class OrderStatus(Enum):
     INVALID = 'INVALID'
     EXPIRED = 'EXPIRED'
     NO_REPORT = 'NO_REPORT'
     WAIT_REPORT = 'WAIT_REPORT'
```

### Comparing `snbpy-1.0.2/src/snbpy/common/domain/snb_config.py` & `snbpy-1.0.6/src/snbpy/common/domain/snb_config.py`

 * *Files identical despite different names*

### Comparing `snbpy-1.0.2/src/snbpy/common/domain/request.py` & `snbpy-1.0.6/src/snbpy/common/domain/request.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import abc
 import logging
 
 from snbpy.common.constant.exceptions import InvalidParamException, INVALID_ORDER_ID
-from snbpy.common.constant.snb_constant import HttpMethod, OrderSide, SecurityType, OrderType, Currency, TimeInForce
+from snbpy.common.constant.snb_constant import HttpMethod, OrderSide, SecurityType, OrderType, Currency, TimeInForce, OrderIdType
 from snbpy.common.util.string_utils import StringUtils
 
 logger = logging.getLogger("snbpy")
 
 class HttpRequest(metaclass=abc.ABCMeta):
 
     @abc.abstractmethod
@@ -144,27 +144,30 @@
 
 
 class PlaceOrderRequest(HttpRequest):
 
     def __init__(self, account_id: str, order_id: str, security_type: SecurityType, symbol: str, exchange: str,
                  side: OrderSide, currency: Currency, quantity: int, price: float = 0,
                  order_type: OrderType = OrderType.LIMIT, tif: TimeInForce = TimeInForce.DAY,
-                 force_only_rth: bool = True):
+                 force_only_rth: bool = True, stop_price: float = 0, parent: str = None, order_id_type: OrderIdType = OrderIdType.CLIENT):
         self._account_id = account_id
         self._order_id = order_id
         self._security_type = security_type
         self._symbol = symbol
         self._exchange = exchange
         self._order_type = order_type
         self._side = side
         self._currency = currency
         self._quantity = quantity
         self._price = price
         self._tif = tif
         self._force_only_rth = force_only_rth
+        self._stop_price = stop_price
+        self._parent = parent
+        self._order_id_type = order_id_type
 
     def auth(self) -> int:
         return 1
 
     def verify(self) -> bool:
         if StringUtils.is_blank(self._order_id):
             logger.error("order id cannot by blank;; order_id: %s", self._order_id)
@@ -186,22 +189,27 @@
                 "exchange": self._exchange,
                 "order_type": self._order_type.value,
                 "side": self._side.value,
                 "currency": self._currency.value,
                 "quantity": self._quantity,
                 "price": self._price,
                 "tif": self._tif.value,
-                "rth": self._force_only_rth}
+                "rth": self._force_only_rth,
+                "stop_price": self._stop_price,
+                "parent": self._parent,
+                "order_id_type": self._order_id_type.value
+                }
 
 
 class CancelOrderRequest(HttpRequest):
-    def __init__(self, account_id: str, order_id: str, origin_order_id: str):
+    def __init__(self, account_id: str, order_id: str, origin_order_id: str, order_id_type: OrderIdType = OrderIdType.CLIENT):
         self._origin_order_id = origin_order_id
         self._order_id = order_id
         self._account_id = account_id
+        self._order_id_type = order_id_type
 
     @property
     def account_id(self) -> str:
         return self._account_id
 
     @account_id.setter
     def account_id(self, value: str):
@@ -234,15 +242,15 @@
         return HttpMethod.DELETE
 
     @property
     def url(self) -> str:
         return "order/%s" % self._origin_order_id
 
     def generate_params(self) -> dict:
-        return {"new_id": self._order_id, "account_id": self._account_id}
+        return {"new_id": self._order_id, "account_id": self._account_id, "order_id_type": self._order_id_type.value}
 
 
 class GetOrderByOrderIdRequest(HttpRequest):
     def __init__(self, account_id: str, order_id: str):
         self._account_id = account_id
         self._order_id = order_id
```

### Comparing `snbpy-1.0.2/src/snbpy/common/domain/response.py` & `snbpy-1.0.6/src/snbpy/common/domain/response.py`

 * *Files identical despite different names*

