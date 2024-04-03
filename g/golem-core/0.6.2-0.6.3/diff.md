# Comparing `tmp/golem_core-0.6.2.tar.gz` & `tmp/golem_core-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "golem_core-0.6.2.tar", max compression
+gzip compressed data, was "golem_core-0.6.3.tar", max compression
```

## Comparing `golem_core-0.6.2.tar` & `golem_core-0.6.3.tar`

### file list

```diff
@@ -1,144 +1,144 @@
--rw-r--r--   0        0        0    35149 2023-09-13 08:05:36.792448 golem_core-0.6.2/LICENSE
--rw-r--r--   0        0        0        0 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/__init__.py
--rw-r--r--   0        0        0       64 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/__main__.py
--rw-r--r--   0        0        0       50 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/cli/__init__.py
--rw-r--r--   0        0        0     2641 2023-11-25 08:20:36.562759 golem_core-0.6.2/golem/cli/cli.py
--rw-r--r--   0        0        0     4463 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/cli/utils.py
--rw-r--r--   0        0        0      151 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/event_bus/__init__.py
--rw-r--r--   0        0        0     1280 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/event_bus/base.py
--rw-r--r--   0        0        0       98 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/event_bus/in_memory/__init__.py
--rw-r--r--   0        0        0     6737 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/event_bus/in_memory/event_bus.py
--rw-r--r--   0        0        0      332 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/exceptions.py
--rw-r--r--   0        0        0     2554 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/managers/__init__.py
--rw-r--r--   0        0        0      475 2023-10-10 09:27:48.015544 golem_core-0.6.2/golem/managers/activity/__init__.py
--rw-r--r--   0        0        0      476 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/managers/activity/defaults.py
--rw-r--r--   0        0        0     2111 2023-10-10 09:27:48.019544 golem_core-0.6.2/golem/managers/activity/mixins.py
--rw-r--r--   0        0        0     3872 2023-10-10 09:27:48.019544 golem_core-0.6.2/golem/managers/activity/pool.py
--rw-r--r--   0        0        0     1734 2023-10-10 09:27:48.019544 golem_core-0.6.2/golem/managers/activity/single_use.py
--rw-r--r--   0        0        0      109 2023-10-03 11:48:04.547546 golem_core-0.6.2/golem/managers/agreement/__init__.py
--rw-r--r--   0        0        0     2406 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/managers/agreement/default.py
--rw-r--r--   0        0        0     5925 2024-03-28 09:34:26.737805 golem_core-0.6.2/golem/managers/base.py
--rw-r--r--   0        0        0      218 2024-02-28 10:31:22.882324 golem_core-0.6.2/golem/managers/demand/__init__.py
--rw-r--r--   0        0        0     2286 2024-02-28 10:31:22.882324 golem_core-0.6.2/golem/managers/demand/aggregating.py
--rw-r--r--   0        0        0     5488 2024-02-15 12:52:48.457251 golem_core-0.6.2/golem/managers/demand/refreshing.py
--rw-r--r--   0        0        0     1658 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/managers/mixins.py
--rw-r--r--   0        0        0      100 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/managers/network/__init__.py
--rw-r--r--   0        0        0     2197 2023-12-13 09:08:00.946133 golem_core-0.6.2/golem/managers/network/single.py
--rw-r--r--   0        0        0      103 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/managers/payment/__init__.py
--rw-r--r--   0        0        0     5682 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/managers/payment/default.py
--rw-r--r--   0        0        0      980 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/managers/proposal/__init__.py
--rw-r--r--   0        0        0     1586 2023-11-02 09:14:12.499044 golem_core-0.6.2/golem/managers/proposal/default.py
--rw-r--r--   0        0        0     1155 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/managers/proposal/plugins/__init__.py
--rw-r--r--   0        0        0     1005 2023-10-13 09:42:33.129828 golem_core-0.6.2/golem/managers/proposal/plugins/blacklist.py
--rw-r--r--   0        0        0     5011 2024-03-20 09:04:31.378487 golem_core-0.6.2/golem/managers/proposal/plugins/buffer.py
--rw-r--r--   0        0        0     1054 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/managers/proposal/plugins/linear_coeffs.py
--rw-r--r--   0        0        0      422 2024-01-23 10:41:17.114958 golem_core-0.6.2/golem/managers/proposal/plugins/negotiating/__init__.py
--rw-r--r--   0        0        0     4671 2024-01-23 10:41:17.114958 golem_core-0.6.2/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py
--rw-r--r--   0        0        0     4879 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py
--rw-r--r--   0        0        0     1567 2024-01-23 10:41:17.114958 golem_core-0.6.2/golem/managers/proposal/plugins/negotiating/payment_platform.py
--rw-r--r--   0        0        0     2441 2024-01-05 09:59:46.197955 golem_core-0.6.2/golem/managers/proposal/plugins/reject_costs_exceeds.py
--rw-r--r--   0        0        0      738 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/managers/proposal/plugins/scoring/__init__.py
--rw-r--r--   0        0        0     1738 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/managers/proposal/plugins/scoring/map.py
--rw-r--r--   0        0        0     4008 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/managers/proposal/plugins/scoring/mixins.py
--rw-r--r--   0        0        0     1938 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/managers/proposal/plugins/scoring/pricings.py
--rw-r--r--   0        0        0     3457 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/managers/proposal/plugins/scoring/property_value_lerp.py
--rw-r--r--   0        0        0      505 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/managers/proposal/plugins/scoring/random.py
--rw-r--r--   0        0        0     4217 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/managers/proposal/plugins/scoring/scoring_buffer.py
--rw-r--r--   0        0        0      996 2023-10-13 09:42:33.129828 golem_core-0.6.2/golem/managers/proposal/plugins/whitelist.py
--rw-r--r--   0        0        0      474 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/managers/work/__init__.py
--rw-r--r--   0        0        0     2087 2023-10-10 09:27:48.019544 golem_core-0.6.2/golem/managers/work/concurrent.py
--rw-r--r--   0        0        0     2024 2023-10-10 09:27:48.019544 golem_core-0.6.2/golem/managers/work/mixins.py
--rw-r--r--   0        0        0     2038 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/managers/work/plugins.py
--rw-r--r--   0        0        0     1201 2023-10-10 09:27:48.019544 golem_core-0.6.2/golem/managers/work/sequential.py
--rw-r--r--   0        0        0      257 2023-11-25 08:20:36.566756 golem_core-0.6.2/golem/node/__init__.py
--rw-r--r--   0        0        0      856 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/node/events.py
--rw-r--r--   0        0        0    16730 2024-01-26 10:08:12.206583 golem_core-0.6.2/golem/node/node.py
--rw-r--r--   0        0        0     1153 2023-11-30 13:59:47.049268 golem_core-0.6.2/golem/payload/__init__.py
--rw-r--r--   0        0        0     6649 2023-11-25 08:20:36.566756 golem_core-0.6.2/golem/payload/base.py
--rw-r--r--   0        0        0     1939 2023-11-30 13:59:47.049268 golem_core-0.6.2/golem/payload/constraints.py
--rw-r--r--   0        0        0     5156 2024-03-28 09:34:15.049644 golem_core-0.6.2/golem/payload/defaults.py
--rw-r--r--   0        0        0      284 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/payload/exceptions.py
--rw-r--r--   0        0        0      973 2023-11-25 08:20:36.566756 golem_core-0.6.2/golem/payload/generic.py
--rw-r--r--   0        0        0     1405 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/payload/mixins.py
--rw-r--r--   0        0        0     1186 2024-01-08 09:28:36.246646 golem_core-0.6.2/golem/payload/parser.py
--rw-r--r--   0        0        0      621 2023-11-25 08:20:36.566756 golem_core-0.6.2/golem/payload/parser.tx
--rw-r--r--   0        0        0      868 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/payload/properties.py
--rw-r--r--   0        0        0     5677 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/payload/vm.py
--rw-r--r--   0        0        0      504 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/pipeline/__init__.py
--rw-r--r--   0        0        0     4535 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/pipeline/buffer.py
--rw-r--r--   0        0        0     1847 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/pipeline/chain.py
--rw-r--r--   0        0        0     3704 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/pipeline/default_payment_handler.py
--rw-r--r--   0        0        0     1363 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/pipeline/exceptions.py
--rw-r--r--   0        0        0      842 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/pipeline/limit.py
--rw-r--r--   0        0        0     3990 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/pipeline/map.py
--rw-r--r--   0        0        0     4152 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/pipeline/sort.py
--rw-r--r--   0        0        0     2453 2023-11-25 08:20:36.566756 golem_core-0.6.2/golem/pipeline/zip.py
--rw-r--r--   0        0        0     3462 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/resources/__init__.py
--rw-r--r--   0        0        0      592 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/resources/activity/__init__.py
--rw-r--r--   0        0        0     6327 2024-03-28 09:34:26.737805 golem_core-0.6.2/golem/resources/activity/activity.py
--rw-r--r--   0        0        0     6903 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/resources/activity/commands.py
--rw-r--r--   0        0        0      391 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/resources/activity/events.py
--rw-r--r--   0        0        0      735 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/resources/activity/pipeline.py
--rw-r--r--   0        0        0      360 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/resources/agreement/__init__.py
--rw-r--r--   0        0        0     6475 2024-03-25 15:48:24.993493 golem_core-0.6.2/golem/resources/agreement/agreement.py
--rw-r--r--   0        0        0      375 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/resources/agreement/data.py
--rw-r--r--   0        0        0      400 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/resources/agreement/events.py
--rw-r--r--   0        0        0      289 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/resources/agreement/pipeline.py
--rw-r--r--   0        0        0      410 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/resources/allocation/__init__.py
--rw-r--r--   0        0        0     3220 2024-03-05 09:03:20.980633 golem_core-0.6.2/golem/resources/allocation/allocation.py
--rw-r--r--   0        0        0      409 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/resources/allocation/events.py
--rw-r--r--   0        0        0      835 2023-09-13 08:05:36.800448 golem_core-0.6.2/golem/resources/allocation/exceptions.py
--rw-r--r--   0        0        0    11150 2024-03-28 09:34:26.737805 golem_core-0.6.2/golem/resources/base.py
--rw-r--r--   0        0        0      372 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/debit_note/__init__.py
--rw-r--r--   0        0        0     9062 2024-03-28 10:05:47.507938 golem_core-0.6.2/golem/resources/debit_note/debit_note.py
--rw-r--r--   0        0        0      784 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/debit_note/event_collectors.py
--rw-r--r--   0        0        0      402 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/debit_note/events.py
--rw-r--r--   0        0        0      379 2023-11-30 13:59:47.049268 golem_core-0.6.2/golem/resources/demand/__init__.py
--rw-r--r--   0        0        0      315 2023-11-30 13:59:47.049268 golem_core-0.6.2/golem/resources/demand/data.py
--rw-r--r--   0        0        0     5532 2024-03-05 09:03:20.984633 golem_core-0.6.2/golem/resources/demand/demand.py
--rw-r--r--   0        0        0     2959 2023-11-25 08:20:36.566756 golem_core-0.6.2/golem/resources/demand/demand_builder.py
--rw-r--r--   0        0        0      373 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/demand/events.py
--rw-r--r--   0        0        0     1559 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/event_collectors.py
--rw-r--r--   0        0        0     4215 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/events.py
--rw-r--r--   0        0        0     1016 2024-03-05 09:03:20.984633 golem_core-0.6.2/golem/resources/exceptions.py
--rw-r--r--   0        0        0      340 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/invoice/__init__.py
--rw-r--r--   0        0        0      760 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/invoice/event_collectors.py
--rw-r--r--   0        0        0      382 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/invoice/events.py
--rw-r--r--   0        0        0     5163 2024-03-28 09:34:26.737805 golem_core-0.6.2/golem/resources/invoice/invoice.py
--rw-r--r--   0        0        0      394 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/network/__init__.py
--rw-r--r--   0        0        0      382 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/network/events.py
--rw-r--r--   0        0        0      590 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/network/exceptions.py
--rw-r--r--   0        0        0     5803 2024-03-05 09:03:20.984633 golem_core-0.6.2/golem/resources/network/network.py
--rw-r--r--   0        0        0      509 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/pooling_batch/__init__.py
--rw-r--r--   0        0        0      456 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/pooling_batch/events.py
--rw-r--r--   0        0        0     2122 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/pooling_batch/exceptions.py
--rw-r--r--   0        0        0     5510 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/pooling_batch/pooling_batch.py
--rw-r--r--   0        0        0      499 2024-03-05 09:03:20.984633 golem_core-0.6.2/golem/resources/proposal/__init__.py
--rw-r--r--   0        0        0      508 2023-11-30 13:59:47.049268 golem_core-0.6.2/golem/resources/proposal/data.py
--rw-r--r--   0        0        0      391 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/proposal/events.py
--rw-r--r--   0        0        0      664 2023-11-02 09:14:12.503044 golem_core-0.6.2/golem/resources/proposal/exceptions.py
--rw-r--r--   0        0        0      860 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/resources/proposal/pipeline.py
--rw-r--r--   0        0        0     9303 2024-02-20 09:06:29.551136 golem_core-0.6.2/golem/resources/proposal/proposal.py
--rw-r--r--   0        0        0        0 2024-03-05 09:03:20.984633 golem_core-0.6.2/golem/resources/utils/__init__.py
--rw-r--r--   0        0        0      626 2024-03-05 09:03:20.984633 golem_core-0.6.2/golem/resources/utils/infrastructure.py
--rw-r--r--   0        0        0     6493 2024-03-28 09:34:26.741806 golem_core-0.6.2/golem/resources/utils/payment.py
--rw-r--r--   0        0        0        0 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/utils/__init__.py
--rw-r--r--   0        0        0      704 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/utils/asyncio/__init__.py
--rw-r--r--   0        0        0    13576 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/utils/asyncio/buffer.py
--rw-r--r--   0        0        0     2044 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/utils/asyncio/queue.py
--rw-r--r--   0        0        0     2056 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/utils/asyncio/semaphore.py
--rw-r--r--   0        0        0     1943 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/utils/asyncio/tasks.py
--rw-r--r--   0        0        0     1726 2024-02-08 13:35:10.791354 golem_core-0.6.2/golem/utils/asyncio/waiter.py
--rw-r--r--   0        0        0      741 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/utils/http.py
--rw-r--r--   0        0        0     7521 2024-02-08 13:35:10.795401 golem_core-0.6.2/golem/utils/logging.py
--rw-r--r--   0        0        0      307 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/utils/low/__init__.py
--rw-r--r--   0        0        0     6571 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/utils/low/api.py
--rw-r--r--   0        0        0     3323 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/utils/low/event_collector.py
--rw-r--r--   0        0        0      105 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/utils/storage/__init__.py
--rw-r--r--   0        0        0     4024 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/utils/storage/base.py
--rw-r--r--   0        0        0       88 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/utils/storage/gftp/__init__.py
--rw-r--r--   0        0        0    16077 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/utils/storage/gftp/provider.py
--rw-r--r--   0        0        0      673 2023-09-13 08:05:36.804448 golem_core-0.6.2/golem/utils/storage/utils.py
--rw-r--r--   0        0        0      767 2024-02-08 13:35:10.795401 golem_core-0.6.2/golem/utils/typing.py
--rw-r--r--   0        0        0     4722 2024-03-28 10:08:18.012255 golem_core-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 golem_core-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-09-13 08:05:36.792448 golem_core-0.6.3/LICENSE
+-rw-r--r--   0        0        0        0 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/__init__.py
+-rw-r--r--   0        0        0       64 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/__main__.py
+-rw-r--r--   0        0        0       50 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/cli/__init__.py
+-rw-r--r--   0        0        0     2641 2023-11-25 08:20:36.562759 golem_core-0.6.3/golem/cli/cli.py
+-rw-r--r--   0        0        0     4463 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/cli/utils.py
+-rw-r--r--   0        0        0      151 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/event_bus/__init__.py
+-rw-r--r--   0        0        0     1280 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/event_bus/base.py
+-rw-r--r--   0        0        0       98 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/event_bus/in_memory/__init__.py
+-rw-r--r--   0        0        0     6737 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/event_bus/in_memory/event_bus.py
+-rw-r--r--   0        0        0      332 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/exceptions.py
+-rw-r--r--   0        0        0     2554 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/__init__.py
+-rw-r--r--   0        0        0      475 2023-10-10 09:27:48.015544 golem_core-0.6.3/golem/managers/activity/__init__.py
+-rw-r--r--   0        0        0      476 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/activity/defaults.py
+-rw-r--r--   0        0        0     2111 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/activity/mixins.py
+-rw-r--r--   0        0        0     3872 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/activity/pool.py
+-rw-r--r--   0        0        0     1734 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/activity/single_use.py
+-rw-r--r--   0        0        0      109 2023-10-03 11:48:04.547546 golem_core-0.6.3/golem/managers/agreement/__init__.py
+-rw-r--r--   0        0        0     2406 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/agreement/default.py
+-rw-r--r--   0        0        0     5925 2024-03-28 09:34:26.737805 golem_core-0.6.3/golem/managers/base.py
+-rw-r--r--   0        0        0      218 2024-02-28 10:31:22.882324 golem_core-0.6.3/golem/managers/demand/__init__.py
+-rw-r--r--   0        0        0     2286 2024-02-28 10:31:22.882324 golem_core-0.6.3/golem/managers/demand/aggregating.py
+-rw-r--r--   0        0        0     5488 2024-02-15 12:52:48.457251 golem_core-0.6.3/golem/managers/demand/refreshing.py
+-rw-r--r--   0        0        0     1658 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/mixins.py
+-rw-r--r--   0        0        0      100 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/network/__init__.py
+-rw-r--r--   0        0        0     2197 2023-12-13 09:08:00.946133 golem_core-0.6.3/golem/managers/network/single.py
+-rw-r--r--   0        0        0      103 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/payment/__init__.py
+-rw-r--r--   0        0        0     5682 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/payment/default.py
+-rw-r--r--   0        0        0      980 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/__init__.py
+-rw-r--r--   0        0        0     1586 2023-11-02 09:14:12.499044 golem_core-0.6.3/golem/managers/proposal/default.py
+-rw-r--r--   0        0        0     1155 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/plugins/__init__.py
+-rw-r--r--   0        0        0     1005 2023-10-13 09:42:33.129828 golem_core-0.6.3/golem/managers/proposal/plugins/blacklist.py
+-rw-r--r--   0        0        0     5011 2024-03-20 09:04:31.378487 golem_core-0.6.3/golem/managers/proposal/plugins/buffer.py
+-rw-r--r--   0        0        0     1054 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/proposal/plugins/linear_coeffs.py
+-rw-r--r--   0        0        0      422 2024-01-23 10:41:17.114958 golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/__init__.py
+-rw-r--r--   0        0        0     4671 2024-01-23 10:41:17.114958 golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py
+-rw-r--r--   0        0        0     4879 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py
+-rw-r--r--   0        0        0     1567 2024-01-23 10:41:17.114958 golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/payment_platform.py
+-rw-r--r--   0        0        0     2441 2024-01-05 09:59:46.197955 golem_core-0.6.3/golem/managers/proposal/plugins/reject_costs_exceeds.py
+-rw-r--r--   0        0        0      738 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/__init__.py
+-rw-r--r--   0        0        0     1738 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/map.py
+-rw-r--r--   0        0        0     4008 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/mixins.py
+-rw-r--r--   0        0        0     1938 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/pricings.py
+-rw-r--r--   0        0        0     3457 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/property_value_lerp.py
+-rw-r--r--   0        0        0      505 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/random.py
+-rw-r--r--   0        0        0     4217 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/proposal/plugins/scoring/scoring_buffer.py
+-rw-r--r--   0        0        0      996 2023-10-13 09:42:33.129828 golem_core-0.6.3/golem/managers/proposal/plugins/whitelist.py
+-rw-r--r--   0        0        0      474 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/managers/work/__init__.py
+-rw-r--r--   0        0        0     2087 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/work/concurrent.py
+-rw-r--r--   0        0        0     2024 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/work/mixins.py
+-rw-r--r--   0        0        0     2038 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/managers/work/plugins.py
+-rw-r--r--   0        0        0     1201 2023-10-10 09:27:48.019544 golem_core-0.6.3/golem/managers/work/sequential.py
+-rw-r--r--   0        0        0      257 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/node/__init__.py
+-rw-r--r--   0        0        0      856 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/node/events.py
+-rw-r--r--   0        0        0    16730 2024-01-26 10:08:12.206583 golem_core-0.6.3/golem/node/node.py
+-rw-r--r--   0        0        0     1153 2023-11-30 13:59:47.049268 golem_core-0.6.3/golem/payload/__init__.py
+-rw-r--r--   0        0        0     6649 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/payload/base.py
+-rw-r--r--   0        0        0     1939 2023-11-30 13:59:47.049268 golem_core-0.6.3/golem/payload/constraints.py
+-rw-r--r--   0        0        0     5156 2024-03-28 09:34:15.049644 golem_core-0.6.3/golem/payload/defaults.py
+-rw-r--r--   0        0        0      284 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/payload/exceptions.py
+-rw-r--r--   0        0        0      973 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/payload/generic.py
+-rw-r--r--   0        0        0     1405 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/payload/mixins.py
+-rw-r--r--   0        0        0     1186 2024-01-08 09:28:36.246646 golem_core-0.6.3/golem/payload/parser.py
+-rw-r--r--   0        0        0      621 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/payload/parser.tx
+-rw-r--r--   0        0        0      868 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/payload/properties.py
+-rw-r--r--   0        0        0     5677 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/payload/vm.py
+-rw-r--r--   0        0        0      504 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/__init__.py
+-rw-r--r--   0        0        0     4535 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/buffer.py
+-rw-r--r--   0        0        0     1847 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/chain.py
+-rw-r--r--   0        0        0     3704 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/default_payment_handler.py
+-rw-r--r--   0        0        0     1363 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/exceptions.py
+-rw-r--r--   0        0        0      842 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/limit.py
+-rw-r--r--   0        0        0     3990 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/map.py
+-rw-r--r--   0        0        0     4152 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/pipeline/sort.py
+-rw-r--r--   0        0        0     2453 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/pipeline/zip.py
+-rw-r--r--   0        0        0     3462 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/resources/__init__.py
+-rw-r--r--   0        0        0      592 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/activity/__init__.py
+-rw-r--r--   0        0        0     6327 2024-03-28 09:34:26.737805 golem_core-0.6.3/golem/resources/activity/activity.py
+-rw-r--r--   0        0        0     6903 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/activity/commands.py
+-rw-r--r--   0        0        0      391 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/activity/events.py
+-rw-r--r--   0        0        0      735 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/activity/pipeline.py
+-rw-r--r--   0        0        0      360 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/agreement/__init__.py
+-rw-r--r--   0        0        0     6475 2024-03-25 15:48:24.993493 golem_core-0.6.3/golem/resources/agreement/agreement.py
+-rw-r--r--   0        0        0      375 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/resources/agreement/data.py
+-rw-r--r--   0        0        0      400 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/agreement/events.py
+-rw-r--r--   0        0        0      289 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/agreement/pipeline.py
+-rw-r--r--   0        0        0      410 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/allocation/__init__.py
+-rw-r--r--   0        0        0     3220 2024-03-05 09:03:20.980633 golem_core-0.6.3/golem/resources/allocation/allocation.py
+-rw-r--r--   0        0        0      409 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/allocation/events.py
+-rw-r--r--   0        0        0      835 2023-09-13 08:05:36.800448 golem_core-0.6.3/golem/resources/allocation/exceptions.py
+-rw-r--r--   0        0        0    11150 2024-03-28 09:34:26.737805 golem_core-0.6.3/golem/resources/base.py
+-rw-r--r--   0        0        0      372 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/debit_note/__init__.py
+-rw-r--r--   0        0        0     9201 2024-04-03 13:30:08.983271 golem_core-0.6.3/golem/resources/debit_note/debit_note.py
+-rw-r--r--   0        0        0      784 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/debit_note/event_collectors.py
+-rw-r--r--   0        0        0      402 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/debit_note/events.py
+-rw-r--r--   0        0        0      379 2023-11-30 13:59:47.049268 golem_core-0.6.3/golem/resources/demand/__init__.py
+-rw-r--r--   0        0        0      315 2023-11-30 13:59:47.049268 golem_core-0.6.3/golem/resources/demand/data.py
+-rw-r--r--   0        0        0     5532 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/demand/demand.py
+-rw-r--r--   0        0        0     2959 2023-11-25 08:20:36.566756 golem_core-0.6.3/golem/resources/demand/demand_builder.py
+-rw-r--r--   0        0        0      373 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/demand/events.py
+-rw-r--r--   0        0        0     1559 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/event_collectors.py
+-rw-r--r--   0        0        0     4215 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/events.py
+-rw-r--r--   0        0        0     1016 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/exceptions.py
+-rw-r--r--   0        0        0      340 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/invoice/__init__.py
+-rw-r--r--   0        0        0      760 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/invoice/event_collectors.py
+-rw-r--r--   0        0        0      382 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/invoice/events.py
+-rw-r--r--   0        0        0     5320 2024-04-03 13:30:08.983271 golem_core-0.6.3/golem/resources/invoice/invoice.py
+-rw-r--r--   0        0        0      394 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/network/__init__.py
+-rw-r--r--   0        0        0      382 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/network/events.py
+-rw-r--r--   0        0        0      590 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/network/exceptions.py
+-rw-r--r--   0        0        0     5803 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/network/network.py
+-rw-r--r--   0        0        0      509 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/pooling_batch/__init__.py
+-rw-r--r--   0        0        0      456 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/pooling_batch/events.py
+-rw-r--r--   0        0        0     2122 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/pooling_batch/exceptions.py
+-rw-r--r--   0        0        0     5510 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/pooling_batch/pooling_batch.py
+-rw-r--r--   0        0        0      499 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/proposal/__init__.py
+-rw-r--r--   0        0        0      508 2023-11-30 13:59:47.049268 golem_core-0.6.3/golem/resources/proposal/data.py
+-rw-r--r--   0        0        0      391 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/proposal/events.py
+-rw-r--r--   0        0        0      664 2023-11-02 09:14:12.503044 golem_core-0.6.3/golem/resources/proposal/exceptions.py
+-rw-r--r--   0        0        0      860 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/resources/proposal/pipeline.py
+-rw-r--r--   0        0        0     9303 2024-02-20 09:06:29.551136 golem_core-0.6.3/golem/resources/proposal/proposal.py
+-rw-r--r--   0        0        0        0 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/utils/__init__.py
+-rw-r--r--   0        0        0      626 2024-03-05 09:03:20.984633 golem_core-0.6.3/golem/resources/utils/infrastructure.py
+-rw-r--r--   0        0        0     6493 2024-03-28 09:34:26.741806 golem_core-0.6.3/golem/resources/utils/payment.py
+-rw-r--r--   0        0        0        0 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/__init__.py
+-rw-r--r--   0        0        0      704 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/__init__.py
+-rw-r--r--   0        0        0    13576 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/buffer.py
+-rw-r--r--   0        0        0     2044 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/queue.py
+-rw-r--r--   0        0        0     2056 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/semaphore.py
+-rw-r--r--   0        0        0     1943 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/tasks.py
+-rw-r--r--   0        0        0     1726 2024-02-08 13:35:10.791354 golem_core-0.6.3/golem/utils/asyncio/waiter.py
+-rw-r--r--   0        0        0      741 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/http.py
+-rw-r--r--   0        0        0     7521 2024-02-08 13:35:10.795401 golem_core-0.6.3/golem/utils/logging.py
+-rw-r--r--   0        0        0      307 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/low/__init__.py
+-rw-r--r--   0        0        0     6571 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/low/api.py
+-rw-r--r--   0        0        0     3323 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/low/event_collector.py
+-rw-r--r--   0        0        0      105 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/storage/__init__.py
+-rw-r--r--   0        0        0     4024 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/storage/base.py
+-rw-r--r--   0        0        0       88 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/storage/gftp/__init__.py
+-rw-r--r--   0        0        0    16077 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/storage/gftp/provider.py
+-rw-r--r--   0        0        0      673 2023-09-13 08:05:36.804448 golem_core-0.6.3/golem/utils/storage/utils.py
+-rw-r--r--   0        0        0      767 2024-02-08 13:35:10.795401 golem_core-0.6.3/golem/utils/typing.py
+-rw-r--r--   0        0        0     4722 2024-04-03 13:30:53.986345 golem_core-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 golem_core-0.6.3/PKG-INFO
```

### Comparing `golem_core-0.6.2/LICENSE` & `golem_core-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/cli/cli.py` & `golem_core-0.6.3/golem/cli/cli.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/cli/utils.py` & `golem_core-0.6.3/golem/cli/utils.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/event_bus/base.py` & `golem_core-0.6.3/golem/event_bus/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/event_bus/in_memory/event_bus.py` & `golem_core-0.6.3/golem/event_bus/in_memory/event_bus.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/__init__.py` & `golem_core-0.6.3/golem/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/activity/mixins.py` & `golem_core-0.6.3/golem/managers/activity/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/activity/pool.py` & `golem_core-0.6.3/golem/managers/activity/pool.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/activity/single_use.py` & `golem_core-0.6.3/golem/managers/activity/single_use.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/agreement/default.py` & `golem_core-0.6.3/golem/managers/agreement/default.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/base.py` & `golem_core-0.6.3/golem/managers/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/demand/aggregating.py` & `golem_core-0.6.3/golem/managers/demand/aggregating.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/demand/refreshing.py` & `golem_core-0.6.3/golem/managers/demand/refreshing.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/mixins.py` & `golem_core-0.6.3/golem/managers/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/network/single.py` & `golem_core-0.6.3/golem/managers/network/single.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/payment/default.py` & `golem_core-0.6.3/golem/managers/payment/default.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/__init__.py` & `golem_core-0.6.3/golem/managers/proposal/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/default.py` & `golem_core-0.6.3/golem/managers/proposal/default.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/__init__.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/blacklist.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/blacklist.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/buffer.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/linear_coeffs.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/linear_coeffs.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/mid_agreement_payments.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/negotiating_plugin.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/negotiating/payment_platform.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/negotiating/payment_platform.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/reject_costs_exceeds.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/reject_costs_exceeds.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/scoring/__init__.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/scoring/map.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/map.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/scoring/mixins.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/scoring/pricings.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/pricings.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/scoring/property_value_lerp.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/property_value_lerp.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/scoring/scoring_buffer.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/scoring/scoring_buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/proposal/plugins/whitelist.py` & `golem_core-0.6.3/golem/managers/proposal/plugins/whitelist.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/work/concurrent.py` & `golem_core-0.6.3/golem/managers/work/concurrent.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/work/mixins.py` & `golem_core-0.6.3/golem/managers/work/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/work/plugins.py` & `golem_core-0.6.3/golem/managers/work/plugins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/managers/work/sequential.py` & `golem_core-0.6.3/golem/managers/work/sequential.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/node/events.py` & `golem_core-0.6.3/golem/node/events.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/node/node.py` & `golem_core-0.6.3/golem/node/node.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/payload/__init__.py` & `golem_core-0.6.3/golem/payload/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/payload/base.py` & `golem_core-0.6.3/golem/payload/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/payload/constraints.py` & `golem_core-0.6.3/golem/payload/constraints.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/payload/defaults.py` & `golem_core-0.6.3/golem/payload/defaults.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/payload/generic.py` & `golem_core-0.6.3/golem/payload/generic.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/payload/mixins.py` & `golem_core-0.6.3/golem/payload/mixins.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/payload/parser.py` & `golem_core-0.6.3/golem/payload/parser.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/payload/parser.tx` & `golem_core-0.6.3/golem/payload/parser.tx`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/payload/properties.py` & `golem_core-0.6.3/golem/payload/properties.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/payload/vm.py` & `golem_core-0.6.3/golem/payload/vm.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/pipeline/buffer.py` & `golem_core-0.6.3/golem/pipeline/buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/pipeline/chain.py` & `golem_core-0.6.3/golem/pipeline/chain.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/pipeline/default_payment_handler.py` & `golem_core-0.6.3/golem/pipeline/default_payment_handler.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/pipeline/exceptions.py` & `golem_core-0.6.3/golem/pipeline/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/pipeline/limit.py` & `golem_core-0.6.3/golem/pipeline/limit.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/pipeline/map.py` & `golem_core-0.6.3/golem/pipeline/map.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/pipeline/sort.py` & `golem_core-0.6.3/golem/pipeline/sort.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/pipeline/zip.py` & `golem_core-0.6.3/golem/pipeline/zip.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/__init__.py` & `golem_core-0.6.3/golem/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/activity/__init__.py` & `golem_core-0.6.3/golem/resources/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/activity/activity.py` & `golem_core-0.6.3/golem/resources/activity/activity.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/activity/commands.py` & `golem_core-0.6.3/golem/resources/activity/commands.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/activity/pipeline.py` & `golem_core-0.6.3/golem/resources/activity/pipeline.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/agreement/agreement.py` & `golem_core-0.6.3/golem/resources/agreement/agreement.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/allocation/allocation.py` & `golem_core-0.6.3/golem/resources/allocation/allocation.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/allocation/exceptions.py` & `golem_core-0.6.3/golem/resources/allocation/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/base.py` & `golem_core-0.6.3/golem/resources/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/debit_note/debit_note.py` & `golem_core-0.6.3/golem/resources/debit_note/debit_note.py`

 * *Files 14% similar despite different names*

```diff
@@ -49,35 +49,37 @@
         """Get previous debit note."""
         return max(
             (dn for dn in self.activity.debit_notes if dn.created_at < self.created_at),
             key=lambda dn: dn.created_at,  # type: ignore[union-attr]
             default=None,
         )
 
-    async def get_previous_payable_debit_note(self) -> Optional["DebitNote"]:
-        """Get previous payable debit note."""
-        return max(
+    async def get_previous_debit_notes_count(self) -> int:
+        """Get previous debit notes count."""
+        return len([dn for dn in self.activity.debit_notes if dn.created_at < self.created_at])
+
+    async def get_previous_payable_debit_notes_count(self) -> int:
+        """Get previous payable debit notes count."""
+        return len(
             [
                 dn
                 for dn in self.activity.debit_notes
                 if dn.created_at < self.created_at
                 and (await dn.get_data()).payment_due_date is not None
-            ],
-            key=lambda dn: dn.created_at,  # type: ignore[union-attr]
-            default=None,
+            ]
         )
 
     @staticmethod
     def validate_mid_agreement_payment(
         activity_created_at: datetime,
         debit_note_created_at: datetime,
         payment_props: PaymentProps,
         payment_due_date: Optional[datetime],
-        previous_debit_note_created_at: Optional[datetime] = None,
-        previous_payable_debit_note_created_at: Optional[datetime] = None,
+        previous_debit_notes_count: int = 0,
+        previous_payable_debit_notes_count: int = 0,
         payment_timeout_grace_period: timedelta = timedelta(minutes=5),
         debit_note_interval_grace_period: timedelta = timedelta(seconds=30),
     ) -> None:
         """Validate debit note mid agreement payment data."""
         if payment_due_date is None:
             return
 
@@ -91,49 +93,44 @@
         received_payment_timeout = payment_due_date - debit_note_created_at
         if received_payment_timeout + payment_timeout_grace_period < payment_timeout_timedelta:
             raise PaymentValidationException(
                 f"Payment timeout is shorter than agreed {payment_due_date=}"
                 f"{received_payment_timeout=} < {payment_timeout_timedelta=}."
             )
 
-        time_since_last_payable_debit_note = debit_note_created_at - (
-            previous_payable_debit_note_created_at
-            if previous_payable_debit_note_created_at
-            else activity_created_at
-        )
+        debit_note_interval = timedelta(seconds=payment_props.debit_note_interval)
+        activity_duration = debit_note_created_at - activity_created_at
         if (
-            time_since_last_payable_debit_note + payment_timeout_grace_period
-            < payment_timeout_timedelta
+            activity_duration + debit_note_interval_grace_period
+            < (previous_debit_notes_count - 1) * debit_note_interval
         ):
             raise PaymentValidationException(
-                f"Time since last payable debit note {time_since_last_payable_debit_note}"
-                f"exceeds agreed timeout {payment_timeout_timedelta=}"
+                f"Too many debit notes received {previous_debit_notes_count=}. "
+                f"{activity_duration + debit_note_interval_grace_period}"
+                f"< {previous_debit_notes_count * debit_note_interval}"
             )
 
-        debit_note_interval_timedelta = timedelta(seconds=payment_props.debit_note_interval)
-        time_since_last_debit_note = (
-            (debit_note_created_at - previous_debit_note_created_at)
-            if previous_debit_note_created_at
-            else None
-        )
+        payable_debit_note_interval = timedelta(seconds=payment_props.payment_timeout)
+        activity_duration = debit_note_created_at - activity_created_at
         if (
-            time_since_last_debit_note is not None
-            and time_since_last_debit_note + debit_note_interval_grace_period
-            < debit_note_interval_timedelta
+            activity_duration + payment_timeout_grace_period
+            < (previous_payable_debit_notes_count - 1) * payable_debit_note_interval
         ):
             raise PaymentValidationException(
-                f"Too many debit notes received {time_since_last_debit_note=}"
-                f" {debit_note_interval_timedelta=}"
+                f"Too many payable debit notes received {previous_payable_debit_notes_count=}."
+                f"{activity_duration + payment_timeout_grace_period}"
+                f"< {previous_payable_debit_notes_count * payable_debit_note_interval}"
             )
 
     def validate_payment_data(
         self,
         debit_note_data: models.DebitNote,
         previous_debit_note: Optional["DebitNote"],
-        previous_payable_debit_note: Optional["DebitNote"],
+        previous_debit_notes_count: int,
+        previous_payable_debit_notes_count: int,
         agreement_data: "AgreementData",
     ) -> Decimal:
         """Validate debit note payment data.
 
         Raises: PaymentValidationException
         """
         if agreement_data.agreement_duration is None:
@@ -141,16 +138,16 @@
 
         payment_props = PaymentProps.from_properties(agreement_data.properties)
         self.validate_mid_agreement_payment(
             self.activity.created_at,
             self.created_at,
             payment_props,
             debit_note_data.payment_due_date,
-            previous_debit_note.created_at if previous_debit_note else None,
-            previous_payable_debit_note.created_at if previous_payable_debit_note else None,
+            previous_debit_notes_count,
+            previous_payable_debit_notes_count,
         )
 
         coeffs = LinearCoeffs.from_properties(agreement_data.properties)
         if coeffs is None:
             raise PaymentValidationException("Unable to retrieve coeffs details")
 
         total_amount_due = eth_decimal(debit_note_data.total_amount_due)
@@ -190,21 +187,23 @@
             return
 
         agreement_data: "AgreementData" = await self.activity.agreement.get_agreement_data(
             force=True
         )
 
         previous_debit_note = await self.get_previous_debit_note()
-        previous_payable_debit_note = await self.get_previous_payable_debit_note()
+        previous_debit_notes_count = await self.get_previous_debit_notes_count()
+        previous_payable_debit_notes_count = await self.get_previous_payable_debit_notes_count()
 
         try:
             total_amount_due = self.validate_payment_data(
                 debit_note_data,
                 previous_debit_note,
-                previous_payable_debit_note,
+                previous_debit_notes_count,
+                previous_payable_debit_notes_count,
                 agreement_data,
             )
         except PaymentValidationException:
             logger.warning(f"Debit Note {self.id} validation failed", exc_info=True)
             return
 
         await self.accept(allocation, total_amount_due)
```

### Comparing `golem_core-0.6.2/golem/resources/debit_note/event_collectors.py` & `golem_core-0.6.3/golem/resources/debit_note/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/demand/demand.py` & `golem_core-0.6.3/golem/resources/demand/demand.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/demand/demand_builder.py` & `golem_core-0.6.3/golem/resources/demand/demand_builder.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/event_collectors.py` & `golem_core-0.6.3/golem/resources/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/events.py` & `golem_core-0.6.3/golem/resources/events.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/exceptions.py` & `golem_core-0.6.3/golem/resources/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/invoice/event_collectors.py` & `golem_core-0.6.3/golem/resources/invoice/event_collectors.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/invoice/invoice.py` & `golem_core-0.6.3/golem/resources/invoice/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
     def __init__(self, node: "GolemNode", id_: str, data: Optional[models.Invoice] = None):
         super().__init__(node, id_, data)
         asyncio.create_task(node.event_bus.emit(NewInvoice(self)))
 
     async def get_time_and_amount_since_latest_debit_notes(
         self, total_amount: Decimal
-    ) -> Tuple[timedelta, Decimal]:
+    ) -> Tuple[Optional[timedelta], Decimal]:
         """Get cumulative time and amount since last debit notes from all activities."""
         cumulative_time_from_all_activities = timedelta()
         cumulative_amount_from_all_activities = Decimal(0)
 
         for activity in self.agreement.activities:
             # Look for a newest Debit Note that came before the invoice
             for debit_note in sorted(
@@ -56,14 +56,17 @@
                 if debit_note.created_at < self.created_at:
                     cumulative_time_from_all_activities += self.created_at - debit_note.created_at
                     cumulative_amount_from_all_activities += eth_decimal(
                         debit_note.data.total_amount_due
                     )
                 break
 
+        if cumulative_time_from_all_activities == timedelta():
+            cumulative_time_from_all_activities = None  # type: ignore[assignment]
+
         return (
             cumulative_time_from_all_activities,
             total_amount - cumulative_amount_from_all_activities,
         )
 
     async def validate_and_accept(self, allocation: Allocation) -> None:
         """Validate invoice and accept using a given :any:`Allocation`."""
```

### Comparing `golem_core-0.6.2/golem/resources/network/exceptions.py` & `golem_core-0.6.3/golem/resources/network/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/network/network.py` & `golem_core-0.6.3/golem/resources/network/network.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/pooling_batch/exceptions.py` & `golem_core-0.6.3/golem/resources/pooling_batch/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/pooling_batch/pooling_batch.py` & `golem_core-0.6.3/golem/resources/pooling_batch/pooling_batch.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/proposal/exceptions.py` & `golem_core-0.6.3/golem/resources/proposal/exceptions.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/proposal/pipeline.py` & `golem_core-0.6.3/golem/resources/proposal/pipeline.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/proposal/proposal.py` & `golem_core-0.6.3/golem/resources/proposal/proposal.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/utils/infrastructure.py` & `golem_core-0.6.3/golem/resources/utils/infrastructure.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/resources/utils/payment.py` & `golem_core-0.6.3/golem/resources/utils/payment.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/asyncio/__init__.py` & `golem_core-0.6.3/golem/utils/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/asyncio/buffer.py` & `golem_core-0.6.3/golem/utils/asyncio/buffer.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/asyncio/queue.py` & `golem_core-0.6.3/golem/utils/asyncio/queue.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/asyncio/semaphore.py` & `golem_core-0.6.3/golem/utils/asyncio/semaphore.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/asyncio/tasks.py` & `golem_core-0.6.3/golem/utils/asyncio/tasks.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/asyncio/waiter.py` & `golem_core-0.6.3/golem/utils/asyncio/waiter.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/http.py` & `golem_core-0.6.3/golem/utils/http.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/logging.py` & `golem_core-0.6.3/golem/utils/logging.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/low/api.py` & `golem_core-0.6.3/golem/utils/low/api.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/low/event_collector.py` & `golem_core-0.6.3/golem/utils/low/event_collector.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/storage/base.py` & `golem_core-0.6.3/golem/utils/storage/base.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/storage/gftp/provider.py` & `golem_core-0.6.3/golem/utils/storage/gftp/provider.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/storage/utils.py` & `golem_core-0.6.3/golem/utils/storage/utils.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/golem/utils/typing.py` & `golem_core-0.6.3/golem/utils/typing.py`

 * *Files identical despite different names*

### Comparing `golem_core-0.6.2/pyproject.toml` & `golem_core-0.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "golem-core"
-version = "0.6.2"
+version = "0.6.3"
 description = "Golem Network (https://golem.network/) API for Python"
 authors = ["Golem Factory <contact@golem.network>"]
 license = "LGPL-3.0-or-later"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Framework :: AsyncIO",
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `golem_core-0.6.2/PKG-INFO` & `golem_core-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: golem-core
-Version: 0.6.2
+Version: 0.6.3
 Summary: Golem Network (https://golem.network/) API for Python
 Home-page: https://github.com/golemfactory/golem-core-python
 License: LGPL-3.0-or-later
 Author: Golem Factory
 Author-email: contact@golem.network
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

