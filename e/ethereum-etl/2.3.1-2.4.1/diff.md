# Comparing `tmp/ethereum-etl-2.3.1.tar.gz` & `tmp/ethereum-etl-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ethereum-etl-2.3.1.tar", last modified: Fri Aug 25 10:15:31 2023, max compression
+gzip compressed data, was "dist/ethereum-etl-2.4.1.tar", last modified: Wed Apr  3 04:44:03 2024, max compression
```

## Comparing `ethereum-etl-2.3.1.tar` & `ethereum-etl-2.4.1.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (999)     7078 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     5080 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/blockchainetl/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1475 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/atomic_counter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1633 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/csv_utils.py
--rw-r--r--   0 runner    (1001) docker     (999)     8631 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/exporters.py
--rw-r--r--   0 runner    (1001) docker     (999)     2529 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/file_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/blockchainetl/jobs/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1393 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/base_job.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     3430 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/composite_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1409 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/console_item_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1931 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/composite_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (999)     2129 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (999)     2041 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (999)     2445 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/list_field_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1849 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/simple_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1663 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py
--rw-r--r--   0 runner    (1001) docker     (999)     4025 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/gcs_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     4330 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1708 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/in_memory_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1701 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/kafka_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     2760 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/kinesis_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1677 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/multi_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     2644 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/jobs/exporters/postgres_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)      382 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/logging_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/blockchainetl/streaming/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      535 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/streaming/postgres_utils.py
--rw-r--r--   0 runner    (1001) docker     (999)     5599 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/streaming/streamer.py
--rw-r--r--   0 runner    (1001) docker     (999)      218 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/streaming/streamer_adapter_stub.py
--rw-r--r--   0 runner    (1001) docker     (999)      448 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/blockchainetl/streaming/streaming_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereum_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     7078 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereum_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     6927 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereum_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereum_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       53 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereum_etl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (999)      392 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereum_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)       32 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereum_etl.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1176 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1475 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/atomic_counter.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/cli/
--rw-r--r--   0 runner    (1001) docker     (999)     3807 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6012 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/export_all.py
--rw-r--r--   0 runner    (1001) docker     (999)     3817 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/export_blocks_and_transactions.py
--rw-r--r--   0 runner    (1001) docker     (999)     3384 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/export_contracts.py
--rw-r--r--   0 runner    (1001) docker     (999)     2853 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/export_geth_traces.py
--rw-r--r--   0 runner    (1001) docker     (999)     3121 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/export_origin.py
--rw-r--r--   0 runner    (1001) docker     (999)     3773 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/export_receipts_and_logs.py
--rw-r--r--   0 runner    (1001) docker     (999)     3120 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/export_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (999)     3088 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/export_tokens.py
--rw-r--r--   0 runner    (1001) docker     (999)     3720 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/export_traces.py
--rw-r--r--   0 runner    (1001) docker     (999)     2680 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/extract_contracts.py
--rw-r--r--   0 runner    (1001) docker     (999)     2069 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/extract_csv_column.py
--rw-r--r--   0 runner    (1001) docker     (999)     1778 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/extract_field.py
--rw-r--r--   0 runner    (1001) docker     (999)     2627 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/extract_geth_traces.py
--rw-r--r--   0 runner    (1001) docker     (999)     3079 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/extract_token_transfers.py
--rw-r--r--   0 runner    (1001) docker     (999)     3430 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/extract_tokens.py
--rw-r--r--   0 runner    (1001) docker     (999)     1925 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/filter_items.py
--rw-r--r--   0 runner    (1001) docker     (999)     2762 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/get_block_range_for_date.py
--rw-r--r--   0 runner    (1001) docker     (999)     2872 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/get_block_range_for_timestamps.py
--rw-r--r--   0 runner    (1001) docker     (999)     1927 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/get_keccak_hash.py
--rw-r--r--   0 runner    (1001) docker     (999)     5551 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/cli/stream.py
--rw-r--r--   0 runner    (1001) docker     (999)     1633 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/csv_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/domain/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1868 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/block.py
--rw-r--r--   0 runner    (1001) docker     (999)     1376 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/contract.py
--rw-r--r--   0 runner    (1001) docker     (999)     1262 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/geth_trace.py
--rw-r--r--   0 runner    (1001) docker     (999)      931 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/origin.py
--rw-r--r--   0 runner    (1001) docker     (999)     1682 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/receipt.py
--rw-r--r--   0 runner    (1001) docker     (999)     1437 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/receipt_log.py
--rw-r--r--   0 runner    (1001) docker     (999)     1360 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/token.py
--rw-r--r--   0 runner    (1001) docker     (999)     1417 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/token_transfer.py
--rw-r--r--   0 runner    (1001) docker     (999)     1758 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/trace.py
--rw-r--r--   0 runner    (1001) docker     (999)     1632 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/domain/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/enumeration/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/enumeration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      368 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/enumeration/entity_type.py
--rw-r--r--   0 runner    (1001) docker     (999)     8039 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/erc20_abi.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/executors/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     5519 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/executors/batch_work_executor.py
--rw-r--r--   0 runner    (1001) docker     (999)     2256 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/executors/bounded_executor.py
--rw-r--r--   0 runner    (1001) docker     (999)     1944 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/executors/fail_safe_executor.py
--rw-r--r--   0 runner    (1001) docker     (999)     8132 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/exporters.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/ipfs/
--rw-r--r--   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/ipfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1028 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/ipfs/client.py
--rw-r--r--   0 runner    (1001) docker     (999)     6099 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/ipfs/origin.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/jobs/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    12978 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/export_all_common.py
--rw-r--r--   0 runner    (1001) docker     (999)     3727 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/export_blocks_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     3734 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/export_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     3188 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/export_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     5671 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/export_origin_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     3498 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/export_receipts_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     4061 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/export_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2882 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/export_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     4665 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/export_traces_job.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/jobs/exporters/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2343 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1601 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/exporters/contracts_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1548 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/exporters/geth_traces_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1190 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/exporters/origin_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     2064 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1697 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/exporters/token_transfers_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1618 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/exporters/tokens_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     1786 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/exporters/traces_item_exporter.py
--rw-r--r--   0 runner    (1001) docker     (999)     3547 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/extract_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2496 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/extract_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2762 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/extract_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     1863 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/jobs/extract_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2620 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/json_rpc_requests.py
--rw-r--r--   0 runner    (1001) docker     (999)    11649 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mainnet_daofork_state_changes.py
--rw-r--r--   0 runner    (1001) docker     (999)   673817 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mainnet_genesis_alloc.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/mappers/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4713 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/block_mapper.py
--rw-r--r--   0 runner    (1001) docker     (999)     1821 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/contract_mapper.py
--rw-r--r--   0 runner    (1001) docker     (999)     1709 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/geth_trace_mapper.py
--rw-r--r--   0 runner    (1001) docker     (999)     1497 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/origin_mapper.py
--rw-r--r--   0 runner    (1001) docker     (999)     4015 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/receipt_log_mapper.py
--rw-r--r--   0 runner    (1001) docker     (999)     3686 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/receipt_mapper.py
--rw-r--r--   0 runner    (1001) docker     (999)     1500 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/token_mapper.py
--rw-r--r--   0 runner    (1001) docker     (999)     1679 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/token_transfer_mapper.py
--rw-r--r--   0 runner    (1001) docker     (999)     7027 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/trace_mapper.py
--rw-r--r--   0 runner    (1001) docker     (999)     3359 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/mappers/transaction_mapper.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/misc/
--rw-r--r--   0 runner    (1001) docker     (999)     1135 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/misc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)       48 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/misc/retriable_value_error.py
--rw-r--r--   0 runner    (1001) docker     (999)     2757 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (999)     3663 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/progress_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/providers/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     2010 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/providers/auto.py
--rw-r--r--   0 runner    (1001) docker     (999)     3146 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/providers/ipc.py
--rw-r--r--   0 runner    (1001) docker     (999)     2032 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/providers/rpc.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/service/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     4258 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/service/eth_contract_service.py
--rw-r--r--   0 runner    (1001) docker     (999)     3463 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/service/eth_service.py
--rw-r--r--   0 runner    (1001) docker     (999)     1894 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/service/eth_special_trace_service.py
--rw-r--r--   0 runner    (1001) docker     (999)     4841 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/service/eth_token_service.py
--rw-r--r--   0 runner    (1001) docker     (999)     5489 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/service/graph_operations.py
--rw-r--r--   0 runner    (1001) docker     (999)     2481 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/service/origin_extractor.py
--rw-r--r--   0 runner    (1001) docker     (999)     3445 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/service/token_transfer_extractor.py
--rw-r--r--   0 runner    (1001) docker     (999)     2943 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/service/trace_id_calculator.py
--rw-r--r--   0 runner    (1001) docker     (999)     2991 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/service/trace_status_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/ethereumetl/streaming/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     6785 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/streaming/enrich.py
--rw-r--r--   0 runner    (1001) docker     (999)     2740 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/streaming/eth_item_id_calculator.py
--rw-r--r--   0 runner    (1001) docker     (999)     1866 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/streaming/eth_item_timestamp_calculator.py
--rw-r--r--   0 runner    (1001) docker     (999)     9750 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/streaming/eth_streamer_adapter.py
--rw-r--r--   0 runner    (1001) docker     (999)     6476 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/streaming/item_exporter_creator.py
--rw-r--r--   0 runner    (1001) docker     (999)     5713 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/streaming/postgres_tables.py
--rw-r--r--   0 runner    (1001) docker     (999)     1639 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/thread_local_proxy.py
--rw-r--r--   0 runner    (1001) docker     (999)     4758 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/utils.py
--rw-r--r--   0 runner    (1001) docker     (999)     1333 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/ethereumetl/web3_utils.py
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (999)     2533 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/tests/ethereumetl/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/
--rw-r--r--   0 runner    (1001) docker     (999)     1260 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)     1379 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/helpers.py
--rw-r--r--   0 runner    (1001) docker     (999)     1807 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/mock_batch_web3_provider.py
--rw-r--r--   0 runner    (1001) docker     (999)      436 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/mock_ipfs_client.py
--rw-r--r--   0 runner    (1001) docker     (999)     1943 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/mock_web3_provider.py
--rw-r--r--   0 runner    (1001) docker     (999)     3722 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_blocks_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2968 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_contracts_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2848 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2401 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_origin_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     3704 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_receipts_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2619 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_token_transfers_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2774 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_tokens_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2843 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2436 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/test_extract_geth_traces_job.py
--rw-r--r--   0 runner    (1001) docker     (999)     2272 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/job/test_extract_token_transfers_job.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/tests/ethereumetl/service/
--rw-r--r--   0 runner    (1001) docker     (999)     1137 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    70321 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/service/test_eth_contract_service.py
--rw-r--r--   0 runner    (1001) docker     (999)     3612 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/service/test_eth_service.py
--rw-r--r--   0 runner    (1001) docker     (999)     2585 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/service/test_token_transfer_extractor.py
--rw-r--r--   0 runner    (1001) docker     (999)     2465 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/ethereumetl/test_progress_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-25 10:15:31.000000 ethereum-etl-2.3.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (999)     1530 2023-08-25 10:15:30.000000 ethereum-etl-2.3.1/tests/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5080 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/blockchainetl/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/atomic_counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/csv_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8631 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/exporters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2529 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/file_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/blockchainetl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/base_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/composite_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/console_item_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/composite_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/list_field_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/simple_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1663 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4025 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/gcs_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4330 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1708 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/in_memory_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/kafka_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/kinesis_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/multi_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/jobs/exporters/postgres_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/logging_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/blockchainetl/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/streaming/postgres_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5599 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/streaming/streamer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/streaming/streamer_adapter_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/blockchainetl/streaming/streaming_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7078 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereum_etl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/atomic_counter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     3807 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3817 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_blocks_and_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3384 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_geth_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3121 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3773 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_receipts_and_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/export_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_contracts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_csv_column.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2627 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_geth_traces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_token_transfers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/extract_tokens.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/filter_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/get_block_range_for_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2872 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/get_block_range_for_timestamps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/get_keccak_hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5551 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/cli/stream.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/csv_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/domain/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/geth_trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/origin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1742 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/receipt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/receipt_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/token_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/trace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/domain/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/enumeration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/enumeration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/enumeration/entity_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8039 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/erc20_abi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/executors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/executors/batch_work_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2256 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/executors/bounded_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/executors/fail_safe_executor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8132 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/exporters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/ipfs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/ipfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/ipfs/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6099 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/ipfs/origin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/jobs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_all_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3727 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_blocks_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3734 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3188 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5671 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_origin_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_receipts_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2882 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4665 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/export_traces_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2444 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/contracts_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/geth_traces_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/origin_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1697 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/token_transfers_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1618 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/tokens_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/exporters/traces_item_exporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/extract_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2496 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/extract_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/extract_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/jobs/extract_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/json_rpc_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11649 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mainnet_daofork_state_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)   673817 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mainnet_genesis_alloc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/mappers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4963 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/block_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/contract_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/geth_trace_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/origin_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/receipt_log_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/receipt_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/token_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/token_transfer_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/trace_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/mappers/transaction_mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/misc/
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/misc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/misc/retriable_value_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/progress_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/providers/auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/providers/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/providers/rpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/eth_contract_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3463 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/eth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/eth_special_trace_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4841 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/eth_token_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/graph_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/origin_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3445 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/token_transfer_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/trace_id_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2991 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/service/trace_status_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/ethereumetl/streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6971 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/eth_item_id_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1866 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/eth_item_timestamp_calculator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9750 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/eth_streamer_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6476 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/item_exporter_creator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/streaming/postgres_tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/thread_local_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4758 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/ethereumetl/web3_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2533 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/tests/ethereumetl/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/mock_batch_web3_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/mock_ipfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/mock_web3_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3801 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_blocks_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_contracts_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_origin_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_receipts_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_token_transfers_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2774 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_tokens_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_extract_geth_traces_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/job/test_extract_token_transfers_job.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/tests/ethereumetl/service/
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70321 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/service/test_eth_contract_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/service/test_eth_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2585 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/service/test_token_transfer_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/ethereumetl/test_progress_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-03 04:44:03.000000 ethereum-etl-2.4.1/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-03 04:44:00.000000 ethereum-etl-2.4.1/tests/resources/__init__.py
```

### Comparing `ethereum-etl-2.3.1/PKG-INFO` & `ethereum-etl-2.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethereum-etl
-Version: 2.3.1
+Version: 2.4.1
 Summary: Tools for exporting Ethereum blockchain data to CSV or JSON
 Home-page: https://github.com/blockchain-etl/ethereum-etl
 Author: Evgeny Medvedev
 Author-email: evge.medvedev@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blockchain-etl/ethereum-etl/issues
 Project-URL: Chat, https://gitter.im/ethereum-etl/Lobby
```

### Comparing `ethereum-etl-2.3.1/README.md` & `ethereum-etl-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/atomic_counter.py` & `ethereum-etl-2.4.1/blockchainetl/atomic_counter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/csv_utils.py` & `ethereum-etl-2.4.1/blockchainetl/csv_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/exporters.py` & `ethereum-etl-2.4.1/blockchainetl/exporters.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/file_utils.py` & `ethereum-etl-2.4.1/blockchainetl/file_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/base_job.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/base_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/composite_item_exporter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/composite_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/console_item_exporter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/console_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/composite_item_converter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/composite_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/int_to_decimal_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/int_to_string_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/list_field_item_converter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/list_field_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/simple_item_converter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/simple_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/converters/unix_timestamp_item_converter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/gcs_item_exporter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/gcs_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/google_pubsub_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/in_memory_item_exporter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/in_memory_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/kafka_exporter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/kafka_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/kinesis_item_exporter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/kinesis_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/multi_item_exporter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/multi_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/jobs/exporters/postgres_item_exporter.py` & `ethereum-etl-2.4.1/blockchainetl/jobs/exporters/postgres_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/streaming/__init__.py` & `ethereum-etl-2.4.1/blockchainetl/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/streaming/postgres_utils.py` & `ethereum-etl-2.4.1/blockchainetl/streaming/postgres_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/blockchainetl/streaming/streamer.py` & `ethereum-etl-2.4.1/blockchainetl/streaming/streamer.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereum_etl.egg-info/PKG-INFO` & `ethereum-etl-2.4.1/ethereum_etl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ethereum-etl
-Version: 2.3.1
+Version: 2.4.1
 Summary: Tools for exporting Ethereum blockchain data to CSV or JSON
 Home-page: https://github.com/blockchain-etl/ethereum-etl
 Author: Evgeny Medvedev
 Author-email: evge.medvedev@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/blockchain-etl/ethereum-etl/issues
 Project-URL: Chat, https://gitter.im/ethereum-etl/Lobby
```

### Comparing `ethereum-etl-2.3.1/ethereum_etl.egg-info/SOURCES.txt` & `ethereum-etl-2.4.1/ethereum_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/__main__.py` & `ethereum-etl-2.4.1/ethereumetl/__main__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/atomic_counter.py` & `ethereum-etl-2.4.1/ethereumetl/atomic_counter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from ethereumetl.cli.get_block_range_for_date import get_block_range_for_date
 from ethereumetl.cli.get_block_range_for_timestamps import get_block_range_for_timestamps
 from ethereumetl.cli.get_keccak_hash import get_keccak_hash
 from ethereumetl.cli.stream import stream
 
 
 @click.group()
-@click.version_option(version='2.3.1')
+@click.version_option(version='2.4.1')
 @click.pass_context
 def cli(ctx):
     pass
 
 
 # export
 cli.add_command(export_all, "export_all")
```

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/export_all.py` & `ethereum-etl-2.4.1/ethereumetl/cli/export_all.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/export_blocks_and_transactions.py` & `ethereum-etl-2.4.1/ethereumetl/cli/export_blocks_and_transactions.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/export_contracts.py` & `ethereum-etl-2.4.1/ethereumetl/cli/export_contracts.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/export_geth_traces.py` & `ethereum-etl-2.4.1/ethereumetl/cli/export_geth_traces.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/export_origin.py` & `ethereum-etl-2.4.1/ethereumetl/cli/export_origin.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/export_receipts_and_logs.py` & `ethereum-etl-2.4.1/ethereumetl/cli/export_receipts_and_logs.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/export_token_transfers.py` & `ethereum-etl-2.4.1/ethereumetl/cli/export_token_transfers.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/export_tokens.py` & `ethereum-etl-2.4.1/ethereumetl/cli/export_tokens.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/export_traces.py` & `ethereum-etl-2.4.1/ethereumetl/cli/export_traces.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/extract_contracts.py` & `ethereum-etl-2.4.1/ethereumetl/cli/extract_contracts.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/extract_csv_column.py` & `ethereum-etl-2.4.1/ethereumetl/cli/extract_csv_column.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/extract_field.py` & `ethereum-etl-2.4.1/ethereumetl/cli/extract_field.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/extract_geth_traces.py` & `ethereum-etl-2.4.1/ethereumetl/cli/extract_geth_traces.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/extract_token_transfers.py` & `ethereum-etl-2.4.1/ethereumetl/cli/extract_token_transfers.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/extract_tokens.py` & `ethereum-etl-2.4.1/ethereumetl/cli/extract_tokens.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/filter_items.py` & `ethereum-etl-2.4.1/ethereumetl/cli/filter_items.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/get_block_range_for_date.py` & `ethereum-etl-2.4.1/ethereumetl/cli/get_block_range_for_date.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/get_block_range_for_timestamps.py` & `ethereum-etl-2.4.1/ethereumetl/cli/get_block_range_for_timestamps.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/get_keccak_hash.py` & `ethereum-etl-2.4.1/ethereumetl/cli/get_keccak_hash.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/cli/stream.py` & `ethereum-etl-2.4.1/ethereumetl/cli/stream.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/csv_utils.py` & `ethereum-etl-2.4.1/ethereumetl/csv_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/domain/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/block.py` & `ethereum-etl-2.4.1/ethereumetl/domain/block.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,7 +42,10 @@
         self.timestamp = None
         self.withdrawals_root = None
 
         self.transactions = []
         self.transaction_count = 0
         self.base_fee_per_gas = 0
         self.withdrawals = []
+
+        self.blob_gas_used = None
+        self.excess_blob_gas = None
```

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/contract.py` & `ethereum-etl-2.4.1/ethereumetl/domain/contract.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/geth_trace.py` & `ethereum-etl-2.4.1/ethereumetl/domain/geth_trace.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/origin.py` & `ethereum-etl-2.4.1/ethereumetl/domain/origin.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/receipt.py` & `ethereum-etl-2.4.1/ethereumetl/domain/receipt.py`

 * *Files 18% similar despite different names*

```diff
@@ -34,8 +34,9 @@
         self.root = None
         self.status = None
         self.effective_gas_price = None
         self.l1_fee = None
         self.l1_gas_used = None
         self.l1_gas_price = None
         self.l1_fee_scalar = None
-        
+        self.blob_gas_price = None
+        self.blob_gas_used = None
```

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/receipt_log.py` & `ethereum-etl-2.4.1/ethereumetl/domain/receipt_log.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/token.py` & `ethereum-etl-2.4.1/ethereumetl/domain/token.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/token_transfer.py` & `ethereum-etl-2.4.1/ethereumetl/domain/token_transfer.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/trace.py` & `ethereum-etl-2.4.1/ethereumetl/domain/trace.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/domain/transaction.py` & `ethereum-etl-2.4.1/ethereumetl/domain/transaction.py`

 * *Files 10% similar despite different names*

```diff
@@ -33,7 +33,9 @@
         self.value = None
         self.gas = None
         self.gas_price = None
         self.input = None
         self.max_fee_per_gas = None
         self.max_priority_fee_per_gas = None
         self.transaction_type = None
+        self.max_fee_per_blob_gas = None
+        self.blob_versioned_hashes = []
```

### Comparing `ethereum-etl-2.3.1/ethereumetl/erc20_abi.py` & `ethereum-etl-2.4.1/ethereumetl/erc20_abi.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/executors/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/executors/batch_work_executor.py` & `ethereum-etl-2.4.1/ethereumetl/executors/batch_work_executor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/executors/bounded_executor.py` & `ethereum-etl-2.4.1/ethereumetl/executors/bounded_executor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/executors/fail_safe_executor.py` & `ethereum-etl-2.4.1/ethereumetl/executors/fail_safe_executor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/exporters.py` & `ethereum-etl-2.4.1/ethereumetl/exporters.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/ipfs/client.py` & `ethereum-etl-2.4.1/ethereumetl/ipfs/client.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/ipfs/origin.py` & `ethereum-etl-2.4.1/ethereumetl/ipfs/origin.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/export_all_common.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/export_all_common.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/export_blocks_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/export_blocks_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/export_contracts_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/export_contracts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/export_geth_traces_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/export_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/export_origin_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/export_origin_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/export_receipts_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/export_receipts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/export_token_transfers_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/export_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/export_tokens_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/export_tokens_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/export_traces_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/export_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/exporters/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/blocks_and_transactions_item_exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,17 @@
     'extra_data',
     'gas_limit',
     'gas_used',
     'timestamp',
     'transaction_count',
     'base_fee_per_gas',
     'withdrawals_root',
-    'withdrawals'
+    'withdrawals',
+    'blob_gas_used',
+    'excess_blob_gas'
 ]
 
 TRANSACTION_FIELDS_TO_EXPORT = [
     'hash',
     'nonce',
     'block_hash',
     'block_number',
@@ -58,15 +60,17 @@
     'value',
     'gas',
     'gas_price',
     'input',
     'block_timestamp',
     'max_fee_per_gas',
     'max_priority_fee_per_gas',
-    'transaction_type'
+    'transaction_type',
+    'max_fee_per_blob_gas',
+    'blob_versioned_hashes'
 ]
 
 
 def blocks_and_transactions_item_exporter(blocks_output=None, transactions_output=None):
     return CompositeItemExporter(
         filename_mapping={
             'block': blocks_output,
```

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/exporters/contracts_item_exporter.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/contracts_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/exporters/geth_traces_item_exporter.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/geth_traces_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/exporters/origin_exporter.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/origin_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/receipts_and_logs_item_exporter.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,16 +33,17 @@
     'contract_address',
     'root',
     'status',
     'effective_gas_price',
     'l1_fee',
     'l1_gas_used',
     'l1_gas_price',
-    'l1_fee_scalar'
-    
+    'l1_fee_scalar',
+    'blob_gas_price',
+    'blob_gas_used'
 ]
 
 LOG_FIELDS_TO_EXPORT = [
     'log_index',
     'transaction_hash',
     'transaction_index',
     'block_hash',
```

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/exporters/token_transfers_item_exporter.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/token_transfers_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/exporters/tokens_item_exporter.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/tokens_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/exporters/traces_item_exporter.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/exporters/traces_item_exporter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/extract_contracts_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/extract_contracts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/extract_geth_traces_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/extract_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/extract_token_transfers_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/extract_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/jobs/extract_tokens_job.py` & `ethereum-etl-2.4.1/ethereumetl/jobs/extract_tokens_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/json_rpc_requests.py` & `ethereum-etl-2.4.1/ethereumetl/json_rpc_requests.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mainnet_daofork_state_changes.py` & `ethereum-etl-2.4.1/ethereumetl/mainnet_daofork_state_changes.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mainnet_genesis_alloc.py` & `ethereum-etl-2.4.1/ethereumetl/mainnet_genesis_alloc.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/block_mapper.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/block_mapper.py`

 * *Files 19% similar despite different names*

```diff
@@ -50,14 +50,16 @@
         block.size = hex_to_dec(json_dict.get('size'))
         block.extra_data = json_dict.get('extraData')
         block.gas_limit = hex_to_dec(json_dict.get('gasLimit'))
         block.gas_used = hex_to_dec(json_dict.get('gasUsed'))
         block.timestamp = hex_to_dec(json_dict.get('timestamp'))
         block.base_fee_per_gas = hex_to_dec(json_dict.get('baseFeePerGas'))
         block.withdrawals_root = json_dict.get('withdrawalsRoot')
+        block.blob_gas_used = hex_to_dec(json_dict.get('blobGasUsed'))
+        block.excess_blob_gas = hex_to_dec(json_dict.get('excessBlobGas'))
 
         if 'transactions' in json_dict:
             block.transactions = [
                 self.transaction_mapper.json_dict_to_transaction(tx, block_timestamp=block.timestamp)
                 for tx in json_dict['transactions']
                 if isinstance(tx, dict)
             ]
@@ -100,8 +102,10 @@
             'gas_limit': block.gas_limit,
             'gas_used': block.gas_used,
             'timestamp': block.timestamp,
             'transaction_count': block.transaction_count,
             'base_fee_per_gas': block.base_fee_per_gas,
             'withdrawals_root': block.withdrawals_root,
             'withdrawals': block.withdrawals,
+            'blob_gas_used': block.blob_gas_used,
+            'excess_blob_gas': block.excess_blob_gas,
         }
```

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/contract_mapper.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/contract_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/geth_trace_mapper.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/geth_trace_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/origin_mapper.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/origin_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/receipt_log_mapper.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/receipt_log_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/receipt_mapper.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/receipt_mapper.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 
         receipt.effective_gas_price = hex_to_dec(json_dict.get('effectiveGasPrice'))
 
         receipt.l1_fee = hex_to_dec(json_dict.get('l1Fee'))
         receipt.l1_gas_used = hex_to_dec(json_dict.get('l1GasUsed'))
         receipt.l1_gas_price = hex_to_dec(json_dict.get('l1GasPrice'))
         receipt.l1_fee_scalar = to_float_or_none(json_dict.get('l1FeeScalar'))
-        
+        receipt.blob_gas_price = hex_to_dec(json_dict.get('blobGasPrice'))
+        receipt.blob_gas_used = hex_to_dec(json_dict.get('blobGasUsed'))
 
         if 'logs' in json_dict:
             receipt.logs = [
                 self.receipt_log_mapper.json_dict_to_receipt_log(log) for log in json_dict['logs']
             ]
 
         return receipt
@@ -75,10 +76,11 @@
             'contract_address': receipt.contract_address,
             'root': receipt.root,
             'status': receipt.status,
             'effective_gas_price': receipt.effective_gas_price,
             'l1_fee': receipt.l1_fee,
             'l1_gas_used': receipt.l1_gas_used,
             'l1_gas_price': receipt.l1_gas_price,
-            'l1_fee_scalar': receipt.l1_fee_scalar
-            
+            'l1_fee_scalar': receipt.l1_fee_scalar,
+            'blob_gas_price': receipt.blob_gas_price,
+            'blob_gas_used': receipt.blob_gas_used
         }
```

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/token_mapper.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/token_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/token_transfer_mapper.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/token_transfer_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/trace_mapper.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/trace_mapper.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/mappers/transaction_mapper.py` & `ethereum-etl-2.4.1/ethereumetl/mappers/transaction_mapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -39,14 +39,19 @@
         transaction.value = hex_to_dec(json_dict.get('value'))
         transaction.gas = hex_to_dec(json_dict.get('gas'))
         transaction.gas_price = hex_to_dec(json_dict.get('gasPrice'))
         transaction.input = json_dict.get('input')
         transaction.max_fee_per_gas = hex_to_dec(json_dict.get('maxFeePerGas'))
         transaction.max_priority_fee_per_gas = hex_to_dec(json_dict.get('maxPriorityFeePerGas'))
         transaction.transaction_type = hex_to_dec(json_dict.get('type'))
+        transaction.max_fee_per_blob_gas = hex_to_dec(json_dict.get('maxFeePerBlobGas'))
+
+        if 'blobVersionedHashes' in json_dict and isinstance(json_dict['blobVersionedHashes'], list):
+            transaction.blob_versioned_hashes = json_dict['blobVersionedHashes']
+
         return transaction
 
     def transaction_to_dict(self, transaction):
         return {
             'type': 'transaction',
             'hash': transaction.hash,
             'nonce': transaction.nonce,
@@ -58,9 +63,11 @@
             'to_address': transaction.to_address,
             'value': transaction.value,
             'gas': transaction.gas,
             'gas_price': transaction.gas_price,
             'input': transaction.input,
             'max_fee_per_gas': transaction.max_fee_per_gas,
             'max_priority_fee_per_gas': transaction.max_priority_fee_per_gas,
-            'transaction_type': transaction.transaction_type
+            'transaction_type': transaction.transaction_type,
+            "max_fee_per_blob_gas": transaction.max_fee_per_blob_gas,
+            "blob_versioned_hashes": transaction.blob_versioned_hashes
         }
```

### Comparing `ethereum-etl-2.3.1/ethereumetl/misc/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/misc/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/misc_utils.py` & `ethereum-etl-2.4.1/ethereumetl/misc_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/progress_logger.py` & `ethereum-etl-2.4.1/ethereumetl/progress_logger.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/providers/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/providers/auto.py` & `ethereum-etl-2.4.1/ethereumetl/providers/auto.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/providers/ipc.py` & `ethereum-etl-2.4.1/ethereumetl/providers/ipc.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/providers/rpc.py` & `ethereum-etl-2.4.1/ethereumetl/providers/rpc.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/service/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/service/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/service/eth_contract_service.py` & `ethereum-etl-2.4.1/ethereumetl/service/eth_contract_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/service/eth_service.py` & `ethereum-etl-2.4.1/ethereumetl/service/eth_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/service/eth_special_trace_service.py` & `ethereum-etl-2.4.1/ethereumetl/service/eth_special_trace_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/service/eth_token_service.py` & `ethereum-etl-2.4.1/ethereumetl/service/eth_token_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/service/graph_operations.py` & `ethereum-etl-2.4.1/ethereumetl/service/graph_operations.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/service/origin_extractor.py` & `ethereum-etl-2.4.1/ethereumetl/service/origin_extractor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/service/token_transfer_extractor.py` & `ethereum-etl-2.4.1/ethereumetl/service/token_transfer_extractor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/service/trace_id_calculator.py` & `ethereum-etl-2.4.1/ethereumetl/service/trace_id_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/service/trace_status_calculator.py` & `ethereum-etl-2.4.1/ethereumetl/service/trace_status_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/streaming/__init__.py` & `ethereum-etl-2.4.1/ethereumetl/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/streaming/enrich.py` & `ethereum-etl-2.4.1/ethereumetl/streaming/enrich.py`

 * *Files 6% similar despite different names*

```diff
@@ -72,28 +72,31 @@
             'gas_price',
             'input',
             'block_timestamp',
             'block_number',
             'block_hash',
             'max_fee_per_gas',
             'max_priority_fee_per_gas',
-            'transaction_type'
+            'transaction_type',
+            'max_fee_per_blob_gas',
+            'blob_versioned_hashes'
         ],
         right_fields=[
             ('cumulative_gas_used', 'receipt_cumulative_gas_used'),
             ('gas_used', 'receipt_gas_used'),
             ('contract_address', 'receipt_contract_address'),
             ('root', 'receipt_root'),
             ('status', 'receipt_status'),
             ('effective_gas_price', 'receipt_effective_gas_price'),
             ('l1_fee', 'receipt_l1_fee'),
             ('l1_gas_used', 'receipt_l1_gas_used'),
             ('l1_gas_price', 'receipt_l1_gas_price'),
-            ('l1_fee_scalar', 'receipt_l1_fee_scalar')
-
+            ('l1_fee_scalar', 'receipt_l1_fee_scalar'),
+            ('blob_gas_price', 'receipt_blob_gas_price'),
+            ('blob_gas_used', 'receipt_blob_gas_used')
         ]))
 
     if len(result) != len(transactions):
         raise ValueError('The number of transactions is wrong ' + str(result))
 
     return result
```

### Comparing `ethereum-etl-2.3.1/ethereumetl/streaming/eth_item_id_calculator.py` & `ethereum-etl-2.4.1/ethereumetl/streaming/eth_item_id_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/streaming/eth_item_timestamp_calculator.py` & `ethereum-etl-2.4.1/ethereumetl/streaming/eth_item_timestamp_calculator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/streaming/eth_streamer_adapter.py` & `ethereum-etl-2.4.1/ethereumetl/streaming/eth_streamer_adapter.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/streaming/item_exporter_creator.py` & `ethereum-etl-2.4.1/ethereumetl/streaming/item_exporter_creator.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/streaming/postgres_tables.py` & `ethereum-etl-2.4.1/ethereumetl/streaming/postgres_tables.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/thread_local_proxy.py` & `ethereum-etl-2.4.1/ethereumetl/thread_local_proxy.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/utils.py` & `ethereum-etl-2.4.1/ethereumetl/utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/ethereumetl/web3_utils.py` & `ethereum-etl-2.4.1/ethereumetl/web3_utils.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/setup.py` & `ethereum-etl-2.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 long_description = read('README.md') if os.path.isfile("README.md") else ""
 
 setup(
     name='ethereum-etl',
-    version='2.3.1',
+    version='2.4.1',
     author='Evgeny Medvedev',
     author_email='evge.medvedev@gmail.com',
     description='Tools for exporting Ethereum blockchain data to CSV or JSON',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/blockchain-etl/ethereum-etl',
     packages=find_packages(exclude=['schemas', 'tests']),
```

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/__init__.py` & `ethereum-etl-2.4.1/tests/ethereumetl/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/__init__.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/helpers.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/helpers.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/mock_batch_web3_provider.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/mock_batch_web3_provider.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/mock_web3_provider.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/mock_web3_provider.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_blocks_job.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_blocks_job.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 
 
 @pytest.mark.parametrize("start_block,end_block,batch_size,resource_group,web3_provider_type,format", [
     (0, 0, 1, 'block_without_transactions', 'mock', 'csv'),
     (483920, 483920, 1, 'block_with_logs', 'mock', 'csv'),
     (47218, 47219, 1, 'blocks_with_transactions', 'mock', 'csv'),
     (47218, 47219, 2, 'blocks_with_transactions', 'mock', 'csv'),
+    (19537146, 19537146, 1, 'blocks_with_dencun_transactions', 'mock', 'csv'),
     skip_if_slow_tests_disabled((0, 0, 1, 'block_without_transactions', 'infura', 'csv')),
     skip_if_slow_tests_disabled((483920, 483920, 1, 'block_with_logs', 'infura', 'csv')),
     skip_if_slow_tests_disabled((47218, 47219, 2, 'blocks_with_transactions', 'infura', 'csv')),
     skip_if_slow_tests_disabled((17173049, 17173050, 2, 'blocks_with_transactions_and_withdrawals', 'infura', 'csv')),
     skip_if_slow_tests_disabled((17173049, 17173050, 2, 'blocks_with_transactions_and_withdrawals', 'infura', 'json')),
 ])
 def test_export_blocks_job(tmpdir, start_block, end_block, batch_size, resource_group, web3_provider_type, format):
```

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_contracts_job.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_contracts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_geth_traces_job.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_origin_job.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_origin_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_receipts_job.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_receipts_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_token_transfers_job.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_tokens_job.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_tokens_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/test_export_traces_job.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/test_export_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/test_extract_geth_traces_job.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/test_extract_geth_traces_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/job/test_extract_token_transfers_job.py` & `ethereum-etl-2.4.1/tests/ethereumetl/job/test_extract_token_transfers_job.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/service/__init__.py` & `ethereum-etl-2.4.1/tests/ethereumetl/service/__init__.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/service/test_eth_contract_service.py` & `ethereum-etl-2.4.1/tests/ethereumetl/service/test_eth_contract_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/service/test_eth_service.py` & `ethereum-etl-2.4.1/tests/ethereumetl/service/test_eth_service.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/service/test_token_transfer_extractor.py` & `ethereum-etl-2.4.1/tests/ethereumetl/service/test_token_transfer_extractor.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/ethereumetl/test_progress_logger.py` & `ethereum-etl-2.4.1/tests/ethereumetl/test_progress_logger.py`

 * *Files identical despite different names*

### Comparing `ethereum-etl-2.3.1/tests/resources/__init__.py` & `ethereum-etl-2.4.1/tests/resources/__init__.py`

 * *Files identical despite different names*

