# Comparing `tmp/pfund-0.0.1.dev4.tar.gz` & `tmp/pfund-0.0.1.dev5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pfund-0.0.1.dev4.tar", max compression
+gzip compressed data, was "pfund-0.0.1.dev5.tar", max compression
```

## Comparing `pfund-0.0.1.dev4.tar` & `pfund-0.0.1.dev5.tar`

### file list

```diff
@@ -1,161 +1,162 @@
--rw-r--r--   0        0        0    11355 2024-02-06 15:08:56.890856 pfund-0.0.1.dev4/LICENSE
--rw-r--r--   0        0        0     9476 2024-02-13 05:03:20.861745 pfund-0.0.1.dev4/README.md
--rw-r--r--   0        0        0      705 2024-02-14 05:41:12.484556 pfund-0.0.1.dev4/pfund/__init__.py
--rw-r--r--   0        0        0      155 2024-01-30 15:01:45.803425 pfund-0.0.1.dev4/pfund/accounts/__init__.py
--rw-r--r--   0        0        0      743 2024-01-30 15:01:45.806625 pfund-0.0.1.dev4/pfund/accounts/account_base.py
--rw-r--r--   0        0        0     1000 2024-01-30 15:01:45.807227 pfund-0.0.1.dev4/pfund/accounts/account_crypto.py
--rw-r--r--   0        0        0      615 2024-01-30 15:01:45.809008 pfund-0.0.1.dev4/pfund/accounts/account_ib.py
--rw-r--r--   0        0        0     2591 2024-02-05 14:53:21.585823 pfund-0.0.1.dev4/pfund/adapter.py
--rw-r--r--   0        0        0      156 2024-01-30 15:01:45.809984 pfund-0.0.1.dev4/pfund/balances/__init__.py
--rw-r--r--   0        0        0     1390 2024-01-30 15:01:45.811449 pfund-0.0.1.dev4/pfund/balances/balance_base.py
--rw-r--r--   0        0        0      449 2024-01-30 15:01:45.811748 pfund-0.0.1.dev4/pfund/balances/balance_crypto.py
--rw-r--r--   0        0        0      953 2024-01-30 15:01:45.812044 pfund-0.0.1.dev4/pfund/balances/balance_ib.py
--rw-r--r--   0        0        0      149 2024-01-30 15:01:45.812406 pfund-0.0.1.dev4/pfund/brokers/__init__.py
--rw-r--r--   0        0        0     3114 2024-01-30 15:01:45.815600 pfund-0.0.1.dev4/pfund/brokers/broker_backtest.py
--rw-r--r--   0        0        0      609 2024-02-04 14:35:55.856380 pfund-0.0.1.dev4/pfund/brokers/broker_base.py
--rw-r--r--   0        0        0    13203 2024-01-30 15:01:45.816495 pfund-0.0.1.dev4/pfund/brokers/broker_crypto.py
--rw-r--r--   0        0        0     3793 2024-02-04 14:36:28.703645 pfund-0.0.1.dev4/pfund/brokers/broker_live.py
--rw-r--r--   0        0        0       41 2024-01-30 15:01:45.817494 pfund-0.0.1.dev4/pfund/brokers/ib/__init__.py
--rw-r--r--   0        0        0    10473 2024-01-30 15:01:45.821478 pfund-0.0.1.dev4/pfund/brokers/ib/broker_ib.py
--rw-r--r--   0        0        0    12505 2024-01-30 15:01:45.821940 pfund-0.0.1.dev4/pfund/brokers/ib/ib_api.py
--rw-r--r--   0        0        0     5565 2024-01-30 15:01:45.822316 pfund-0.0.1.dev4/pfund/brokers/ib/ib_client.py
--rw-r--r--   0        0        0     9434 2024-01-30 15:01:45.822738 pfund-0.0.1.dev4/pfund/brokers/ib/ib_wrapper.py
--rw-r--r--   0        0        0       66 2024-02-09 08:16:05.819131 pfund-0.0.1.dev4/pfund/cli/__init__.py
--rw-r--r--   0        0        0        0 2024-02-09 08:11:30.211353 pfund-0.0.1.dev4/pfund/cli/commands/__init__.py
--rw-r--r--   0        0        0     2844 2024-02-14 08:43:49.332041 pfund-0.0.1.dev4/pfund/cli/commands/config.py
--rw-r--r--   0        0        0     1306 2024-02-14 06:30:45.658614 pfund-0.0.1.dev4/pfund/cli/commands/docker_compose.py
--rw-r--r--   0        0        0      482 2024-02-14 07:33:56.424587 pfund-0.0.1.dev4/pfund/cli/main.py
--rw-r--r--   0        0        0     1965 2024-01-30 15:01:45.824055 pfund-0.0.1.dev4/pfund/config/bybit/config.yml
--rw-r--r--   0        0        0      213 2024-01-30 15:01:45.824270 pfund-0.0.1.dev4/pfund/config/bybit/lot_sizes_inverse.yml
--rw-r--r--   0        0        0     6131 2024-01-30 15:01:45.824581 pfund-0.0.1.dev4/pfund/config/bybit/lot_sizes_linear.yml
--rw-r--r--   0        0        0    13804 2024-01-30 15:01:45.824913 pfund-0.0.1.dev4/pfund/config/bybit/lot_sizes_option.yml
--rw-r--r--   0        0        0    10101 2024-01-30 15:01:45.825238 pfund-0.0.1.dev4/pfund/config/bybit/lot_sizes_spot.yml
--rw-r--r--   0        0        0      178 2024-01-30 15:01:45.825531 pfund-0.0.1.dev4/pfund/config/bybit/pdt_matchings_inverse.yml
--rw-r--r--   0        0        0     6765 2024-01-30 15:01:45.825785 pfund-0.0.1.dev4/pfund/config/bybit/pdt_matchings_linear.yml
--rw-r--r--   0        0        0        3 2024-01-30 15:01:45.826011 pfund-0.0.1.dev4/pfund/config/bybit/pdt_matchings_option.yml
--rw-r--r--   0        0        0    10720 2024-01-30 15:01:45.826379 pfund-0.0.1.dev4/pfund/config/bybit/pdt_matchings_spot.yml
--rw-r--r--   0        0        0      257 2024-01-30 15:01:45.826793 pfund-0.0.1.dev4/pfund/config/bybit/tick_sizes_inverse.yml
--rw-r--r--   0        0        0     7181 2024-01-30 15:01:45.827089 pfund-0.0.1.dev4/pfund/config/bybit/tick_sizes_linear.yml
--rw-r--r--   0        0        0    12304 2024-01-30 15:01:45.827403 pfund-0.0.1.dev4/pfund/config/bybit/tick_sizes_option.yml
--rw-r--r--   0        0        0    11241 2024-01-30 15:01:45.827703 pfund-0.0.1.dev4/pfund/config/bybit/tick_sizes_spot.yml
--rw-r--r--   0        0        0     2204 2024-02-08 09:02:40.122820 pfund-0.0.1.dev4/pfund/config/configuration.py
--rw-r--r--   0        0        0      563 2024-01-30 15:01:45.828458 pfund-0.0.1.dev4/pfund/config/ib/config.yml
--rw-r--r--   0        0        0     2810 2024-02-04 11:34:42.470879 pfund-0.0.1.dev4/pfund/config/logging.yml
--rw-r--r--   0        0        0     4115 2024-02-14 07:29:39.297812 pfund-0.0.1.dev4/pfund/config_handler.py
--rw-r--r--   0        0        0       65 2024-01-30 15:01:45.829160 pfund-0.0.1.dev4/pfund/const/__init__.py
--rw-r--r--   0        0        0     1686 2024-01-30 15:01:45.830903 pfund-0.0.1.dev4/pfund/const/_zmq_routes.py
--rw-r--r--   0        0        0      941 2024-01-30 15:01:45.831102 pfund-0.0.1.dev4/pfund/const/commons.py
--rw-r--r--   0        0        0      724 2024-02-14 07:53:14.358697 pfund-0.0.1.dev4/pfund/const/paths.py
--rw-r--r--   0        0        0     1705 2024-01-30 15:01:45.832828 pfund-0.0.1.dev4/pfund/data_tools/data_tool_base.py
--rw-r--r--   0        0        0     9285 2024-01-30 15:01:45.833140 pfund-0.0.1.dev4/pfund/data_tools/data_tool_pandas.py
--rw-r--r--   0        0        0      171 2024-01-30 15:01:45.833717 pfund-0.0.1.dev4/pfund/datas/__init__.py
--rw-r--r--   0        0        0     6716 2024-01-30 15:01:45.838564 pfund-0.0.1.dev4/pfund/datas/data_bar.py
--rw-r--r--   0        0        0      480 2024-01-30 15:01:45.838818 pfund-0.0.1.dev4/pfund/datas/data_base.py
--rw-r--r--   0        0        0     1455 2024-01-30 15:01:45.839101 pfund-0.0.1.dev4/pfund/datas/data_quote.py
--rw-r--r--   0        0        0     1291 2024-01-30 15:01:45.839333 pfund-0.0.1.dev4/pfund/datas/data_tick.py
--rw-r--r--   0        0        0     1845 2024-01-30 15:01:45.839539 pfund-0.0.1.dev4/pfund/datas/data_time_based.py
--rw-r--r--   0        0        0     2978 2024-01-30 15:01:45.839747 pfund-0.0.1.dev4/pfund/datas/resolution.py
--rw-r--r--   0        0        0     1647 2024-01-30 15:01:45.839977 pfund-0.0.1.dev4/pfund/datas/timeframe.py
--rw-r--r--   0        0        0      207 2024-01-30 15:01:45.840501 pfund-0.0.1.dev4/pfund/engines/__init__.py
--rw-r--r--   0        0        0     7474 2024-02-14 08:06:20.800883 pfund-0.0.1.dev4/pfund/engines/backtest_engine.py
--rw-r--r--   0        0        0     3966 2024-02-14 09:55:46.614176 pfund-0.0.1.dev4/pfund/engines/base_engine.py
--rw-r--r--   0        0        0      602 2024-02-05 14:57:27.586210 pfund-0.0.1.dev4/pfund/engines/test_engine.py
--rw-r--r--   0        0        0     8222 2024-02-05 14:57:55.867148 pfund-0.0.1.dev4/pfund/engines/trade_engine.py
--rw-r--r--   0        0        0      921 2024-02-05 14:58:03.193524 pfund-0.0.1.dev4/pfund/engines/train_engine.py
--rw-r--r--   0        0        0      120 2024-01-30 15:01:45.844589 pfund-0.0.1.dev4/pfund/errors.py
--rw-r--r--   0        0        0        0 2024-01-30 15:01:45.844855 pfund-0.0.1.dev4/pfund/exchanges/__init__.py
--rw-r--r--   0        0        0      258 2024-01-30 15:01:45.848467 pfund-0.0.1.dev4/pfund/exchanges/bybit/__init__.py
--rw-r--r--   0        0        0    17615 2024-02-08 05:38:48.280133 pfund-0.0.1.dev4/pfund/exchanges/bybit/exchange.py
--rw-r--r--   0        0        0    11498 2024-01-30 15:01:45.852818 pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api.py
--rw-r--r--   0        0        0     9650 2024-01-30 15:01:45.853371 pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse
--rw-r--r--   0        0        0   164823 2024-01-30 15:01:45.854380 pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear
--rw-r--r--   0        0        0   227045 2024-01-30 15:01:45.855347 pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option
--rw-r--r--   0        0        0    99033 2024-01-30 15:01:45.855940 pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot
--rw-r--r--   0        0        0    15516 2024-01-30 15:01:45.856319 pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse
--rw-r--r--   0        0        0   262316 2024-01-30 15:01:45.857183 pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear
--rw-r--r--   0        0        0   395202 2024-01-30 15:01:45.858710 pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option
--rw-r--r--   0        0        0   155302 2024-01-30 15:01:45.860232 pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot
--rw-r--r--   0        0        0       86 2024-01-30 15:01:45.861200 pfund-0.0.1.dev4/pfund/exchanges/bybit/types.py
--rw-r--r--   0        0        0    18581 2024-01-30 15:01:45.861449 pfund-0.0.1.dev4/pfund/exchanges/bybit/ws_api.py
--rw-r--r--   0        0        0    20510 2024-02-08 05:51:42.362247 pfund-0.0.1.dev4/pfund/exchanges/exchange_base.py
--rw-r--r--   0        0        0     4112 2024-01-30 15:01:45.862894 pfund-0.0.1.dev4/pfund/exchanges/rest_api_base.py
--rw-r--r--   0        0        0    26589 2024-01-30 15:01:45.865158 pfund-0.0.1.dev4/pfund/exchanges/ws_api_base.py
--rw-r--r--   0        0        0      481 2024-01-30 15:01:45.876419 pfund-0.0.1.dev4/pfund/externals/ibapi/__init__.py
--rw-r--r--   0        0        0     2027 2024-01-30 15:01:45.902207 pfund-0.0.1.dev4/pfund/externals/ibapi/account_summary_tags.py
--rw-r--r--   0        0        0   149406 2024-01-30 15:01:45.902893 pfund-0.0.1.dev4/pfund/externals/ibapi/client.py
--rw-r--r--   0        0        0     2297 2024-01-30 15:01:45.903103 pfund-0.0.1.dev4/pfund/externals/ibapi/comm.py
--rw-r--r--   0        0        0      892 2024-01-30 15:01:45.903285 pfund-0.0.1.dev4/pfund/externals/ibapi/commission_report.py
--rw-r--r--   0        0        0     7841 2024-01-30 15:01:45.903569 pfund-0.0.1.dev4/pfund/externals/ibapi/common.py
--rw-r--r--   0        0        0     3755 2024-01-30 15:01:45.903915 pfund-0.0.1.dev4/pfund/externals/ibapi/connection.py
--rw-r--r--   0        0        0     6642 2024-01-30 15:01:45.904226 pfund-0.0.1.dev4/pfund/externals/ibapi/contract.py
--rw-r--r--   0        0        0    59604 2024-01-30 15:01:45.904561 pfund-0.0.1.dev4/pfund/externals/ibapi/decoder.py
--rw-r--r--   0        0        0      520 2024-01-30 15:01:45.904809 pfund-0.0.1.dev4/pfund/externals/ibapi/enum_implem.py
--rw-r--r--   0        0        0     1635 2024-01-30 15:01:45.905010 pfund-0.0.1.dev4/pfund/externals/ibapi/errors.py
--rw-r--r--   0        0        0     2027 2024-01-30 15:01:45.905259 pfund-0.0.1.dev4/pfund/externals/ibapi/execution.py
--rw-r--r--   0        0        0     2211 2024-01-30 15:01:45.905484 pfund-0.0.1.dev4/pfund/externals/ibapi/ibapi.pyproj
--rw-r--r--   0        0        0     6366 2024-01-30 15:01:45.905865 pfund-0.0.1.dev4/pfund/externals/ibapi/message.py
--rw-r--r--   0        0        0      507 2024-01-30 15:01:45.906062 pfund-0.0.1.dev4/pfund/externals/ibapi/news.py
--rw-r--r--   0        0        0      358 2024-01-30 15:01:45.906261 pfund-0.0.1.dev4/pfund/externals/ibapi/object_implem.py
--rw-r--r--   0        0        0     9369 2024-01-30 15:01:45.906706 pfund-0.0.1.dev4/pfund/externals/ibapi/order.py
--rw-r--r--   0        0        0     8243 2024-01-30 15:01:45.907140 pfund-0.0.1.dev4/pfund/externals/ibapi/order_condition.py
--rw-r--r--   0        0        0      943 2024-01-30 15:01:45.907503 pfund-0.0.1.dev4/pfund/externals/ibapi/order_state.py
--rw-r--r--   0        0        0    19630 2024-01-30 15:01:45.907745 pfund-0.0.1.dev4/pfund/externals/ibapi/orderdecoder.py
--rw-r--r--   0        0        0     1625 2024-01-30 15:01:45.907978 pfund-0.0.1.dev4/pfund/externals/ibapi/reader.py
--rw-r--r--   0        0        0     2020 2024-01-30 15:01:45.908359 pfund-0.0.1.dev4/pfund/externals/ibapi/scanner.py
--rw-r--r--   0        0        0     5580 2024-01-30 15:01:45.908580 pfund-0.0.1.dev4/pfund/externals/ibapi/server_versions.py
--rw-r--r--   0        0        0      553 2024-01-30 15:01:45.908832 pfund-0.0.1.dev4/pfund/externals/ibapi/softdollartier.py
--rw-r--r--   0        0        0      714 2024-01-30 15:01:45.909202 pfund-0.0.1.dev4/pfund/externals/ibapi/tag_value.py
--rw-r--r--   0        0        0     3876 2024-01-30 15:01:45.909614 pfund-0.0.1.dev4/pfund/externals/ibapi/ticktype.py
--rw-r--r--   0        0        0     4130 2024-01-30 15:01:45.909848 pfund-0.0.1.dev4/pfund/externals/ibapi/utils.py
--rw-r--r--   0        0        0    31944 2024-01-30 15:01:45.910151 pfund-0.0.1.dev4/pfund/externals/ibapi/wrapper.py
--rw-r--r--   0        0        0      200 2024-01-30 15:01:45.910543 pfund-0.0.1.dev4/pfund/indicators/__init__.py
--rw-r--r--   0        0        0     2827 2024-01-30 15:01:45.914261 pfund-0.0.1.dev4/pfund/indicators/indicator_base.py
--rw-r--r--   0        0        0     4205 2024-01-30 15:01:45.915035 pfund-0.0.1.dev4/pfund/indicators/ta_indicator.py
--rw-r--r--   0        0        0     2139 2024-01-30 15:01:45.915296 pfund-0.0.1.dev4/pfund/indicators/talib_indicator.py
--rw-r--r--   0        0        0      159 2024-02-09 08:17:15.066455 pfund-0.0.1.dev4/pfund/main.py
--rw-r--r--   0        0        0      396 2024-01-30 15:01:45.921058 pfund-0.0.1.dev4/pfund/managers/__init__.py
--rw-r--r--   0        0        0      997 2024-02-04 11:33:27.199191 pfund-0.0.1.dev4/pfund/managers/base_manager.py
--rw-r--r--   0        0        0     7659 2024-01-30 15:01:45.927572 pfund-0.0.1.dev4/pfund/managers/connection_manager.py
--rw-r--r--   0        0        0    13773 2024-01-30 15:01:45.927876 pfund-0.0.1.dev4/pfund/managers/data_manager.py
--rw-r--r--   0        0        0    12813 2024-01-30 15:01:45.928588 pfund-0.0.1.dev4/pfund/managers/order_manager.py
--rw-r--r--   0        0        0     3893 2024-01-30 15:01:45.929260 pfund-0.0.1.dev4/pfund/managers/portfolio_manager.py
--rw-r--r--   0        0        0      175 2024-01-30 15:01:45.930796 pfund-0.0.1.dev4/pfund/managers/risk_manager.py
--rw-r--r--   0        0        0     8106 2024-02-04 11:33:27.188479 pfund-0.0.1.dev4/pfund/managers/strategy_manager.py
--rw-r--r--   0        0        0     7324 2024-02-14 09:38:39.166200 pfund-0.0.1.dev4/pfund/mixins/backtest.py
--rw-r--r--   0        0        0      236 2024-02-08 07:22:22.864364 pfund-0.0.1.dev4/pfund/models/__init__.py
--rw-r--r--   0        0        0     4510 2024-01-30 15:01:45.938574 pfund-0.0.1.dev4/pfund/models/model_backtest.py
--rw-r--r--   0        0        0    17953 2024-02-08 07:21:19.270141 pfund-0.0.1.dev4/pfund/models/model_base.py
--rw-r--r--   0        0        0     2032 2024-01-30 15:01:45.939214 pfund-0.0.1.dev4/pfund/models/model_meta.py
--rw-r--r--   0        0        0     2659 2024-01-30 15:01:45.939461 pfund-0.0.1.dev4/pfund/models/pytorch_model.py
--rw-r--r--   0        0        0     1188 2024-01-30 15:01:45.939751 pfund-0.0.1.dev4/pfund/models/sklearn_model.py
--rw-r--r--   0        0        0      138 2024-01-30 15:01:45.940227 pfund-0.0.1.dev4/pfund/orders/__init__.py
--rw-r--r--   0        0        0    10415 2024-01-30 15:01:45.943085 pfund-0.0.1.dev4/pfund/orders/order_base.py
--rw-r--r--   0        0        0     1531 2024-01-30 15:01:45.943516 pfund-0.0.1.dev4/pfund/orders/order_crypto.py
--rw-r--r--   0        0        0      230 2024-01-30 15:01:45.943750 pfund-0.0.1.dev4/pfund/orders/order_ib.py
--rw-r--r--   0        0        0      781 2024-01-30 15:01:45.943960 pfund-0.0.1.dev4/pfund/orders/order_statuses.py
--rw-r--r--   0        0        0      150 2024-01-30 15:01:45.944152 pfund-0.0.1.dev4/pfund/orders/order_time_in_force.py
--rw-r--r--   0        0        0     3332 2024-02-14 09:58:56.776886 pfund-0.0.1.dev4/pfund/plogging/__init__.py
--rw-r--r--   0        0        0     3269 2024-02-14 09:55:02.600095 pfund-0.0.1.dev4/pfund/plogging/config.py
--rw-r--r--   0        0        0      409 2024-01-30 15:01:45.920021 pfund-0.0.1.dev4/pfund/plogging/filters.py
--rw-r--r--   0        0        0      578 2024-01-30 15:01:45.920250 pfund-0.0.1.dev4/pfund/plogging/formatter.py
--rw-r--r--   0        0        0     1538 2024-01-30 15:01:45.920455 pfund-0.0.1.dev4/pfund/plogging/handlers.py
--rw-r--r--   0        0        0      134 2024-01-30 15:01:45.944356 pfund-0.0.1.dev4/pfund/portfolio.py
--rw-r--r--   0        0        0      165 2024-01-30 15:01:45.944846 pfund-0.0.1.dev4/pfund/positions/__init__.py
--rw-r--r--   0        0        0     1300 2024-01-30 15:01:45.950043 pfund-0.0.1.dev4/pfund/positions/position_base.py
--rw-r--r--   0        0        0     3655 2024-01-30 15:01:45.950417 pfund-0.0.1.dev4/pfund/positions/position_crypto.py
--rw-r--r--   0        0        0     2304 2024-01-30 15:01:45.950721 pfund-0.0.1.dev4/pfund/positions/position_ib.py
--rw-r--r--   0        0        0      155 2024-01-30 15:01:45.952029 pfund-0.0.1.dev4/pfund/products/__init__.py
--rw-r--r--   0        0        0     1593 2024-01-30 15:01:45.958189 pfund-0.0.1.dev4/pfund/products/product_base.py
--rw-r--r--   0        0        0     3275 2024-01-30 15:01:45.958561 pfund-0.0.1.dev4/pfund/products/product_crypto.py
--rw-r--r--   0        0        0     2334 2024-01-30 15:01:45.958836 pfund-0.0.1.dev4/pfund/products/product_ib.py
--rw-r--r--   0        0        0       71 2024-01-30 15:01:45.959095 pfund-0.0.1.dev4/pfund/risk_monitor.py
--rw-r--r--   0        0        0       82 2024-01-30 15:01:45.959597 pfund-0.0.1.dev4/pfund/strategies/__init__.py
--rw-r--r--   0        0        0     1975 2024-01-30 15:01:45.961524 pfund-0.0.1.dev4/pfund/strategies/strategy_backtest.py
--rw-r--r--   0        0        0    23624 2024-02-04 11:33:27.199250 pfund-0.0.1.dev4/pfund/strategies/strategy_base.py
--rw-r--r--   0        0        0      930 2024-01-30 15:01:45.962352 pfund-0.0.1.dev4/pfund/strategies/strategy_meta.py
--rw-r--r--   0        0        0     2335 2024-01-30 15:01:45.966041 pfund-0.0.1.dev4/pfund/utils/aliases.py
--rw-r--r--   0        0        0      591 2024-01-30 15:01:45.966245 pfund-0.0.1.dev4/pfund/utils/envs.py
--rw-r--r--   0        0        0     5166 2024-02-05 14:53:16.326926 pfund-0.0.1.dev4/pfund/utils/utils.py
--rw-r--r--   0        0        0     4033 2024-01-30 15:01:45.966936 pfund-0.0.1.dev4/pfund/zeromq.py
--rw-r--r--   0        0        0     1532 2024-02-14 14:17:56.983372 pfund-0.0.1.dev4/pyproject.toml
--rw-r--r--   0        0        0    11001 1970-01-01 00:00:00.000000 pfund-0.0.1.dev4/PKG-INFO
+-rw-r--r--   0        0        0    11355 2024-04-03 08:14:20.573937 pfund-0.0.1.dev5/LICENSE
+-rw-r--r--   0        0        0    11097 2024-04-03 08:14:20.573937 pfund-0.0.1.dev5/README.md
+-rw-r--r--   0        0        0      321 2024-04-03 08:14:20.573937 pfund-0.0.1.dev5/pfund/CONTRIBUTING.md
+-rw-r--r--   0        0        0      952 2024-04-03 08:14:20.573937 pfund-0.0.1.dev5/pfund/__init__.py
+-rw-r--r--   0        0        0      155 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/accounts/__init__.py
+-rw-r--r--   0        0        0      743 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/accounts/account_base.py
+-rw-r--r--   0        0        0     1000 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/accounts/account_crypto.py
+-rw-r--r--   0        0        0      615 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/accounts/account_ib.py
+-rw-r--r--   0        0        0     2599 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/adapter.py
+-rw-r--r--   0        0        0      156 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/balances/__init__.py
+-rw-r--r--   0        0        0     1390 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/balances/balance_base.py
+-rw-r--r--   0        0        0      449 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/balances/balance_crypto.py
+-rw-r--r--   0        0        0      953 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/balances/balance_ib.py
+-rw-r--r--   0        0        0      149 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/__init__.py
+-rw-r--r--   0        0        0     3114 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/broker_backtest.py
+-rw-r--r--   0        0        0      609 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/broker_base.py
+-rw-r--r--   0        0        0    13203 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/broker_crypto.py
+-rw-r--r--   0        0        0     3793 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/broker_live.py
+-rw-r--r--   0        0        0       41 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/ib/__init__.py
+-rw-r--r--   0        0        0    10473 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/ib/broker_ib.py
+-rw-r--r--   0        0        0    12505 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/ib/ib_api.py
+-rw-r--r--   0        0        0     5565 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/ib/ib_client.py
+-rw-r--r--   0        0        0     9434 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/brokers/ib/ib_wrapper.py
+-rw-r--r--   0        0        0       66 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/cli/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2995 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/cli/commands/config.py
+-rw-r--r--   0        0        0     1379 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/cli/commands/docker_compose.py
+-rw-r--r--   0        0        0      482 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/cli/main.py
+-rw-r--r--   0        0        0     1968 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/config.yml
+-rw-r--r--   0        0        0      213 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_inverse.yml
+-rw-r--r--   0        0        0     6131 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_linear.yml
+-rw-r--r--   0        0        0    13804 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_option.yml
+-rw-r--r--   0        0        0    10101 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_spot.yml
+-rw-r--r--   0        0        0      178 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_inverse.yml
+-rw-r--r--   0        0        0     6765 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_linear.yml
+-rw-r--r--   0        0        0        3 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_option.yml
+-rw-r--r--   0        0        0    10720 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_spot.yml
+-rw-r--r--   0        0        0      257 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_inverse.yml
+-rw-r--r--   0        0        0     7181 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_linear.yml
+-rw-r--r--   0        0        0    12304 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_option.yml
+-rw-r--r--   0        0        0    11241 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_spot.yml
+-rw-r--r--   0        0        0     2204 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/configuration.py
+-rw-r--r--   0        0        0      563 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/ib/config.yml
+-rw-r--r--   0        0        0     2810 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config/logging.yml
+-rw-r--r--   0        0        0     3957 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/config_handler.py
+-rw-r--r--   0        0        0       65 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/const/__init__.py
+-rw-r--r--   0        0        0     1686 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/const/_zmq_routes.py
+-rw-r--r--   0        0        0      941 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/const/commons.py
+-rw-r--r--   0        0        0      713 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/const/paths.py
+-rw-r--r--   0        0        0     1705 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/data_tools/data_tool_base.py
+-rw-r--r--   0        0        0     9285 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/data_tools/data_tool_pandas.py
+-rw-r--r--   0        0        0      171 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/__init__.py
+-rw-r--r--   0        0        0     6716 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/data_bar.py
+-rw-r--r--   0        0        0      480 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/data_base.py
+-rw-r--r--   0        0        0     1455 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/data_quote.py
+-rw-r--r--   0        0        0     1291 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/data_tick.py
+-rw-r--r--   0        0        0     1845 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/data_time_based.py
+-rw-r--r--   0        0        0     3105 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/resolution.py
+-rw-r--r--   0        0        0     1647 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/datas/timeframe.py
+-rw-r--r--   0        0        0      207 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/__init__.py
+-rw-r--r--   0        0        0     7993 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/backtest_engine.py
+-rw-r--r--   0        0        0     3966 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/base_engine.py
+-rw-r--r--   0        0        0      602 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/test_engine.py
+-rw-r--r--   0        0        0     8222 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/trade_engine.py
+-rw-r--r--   0        0        0      921 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/engines/train_engine.py
+-rw-r--r--   0        0        0      120 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/errors.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/__init__.py
+-rw-r--r--   0        0        0      258 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/bybit/__init__.py
+-rw-r--r--   0        0        0    17330 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/bybit/exchange.py
+-rw-r--r--   0        0        0    11498 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api.py
+-rw-r--r--   0        0        0     9650 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse
+-rw-r--r--   0        0        0   164823 2024-04-03 08:14:20.577937 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear
+-rw-r--r--   0        0        0   227045 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option
+-rw-r--r--   0        0        0    99033 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot
+-rw-r--r--   0        0        0    15516 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse
+-rw-r--r--   0        0        0   262316 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear
+-rw-r--r--   0        0        0   395202 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option
+-rw-r--r--   0        0        0   155302 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot
+-rw-r--r--   0        0        0       86 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/types.py
+-rw-r--r--   0        0        0    18581 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/bybit/ws_api.py
+-rw-r--r--   0        0        0    20498 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/exchange_base.py
+-rw-r--r--   0        0        0     4112 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/rest_api_base.py
+-rw-r--r--   0        0        0    26589 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/exchanges/ws_api_base.py
+-rw-r--r--   0        0        0      481 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/externals/ibapi/__init__.py
+-rw-r--r--   0        0        0     2027 2024-04-03 08:14:20.581936 pfund-0.0.1.dev5/pfund/externals/ibapi/account_summary_tags.py
+-rw-r--r--   0        0        0   149406 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/client.py
+-rw-r--r--   0        0        0     2297 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/comm.py
+-rw-r--r--   0        0        0      892 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/commission_report.py
+-rw-r--r--   0        0        0     7841 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/common.py
+-rw-r--r--   0        0        0     3755 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/connection.py
+-rw-r--r--   0        0        0     6642 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/contract.py
+-rw-r--r--   0        0        0    59604 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/decoder.py
+-rw-r--r--   0        0        0      520 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/enum_implem.py
+-rw-r--r--   0        0        0     1635 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/errors.py
+-rw-r--r--   0        0        0     2027 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/execution.py
+-rw-r--r--   0        0        0     2211 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/ibapi.pyproj
+-rw-r--r--   0        0        0     6366 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/message.py
+-rw-r--r--   0        0        0      507 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/news.py
+-rw-r--r--   0        0        0      358 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/object_implem.py
+-rw-r--r--   0        0        0     9369 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/order.py
+-rw-r--r--   0        0        0     8243 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/order_condition.py
+-rw-r--r--   0        0        0      943 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/order_state.py
+-rw-r--r--   0        0        0    19630 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/orderdecoder.py
+-rw-r--r--   0        0        0     1625 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/reader.py
+-rw-r--r--   0        0        0     2020 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/scanner.py
+-rw-r--r--   0        0        0     5580 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/server_versions.py
+-rw-r--r--   0        0        0      553 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/softdollartier.py
+-rw-r--r--   0        0        0      714 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/tag_value.py
+-rw-r--r--   0        0        0     3876 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/ticktype.py
+-rw-r--r--   0        0        0     4130 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/utils.py
+-rw-r--r--   0        0        0    31944 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/externals/ibapi/wrapper.py
+-rw-r--r--   0        0        0      200 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/indicators/__init__.py
+-rw-r--r--   0        0        0     2827 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/indicators/indicator_base.py
+-rw-r--r--   0        0        0     4205 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/indicators/ta_indicator.py
+-rw-r--r--   0        0        0     2139 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/indicators/talib_indicator.py
+-rw-r--r--   0        0        0      159 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/main.py
+-rw-r--r--   0        0        0      396 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/__init__.py
+-rw-r--r--   0        0        0      997 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/base_manager.py
+-rw-r--r--   0        0        0     7659 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/connection_manager.py
+-rw-r--r--   0        0        0    13773 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/data_manager.py
+-rw-r--r--   0        0        0    12813 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/order_manager.py
+-rw-r--r--   0        0        0     3893 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/portfolio_manager.py
+-rw-r--r--   0        0        0      175 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/risk_manager.py
+-rw-r--r--   0        0        0     8106 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/managers/strategy_manager.py
+-rw-r--r--   0        0        0     7947 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/mixins/backtest.py
+-rw-r--r--   0        0        0      236 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/__init__.py
+-rw-r--r--   0        0        0     4510 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/model_backtest.py
+-rw-r--r--   0        0        0    18416 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/model_base.py
+-rw-r--r--   0        0        0     2032 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/model_meta.py
+-rw-r--r--   0        0        0     2659 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/pytorch_model.py
+-rw-r--r--   0        0        0     1188 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/models/sklearn_model.py
+-rw-r--r--   0        0        0      138 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/__init__.py
+-rw-r--r--   0        0        0    10415 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/order_base.py
+-rw-r--r--   0        0        0     1531 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/order_crypto.py
+-rw-r--r--   0        0        0      230 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/order_ib.py
+-rw-r--r--   0        0        0      781 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/order_statuses.py
+-rw-r--r--   0        0        0      150 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/orders/order_time_in_force.py
+-rw-r--r--   0        0        0     3501 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/plogging/__init__.py
+-rw-r--r--   0        0        0     3269 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/plogging/config.py
+-rw-r--r--   0        0        0      409 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/plogging/filters.py
+-rw-r--r--   0        0        0      578 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/plogging/formatter.py
+-rw-r--r--   0        0        0     1538 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/plogging/handlers.py
+-rw-r--r--   0        0        0      134 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/portfolio.py
+-rw-r--r--   0        0        0      165 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/positions/__init__.py
+-rw-r--r--   0        0        0     1300 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/positions/position_base.py
+-rw-r--r--   0        0        0     3655 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/positions/position_crypto.py
+-rw-r--r--   0        0        0     2304 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/positions/position_ib.py
+-rw-r--r--   0        0        0      155 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/products/__init__.py
+-rw-r--r--   0        0        0     1593 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/products/product_base.py
+-rw-r--r--   0        0        0     3275 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/products/product_crypto.py
+-rw-r--r--   0        0        0     2334 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/products/product_ib.py
+-rw-r--r--   0        0        0       71 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/risk_monitor.py
+-rw-r--r--   0        0        0       82 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/strategies/__init__.py
+-rw-r--r--   0        0        0     1975 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/strategies/strategy_backtest.py
+-rw-r--r--   0        0        0    24139 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/strategies/strategy_base.py
+-rw-r--r--   0        0        0      930 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/strategies/strategy_meta.py
+-rw-r--r--   0        0        0     2455 2024-04-03 08:14:20.585937 pfund-0.0.1.dev5/pfund/utils/aliases.py
+-rw-r--r--   0        0        0      591 2024-04-03 08:14:20.589937 pfund-0.0.1.dev5/pfund/utils/envs.py
+-rw-r--r--   0        0        0     5166 2024-04-03 08:14:20.589937 pfund-0.0.1.dev5/pfund/utils/utils.py
+-rw-r--r--   0        0        0     4033 2024-04-03 08:14:20.589937 pfund-0.0.1.dev5/pfund/zeromq.py
+-rw-r--r--   0        0        0     1676 2024-04-03 08:14:20.589937 pfund-0.0.1.dev5/pyproject.toml
+-rw-r--r--   0        0        0    12506 1970-01-01 00:00:00.000000 pfund-0.0.1.dev5/PKG-INFO
```

### Comparing `pfund-0.0.1.dev4/LICENSE` & `pfund-0.0.1.dev5/LICENSE`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/README.md` & `pfund-0.0.1.dev5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,47 @@
 # PFund: Algo-Trading Framework for Machine Learning, TradFi, CeFi and DeFi ready.
 
-[![Jupyter Book Badge](docs/images/jupyterbook.svg)](https://jupyterbook.org)
-[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
+![GitHub stars](https://img.shields.io/github/stars/PFund-Software-Ltd/pfund?style=social)
+![PyPI downloads](https://img.shields.io/pypi/dm/pfund)
 [![PyPI](https://img.shields.io/pypi/v/pfund.svg)](https://pypi.org/project/pfund)
 ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/pfund)
+[![Jupyter Book Badge](https://raw.githubusercontent.com/PFund-Software-Ltd/pfund/main/docs/images/jupyterbook.svg
+)](https://jupyterbook.org)
+[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 
-PFund (/piː fʌnd/), which stands for "Personal Fund", is an algo-trading framework designed for using machine learning models to trade across TradFi (Traditional Finance, e.g. Interactive Brokers), CeFi (Centralized Finance, e.g. Binance) and DeFi (Decentralized Finance, e.g. [dYdX](https://dydx.exchange)), or in simple terms, **Stocks** and **Cryptos**.
+[TradFi]: https://www.techopedia.com/definition/traditional-finance-tradfi
+[CeFi]: https://www.techopedia.com/definition/centralized-finance-cefi
+[DeFi]: https://www.coinbase.com/learn/crypto-basics/what-is-defi
+[pytrade.org]: https://pytrade.org
+[dYdX]: https://dydx.exchange
+[polars]: https://pola.rs/
+[PFund.ai]: https://pfund.ai
+[PFeed]: https://github.com/PFund-Software-Ltd/pfeed
+[Bybit]: https://bybit.com/
+[PyTorch]: https://pytorch.org/
+[Poetry]: https://python-poetry.org
+[Futu]: https://www.futunn.com
+[FirstRate Data]: https://firstratedata.com
+[Mantine UI]: https://ui.mantine.dev/
+
+PFund (/piː fʌnd/), which stands for "**Personal Fund**", is an **algo-trading framework** designed for using **machine learning** models to trade across [TradFi] (Traditional Finance, e.g. **Interactive Brokers**), [CeFi] (Centralized Finance, e.g. Binance) and [DeFi] (Decentralized Finance, e.g. [dYdX]), or in simple terms, **Stocks** and **Cryptos**.
 
 PFund allows traders to:
 - perform vectorized or event-driven backtesting with
   - different resolutions of data, e.g. orderbook data, tick data, bar data etc.
-  - different data tools, e.g. pandas, [polars](https://pola.rs/) etc.
+  - different data tools, e.g. pandas, [polars] etc.
 - train machine learning models using their favorite frameworks, i.e. PFund is **ML-framework agnostic**
 - tune strategy (hyper)parameters by splitting data into training sets, development sets and test sets
 - go from backtesting to live trading by just changing **ONE line of code!!**
+- execute trades manually/semi-manually via a trading app (frontend+backend)
 
-It is created to enable trading for [PFund.ai](https://pfund.ai) - a trading platform that bridges algo-trading and manual trading using AI (LLM).
+It is created to enable trading for [PFund.ai] - a trading platform that bridges algo-trading and manual trading using AI (LLM).
 
 Since PFund's sole purpose is for trading only, for all the data work, there is a separate library to handle that: \
-[PFeed](https://github.com/PFund-Software-Ltd/pfeed) - Data pipeline for algo-trading, helping traders in getting real-time and historical data, and storing them in a local data lake for quantitative research.
+[PFeed] - Data pipeline for algo-trading, helping traders in getting real-time and historical data, and storing them in a local data lake for quantitative research.
 
 
 <details>
 <summary>Table of Contents</summary>
 
 - [Project Status](#project-status)
 - [Mission](#mission)
@@ -41,20 +60,20 @@
 </details>
 
 
 ## Project Status
 **_Caution: PFund is at a VERY EARLY stage, use it at your own risk._**
 
 PFund is currently under active development, the framework design will be prioritized first over
-stability and scalability. 
+stability and scalability.
 
 Please note that the available version is a *dev* version, not a *stable* one. \
 You are encouraged to play with the *dev* version, but only use it when a *stable* version is released.
 
-> PFund for the time being **_only supports vectorized backtesting_** using [Bybit](https://bybit.com/) and Yahoo Finance data for testing purpose.
+> PFund for the time being **_only supports vectorized backtesting_** using [Bybit] and Yahoo Finance data for testing purpose.
 
 
 ## Mission
 As an algo-trader, if you aim to quickly try out some trading ideas to see if they work, and if they do, deploy them for live traidng, it is actually not a trivial task since it involves multiple stages:
 - Ideation
 - Strategy development
 - Backtesting
@@ -62,39 +81,55 @@
 - Model training (if using machine learning)
 - Parameter training / hyperparameter tuning
 - Strategy deployment
 - Portfolio monitoring
 
 This overview already omits some intricate steps, such as data handling and API integration.
 
-> PFund's mission is to **_enable traders to concentrate solely on strategy formulation_** while the framework manages the rest. With PFund serving as the core trade engine, it empowers retail traders to have a fund management experience on [PFund.ai](https://pfund.ai) as if they are operating their personal hedge fund, hence the name *PFund*.
+> PFund's mission is to **_enable traders to concentrate solely on strategy formulation_** while the framework manages the rest. With PFund serving as the core trade engine, it empowers retail traders to have a fund management experience on [PFund.ai] as if they are operating their personal hedge fund, hence the name *PFund*.
 
 
 ## Core Features
 - [x] Easily switch environments with just one line of code, transitioning from backtesting to live trading
 - [x] Supports machine learning models, features, technical analysis indicators
 - [x] Both Strategy() and Model() are treated as first-class citizens
 - [x] Offers LEGO-style strategy and model building, allowing strategies to add other strategies, models to add other models
 - [x] Streamlines the algo-trading flow, from vectorized backtesting for strategy prototyping and event-driven backtesting for strategy development, to live trading for strategy deployment
 - [x] Enables parallel data processing, e.g. Interactive Brokers and Binance each have their own process for receiving data feeds
 - [ ] Allows choosing your preferred data tool, e.g. pandas, polars, pyspark etc.
-- [ ] Features a modern frontend using [Mantine UI](https://ui.mantine.dev/) and TradingView's Charts library
-
+- [ ] Features a modern frontend using [Mantine UI] and TradingView's Charts library
+- [ ] Supports manual/semi-manual trading using the frontend
 
 
 ## Installation
-### Using [Poetry](https://python-poetry.org) (Recommended)
+> Python 3.12 is not supported until [PyTorch]supports it
+
+### Using [Poetry] (Recommended)
 ```bash
 poetry add pfund
+
+# update to the latest version:
+poetry update pfund
 ```
 
 
 ### Using Pip
 ```bash
 pip install pfund
+
+# install the latest version:
+pip install -U pfund
+```
+
+
+### Checking your installation
+```bash
+$ pfund --version
+
+pfund, version 0.0.1.dev4
 ```
 
 
 ## Quick Start
 ### Backtesting
 ```python
 import pfund as pf
@@ -102,31 +137,47 @@
 # NOTE: for more exciting strategies, please visit pfund.ai
 class YourStrategy(pf.Strategy):
     # triggered by bar/kline data (e.g. 1-minute data)
     def on_bar(self):
         # write your trading logic here
         pass
 
-engine = pf.BacktestEngine(...)
-strategy = engine.add_strategy(YourStrategy())
-strategy.add_data(...)
-strategy.add_model(...)
+
+engine = pf.BacktestEngine(mode='vectorized')
+strategy = engine.add_strategy(YourStrategy(), name='your_strategy')
+strategy.add_data(
+  'IB', 'AAPL', 'USD', 'STK', resolutions=['1d'],
+  backtest={
+    # NOTE: since IB does not provide any historical data for backtesting purpose, use data from 'YAHOO_FINANCE'
+    'data_source': 'YAHOO_FINANCE',
+    'start_date': '2024-01-01',
+    'end_date': '2024-02-01',
+  }
+)
 engine.run()
 ```
 
 
 ### Live Trading
 > Just change one line of code, from '**BacktestEngine**' to '**TradeEngine**'. BOOM! you can now start live trading.
 ```python
 import pfund as pf
 
 engine = pf.TradeEngine(env='LIVE')
-strategy = engine.add_strategy(YourStrategy())
-strategy.add_data(...)
-strategy.add_model(...)
+strategy = engine.add_strategy(YourStrategy(), name='your_strategy')
+strategy.add_data(
+  'IB', 'AAPL', 'USD', 'STK', resolutions=['1d'],
+  # for convenience, you can keep the kwarg `backtest`, `TradeEngine` will ignore it
+  backtest={
+    # NOTE: since IB does not provide any historical data for backtesting purpose, use data from 'YAHOO_FINANCE'
+    'data_source': 'YAHOO_FINANCE',
+    'start_date': '2024-01-01',
+    'end_date': '2024-02-01',
+  }
+)
 engine.run()
 ```
 
 ### Parameter Training / Hyperparameter Tuning
 > The correct term should be "Hyperparameter Tuning", but since not all traders are familiar with machine learning, the framework uses a more well-known term "training".
 
 ```python
@@ -156,37 +207,38 @@
 engine.run()
 ```
 
 
 ## Model Hub
 Imagine a space where algo-traders can share their machine learning models with one another.
 Strategy and model development could be so much faster since you can build on top of an existing working model.
-> Model Hub is coming soon in [PFund.ai](https://pfund.ai), Stay Tuned!
+> Model Hub is coming soon on [PFund.ai], Stay Tuned!
 
 
 ## Supported Trading Venues
-| Trading Venue                   | Vectorized Backtesting | Event-Driven Backtesting | Paper Trading | Live Trading |
-| ------------------------------- | ---------------------- | ------------------------ | ------------- | ------------ |
-| Bybit                           | 🟢                     | 🟡                       | 🟡            | 🟡           |
-| *Interactive Brokers (IB)       | 🟡                     | 🟡                       | 🟡            | 🟡           |
-| Binance                         | 🔴                     | 🔴                       | 🔴            | 🔴           |
-| OKX                             | 🔴                     | 🔴                       | 🔴            | 🔴           |
-| *Alpaca                         | 🔴                     | 🔴                       | 🔴            | 🔴           |
-| *[Futu](https://www.futunn.com) | 🔴                     | 🔴                       | 🔴            | 🔴           |
-| dYdX                            | 🔴                     | 🔴                       | 🔴            | 🔴           |
+| Trading Venue             | Vectorized Backtesting | Event-Driven Backtesting | Paper Trading | Live Trading |
+| ------------------------- | ---------------------- | ------------------------ | ------------- | ------------ |
+| Bybit                     | 🟢                     | 🟡                       | 🟡            | 🟡           |
+| *Interactive Brokers (IB) | 🟡                     | 🟡                       | 🟡            | 🟡           |
+| Binance                   | 🔴                     | 🔴                       | 🔴            | 🔴           |
+| OKX                       | 🔴                     | 🔴                       | 🔴            | 🔴           |
+| *Alpaca                   | 🔴                     | 🔴                       | 🔴            | 🔴           |
+| *[Futu]                   | 🔴                     | 🔴                       | 🔴            | 🔴           |
+| dYdX                      | 🔴                     | 🔴                       | 🔴            | 🔴           |
 
 🟢 = finished \
 🟡 = in progress \
 🔴 = todo \
-\* = use a **_separate data source_** (e.g. [FirstRate Data](https://firstratedata.com)) for backtesting
+\* = use a **_separate data source_** (e.g. [FirstRate Data]) for backtesting
 
 
 ## Related Projects
-- [PFeed](https://github.com/PFund-Software-Ltd/pfeed) — Data pipeline for algo-trading, helping traders in getting real-time and historical data, and storing them in a local data lake for quantitative research.
+- [PFeed] — Data pipeline for algo-trading, helping traders in getting real-time and historical data, and storing them in a local data lake for quantitative research.
+- [PyTrade.org] - A curated list of Python libraries and resources for algorithmic trading.
 
 
 ## Disclaimer
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF, OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 This algo-trading framework is intended for educational and research purposes only. It should not be used for real trading without understanding the risks involved. Trading in financial markets involves significant risk, and there is always the potential for loss. Your trading results may vary. No representation is being made that any account will or is likely to achieve profits or losses similar to those discussed on this platform.
 
-The developers of this framework are not responsible for any financial losses incurred from using this software. Users should conduct their due diligence and consult with a professional financial advisor before engaging in real trading activities.
+The developers of this framework are not responsible for any financial losses incurred from using this software. Users should conduct their due diligence and consult with a professional financial advisor before engaging in real trading activities.
```

### Comparing `pfund-0.0.1.dev4/pfund/__init__.py` & `pfund-0.0.1.dev5/pfund/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,18 @@
+import sys
 from importlib.metadata import version
 
+from pfund.const.paths import PROJ_PATH
+# add python path so that for files like "ibapi" (official python code from IB) can find their modules
+sys.path.append(f'{PROJ_PATH}/externals')
 from pfund.config_handler import configure
 from pfund.engines import BacktestEngine, TrainEngine, TestEngine, TradeEngine
 from pfund.strategies import Strategy
 from pfund.models import Feature, Model
+from pfund.utils.aliases import ALIASES
 try:
     from pfund.models import PyTorchModel
 except ImportError:
     pass
 try:
     from pfund.models import SKLearnModel
 except ImportError:
@@ -16,12 +21,12 @@
 
 
 __version__ = version('pfund')
 
 
 __all__ = (
     '__version__',
-    'configure',
+    'configure', 'ALIASES',
     'BacktestEngine', 'TrainEngine', 'TestEngine', 'TradeEngine',
     'Strategy', 'Model', 'PyTorchModel', 'SKLearnModel',
     'Feature', 'TAIndicator', 'TALibIndicator',
 )
```

### Comparing `pfund-0.0.1.dev4/pfund/accounts/account_base.py` & `pfund-0.0.1.dev5/pfund/accounts/account_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/accounts/account_crypto.py` & `pfund-0.0.1.dev5/pfund/accounts/account_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/accounts/account_ib.py` & `pfund-0.0.1.dev5/pfund/accounts/account_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/adapter.py` & `pfund-0.0.1.dev5/pfund/adapter.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self.load_pdt_matchings()
 
     def build_internal_pdt_format(self, bccy, qccy, ptype):
         pdt = '_'.join([bccy, qccy, ptype])
         return pdt
 
     def load_pdt_matchings(self):
-        file_path = f'{PROJ_CONFIG_PATH}/{self._trading_venue}'
+        file_path = f'{PROJ_CONFIG_PATH}/{self._trading_venue.lower()}'
         config_name = 'pdt_matchings'
         for file_name in os.listdir(file_path):
             if not file_name.startswith(config_name):
                 continue
             file_splits = file_name.split('_')
             if len(file_splits) > 2:
                 category = file_splits[-1].split('.')[0]
```

### Comparing `pfund-0.0.1.dev4/pfund/balances/balance_base.py` & `pfund-0.0.1.dev5/pfund/balances/balance_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/balances/balance_ib.py` & `pfund-0.0.1.dev5/pfund/balances/balance_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/brokers/broker_backtest.py` & `pfund-0.0.1.dev5/pfund/brokers/broker_backtest.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/brokers/broker_base.py` & `pfund-0.0.1.dev5/pfund/brokers/broker_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/brokers/broker_crypto.py` & `pfund-0.0.1.dev5/pfund/brokers/broker_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/brokers/broker_live.py` & `pfund-0.0.1.dev5/pfund/brokers/broker_live.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/brokers/ib/broker_ib.py` & `pfund-0.0.1.dev5/pfund/brokers/ib/broker_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/brokers/ib/ib_api.py` & `pfund-0.0.1.dev5/pfund/brokers/ib/ib_api.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/brokers/ib/ib_client.py` & `pfund-0.0.1.dev5/pfund/brokers/ib/ib_client.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/brokers/ib/ib_wrapper.py` & `pfund-0.0.1.dev5/pfund/brokers/ib/ib_wrapper.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/cli/commands/config.py` & `pfund-0.0.1.dev5/pfund/cli/commands/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 import click
 
 from pfund.const.paths import USER_CONFIG_FILE_PATH
 from pfund.config_handler import ConfigHandler
 
 
 def save_config(config: ConfigHandler, config_file_path: str | Path):
+    if type(config_file_path) is str:
+        config_file_path = Path(config_file_path)
+    config_file_path.parent.mkdir(parents=True, exist_ok=True)
     with open(config_file_path, 'w') as f:
         yaml.dump(config.__dict__, f, default_flow_style=False)
         
 
 def remove_config(config_file_path: str | Path):
     config_file_path = Path(config_file_path)
     if config_file_path.is_file():
```

### Comparing `pfund-0.0.1.dev4/pfund/cli/commands/docker_compose.py` & `pfund-0.0.1.dev5/pfund/cli/commands/docker_compose.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,16 +14,18 @@
 ))
 @click.pass_context
 @click.option('--env-file', 'env_file_path', type=click.Path(exists=True), help='Path to the .env file')
 @click.option('--docker-file', 'docker_file_path', type=click.Path(exists=True), help='Path to the docker-compose.yml file')
 def docker_compose(ctx, env_file_path, docker_file_path):
     """Forwards commands to docker-compose with the package's docker-compose.yml file if not specified."""
     if not env_file_path:
-        env_file_path = find_dotenv(usecwd=True, raise_error_if_not_found=True)
-        click.echo(f'.env file path is not specified, using env file in "{env_file_path}"')
+        if env_file_path := find_dotenv(usecwd=True, raise_error_if_not_found=False):
+            click.echo(f'.env file path is not specified, using env file in "{env_file_path}"')
+        else:
+            click.echo('.env file is not found')
     load_dotenv(env_file_path, override=True)
     if not docker_file_path:
         package_dir = Path(importlib.resources.files(PROJ_NAME)).resolve().parents[0]
         docker_file_path = package_dir / 'docker-compose.yml'
     else:
         click.echo(f'loaded custom docker-compose.yml file from "{docker_file_path}"')
     command = ['docker-compose', '-f', str(docker_file_path)] + ctx.args
```

### Comparing `pfund-0.0.1.dev4/pfund/config/bybit/config.yml` & `pfund-0.0.1.dev5/pfund/config/bybit/config.yml`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     R---: 'Rejected'
     O---: 'New'
     OP--: 'PartiallyFilled'
     CPC-: 'PartiallyFilledCanceled'
     CF--: 'Filled'
     C-C-: 'Cancelled'
   offset: {}
-  px_directions: {
+  price_directions: {
     # internal definitions:
     # PlusTick: ...,
     # ZeroPlusTick: ...,
     # MinusTick: ...,
     # ZeroMinusTick: ...
   }
   public_channels: {
```

### Comparing `pfund-0.0.1.dev4/pfund/config/bybit/lot_sizes_linear.yml` & `pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_linear.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config/bybit/lot_sizes_option.yml` & `pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_option.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config/bybit/lot_sizes_spot.yml` & `pfund-0.0.1.dev5/pfund/config/bybit/lot_sizes_spot.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config/bybit/pdt_matchings_linear.yml` & `pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_linear.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config/bybit/pdt_matchings_spot.yml` & `pfund-0.0.1.dev5/pfund/config/bybit/pdt_matchings_spot.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config/bybit/tick_sizes_linear.yml` & `pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_linear.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config/bybit/tick_sizes_option.yml` & `pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_option.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config/bybit/tick_sizes_spot.yml` & `pfund-0.0.1.dev5/pfund/config/bybit/tick_sizes_spot.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config/configuration.py` & `pfund-0.0.1.dev5/pfund/config/configuration.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config/ib/config.yml` & `pfund-0.0.1.dev5/pfund/config/ib/config.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config/logging.yml` & `pfund-0.0.1.dev5/pfund/config/logging.yml`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/config_handler.py` & `pfund-0.0.1.dev5/pfund/config_handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,19 +5,16 @@
 import logging
 from types import TracebackType
 from dataclasses import dataclass
 
 import yaml
 # from rich.traceback import install
 
-from pfund.const.paths import PROJ_NAME, PROJ_PATH, LOG_PATH, PROJ_CONFIG_PATH, DATA_PATH, USER_CONFIG_FILE_PATH
+from pfund.const.paths import PROJ_NAME, LOG_PATH, PROJ_CONFIG_PATH, DATA_PATH, USER_CONFIG_FILE_PATH
 
-# add python path so that for files like "ibapi" (official python code from IB)
-# can find their modules
-sys.path.append(f'{PROJ_PATH}/externals')
 # install(show_locals=False)  # rich will set its own sys.excepthook
 # rich_excepthook = sys.excepthook  # get rich's excepthook
 
 
 def _custom_excepthook(exception_class: type[BaseException], exception: BaseException, traceback: TracebackType):
     '''Catches any uncaught exceptions and logs them'''
     # sys.__excepthook__(exception_class, exception, traceback)
```

### Comparing `pfund-0.0.1.dev4/pfund/const/_zmq_routes.py` & `pfund-0.0.1.dev5/pfund/const/_zmq_routes.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/const/commons.py` & `pfund-0.0.1.dev5/pfund/const/commons.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/const/paths.py` & `pfund-0.0.1.dev5/pfund/const/paths.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from pathlib import Path
 from platformdirs import user_log_dir, user_data_dir, user_config_dir
 
 
 # project paths
-PROJ_NAME = Path(__file__).resolve().parents[2].name
-MAIN_PATH = Path(__file__).resolve().parents[3]
-PROJ_PATH = MAIN_PATH / PROJ_NAME / PROJ_NAME
+PROJ_NAME = Path(__file__).resolve().parents[1].name
+MAIN_PATH = Path(__file__).resolve().parents[2]
+PROJ_PATH = MAIN_PATH / PROJ_NAME
+
 EXCHANGE_PATH = PROJ_PATH / 'exchanges'
 PROJ_CONFIG_PATH = PROJ_PATH / 'config'
 
 
 # user paths
 LOG_PATH = Path(user_log_dir()) / PROJ_NAME
 USER_CONFIG_PATH = Path(user_config_dir()) / PROJ_NAME
```

### Comparing `pfund-0.0.1.dev4/pfund/data_tools/data_tool_base.py` & `pfund-0.0.1.dev5/pfund/data_tools/data_tool_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/data_tools/data_tool_pandas.py` & `pfund-0.0.1.dev5/pfund/data_tools/data_tool_pandas.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/datas/data_bar.py` & `pfund-0.0.1.dev5/pfund/datas/data_bar.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/datas/data_quote.py` & `pfund-0.0.1.dev5/pfund/datas/data_quote.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/datas/data_tick.py` & `pfund-0.0.1.dev5/pfund/datas/data_tick.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/datas/data_time_based.py` & `pfund-0.0.1.dev5/pfund/datas/data_time_based.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/datas/resolution.py` & `pfund-0.0.1.dev5/pfund/datas/resolution.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pfund.datas.timeframe import Timeframe, TimeframeUnits
 from pfund.const.commons import SUPPORTED_TIMEFRAMES
 
 
 class Resolution:
     def __init__(self, resolution: str):
+        assert re.match(r"^\d+[a-zA-Z]+$", resolution), f"Invalid {resolution=}, pattern should be e.g. '1d', '2m', '3h' etc."
         self._resolution = self._standardize(resolution)
         # split resolution (e.g. '1m') into period (e.g. '1') and timeframe (e.g. 'm')
         self.period, timeframe = re.split('(\d+)', self._resolution.strip())[1:]
         self.period = int(self.period)
         assert self.period > 0
         self.timeframe = Timeframe(timeframe)
```

### Comparing `pfund-0.0.1.dev4/pfund/datas/timeframe.py` & `pfund-0.0.1.dev5/pfund/datas/timeframe.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/engines/backtest_engine.py` & `pfund-0.0.1.dev5/pfund/engines/backtest_engine.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import Literal
 
 from pfund.data_tools.data_tool_base import DataTool
 from pfund.engines.base_engine import BaseEngine
-from pfund.models.model_base import BaseModel
+from pfund.models.model_base import BaseModel, BaseFeature
+from pfund.indicators.indicator_base import BaseIndicator
 from pfund.brokers.broker_backtest import BacktestBroker
 from pfund.strategies.strategy_base import BaseStrategy
 from pfund.strategies.strategy_backtest import BacktestStrategy
 from pfund.const.commons import *
 from pfund.config_handler import ConfigHandler
 
 
@@ -52,14 +53,20 @@
             event_driven_funcs = ['on_quote', 'on_tick', 'on_bar', 'on_position', 'on_balance', 'on_order', 'on_trade']
             for func in event_driven_funcs:
                 setattr(strategy, func, empty_function)
         assert not strategy.models, 'Adding more than 1 model to dummy strategy in backtesting is not supported, you should train and dump your models one by one'
         model = strategy.add_model(model, name=name, model_path=model_path, is_load=is_load)
         return model
     
+    def add_feature(self, feature: BaseFeature, name: str='', feature_path: str='', is_load: bool=True) -> BaseFeature:
+        return self.add_model(feature, name=name, model_path=feature_path, is_load=is_load)
+    
+    def add_indicator(self, indicator: BaseIndicator, name: str='', indicator_path: str='', is_load: bool=True) -> BaseIndicator:
+        return self.add_model(indicator, name=name, model_path=indicator_path, is_load=is_load)
+    
     def add_broker(self, bkr: str):
         bkr = bkr.upper()
         if bkr in self.brokers:
             return self.get_broker(bkr)
         Broker = self.get_Broker(bkr)
         broker = BacktestBroker(Broker)
         bkr = broker.name
```

### Comparing `pfund-0.0.1.dev4/pfund/engines/base_engine.py` & `pfund-0.0.1.dev5/pfund/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/engines/test_engine.py` & `pfund-0.0.1.dev5/pfund/engines/test_engine.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/engines/trade_engine.py` & `pfund-0.0.1.dev5/pfund/engines/trade_engine.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/engines/train_engine.py` & `pfund-0.0.1.dev5/pfund/engines/train_engine.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/exchange.py` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/exchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,36 +14,29 @@
 
 class Exchange(BaseExchange):
     SUPPORTED_CATEGORIES = ['linear', 'inverse', 'spot', 'option']
     # NOTE, bybit only supports place_batch_orders for category `options`
     # TODO, come back to this if bybit supports more
     # SUPPORT_PLACE_BATCH_ORDERS = True
     # SUPPORT_CANCEL_BATCH_ORDERS = True
+    
+    PTYPE_TO_CATEGORY = {
+        'PERP': 'linear',
+        'FUT': 'linear',
+        'IPERP': 'inverse',
+        'IFUT': 'inverse',
+        'SPOT': 'spot',
+        'OPT': 'option',
+    }
 
     _MAX_NUM_OF_PLACE_BATCH_ORDERS = 20
     _MAX_NUM_OF_CANEL_BATCH_ORDERS = 20
 
     def __init__(self, env):
         super().__init__(env, 'BYBIT')
-
-    @staticmethod
-    def categorize_product_type(ptype):
-        is_spot = (ptype == 'SPOT')
-        is_inverse = (ptype in ['IPERP', 'IFUT'])
-        is_linear = not is_inverse and not is_spot
-        is_option = (ptype == 'OPT')
-        if is_linear:
-            category = 'linear'
-        elif is_inverse:
-            category = 'inverse'
-        elif is_spot:
-            category = 'spot'
-        elif is_option:
-            category = 'option'
-        return category
     
     def _create_pdt_matchings_config(
             # general to exchanges
             self, 
             markets,
             # specific to bybit
             category: Category
```

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api.py` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_inverse`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_linear`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_option`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_result_spot`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_inverse`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_linear`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_option`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/rest_api_samples/get_markets_return_spot`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/bybit/ws_api.py` & `pfund-0.0.1.dev5/pfund/exchanges/bybit/ws_api.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/exchange_base.py` & `pfund-0.0.1.dev5/pfund/exchanges/exchange_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
             self.add_channel(channel, type_='private')
 
     def add_category(self, category):
         if category not in self.categories:
             self.categories.append(category)
 
     def create_product(self, bccy, qccy, ptype, *args, **kwargs) -> CryptoProduct:
-        if category := self.categorize_product_type(ptype) if hasattr(self, 'categorize_product_type') else '':
+        if category := self.PTYPE_TO_CATEGORY[ptype] if hasattr(self, 'PTYPE_TO_CATEGORY') else '':
             self.add_category(category)
         product = CryptoProduct(self.exch, bccy, qccy, ptype, *args, category=category, **kwargs)
         product.load_configs(self.configs)
         return product
 
     def get_product(self, pdt: str) -> CryptoProduct | None:
         return self.products.get(pdt.upper(), None)
```

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/rest_api_base.py` & `pfund-0.0.1.dev5/pfund/exchanges/rest_api_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/exchanges/ws_api_base.py` & `pfund-0.0.1.dev5/pfund/exchanges/ws_api_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/account_summary_tags.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/account_summary_tags.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/client.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/client.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/comm.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/comm.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/commission_report.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/commission_report.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/common.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/common.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/connection.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/connection.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/contract.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/contract.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/decoder.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/decoder.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/enum_implem.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/enum_implem.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/errors.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/errors.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/execution.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/execution.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/ibapi.pyproj` & `pfund-0.0.1.dev5/pfund/externals/ibapi/ibapi.pyproj`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/message.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/message.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/order.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/order.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/order_condition.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/order_condition.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/order_state.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/order_state.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/orderdecoder.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/orderdecoder.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/reader.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/reader.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/scanner.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/scanner.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/server_versions.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/server_versions.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/softdollartier.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/softdollartier.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/tag_value.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/tag_value.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/ticktype.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/ticktype.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/utils.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/utils.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/externals/ibapi/wrapper.py` & `pfund-0.0.1.dev5/pfund/externals/ibapi/wrapper.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/indicators/indicator_base.py` & `pfund-0.0.1.dev5/pfund/indicators/indicator_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/indicators/ta_indicator.py` & `pfund-0.0.1.dev5/pfund/indicators/ta_indicator.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/indicators/talib_indicator.py` & `pfund-0.0.1.dev5/pfund/indicators/talib_indicator.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/managers/base_manager.py` & `pfund-0.0.1.dev5/pfund/managers/base_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/managers/connection_manager.py` & `pfund-0.0.1.dev5/pfund/managers/connection_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/managers/data_manager.py` & `pfund-0.0.1.dev5/pfund/managers/data_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/managers/order_manager.py` & `pfund-0.0.1.dev5/pfund/managers/order_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/managers/portfolio_manager.py` & `pfund-0.0.1.dev5/pfund/managers/portfolio_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/managers/strategy_manager.py` & `pfund-0.0.1.dev5/pfund/managers/strategy_manager.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/mixins/backtest.py` & `pfund-0.0.1.dev5/pfund/mixins/backtest.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,16 @@
 from typing import TYPE_CHECKING
 if TYPE_CHECKING:
     from pfeed.feeds.base_feed import BaseFeed
     from pfund.datas.data_base import BaseData
 
 from pfund.managers.data_manager import get_resolutions_from_kwargs
 from pfund.models.model_backtest import BacktestModel
-from pfund.models.model_base import BaseModel
+from pfund.models.model_base import BaseModel, BaseFeature
+from pfund.indicators.indicator_base import BaseIndicator
 
 
 _PFUND_BACKTEST_KWARGS = ['data_source', 'rollback_period', 'start_date', 'end_date']
 _EVENT_DRIVEN_BACKTEST_KWARGS = ['resamples', 'shifts', 'auto_resample']
 
 
 class BacktestMixin:
@@ -39,14 +40,20 @@
                 self.add_raw_df(data, df)
         return datas
         
     def add_model(self, model: BaseModel, name: str='', model_path: str='', is_load: bool=True) -> BaseModel:
         name = name or model.__class__.__name__
         model = BacktestModel(type(model), model.ml_model, *model._args, **model._kwargs)
         return super().add_model(model, name=name, model_path=model_path, is_load=is_load)
+    
+    def add_feature(self, feature: BaseFeature, name: str='', feature_path: str='', is_load: bool=True) -> BaseFeature:
+        return self.add_model(feature, name=name, model_path=feature_path, is_load=is_load)
+        
+    def add_indicator(self, indicator: BaseIndicator, name: str='', indicator_path: str='', is_load: bool=True) -> BaseIndicator:
+        return self.add_model(indicator, name=name, model_path=indicator_path, is_load=is_load)
         
     def _get_data_source(self, trading_venue: str, backtest_kwargs: dict):
         from pfeed.const.commons import SUPPORTED_DATA_FEEDS
         trading_venue = trading_venue.upper()
         # if data_source is not defined, use trading_venue as data_source
         if trading_venue in SUPPORTED_DATA_FEEDS and 'data_source' not in backtest_kwargs:
             backtest_kwargs['data_source'] = trading_venue
@@ -133,14 +140,17 @@
             assert not df.empty, f"dataframe is empty for {pdt_or_symbol=}"
             df.reset_index(inplace=True)
             latest_date = str(df['ts'][0])
             if feed.name == 'YAHOO_FINANCE' and latest_date == utcnow_date:
                 print(f'To avoid non-deterministic metrics, Yahoo Finance data on {latest_date} is removed since it might be being updated in real-time')
                 df = df[:-1]
             
+            if 'symbol' in df.columns:
+                df = df.drop('symbol', axis=1) 
+            
             df['product'] = product
             df['resolution'] = resolution
             dfs.append(df)
             
             # don't sleep on the last one loop, waste of time
             if feed.name == 'YAHOO_FINANCE' and n != len(datas) - 1:
                 time.sleep(rate_limit)
```

### Comparing `pfund-0.0.1.dev4/pfund/models/model_backtest.py` & `pfund-0.0.1.dev5/pfund/models/model_backtest.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/models/model_base.py` & `pfund-0.0.1.dev5/pfund/models/model_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     pass
 import numpy as np
 import pandas as pd
 
 if TYPE_CHECKING:
     from pfund.strategies.strategy_base import BaseStrategy
     from pfund.models import PyTorchModel, SKLearnModel
-    from pfund.indicators.indicator_base import TAFunction, TALibFunction
+    from pfund.indicators.indicator_base import BaseIndicator, TAFunction, TALibFunction
     MachineLearningModel = Union[
         nn.Module,
         BaseEstimator,
         ClassifierMixin,
         RegressorMixin, 
         Pipeline,
         TAFunction,  # ta.utils.IndicatorMixin
@@ -316,14 +316,20 @@
             raise Exception(f"model '{mdl}' already exists in model '{self.name}'")
         model.set_consumer(self)
         model.set_is_load(is_load)
         self.models[mdl] = model
         self.logger.debug(f"added model '{mdl}'")
         return model
     
+    def add_feature(self, feature: BaseFeature, name: str='', feature_path: str='', is_load: bool=True) -> BaseFeature:
+        return self.add_model(feature, name=name, model_path=feature_path, is_load=is_load)
+    
+    def add_indicator(self, indicator: BaseIndicator, name: str='', indicator_path: str='', is_load: bool=True) -> BaseIndicator:
+        return self.add_model(indicator, name=name, model_path=indicator_path, is_load=is_load)
+    
     def update_quote(self, data: QuoteData, **kwargs):
         product, bids, asks, ts = data.product, data.bids, data.asks, data.ts
         self.data = data
         for listener in self._listeners[data]:
             model = listener
             model.update_quote(data, **kwargs)
             self.update_predictions(model)
```

### Comparing `pfund-0.0.1.dev4/pfund/models/model_meta.py` & `pfund-0.0.1.dev5/pfund/models/model_meta.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/models/pytorch_model.py` & `pfund-0.0.1.dev5/pfund/models/pytorch_model.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/models/sklearn_model.py` & `pfund-0.0.1.dev5/pfund/models/sklearn_model.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/orders/order_base.py` & `pfund-0.0.1.dev5/pfund/orders/order_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/orders/order_crypto.py` & `pfund-0.0.1.dev5/pfund/orders/order_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/orders/order_statuses.py` & `pfund-0.0.1.dev5/pfund/orders/order_statuses.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/plogging/__init__.py` & `pfund-0.0.1.dev5/pfund/plogging/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,19 @@
             print(name, logger, logger.handlers)
 
 
 def set_up_loggers(log_path, logging_config_file_path, user_logging_config: dict | None=None) -> LoggingDictConfigurator:
     def deep_update(default_dict, override_dict, raise_if_key_not_exist=False):
         '''Updates a default dictionary with an override dictionary, supports nested dictionaries.'''
         for key, value in override_dict.items():
+            
+            # make sure log level is in uppercase, 'debug' -> 'DEBUG'
+            if key == 'level':
+                value = value.upper()
+                
             if raise_if_key_not_exist and key not in default_dict:
                 # Raise an exception if the key from override_dict doesn't exist in default_dict
                 raise KeyError(f"Key '{key}' is not supported in logging config.")
             if isinstance(value, dict):
                 # Get the default_dict value for key, if not exist, create a new empty dict
                 default_value = default_dict.get(key, {})
                 if isinstance(default_value, dict):
```

### Comparing `pfund-0.0.1.dev4/pfund/plogging/config.py` & `pfund-0.0.1.dev5/pfund/plogging/config.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/plogging/formatter.py` & `pfund-0.0.1.dev5/pfund/plogging/formatter.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/plogging/handlers.py` & `pfund-0.0.1.dev5/pfund/plogging/handlers.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/positions/position_base.py` & `pfund-0.0.1.dev5/pfund/positions/position_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/positions/position_crypto.py` & `pfund-0.0.1.dev5/pfund/positions/position_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/positions/position_ib.py` & `pfund-0.0.1.dev5/pfund/positions/position_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/products/product_base.py` & `pfund-0.0.1.dev5/pfund/products/product_base.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/products/product_crypto.py` & `pfund-0.0.1.dev5/pfund/products/product_crypto.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/products/product_ib.py` & `pfund-0.0.1.dev5/pfund/products/product_ib.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/strategies/strategy_backtest.py` & `pfund-0.0.1.dev5/pfund/strategies/strategy_backtest.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/strategies/strategy_base.py` & `pfund-0.0.1.dev5/pfund/strategies/strategy_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,16 @@
 
 from typing import Literal, TYPE_CHECKING
 
 if TYPE_CHECKING:
     from pfund.brokers.broker_base import BaseBroker
     from pfund.exchanges.exchange_base import BaseExchange
     from pfund.datas.data_bar import Bar
-from pfund.models.model_base import BaseModel
+from pfund.models.model_base import BaseModel, BaseFeature
+from pfund.indicators.indicator_base import BaseIndicator
 from pfund.datas import BaseData, BarData, TickData, QuoteData
 from pfund.products.product_base import BaseProduct
 from pfund.accounts.account_base import BaseAccount
 from pfund.orders.order_base import BaseOrder
 from pfund.zeromq import ZeroMQ
 from pfund.portfolio import Portfolio
 from pfund.risk_monitor import RiskMonitor
@@ -153,15 +154,21 @@
         if mdl in self.models:
             raise Exception(f"model '{mdl}' already exists in strategy '{self.name}'")
         model.set_consumer(self)
         model.set_is_load(is_load)
         self.models[mdl] = model
         self.logger.debug(f"added model '{mdl}'")
         return model
-        
+    
+    def add_feature(self, feature: BaseFeature, name: str='', feature_path: str='', is_load: bool=True) -> BaseFeature:
+        return self.add_model(feature, name=name, model_path=feature_path, is_load=is_load)
+    
+    def add_indicator(self, indicator: BaseIndicator, name: str='', indicator_path: str='', is_load: bool=True) -> BaseIndicator:
+        return self.add_model(indicator, name=name, model_path=indicator_path, is_load=is_load)
+    
     # TODO
     def add_custom_data(self):
         pass
     
     def get_datas(self) -> list[BaseData]:
         datas = []
         for product in self.datas:
```

### Comparing `pfund-0.0.1.dev4/pfund/strategies/strategy_meta.py` & `pfund-0.0.1.dev5/pfund/strategies/strategy_meta.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/utils/aliases.py` & `pfund-0.0.1.dev5/pfund/utils/aliases.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ALIASES = {
     'proj': 'project',
-    'conf': 'configuration',
+    'config': 'configuration',
     'const': 'constant',
     'dir': 'directory',
     'env': 'environment',
     'fh': 'file_handler',
     'fh_name': 'file_handler_name',
     'fh_kwargs': 'file_handler_keyword_arguments',
     'fh_lv': 'file_handler_level',
@@ -31,17 +31,19 @@
     'exch': 'exchange',
     'strat': 'strategy',
     'pdt': 'product',
     'epdt': 'external_product',
     'bccy': 'base_currency',
     'qccy': 'quote_currency',
     'ccy': 'currency',
+    'eccy': 'external_currency',
     'px': 'price',
     'qty': 'quantity',
     'ptype': 'product_type',
+    'eptype': 'external_product_type',
     'otype': 'order_type',
     'acc': 'account',
     'mdl': 'model',
     'ftr': 'feature',
 
     'o': 'order',
     'ltp': 'last_traded_price',
@@ -50,14 +52,16 @@
     'ltt': 'last_traded_time',
 
     'PERP': 'linear perpetual',
     'IPERP': 'inverse perpetual',
     'FUT': 'linear futures',
     'IFUT': 'inverse futures',
     'OPT': 'linear options',
+    'STK': 'stock',
+    'CMDTY': 'commodity',
     'CW': 'current_week',
     'NW': 'next_week',
     'CM': 'current_month',
     'NM': 'next_month',
     'CQ': 'current_quarter',
     'NQ': 'next_quarter',
```

### Comparing `pfund-0.0.1.dev4/pfund/utils/envs.py` & `pfund-0.0.1.dev5/pfund/utils/envs.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/utils/utils.py` & `pfund-0.0.1.dev5/pfund/utils/utils.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/pfund/zeromq.py` & `pfund-0.0.1.dev5/pfund/zeromq.py`

 * *Files identical despite different names*

### Comparing `pfund-0.0.1.dev4/PKG-INFO` & `pfund-0.0.1.dev5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,61 +1,77 @@
 Metadata-Version: 2.1
 Name: pfund
-Version: 0.0.1.dev4
+Version: 0.0.1.dev5
 Summary: A Complete Algo-Trading Framework for Machine Learning, enabling trading across TradFi, CeFi and DeFi. Supports Vectorized and Event-Driven Backtesting, Paper and Live Trading
 Home-page: https://pfund.ai
 License: Apache-2.0
 Keywords: trading,algo-trading,stocks,cryptos,cryptocurrencies,TradFi,CeFi,DeFi,portfolio management,investment,backtesting,machine learning
 Author: Stephen Yau
 Author-email: softwareentrepreneer+pfund@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.7,<9.0.0)
 Requires-Dist: orjson (>=3.9.14,<4.0.0)
-Requires-Dist: pandas (>=2.2.0,<3.0.0)
-Requires-Dist: pfeed (>=0.0.1.dev4,<0.0.2)
+Requires-Dist: pfeed (>=0.0.1.dev5,<0.0.2)
 Requires-Dist: platformdirs (>=4.2.0,<5.0.0)
 Requires-Dist: psutil (>=5.9.8,<6.0.0)
 Requires-Dist: python-telegram-bot (>=20.7,<21.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
 Requires-Dist: pyzmq (>=25.1.2,<26.0.0)
 Requires-Dist: rich (>=13.7.0,<14.0.0)
 Requires-Dist: schedule (>=1.2.1,<2.0.0)
-Requires-Dist: scikit-learn (>=1.4.0,<2.0.0)
 Requires-Dist: ta (>=0.11.0,<0.12.0)
-Requires-Dist: torch (>=2.1.2,<3.0.0)
 Requires-Dist: websocket-client (>=1.7.0,<2.0.0)
-Project-URL: Documentation, https://pfund.ai/docs
+Project-URL: Documentation, https://pfund-docs.pfund.ai
 Project-URL: Repository, https://github.com/PFund-Software-Ltd/pfund
 Description-Content-Type: text/markdown
 
 # PFund: Algo-Trading Framework for Machine Learning, TradFi, CeFi and DeFi ready.
 
-[![Jupyter Book Badge](docs/images/jupyterbook.svg)](https://jupyterbook.org)
-[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
+![GitHub stars](https://img.shields.io/github/stars/PFund-Software-Ltd/pfund?style=social)
+![PyPI downloads](https://img.shields.io/pypi/dm/pfund)
 [![PyPI](https://img.shields.io/pypi/v/pfund.svg)](https://pypi.org/project/pfund)
 ![PyPI - Support Python Versions](https://img.shields.io/pypi/pyversions/pfund)
+[![Jupyter Book Badge](https://raw.githubusercontent.com/PFund-Software-Ltd/pfund/main/docs/images/jupyterbook.svg
+)](https://jupyterbook.org)
+[![Poetry](https://img.shields.io/endpoint?url=https://python-poetry.org/badge/v0.json)](https://python-poetry.org/)
 
-PFund (/piː fʌnd/), which stands for "Personal Fund", is an algo-trading framework designed for using machine learning models to trade across TradFi (Traditional Finance, e.g. Interactive Brokers), CeFi (Centralized Finance, e.g. Binance) and DeFi (Decentralized Finance, e.g. [dYdX](https://dydx.exchange)), or in simple terms, **Stocks** and **Cryptos**.
+[TradFi]: https://www.techopedia.com/definition/traditional-finance-tradfi
+[CeFi]: https://www.techopedia.com/definition/centralized-finance-cefi
+[DeFi]: https://www.coinbase.com/learn/crypto-basics/what-is-defi
+[pytrade.org]: https://pytrade.org
+[dYdX]: https://dydx.exchange
+[polars]: https://pola.rs/
+[PFund.ai]: https://pfund.ai
+[PFeed]: https://github.com/PFund-Software-Ltd/pfeed
+[Bybit]: https://bybit.com/
+[PyTorch]: https://pytorch.org/
+[Poetry]: https://python-poetry.org
+[Futu]: https://www.futunn.com
+[FirstRate Data]: https://firstratedata.com
+[Mantine UI]: https://ui.mantine.dev/
+
+PFund (/piː fʌnd/), which stands for "**Personal Fund**", is an **algo-trading framework** designed for using **machine learning** models to trade across [TradFi] (Traditional Finance, e.g. **Interactive Brokers**), [CeFi] (Centralized Finance, e.g. Binance) and [DeFi] (Decentralized Finance, e.g. [dYdX]), or in simple terms, **Stocks** and **Cryptos**.
 
 PFund allows traders to:
 - perform vectorized or event-driven backtesting with
   - different resolutions of data, e.g. orderbook data, tick data, bar data etc.
-  - different data tools, e.g. pandas, [polars](https://pola.rs/) etc.
+  - different data tools, e.g. pandas, [polars] etc.
 - train machine learning models using their favorite frameworks, i.e. PFund is **ML-framework agnostic**
 - tune strategy (hyper)parameters by splitting data into training sets, development sets and test sets
 - go from backtesting to live trading by just changing **ONE line of code!!**
+- execute trades manually/semi-manually via a trading app (frontend+backend)
 
-It is created to enable trading for [PFund.ai](https://pfund.ai) - a trading platform that bridges algo-trading and manual trading using AI (LLM).
+It is created to enable trading for [PFund.ai] - a trading platform that bridges algo-trading and manual trading using AI (LLM).
 
 Since PFund's sole purpose is for trading only, for all the data work, there is a separate library to handle that: \
-[PFeed](https://github.com/PFund-Software-Ltd/pfeed) - Data pipeline for algo-trading, helping traders in getting real-time and historical data, and storing them in a local data lake for quantitative research.
+[PFeed] - Data pipeline for algo-trading, helping traders in getting real-time and historical data, and storing them in a local data lake for quantitative research.
 
 
 <details>
 <summary>Table of Contents</summary>
 
 - [Project Status](#project-status)
 - [Mission](#mission)
@@ -74,20 +90,20 @@
 </details>
 
 
 ## Project Status
 **_Caution: PFund is at a VERY EARLY stage, use it at your own risk._**
 
 PFund is currently under active development, the framework design will be prioritized first over
-stability and scalability. 
+stability and scalability.
 
 Please note that the available version is a *dev* version, not a *stable* one. \
 You are encouraged to play with the *dev* version, but only use it when a *stable* version is released.
 
-> PFund for the time being **_only supports vectorized backtesting_** using [Bybit](https://bybit.com/) and Yahoo Finance data for testing purpose.
+> PFund for the time being **_only supports vectorized backtesting_** using [Bybit] and Yahoo Finance data for testing purpose.
 
 
 ## Mission
 As an algo-trader, if you aim to quickly try out some trading ideas to see if they work, and if they do, deploy them for live traidng, it is actually not a trivial task since it involves multiple stages:
 - Ideation
 - Strategy development
 - Backtesting
@@ -95,39 +111,55 @@
 - Model training (if using machine learning)
 - Parameter training / hyperparameter tuning
 - Strategy deployment
 - Portfolio monitoring
 
 This overview already omits some intricate steps, such as data handling and API integration.
 
-> PFund's mission is to **_enable traders to concentrate solely on strategy formulation_** while the framework manages the rest. With PFund serving as the core trade engine, it empowers retail traders to have a fund management experience on [PFund.ai](https://pfund.ai) as if they are operating their personal hedge fund, hence the name *PFund*.
+> PFund's mission is to **_enable traders to concentrate solely on strategy formulation_** while the framework manages the rest. With PFund serving as the core trade engine, it empowers retail traders to have a fund management experience on [PFund.ai] as if they are operating their personal hedge fund, hence the name *PFund*.
 
 
 ## Core Features
 - [x] Easily switch environments with just one line of code, transitioning from backtesting to live trading
 - [x] Supports machine learning models, features, technical analysis indicators
 - [x] Both Strategy() and Model() are treated as first-class citizens
 - [x] Offers LEGO-style strategy and model building, allowing strategies to add other strategies, models to add other models
 - [x] Streamlines the algo-trading flow, from vectorized backtesting for strategy prototyping and event-driven backtesting for strategy development, to live trading for strategy deployment
 - [x] Enables parallel data processing, e.g. Interactive Brokers and Binance each have their own process for receiving data feeds
 - [ ] Allows choosing your preferred data tool, e.g. pandas, polars, pyspark etc.
-- [ ] Features a modern frontend using [Mantine UI](https://ui.mantine.dev/) and TradingView's Charts library
-
+- [ ] Features a modern frontend using [Mantine UI] and TradingView's Charts library
+- [ ] Supports manual/semi-manual trading using the frontend
 
 
 ## Installation
-### Using [Poetry](https://python-poetry.org) (Recommended)
+> Python 3.12 is not supported until [PyTorch]supports it
+
+### Using [Poetry] (Recommended)
 ```bash
 poetry add pfund
+
+# update to the latest version:
+poetry update pfund
 ```
 
 
 ### Using Pip
 ```bash
 pip install pfund
+
+# install the latest version:
+pip install -U pfund
+```
+
+
+### Checking your installation
+```bash
+$ pfund --version
+
+pfund, version 0.0.1.dev4
 ```
 
 
 ## Quick Start
 ### Backtesting
 ```python
 import pfund as pf
@@ -135,31 +167,47 @@
 # NOTE: for more exciting strategies, please visit pfund.ai
 class YourStrategy(pf.Strategy):
     # triggered by bar/kline data (e.g. 1-minute data)
     def on_bar(self):
         # write your trading logic here
         pass
 
-engine = pf.BacktestEngine(...)
-strategy = engine.add_strategy(YourStrategy())
-strategy.add_data(...)
-strategy.add_model(...)
+
+engine = pf.BacktestEngine(mode='vectorized')
+strategy = engine.add_strategy(YourStrategy(), name='your_strategy')
+strategy.add_data(
+  'IB', 'AAPL', 'USD', 'STK', resolutions=['1d'],
+  backtest={
+    # NOTE: since IB does not provide any historical data for backtesting purpose, use data from 'YAHOO_FINANCE'
+    'data_source': 'YAHOO_FINANCE',
+    'start_date': '2024-01-01',
+    'end_date': '2024-02-01',
+  }
+)
 engine.run()
 ```
 
 
 ### Live Trading
 > Just change one line of code, from '**BacktestEngine**' to '**TradeEngine**'. BOOM! you can now start live trading.
 ```python
 import pfund as pf
 
 engine = pf.TradeEngine(env='LIVE')
-strategy = engine.add_strategy(YourStrategy())
-strategy.add_data(...)
-strategy.add_model(...)
+strategy = engine.add_strategy(YourStrategy(), name='your_strategy')
+strategy.add_data(
+  'IB', 'AAPL', 'USD', 'STK', resolutions=['1d'],
+  # for convenience, you can keep the kwarg `backtest`, `TradeEngine` will ignore it
+  backtest={
+    # NOTE: since IB does not provide any historical data for backtesting purpose, use data from 'YAHOO_FINANCE'
+    'data_source': 'YAHOO_FINANCE',
+    'start_date': '2024-01-01',
+    'end_date': '2024-02-01',
+  }
+)
 engine.run()
 ```
 
 ### Parameter Training / Hyperparameter Tuning
 > The correct term should be "Hyperparameter Tuning", but since not all traders are familiar with machine learning, the framework uses a more well-known term "training".
 
 ```python
@@ -189,38 +237,38 @@
 engine.run()
 ```
 
 
 ## Model Hub
 Imagine a space where algo-traders can share their machine learning models with one another.
 Strategy and model development could be so much faster since you can build on top of an existing working model.
-> Model Hub is coming soon in [PFund.ai](https://pfund.ai), Stay Tuned!
+> Model Hub is coming soon on [PFund.ai], Stay Tuned!
 
 
 ## Supported Trading Venues
-| Trading Venue                   | Vectorized Backtesting | Event-Driven Backtesting | Paper Trading | Live Trading |
-| ------------------------------- | ---------------------- | ------------------------ | ------------- | ------------ |
-| Bybit                           | 🟢                     | 🟡                       | 🟡            | 🟡           |
-| *Interactive Brokers (IB)       | 🟡                     | 🟡                       | 🟡            | 🟡           |
-| Binance                         | 🔴                     | 🔴                       | 🔴            | 🔴           |
-| OKX                             | 🔴                     | 🔴                       | 🔴            | 🔴           |
-| *Alpaca                         | 🔴                     | 🔴                       | 🔴            | 🔴           |
-| *[Futu](https://www.futunn.com) | 🔴                     | 🔴                       | 🔴            | 🔴           |
-| dYdX                            | 🔴                     | 🔴                       | 🔴            | 🔴           |
+| Trading Venue             | Vectorized Backtesting | Event-Driven Backtesting | Paper Trading | Live Trading |
+| ------------------------- | ---------------------- | ------------------------ | ------------- | ------------ |
+| Bybit                     | 🟢                     | 🟡                       | 🟡            | 🟡           |
+| *Interactive Brokers (IB) | 🟡                     | 🟡                       | 🟡            | 🟡           |
+| Binance                   | 🔴                     | 🔴                       | 🔴            | 🔴           |
+| OKX                       | 🔴                     | 🔴                       | 🔴            | 🔴           |
+| *Alpaca                   | 🔴                     | 🔴                       | 🔴            | 🔴           |
+| *[Futu]                   | 🔴                     | 🔴                       | 🔴            | 🔴           |
+| dYdX                      | 🔴                     | 🔴                       | 🔴            | 🔴           |
 
 🟢 = finished \
 🟡 = in progress \
 🔴 = todo \
-\* = use a **_separate data source_** (e.g. [FirstRate Data](https://firstratedata.com)) for backtesting
+\* = use a **_separate data source_** (e.g. [FirstRate Data]) for backtesting
 
 
 ## Related Projects
-- [PFeed](https://github.com/PFund-Software-Ltd/pfeed) — Data pipeline for algo-trading, helping traders in getting real-time and historical data, and storing them in a local data lake for quantitative research.
+- [PFeed] — Data pipeline for algo-trading, helping traders in getting real-time and historical data, and storing them in a local data lake for quantitative research.
+- [PyTrade.org] - A curated list of Python libraries and resources for algorithmic trading.
 
 
 ## Disclaimer
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE, AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES, OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF, OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 
 This algo-trading framework is intended for educational and research purposes only. It should not be used for real trading without understanding the risks involved. Trading in financial markets involves significant risk, and there is always the potential for loss. Your trading results may vary. No representation is being made that any account will or is likely to achieve profits or losses similar to those discussed on this platform.
 
 The developers of this framework are not responsible for any financial losses incurred from using this software. Users should conduct their due diligence and consult with a professional financial advisor before engaging in real trading activities.
-
```

