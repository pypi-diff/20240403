# Comparing `tmp/rcquant_sdk-0.0.8.tar.gz` & `tmp/rcquant_sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcquant_sdk-0.0.8.tar", last modified: Mon Dec 11 06:18:53 2023, max compression
+gzip compressed data, was "rcquant_sdk-0.0.9.tar", last modified: Mon Dec 11 08:34:04 2023, max compression
```

## Comparing `rcquant_sdk-0.0.8.tar` & `rcquant_sdk-0.0.9.tar`

### file list

```diff
@@ -1,112 +1,112 @@
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.383454 rcquant_sdk-0.0.8/
--rw-rw-rw-   0        0        0      392 2023-12-11 06:18:53.382458 rcquant_sdk-0.0.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.188974 rcquant_sdk-0.0.8/rcquant_sdk/
--rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/__init__.py
--rw-rw-rw-   0        0        0    25131 2023-12-11 03:08:24.000000 rcquant_sdk-0.0.8/rcquant_sdk/api.py
--rw-rw-rw-   0        0        0     2430 2023-12-07 03:15:22.000000 rcquant_sdk-0.0.8/rcquant_sdk/client.py
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.212911 rcquant_sdk-0.0.8/rcquant_sdk/data/
--rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.246820 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/
--rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/__init__.py
--rw-rw-rw-   0        0        0     6128 2023-12-08 08:23:00.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/bar_graph_param_data.py
--rw-rw-rw-   0        0        0     6408 2023-12-08 06:34:11.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/chart_init_param_data.py
--rw-rw-rw-   0        0        0     6940 2023-12-08 08:29:12.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/financial_graph_param_data.py
--rw-rw-rw-   0        0        0     1065 2023-12-08 06:34:44.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/graph_value_data.py
--rw-rw-rw-   0        0        0      565 2023-12-08 06:34:59.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/graph_value_list_data.py
--rw-rw-rw-   0        0        0     3620 2023-12-08 06:35:17.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/legend_item_param_data.py
--rw-rw-rw-   0        0        0     4728 2023-12-08 06:35:34.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/line_graph_param_data.py
--rw-rw-rw-   0        0        0     4500 2023-12-08 06:35:49.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/marker_graph_param_data.py
--rw-rw-rw-   0        0        0      697 2023-12-08 06:36:02.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/ohlc_value_data.py
--rw-rw-rw-   0        0        0      566 2023-12-08 06:36:17.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/ohlc_value_list_data.py
--rw-rw-rw-   0        0        0     3531 2023-12-08 06:36:30.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/plot_param_data.py
--rw-rw-rw-   0        0        0     2670 2023-12-08 06:36:48.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/text_graph_param_data.py
--rw-rw-rw-   0        0        0      686 2023-12-08 06:37:04.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/time_axis_param_data.py
--rw-rw-rw-   0        0        0     1538 2023-12-08 06:37:26.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/time_span_gvlist_data.py
--rw-rw-rw-   0        0        0     2400 2023-12-08 06:37:47.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/chart/value_axis_param_data.py
--rw-rw-rw-   0        0        0      636 2023-12-08 06:33:13.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/login_data.py
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.262778 rcquant_sdk-0.0.8/rcquant_sdk/data/market/
--rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/market/__init__.py
--rw-rw-rw-   0        0        0     2238 2023-12-08 03:08:19.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/market/history_ohlc_param_data.py
--rw-rw-rw-   0        0        0      471 2023-12-08 03:21:00.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/market/market_param_data.py
--rw-rw-rw-   0        0        0     9867 2023-12-08 03:21:15.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/market/ohlc_data.py
--rw-rw-rw-   0        0        0     4290 2023-12-08 03:21:34.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/market/query_param_data.py
--rw-rw-rw-   0        0        0    10821 2023-12-11 01:04:40.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/market/save_ohlc_list_param_data.py
--rw-rw-rw-   0        0        0     9805 2023-12-11 02:50:07.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/market/save_tick_list_param_data.py
--rw-rw-rw-   0        0        0     1181 2023-12-08 03:22:13.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/market/sub_ohlc_param_data.py
--rw-rw-rw-   0        0        0     2893 2023-12-08 03:22:23.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/market/tick_data.py
--rw-rw-rw-   0        0        0     1996 2023-12-08 06:33:23.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/message_data.py
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.286712 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/
--rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/__init__.py
--rw-rw-rw-   0        0        0     7875 2023-12-08 03:30:19.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/account_data.py
--rw-rw-rw-   0        0        0      744 2023-12-08 03:30:48.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/get_account_param_data.py
--rw-rw-rw-   0        0        0      768 2023-12-08 03:32:09.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/get_orders_param_data.py
--rw-rw-rw-   0        0        0     1289 2023-12-08 03:36:52.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/get_positions_param_data.py
--rw-rw-rw-   0        0        0      813 2023-12-08 03:37:41.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/get_tradeorders_param_data.py
--rw-rw-rw-   0        0        0    11917 2023-12-08 03:36:28.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/order_data.py
--rw-rw-rw-   0        0        0    20702 2023-12-08 06:15:42.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/position_data.py
--rw-rw-rw-   0        0        0     1045 2023-12-08 06:16:01.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/read_history_order_param_data.py
--rw-rw-rw-   0        0        0     1090 2023-12-08 06:16:21.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/read_history_tradeorder_param_data.py
--rw-rw-rw-   0        0        0      458 2023-12-08 03:37:59.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/trade_param_data.py
--rw-rw-rw-   0        0        0     5541 2023-12-08 06:18:05.000000 rcquant_sdk-0.0.8/rcquant_sdk/data/trade/tradeorder_data.py
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.297683 rcquant_sdk-0.0.8/rcquant_sdk/handle/
--rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/handle/__init__.py
--rw-rw-rw-   0        0        0     1906 2023-12-08 06:33:22.000000 rcquant_sdk-0.0.8/rcquant_sdk/handle/base_handle.py
--rw-rw-rw-   0        0        0     5064 2023-12-08 06:33:22.000000 rcquant_sdk-0.0.8/rcquant_sdk/handle/chart_handle.py
--rw-rw-rw-   0        0        0     7115 2023-12-11 02:56:01.000000 rcquant_sdk-0.0.8/rcquant_sdk/handle/market_handle.py
--rw-rw-rw-   0        0        0     1664 2023-12-08 06:33:22.000000 rcquant_sdk-0.0.8/rcquant_sdk/handle/req_rsp.py
--rw-rw-rw-   0        0        0     8337 2023-12-08 06:33:22.000000 rcquant_sdk-0.0.8/rcquant_sdk/handle/trade_handle.py
--rw-rw-rw-   0        0        0     2772 2023-12-11 02:55:39.000000 rcquant_sdk-0.0.8/rcquant_sdk/interface.py
--rw-rw-rw-   0        0        0      728 2023-12-08 03:37:41.000000 rcquant_sdk-0.0.8/rcquant_sdk/listener.py
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.302670 rcquant_sdk-0.0.8/rcquant_sdk/packer/
--rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.332590 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/
--rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/__init__.py
--rw-rw-rw-   0        0        0     1563 2023-12-07 01:20:17.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/bar_graph_param_data_packer.py
--rw-rw-rw-   0        0        0     2727 2023-11-15 01:07:43.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/chart_init_param_data_packer.py
--rw-rw-rw-   0        0        0     1718 2023-12-08 06:34:30.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/financial_graph_param_data_packer.py
--rw-rw-rw-   0        0        0      551 2023-11-03 01:33:17.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/graph_value_data_packer.py
--rw-rw-rw-   0        0        0      457 2023-11-03 01:33:13.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/graph_value_list_data_packer.py
--rw-rw-rw-   0        0        0     1349 2023-11-13 03:19:22.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/legend_item_param_data_packer.py
--rw-rw-rw-   0        0        0     1560 2023-11-03 01:33:06.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/line_graph_param_data_packer.py
--rw-rw-rw-   0        0        0     1548 2023-11-03 01:33:02.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/marker_graph_param_data_packer.py
--rw-rw-rw-   0        0        0      440 2023-11-03 01:32:58.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/ohlc_value_data_packer.py
--rw-rw-rw-   0        0        0      464 2023-11-03 01:32:54.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/ohlc_value_list_data_packer.py
--rw-rw-rw-   0        0        0     1253 2023-11-03 01:32:49.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/plot_param_data_packer.py
--rw-rw-rw-   0        0        0     1049 2023-11-03 01:32:46.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/text_graph_param_data_packer.py
--rw-rw-rw-   0        0        0      432 2023-11-03 01:32:42.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/time_axis_param_data_packer.py
--rw-rw-rw-   0        0        0      512 2023-11-15 01:07:27.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/time_span_gvlist_data_packer.py
--rw-rw-rw-   0        0        0      957 2023-12-08 06:37:48.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/value_axis_param_data_packer.py
--rw-rw-rw-   0        0        0      417 2023-12-08 03:27:12.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/login_data_packer.py
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.351539 rcquant_sdk-0.0.8/rcquant_sdk/packer/market/
--rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/market/__init__.py
--rw-rw-rw-   0        0        0      783 2023-11-13 03:15:26.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/market/history_ohlc_param_data_packer.py
--rw-rw-rw-   0        0        0      370 2023-12-08 03:21:01.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/market/market_param_data_packer.py
--rw-rw-rw-   0        0        0     3086 2023-11-03 01:25:29.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/market/ohlc_data_packer.py
--rw-rw-rw-   0        0        0     1469 2023-12-08 03:21:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/market/query_param_data_packer.py
--rw-rw-rw-   0        0        0     3169 2023-12-05 09:29:29.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/market/save_ohlc_list_param_data_packer.py
--rw-rw-rw-   0        0        0     2836 2023-12-11 02:53:40.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/market/save_tick_list_param_data_packer.py
--rw-rw-rw-   0        0        0      569 2023-11-03 01:25:37.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/market/sub_ohlc_param_data_packer.py
--rw-rw-rw-   0        0        0     1075 2023-12-08 03:22:23.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/market/tick_data_packer.py
--rw-rw-rw-   0        0        0      818 2023-12-08 03:27:23.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/message_data_packer.py
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.380462 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/
--rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/__init__.py
--rw-rw-rw-   0        0        0     2549 2023-11-03 01:32:06.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/account_data_packer.py
--rw-rw-rw-   0        0        0      454 2023-11-03 01:32:02.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/get_account_param_data_packer.py
--rw-rw-rw-   0        0        0      705 2023-12-08 03:32:09.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/get_orders_param_data_packer.py
--rw-rw-rw-   0        0        0      857 2023-12-08 03:36:52.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/get_positions_param_data_packer.py
--rw-rw-rw-   0        0        0      725 2023-12-08 03:37:41.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/get_tradeorders_param_data_packer.py
--rw-rw-rw-   0        0        0     3715 2023-11-03 01:31:46.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/order_data_packer.py
--rw-rw-rw-   0        0        0     6190 2023-11-03 01:31:43.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/position_data_packer.py
--rw-rw-rw-   0        0        0      774 2023-12-08 03:32:09.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/read_history_order_param_data_packer.py
--rw-rw-rw-   0        0        0      794 2023-12-08 03:37:41.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/read_history_tradeorder_param_data_packer.py
--rw-rw-rw-   0        0        0      367 2023-12-08 03:26:57.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/trade_param_data_packer.py
--rw-rw-rw-   0        0        0     1855 2023-11-03 01:31:26.000000 rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/tradeorder_data_packer.py
--rw-rw-rw-   0        0        0     5065 2023-12-08 06:33:22.000000 rcquant_sdk-0.0.8/rcquant_sdk/tsocket.py
-drwxrwxrwx   0        0        0        0 2023-12-11 06:18:53.203935 rcquant_sdk-0.0.8/rcquant_sdk.egg-info/
--rw-rw-rw-   0        0        0      392 2023-12-11 06:18:53.000000 rcquant_sdk-0.0.8/rcquant_sdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4438 2023-12-11 06:18:53.000000 rcquant_sdk-0.0.8/rcquant_sdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-11 06:18:53.000000 rcquant_sdk-0.0.8/rcquant_sdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-12-11 06:18:53.000000 rcquant_sdk-0.0.8/rcquant_sdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-12-11 06:18:53.000000 rcquant_sdk-0.0.8/rcquant_sdk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-11 06:18:53.383454 rcquant_sdk-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      532 2023-12-11 06:18:49.000000 rcquant_sdk-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.415472 rcquant_sdk-0.0.9/
+-rw-rw-rw-   0        0        0      392 2023-12-11 08:34:04.414475 rcquant_sdk-0.0.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.213014 rcquant_sdk-0.0.9/rcquant_sdk/
+-rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/__init__.py
+-rw-rw-rw-   0        0        0    25163 2023-12-11 06:48:24.000000 rcquant_sdk-0.0.9/rcquant_sdk/api.py
+-rw-rw-rw-   0        0        0     2430 2023-12-07 03:15:22.000000 rcquant_sdk-0.0.9/rcquant_sdk/client.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.228971 rcquant_sdk-0.0.9/rcquant_sdk/data/
+-rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.260885 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/
+-rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/__init__.py
+-rw-rw-rw-   0        0        0     6128 2023-12-08 08:23:00.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/bar_graph_param_data.py
+-rw-rw-rw-   0        0        0     6408 2023-12-08 06:34:11.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/chart_init_param_data.py
+-rw-rw-rw-   0        0        0     6940 2023-12-08 08:29:12.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/financial_graph_param_data.py
+-rw-rw-rw-   0        0        0     1065 2023-12-08 06:34:44.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/graph_value_data.py
+-rw-rw-rw-   0        0        0      565 2023-12-08 06:34:59.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/graph_value_list_data.py
+-rw-rw-rw-   0        0        0     3620 2023-12-08 06:35:17.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/legend_item_param_data.py
+-rw-rw-rw-   0        0        0     4728 2023-12-08 06:35:34.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/line_graph_param_data.py
+-rw-rw-rw-   0        0        0     4500 2023-12-08 06:35:49.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/marker_graph_param_data.py
+-rw-rw-rw-   0        0        0      697 2023-12-08 06:36:02.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/ohlc_value_data.py
+-rw-rw-rw-   0        0        0      566 2023-12-08 06:36:17.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/ohlc_value_list_data.py
+-rw-rw-rw-   0        0        0     3531 2023-12-08 06:36:30.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/plot_param_data.py
+-rw-rw-rw-   0        0        0     2670 2023-12-08 06:36:48.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/text_graph_param_data.py
+-rw-rw-rw-   0        0        0      686 2023-12-08 06:37:04.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/time_axis_param_data.py
+-rw-rw-rw-   0        0        0     1538 2023-12-08 06:37:26.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/time_span_gvlist_data.py
+-rw-rw-rw-   0        0        0     2400 2023-12-08 06:37:47.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/chart/value_axis_param_data.py
+-rw-rw-rw-   0        0        0      636 2023-12-08 06:33:13.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/login_data.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.281830 rcquant_sdk-0.0.9/rcquant_sdk/data/market/
+-rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/market/__init__.py
+-rw-rw-rw-   0        0        0     2238 2023-12-08 03:08:19.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/market/history_ohlc_param_data.py
+-rw-rw-rw-   0        0        0      471 2023-12-08 03:21:00.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/market/market_param_data.py
+-rw-rw-rw-   0        0        0     9867 2023-12-08 03:21:15.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/market/ohlc_data.py
+-rw-rw-rw-   0        0        0     4290 2023-12-08 03:21:34.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/market/query_param_data.py
+-rw-rw-rw-   0        0        0    10831 2023-12-11 06:49:00.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/market/save_ohlc_list_param_data.py
+-rw-rw-rw-   0        0        0     9589 2023-12-11 07:49:58.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/market/save_tick_list_param_data.py
+-rw-rw-rw-   0        0        0     1181 2023-12-08 03:22:13.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/market/sub_ohlc_param_data.py
+-rw-rw-rw-   0        0        0     2893 2023-12-08 03:22:23.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/market/tick_data.py
+-rw-rw-rw-   0        0        0     1996 2023-12-08 06:33:23.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/message_data.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.304768 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/
+-rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/__init__.py
+-rw-rw-rw-   0        0        0     7875 2023-12-08 03:30:19.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/account_data.py
+-rw-rw-rw-   0        0        0      744 2023-12-08 03:30:48.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/get_account_param_data.py
+-rw-rw-rw-   0        0        0      768 2023-12-08 03:32:09.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/get_orders_param_data.py
+-rw-rw-rw-   0        0        0     1289 2023-12-08 03:36:52.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/get_positions_param_data.py
+-rw-rw-rw-   0        0        0      813 2023-12-08 03:37:41.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/get_tradeorders_param_data.py
+-rw-rw-rw-   0        0        0    11917 2023-12-08 03:36:28.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/order_data.py
+-rw-rw-rw-   0        0        0    20702 2023-12-08 06:15:42.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/position_data.py
+-rw-rw-rw-   0        0        0     1045 2023-12-08 06:16:01.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/read_history_order_param_data.py
+-rw-rw-rw-   0        0        0     1090 2023-12-08 06:16:21.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/read_history_tradeorder_param_data.py
+-rw-rw-rw-   0        0        0      458 2023-12-08 03:37:59.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/trade_param_data.py
+-rw-rw-rw-   0        0        0     5541 2023-12-08 06:18:05.000000 rcquant_sdk-0.0.9/rcquant_sdk/data/trade/tradeorder_data.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.314741 rcquant_sdk-0.0.9/rcquant_sdk/handle/
+-rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/handle/__init__.py
+-rw-rw-rw-   0        0        0     1906 2023-12-08 06:33:22.000000 rcquant_sdk-0.0.9/rcquant_sdk/handle/base_handle.py
+-rw-rw-rw-   0        0        0     5064 2023-12-08 06:33:22.000000 rcquant_sdk-0.0.9/rcquant_sdk/handle/chart_handle.py
+-rw-rw-rw-   0        0        0     7115 2023-12-11 07:12:28.000000 rcquant_sdk-0.0.9/rcquant_sdk/handle/market_handle.py
+-rw-rw-rw-   0        0        0     1664 2023-12-08 06:33:22.000000 rcquant_sdk-0.0.9/rcquant_sdk/handle/req_rsp.py
+-rw-rw-rw-   0        0        0     8337 2023-12-08 06:33:22.000000 rcquant_sdk-0.0.9/rcquant_sdk/handle/trade_handle.py
+-rw-rw-rw-   0        0        0     2772 2023-12-11 02:55:39.000000 rcquant_sdk-0.0.9/rcquant_sdk/interface.py
+-rw-rw-rw-   0        0        0      728 2023-12-08 03:37:41.000000 rcquant_sdk-0.0.9/rcquant_sdk/listener.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.321723 rcquant_sdk-0.0.9/rcquant_sdk/packer/
+-rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.361617 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/
+-rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/__init__.py
+-rw-rw-rw-   0        0        0     1563 2023-12-07 01:20:17.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/bar_graph_param_data_packer.py
+-rw-rw-rw-   0        0        0     2727 2023-11-15 01:07:43.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/chart_init_param_data_packer.py
+-rw-rw-rw-   0        0        0     1718 2023-12-08 06:34:30.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/financial_graph_param_data_packer.py
+-rw-rw-rw-   0        0        0      551 2023-11-03 01:33:17.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/graph_value_data_packer.py
+-rw-rw-rw-   0        0        0      457 2023-11-03 01:33:13.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/graph_value_list_data_packer.py
+-rw-rw-rw-   0        0        0     1349 2023-11-13 03:19:22.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/legend_item_param_data_packer.py
+-rw-rw-rw-   0        0        0     1560 2023-11-03 01:33:06.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/line_graph_param_data_packer.py
+-rw-rw-rw-   0        0        0     1548 2023-11-03 01:33:02.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/marker_graph_param_data_packer.py
+-rw-rw-rw-   0        0        0      440 2023-11-03 01:32:58.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/ohlc_value_data_packer.py
+-rw-rw-rw-   0        0        0      464 2023-11-03 01:32:54.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/ohlc_value_list_data_packer.py
+-rw-rw-rw-   0        0        0     1253 2023-11-03 01:32:49.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/plot_param_data_packer.py
+-rw-rw-rw-   0        0        0     1049 2023-11-03 01:32:46.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/text_graph_param_data_packer.py
+-rw-rw-rw-   0        0        0      432 2023-11-03 01:32:42.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/time_axis_param_data_packer.py
+-rw-rw-rw-   0        0        0      512 2023-11-15 01:07:27.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/time_span_gvlist_data_packer.py
+-rw-rw-rw-   0        0        0      957 2023-12-08 06:37:48.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/value_axis_param_data_packer.py
+-rw-rw-rw-   0        0        0      417 2023-12-08 03:27:12.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/login_data_packer.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.382561 rcquant_sdk-0.0.9/rcquant_sdk/packer/market/
+-rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/market/__init__.py
+-rw-rw-rw-   0        0        0      783 2023-11-13 03:15:26.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/market/history_ohlc_param_data_packer.py
+-rw-rw-rw-   0        0        0      370 2023-12-08 03:21:01.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/market/market_param_data_packer.py
+-rw-rw-rw-   0        0        0     3086 2023-11-03 01:25:29.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/market/ohlc_data_packer.py
+-rw-rw-rw-   0        0        0     1469 2023-12-08 03:21:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/market/query_param_data_packer.py
+-rw-rw-rw-   0        0        0     3340 2023-12-11 07:17:14.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/market/save_ohlc_list_param_data_packer.py
+-rw-rw-rw-   0        0        0     3035 2023-12-11 07:34:34.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/market/save_tick_list_param_data_packer.py
+-rw-rw-rw-   0        0        0      569 2023-11-03 01:25:37.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/market/sub_ohlc_param_data_packer.py
+-rw-rw-rw-   0        0        0     1075 2023-12-08 03:22:23.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/market/tick_data_packer.py
+-rw-rw-rw-   0        0        0      818 2023-12-08 03:27:23.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/message_data_packer.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.412481 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/
+-rw-rw-rw-   0        0        0        0 2023-11-03 06:37:35.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/__init__.py
+-rw-rw-rw-   0        0        0     2549 2023-11-03 01:32:06.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/account_data_packer.py
+-rw-rw-rw-   0        0        0      454 2023-11-03 01:32:02.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/get_account_param_data_packer.py
+-rw-rw-rw-   0        0        0      705 2023-12-08 03:32:09.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/get_orders_param_data_packer.py
+-rw-rw-rw-   0        0        0      857 2023-12-08 03:36:52.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/get_positions_param_data_packer.py
+-rw-rw-rw-   0        0        0      725 2023-12-08 03:37:41.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/get_tradeorders_param_data_packer.py
+-rw-rw-rw-   0        0        0     3715 2023-11-03 01:31:46.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/order_data_packer.py
+-rw-rw-rw-   0        0        0     6190 2023-11-03 01:31:43.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/position_data_packer.py
+-rw-rw-rw-   0        0        0      774 2023-12-08 03:32:09.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/read_history_order_param_data_packer.py
+-rw-rw-rw-   0        0        0      794 2023-12-08 03:37:41.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/read_history_tradeorder_param_data_packer.py
+-rw-rw-rw-   0        0        0      367 2023-12-08 03:26:57.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/trade_param_data_packer.py
+-rw-rw-rw-   0        0        0     1855 2023-11-03 01:31:26.000000 rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/tradeorder_data_packer.py
+-rw-rw-rw-   0        0        0     5065 2023-12-08 06:33:22.000000 rcquant_sdk-0.0.9/rcquant_sdk/tsocket.py
+drwxrwxrwx   0        0        0        0 2023-12-11 08:34:04.223984 rcquant_sdk-0.0.9/rcquant_sdk.egg-info/
+-rw-rw-rw-   0        0        0      392 2023-12-11 08:34:04.000000 rcquant_sdk-0.0.9/rcquant_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4438 2023-12-11 08:34:04.000000 rcquant_sdk-0.0.9/rcquant_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-11 08:34:04.000000 rcquant_sdk-0.0.9/rcquant_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-12-11 08:34:04.000000 rcquant_sdk-0.0.9/rcquant_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-12-11 08:34:04.000000 rcquant_sdk-0.0.9/rcquant_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-11 08:34:04.415472 rcquant_sdk-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      532 2023-12-11 08:33:54.000000 rcquant_sdk-0.0.9/setup.py
```

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/api.py` & `rcquant_sdk-0.0.9/rcquant_sdk/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,16 +324,16 @@
 
 def save_ohlc_list(
     market_name: str = '',
     exchange_id: str = '',
     instrument_id: str = '',
     range: int = 60,
     trading_day: str = '',
-    action_day: str = '',
     pre_settlement_price: float = 0.0,
+    action_day_list: List[str] = [],
     action_timespan_list: List[int] = [],
     trading_time_list: List[str] = [],
     start_time_list: List[str] = [],
     end_time_list: List[str] = [],
     total_turnover_list: List[float] = [],
     open_interest_list: List[float] = [],
     open_price_list: List[float] = [],
@@ -361,16 +361,16 @@
 
     Args:
         market_name (str, optional): 行情名称. Defaults to ''.
         exchange_id (str, optional): 交易所编码. Defaults to ''.
         instrument_id (str, optional): 合约编码. Defaults to ''.
         range (int, optional): 周期. Defaults to 60.
         trading_day (str, optional): 交易日. Defaults to ''.
-        action_day (str, optional): 自然日. Defaults to ''.
         pre_settlement_price (float, optional): 昨结算价. Defaults to 0.0.
+        action_day_list (List[str], optional): 自然日. Defaults to ''.
         action_timespan_list (List[int], optional): 自然日时间戳. Defaults to [].
         trading_time_list (List[str], optional): 交易时间. Defaults to [].
         start_time_list (List[str], optional): 开始时间. Defaults to [].
         end_time_list (List[str], optional): 结束时间. Defaults to [].
         total_turnover_list (List[float], optional): 成交金额. Defaults to [].
         open_interest_list (List[float], optional): 持仓量. Defaults to [].
         open_price_list (List[float], optional): 开盘价. Defaults to [].
@@ -399,15 +399,15 @@
     """
     return FinClient.instance().market_handle().save_ohlc_list(
         SaveOHLCListParamData(market_name=market_name,
                               exchange_id=exchange_id,
                               instrument_id=instrument_id,
                               range=range,
                               trading_day=trading_day,
-                              action_day=action_day,
+                              action_day_list=action_day_list,
                               pre_settlement_price=pre_settlement_price,
                               action_timespan_list=action_timespan_list,
                               trading_time_list=trading_time_list,
                               start_time_list=start_time_list,
                               end_time_list=end_time_list,
                               total_turnover_list=total_turnover_list,
                               open_interest_list=open_interest_list,
```

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/client.py` & `rcquant_sdk-0.0.9/rcquant_sdk/client.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/bar_graph_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/bar_graph_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/chart_init_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/chart_init_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/financial_graph_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/financial_graph_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/graph_value_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/graph_value_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/graph_value_list_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/graph_value_list_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/legend_item_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/legend_item_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/line_graph_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/line_graph_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/marker_graph_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/marker_graph_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/ohlc_value_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/ohlc_value_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/ohlc_value_list_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/ohlc_value_list_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/plot_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/plot_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/text_graph_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/text_graph_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/time_axis_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/time_axis_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/time_span_gvlist_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/time_span_gvlist_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/chart/value_axis_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/chart/value_axis_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/login_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/login_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/market/history_ohlc_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/market/history_ohlc_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/market/ohlc_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/market/ohlc_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/market/query_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/market/query_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/market/save_ohlc_list_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/market/save_ohlc_list_param_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                  ):
         super().__init__(SaveOHLCListParamDataPacker(self))
         self._MarketName: str = market_name
         self._ExchangeID: str = exchange_id
         self._InstrumentID: str = instrument_id
         self._Range: int = range
         self._TradingDay: str = trading_day
-        self._ActionDayList: str = action_day_list
+        self._ActionDayList: List[str] = action_day_list
         self._PreSettlementPrice: float = pre_settlement_price
         self._ActionTimespanList: List[int] = action_timespan_list
         self._TradingTimeList: List[str] = trading_time_list
         self._StartTimeList: List[str] = start_time_list
         self._EndTimeList: List[str] = end_time_list
         self._TotalTurnoverList: List[float] = total_turnover_list
         self._OpenInterestList: List[float] = open_interest_list
@@ -113,15 +113,15 @@
         self._TradingDay = value
 
     @property
     def ActionDayList(self):
         return self._ActionDayList
 
     @ActionDayList.setter
-    def ActionDay(self, value: List[str]):
+    def ActionDayList(self, value: List[str]):
         self._ActionDayList = value
 
     @property
     def PreSettlementPrice(self):
         return self._PreSettlementPrice
 
     @PreSettlementPrice.setter
```

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/market/save_tick_list_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/market/save_tick_list_param_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import List
 from ...interface import IData
 from ...packer.market.save_tick_list_param_data_packer import SaveTickListParamDataPacker
 
 
 class SaveTickListParamData(IData):
+    _PreClosePrice: float = -1.0
+
     def __init__(self,
                  market_name: str = '',
                  exchange_id: str = '',
                  instrument_id: str = '',
                  product_id: str = '',
                  trading_day: str = '',
-                 pre_close_price: float = float("NaN"),
-                 pre_settlement_price: float = float("NaN"),
-                 pre_open_interest: float = float("NaN"),
-                 upper_limit_price: float = float("NaN"),
-                 lower_limit_price: float = float("NaN"),
+                 pre_close_price: float = -1.0,
+                 pre_settlement_price: float = -1.0,
+                 pre_open_interest: float = -1.0,
+                 upper_limit_price: float = -1.0,
+                 lower_limit_price: float = -1.0,
                  action_day_list: List[str] = [],
                  trading_time_list: List[str] = [],
                  update_mill_sec_list: List[int] = [],
                  local_time_list: List[int] = [],
                  last_price_list: List[float] = [],
                  last_volume_list: List[int] = [],
                  bid_price_list: List[float] = [],
@@ -38,39 +40,39 @@
                  ):
         super().__init__(SaveTickListParamDataPacker(self))
         self._MarketName: str = market_name
         self._ExchangeID: str = exchange_id
         self._InstrumentID: str = instrument_id
         self._ProductID: str = product_id
         self._TradingDay: str = trading_day
-        self._PreClosePrice: float = pre_close_price,
-        self._PreSettlementPrice: float = pre_settlement_price,
-        self._PreOpenInterest: float = pre_open_interest,
-        self._UpperLimitPrice: float = upper_limit_price,
-        self._LowerLimitPrice: float = lower_limit_price,
-        self._ActionDayList: List[str] = action_day_list,
-        self._TradingTimeList: List[str] = trading_time_list,
-        self._UpdateMillSecList: List[int] = update_mill_sec_list,
-        self._LocalTimeList: List[int] = local_time_list,
-        self._LastPriceList: List[float] = last_price_list,
-        self._LastVolumeList: List[int] = last_volume_list,
-        self._BidPriceList: List[float] = bid_price_list,
-        self._BidVolumeList: List[int] = bid_volume_list,
-        self._AskPriceList: List[float] = ask_price_list,
-        self._AskVolumeList: List[int] = ask_volume_list,
-        self._AvgPriceList: List[float] = avg_price_list,
-        self._OpenPriceList: List[float] = open_price_list,
-        self._HighPriceList: List[float] = high_price_list,
-        self._LowerPriceList: List[float] = lower_price_list,
-        self._TotalTurnoverList: List[float] = total_turnover_list,
-        self._TotalVolumeList: List[int] = total_volume_list,
-        self._OpenInterestList: List[float] = open_interest_list,
-        self._ClosePriceList: List[float] = close_price_list,
-        self._SettlementPriceList: List[float] = settlement_price_list,
-        self._TotalValueList: List[float] = total_value_list,
+        self._PreClosePrice: float = float(pre_close_price)
+        self._PreSettlementPrice: float = pre_settlement_price
+        self._PreOpenInterest: float = pre_open_interest
+        self._UpperLimitPrice: float = upper_limit_price
+        self._LowerLimitPrice: float = lower_limit_price
+        self._ActionDayList: List[str] = action_day_list
+        self._TradingTimeList: List[str] = trading_time_list
+        self._UpdateMillSecList: List[int] = update_mill_sec_list
+        self._LocalTimeList: List[int] = local_time_list
+        self._LastPriceList: List[float] = last_price_list
+        self._LastVolumeList: List[int] = last_volume_list
+        self._BidPriceList: List[float] = bid_price_list
+        self._BidVolumeList: List[int] = bid_volume_list
+        self._AskPriceList: List[float] = ask_price_list
+        self._AskVolumeList: List[int] = ask_volume_list
+        self._AvgPriceList: List[float] = avg_price_list
+        self._OpenPriceList: List[float] = open_price_list
+        self._HighPriceList: List[float] = high_price_list
+        self._LowerPriceList: List[float] = lower_price_list
+        self._TotalTurnoverList: List[float] = total_turnover_list
+        self._TotalVolumeList: List[int] = total_volume_list
+        self._OpenInterestList: List[float] = open_interest_list
+        self._ClosePriceList: List[float] = close_price_list
+        self._SettlementPriceList: List[float] = settlement_price_list
+        self._TotalValueList: List[float] = total_value_list
 
     @property
     def MarketName(self):
         return self._MarketName
 
     @MarketName.setter
     def MarketName(self, value: str):
@@ -230,22 +232,14 @@
 
     @property
     def AvgPriceList(self):
         return self._AvgPriceList
 
     @AvgPriceList.setter
     def AvgPriceList(self, value: List[float]):
-        self._AvgPriceList = value
-
-    @property
-    def AvgPriceList(self):
-        return self._AvgPriceList
-
-    @AvgPriceList.setter
-    def AvgPriceList(self, value: List[float]):
         self._AvgPriceList = value
 
     @property
     def OpenPriceList(self):
         return self._OpenPriceList
 
     @OpenPriceList.setter
```

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/market/sub_ohlc_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/market/sub_ohlc_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/market/tick_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/market/tick_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/message_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/message_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/trade/account_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/trade/account_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/trade/get_account_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/trade/get_account_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/trade/get_orders_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/trade/get_orders_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/trade/get_positions_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/trade/get_positions_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/trade/get_tradeorders_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/trade/get_tradeorders_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/trade/order_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/trade/order_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/trade/position_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/trade/position_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/trade/read_history_order_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/trade/read_history_order_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/trade/read_history_tradeorder_param_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/trade/read_history_tradeorder_param_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/data/trade/tradeorder_data.py` & `rcquant_sdk-0.0.9/rcquant_sdk/data/trade/tradeorder_data.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/handle/base_handle.py` & `rcquant_sdk-0.0.9/rcquant_sdk/handle/base_handle.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/handle/chart_handle.py` & `rcquant_sdk-0.0.9/rcquant_sdk/handle/chart_handle.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/handle/market_handle.py` & `rcquant_sdk-0.0.9/rcquant_sdk/handle/market_handle.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     def subscribe_ohlc(self, params: SubOHLCParamData) -> Tuple[bool, str]:
         return self.__wait_send_msg(int(MsgID.MSGID_Market_SubOHLC.value), params)
 
     def save_ohlc_list(self, params: SaveOHLCListParamData) -> Tuple[bool, str]:
         return self.__wait_send_msg(int(MsgID.MSGID_Market_SaveOHLCList.value), params)
 
     def save_tick_list(self, params: SaveTickListParamData) -> Tuple[bool, str]:
-        return self.__wait_send_msg(int(MsgID.MSGID_Market_SaveOHLCList.value), params)
+        return self.__wait_send_msg(int(MsgID.MSGID_Market_SaveTickList.value), params)
 
     def get_history_ohlc(self, params: HistoryOHLCParamData) -> Tuple[bool, str, pd.DataFrame]:
         self.__ReqID = self.__ReqID + 1
         mid = int(MsgID.MSGID_Market_GetHistoryOHLC.value)
         msg = MessageData(mid=mid, request_id=self.__ReqID)
         if params is not None:
             msg.UData = params.pack()
```

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/handle/req_rsp.py` & `rcquant_sdk-0.0.9/rcquant_sdk/handle/req_rsp.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/handle/trade_handle.py` & `rcquant_sdk-0.0.9/rcquant_sdk/handle/trade_handle.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/interface.py` & `rcquant_sdk-0.0.9/rcquant_sdk/interface.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/listener.py` & `rcquant_sdk-0.0.9/rcquant_sdk/listener.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/bar_graph_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/bar_graph_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/chart_init_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/chart_init_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/financial_graph_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/financial_graph_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/graph_value_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/graph_value_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/legend_item_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/legend_item_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/line_graph_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/line_graph_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/marker_graph_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/marker_graph_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/plot_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/plot_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/text_graph_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/text_graph_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/time_span_gvlist_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/time_span_gvlist_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/chart/value_axis_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/chart/value_axis_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/market/history_ohlc_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/market/history_ohlc_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/market/ohlc_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/market/ohlc_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/market/query_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/market/query_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/market/sub_ohlc_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/market/sub_ohlc_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/market/tick_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/market/tick_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/message_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/message_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/account_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/account_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/get_orders_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/get_orders_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/get_positions_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/get_positions_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/get_tradeorders_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/get_tradeorders_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/order_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/order_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/position_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/position_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/read_history_order_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/read_history_order_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/read_history_tradeorder_param_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/read_history_tradeorder_param_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/packer/trade/tradeorder_data_packer.py` & `rcquant_sdk-0.0.9/rcquant_sdk/packer/trade/tradeorder_data_packer.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk/tsocket.py` & `rcquant_sdk-0.0.9/rcquant_sdk/tsocket.py`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/rcquant_sdk.egg-info/SOURCES.txt` & `rcquant_sdk-0.0.9/rcquant_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rcquant_sdk-0.0.8/setup.py` & `rcquant_sdk-0.0.9/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='rcquant_sdk',
-    version='0.0.8',
+    version='0.0.9',
     description='rcquant_sdk',
     author='rcquant_sdk',
     author_email='rcquant_sdk@example.com',
     packages=find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
```

