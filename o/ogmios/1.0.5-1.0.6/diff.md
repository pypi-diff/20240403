# Comparing `tmp/ogmios-1.0.5.tar.gz` & `tmp/ogmios-1.0.6.tar.gz`

## Comparing `ogmios-1.0.5.tar` & `ogmios-1.0.6.tar`

### file list

```diff
@@ -1,103 +1,104 @@
--rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 ogmios-1.0.5/.readthedocs.yaml
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ogmios-1.0.5/examples/async_queries.py
--rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 ogmios-1.0.5/examples/build_tx_cardanotools.py
--rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 ogmios-1.0.5/examples/build_tx_pycardano.py
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 ogmios-1.0.5/examples/find_wallet_transactions.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 ogmios-1.0.5/examples/get_mempool_contents.py
--rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ogmios-1.0.5/examples/live_block_viewer.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 ogmios-1.0.5/examples/print_first_shelley_blocks.py
--rwxr-xr-x   0        0        0      344 2020-02-02 00:00:00.000000 ogmios-1.0.5/scripts/generate_models.sh
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/__about__.py
--rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/__init__.py
--rw-r--r--   0        0        0    12012 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/chain_context.py
--rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/client.py
--rw-r--r--   0        0        0    39598 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/datatypes.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/errors.py
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/logger.py
--rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/response_handler.py
--rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/utils.py
--rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/chainsync/FindIntersection.py
--rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/chainsync/NextBlock.py
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/chainsync/__init__.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/mempool/AcquireMempool.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/mempool/HasTransaction.py
--rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/mempool/NextTransaction.py
--rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/mempool/ReleaseMempool.py
--rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/mempool/SizeOfMempool.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/mempool/__init__.py
--rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/model/README.md
--rw-r--r--   0        0        0    84579 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/model/cardano.json
--rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/model/cardano_model.py
--rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/model/model_map.py
--rw-r--r--   0        0        0   155521 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/model/ogmios.json
--rw-r--r--   0        0        0   118872 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/model/ogmios_model.py
--rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/AcquireLedgerState.py
--rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryBlockHeight.py
--rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryEpoch.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryEraStart.py
--rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryEraSummaries.py
--rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryGenesisConfiguration.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryLedgerTip.py
--rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryLiveStakeDistribution.py
--rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryNetworkTip.py
--rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryProjectedRewards.py
--rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryProposedProtocolParameters.py
--rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryProtocolParameters.py
--rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryRewardAccountSummaries.py
--rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryRewardsProvenance.py
--rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryStakePools.py
--rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryStartTime.py
--rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/QueryUtxo.py
--rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/statequery/__init__.py
--rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/txsubmit/EvaluateTransaction.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/txsubmit/SubmitTransaction.py
--rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ogmios-1.0.5/src/ogmios/txsubmit/__init__.py
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/__init__.py
--rw-r--r--   0        0        0    29640 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_datatypes.py
--rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/test_fixtures.py
--rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/chainsync/test_FindIntersection.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/chainsync/test_NextBlock.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/mempool/test_AcquireMempool.py
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/mempool/test_HasTransaction.py
--rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/mempool/test_MempoolE2E.py
--rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/mempool/test_NextTransaction.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/mempool/test_ReleaseMempool.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/mempool/test_SizeOfMempool.py
--rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_AcquireLedgerState.py
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryBlockHeight.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryEpoch.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryEraStart.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryEraSummaries.py
--rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryGenesisConfiguration.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryLedgerTip.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryLiveStakeDistribution.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryNetworkTip.py
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryProjectedRewards.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryProposedProtocolParameters.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryProtocolParameters.py
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryRewardAccountSummaries.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryRewardsProvenance.py
--rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryStakePools.py
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryStartTime.py
--rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/statequery/test_QueryUtxo.py
--rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/txsubmit/test_EvaluateTransaction.py
--rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/ogmios/txsubmit/test_SubmitTransaction.py
--rwxr-xr-x   0        0        0     1857 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/generate_keys.sh
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test.seed
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test2_addr0.skey
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test2_stake.skey
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test_addr0.addr
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test_addr0.prv
--rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test_addr0.skey
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test_addr0.vkey
--rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test_ext_addr0.vkey
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test_ext_stake.vkey
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test_root.xsk
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test_stake.prv
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test_stake.skey
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 ogmios-1.0.5/tests/test_wallet/test_stake.vkey
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 ogmios-1.0.5/.gitignore
--rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 ogmios-1.0.5/LICENSE.txt
--rw-r--r--   0        0        0     2469 2020-02-02 00:00:00.000000 ogmios-1.0.5/README.md
--rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 ogmios-1.0.5/pyproject.toml
--rw-r--r--   0        0        0     4170 2020-02-02 00:00:00.000000 ogmios-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0      832 2020-02-02 00:00:00.000000 ogmios-1.0.6/.readthedocs.yaml
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 ogmios-1.0.6/codecov.yml
+-rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 ogmios-1.0.6/examples/async_queries.py
+-rw-r--r--   0        0        0     2314 2020-02-02 00:00:00.000000 ogmios-1.0.6/examples/build_tx_cardanotools.py
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 ogmios-1.0.6/examples/build_tx_pycardano.py
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 ogmios-1.0.6/examples/find_wallet_transactions.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 ogmios-1.0.6/examples/get_mempool_contents.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 ogmios-1.0.6/examples/live_block_viewer.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 ogmios-1.0.6/examples/print_first_shelley_blocks.py
+-rwxr-xr-x   0        0        0      344 2020-02-02 00:00:00.000000 ogmios-1.0.6/scripts/generate_models.sh
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/__about__.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/__init__.py
+-rw-r--r--   0        0        0    12312 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/chain_context.py
+-rw-r--r--   0        0        0     4795 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/client.py
+-rw-r--r--   0        0        0    39598 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/datatypes.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/errors.py
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/logger.py
+-rw-r--r--   0        0        0     5228 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/response_handler.py
+-rw-r--r--   0        0        0     3214 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/utils.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/chainsync/FindIntersection.py
+-rw-r--r--   0        0        0     4224 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/chainsync/NextBlock.py
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/chainsync/__init__.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/mempool/AcquireMempool.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/mempool/HasTransaction.py
+-rw-r--r--   0        0        0     3220 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/mempool/NextTransaction.py
+-rw-r--r--   0        0        0     2653 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/mempool/ReleaseMempool.py
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/mempool/SizeOfMempool.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/mempool/__init__.py
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/model/README.md
+-rw-r--r--   0        0        0    84579 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/model/cardano.json
+-rw-r--r--   0        0        0    42498 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/model/cardano_model.py
+-rw-r--r--   0        0        0     3857 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/model/model_map.py
+-rw-r--r--   0        0        0   155521 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/model/ogmios.json
+-rw-r--r--   0        0        0   118872 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/model/ogmios_model.py
+-rw-r--r--   0        0        0     3504 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/AcquireLedgerState.py
+-rw-r--r--   0        0        0     3049 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryBlockHeight.py
+-rw-r--r--   0        0        0     2774 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryEpoch.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryEraStart.py
+-rw-r--r--   0        0        0     4216 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryEraSummaries.py
+-rw-r--r--   0        0        0     8467 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryGenesisConfiguration.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryLedgerTip.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryLiveStakeDistribution.py
+-rw-r--r--   0        0        0     2866 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryNetworkTip.py
+-rw-r--r--   0        0        0     4672 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryProjectedRewards.py
+-rw-r--r--   0        0        0     3282 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryProposedProtocolParameters.py
+-rw-r--r--   0        0        0     3057 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryProtocolParameters.py
+-rw-r--r--   0        0        0     3943 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryRewardAccountSummaries.py
+-rw-r--r--   0        0        0     2945 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryRewardsProvenance.py
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryStakePools.py
+-rw-r--r--   0        0        0     2857 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryStartTime.py
+-rw-r--r--   0        0        0     4393 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/QueryUtxo.py
+-rw-r--r--   0        0        0     1354 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/statequery/__init__.py
+-rw-r--r--   0        0        0     3619 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/txsubmit/EvaluateTransaction.py
+-rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/txsubmit/SubmitTransaction.py
+-rw-r--r--   0        0        0      158 2020-02-02 00:00:00.000000 ogmios-1.0.6/src/ogmios/txsubmit/__init__.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/__init__.py
+-rw-r--r--   0        0        0    29640 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_datatypes.py
+-rw-r--r--   0        0        0     1708 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/test_fixtures.py
+-rw-r--r--   0        0        0     3079 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/chainsync/test_FindIntersection.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/chainsync/test_NextBlock.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/mempool/test_AcquireMempool.py
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/mempool/test_HasTransaction.py
+-rw-r--r--   0        0        0     1473 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/mempool/test_MempoolE2E.py
+-rw-r--r--   0        0        0      668 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/mempool/test_NextTransaction.py
+-rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/mempool/test_ReleaseMempool.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/mempool/test_SizeOfMempool.py
+-rw-r--r--   0        0        0      916 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_AcquireLedgerState.py
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryBlockHeight.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryEpoch.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryEraStart.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryEraSummaries.py
+-rw-r--r--   0        0        0     1871 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryGenesisConfiguration.py
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryLedgerTip.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryLiveStakeDistribution.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryNetworkTip.py
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryProjectedRewards.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryProposedProtocolParameters.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryProtocolParameters.py
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryRewardAccountSummaries.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryRewardsProvenance.py
+-rw-r--r--   0        0        0      880 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryStakePools.py
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryStartTime.py
+-rw-r--r--   0        0        0     1790 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/statequery/test_QueryUtxo.py
+-rw-r--r--   0        0        0      931 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/txsubmit/test_EvaluateTransaction.py
+-rw-r--r--   0        0        0      954 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/ogmios/txsubmit/test_SubmitTransaction.py
+-rwxr-xr-x   0        0        0     1857 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/generate_keys.sh
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test.seed
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test2_addr0.skey
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test2_stake.skey
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test_addr0.addr
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test_addr0.prv
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test_addr0.skey
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test_addr0.vkey
+-rw-r--r--   0        0        0      244 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test_ext_addr0.vkey
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test_ext_stake.vkey
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test_root.xsk
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test_stake.prv
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test_stake.skey
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 ogmios-1.0.6/tests/test_wallet/test_stake.vkey
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ogmios-1.0.6/.gitignore
+-rw-r--r--   0        0        0    34670 2020-02-02 00:00:00.000000 ogmios-1.0.6/LICENSE.txt
+-rw-r--r--   0        0        0     2699 2020-02-02 00:00:00.000000 ogmios-1.0.6/README.md
+-rw-r--r--   0        0        0     4049 2020-02-02 00:00:00.000000 ogmios-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4400 2020-02-02 00:00:00.000000 ogmios-1.0.6/PKG-INFO
```

### Comparing `ogmios-1.0.5/.readthedocs.yaml` & `ogmios-1.0.6/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/examples/async_queries.py` & `ogmios-1.0.6/examples/async_queries.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/examples/build_tx_cardanotools.py` & `ogmios-1.0.6/examples/build_tx_cardanotools.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/examples/build_tx_pycardano.py` & `ogmios-1.0.6/examples/build_tx_pycardano.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/examples/find_wallet_transactions.py` & `ogmios-1.0.6/examples/find_wallet_transactions.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/examples/get_mempool_contents.py` & `ogmios-1.0.6/examples/get_mempool_contents.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/examples/live_block_viewer.py` & `ogmios-1.0.6/examples/live_block_viewer.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/examples/print_first_shelley_blocks.py` & `ogmios-1.0.6/examples/print_first_shelley_blocks.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/__init__.py` & `ogmios-1.0.6/src/ogmios/__init__.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/chain_context.py` & `ogmios-1.0.6/src/ogmios/chain_context.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,18 +34,20 @@
         self,
         host: str = "localhost",
         port: int = 1337,
         secure: bool = False,
         refetch_chain_tip_interval: Optional[float] = None,
         utxo_cache_size: int = 10000,
         datum_cache_size: int = 10000,
+        network: pyc.Network = pyc.Network.TESTNET,
     ):
         self.host = host
         self.port = port
         self.secure = secure
+        self._network = network
         self._service_name = "ogmios"
         self._last_known_block_slot = 0
         self._refetch_chain_tip_interval = (
             refetch_chain_tip_interval if refetch_chain_tip_interval is not None else DEFAULT_REFETCH_INTERVAL
         )
         self._last_chain_tip_fetch = 0
         self._genesis_param = None
@@ -108,15 +110,15 @@
                 min_fee_constant=protocol_parameters.min_fee_constant.lovelace,
                 min_fee_coefficient=protocol_parameters.min_fee_coefficient,
                 min_pool_cost=protocol_parameters.min_stake_pool_cost.lovelace,
                 max_block_size=protocol_parameters.max_block_body_size.get("bytes"),
                 max_tx_size=protocol_parameters.max_transaction_size.get("bytes"),
                 max_block_header_size=protocol_parameters.max_block_header_size.get("bytes"),
                 key_deposit=protocol_parameters.stake_credential_deposit.lovelace,
-                pool_deposit=protocol_parameters.stake_pool_deposit,
+                pool_deposit=protocol_parameters.stake_pool_deposit.lovelace,
                 pool_influence=eval(protocol_parameters.stake_pool_pledge_influence),
                 monetary_expansion=eval(protocol_parameters.monetary_expansion),
                 treasury_expansion=eval(protocol_parameters.treasury_expansion),
                 decentralization_param=None,  # TODO
                 extra_entropy=protocol_parameters.extra_entropy,
                 protocol_major_version=protocol_parameters.version.get("major"),
                 protocol_minor_version=protocol_parameters.version.get("minor"),
@@ -262,15 +264,19 @@
     def evaluate_tx_cbor(self, cbor: Union[bytes, str]) -> Dict[str, pyc.ExecutionUnits]:
         if isinstance(cbor, bytes):
             cbor = cbor.hex()
         with Client(self.host, self.port, self.secure) as client:
             result, _ = client.evaluate_transaction.execute(cbor)
             result_dict = {}
             for res in result:
-                result_dict[f"{res['validator']['purpose']}:{res['validator']['index']}"] = pyc.ExecutionUnits(
+                purpose = res['validator']['purpose']
+                # Hotfix: this purpose has been renamed in the latest version of Ogmios
+                if purpose == "withdraw":
+                    purpose = "withdrawal"
+                result_dict[f"{purpose}:{res['validator']['index']}"] = pyc.ExecutionUnits(
                     mem=res["budget"]["memory"],
                     steps=res["budget"]["cpu"],
                 )
             return result_dict
 
     def _parse_cost_models(self, plutus_cost_models):
         ogmios_cost_models = plutus_cost_models or {}
```

### Comparing `ogmios-1.0.5/src/ogmios/client.py` & `ogmios-1.0.6/src/ogmios/client.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/datatypes.py` & `ogmios-1.0.6/src/ogmios/datatypes.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/response_handler.py` & `ogmios-1.0.6/src/ogmios/response_handler.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/utils.py` & `ogmios-1.0.6/src/ogmios/utils.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/chainsync/FindIntersection.py` & `ogmios-1.0.6/src/ogmios/chainsync/FindIntersection.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/chainsync/NextBlock.py` & `ogmios-1.0.6/src/ogmios/chainsync/NextBlock.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/mempool/AcquireMempool.py` & `ogmios-1.0.6/src/ogmios/mempool/AcquireMempool.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/mempool/HasTransaction.py` & `ogmios-1.0.6/src/ogmios/mempool/HasTransaction.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/mempool/NextTransaction.py` & `ogmios-1.0.6/src/ogmios/mempool/NextTransaction.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/mempool/ReleaseMempool.py` & `ogmios-1.0.6/src/ogmios/mempool/ReleaseMempool.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/mempool/SizeOfMempool.py` & `ogmios-1.0.6/src/ogmios/mempool/SizeOfMempool.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/model/README.md` & `ogmios-1.0.6/src/ogmios/model/README.md`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/model/cardano.json` & `ogmios-1.0.6/src/ogmios/model/cardano.json`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/model/cardano_model.py` & `ogmios-1.0.6/src/ogmios/model/cardano_model.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/model/model_map.py` & `ogmios-1.0.6/src/ogmios/model/model_map.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/model/ogmios.json` & `ogmios-1.0.6/src/ogmios/model/ogmios.json`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/model/ogmios_model.py` & `ogmios-1.0.6/src/ogmios/model/ogmios_model.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/AcquireLedgerState.py` & `ogmios-1.0.6/src/ogmios/statequery/AcquireLedgerState.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryBlockHeight.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryBlockHeight.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryEpoch.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryEpoch.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryEraStart.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryEraStart.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryEraSummaries.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryEraSummaries.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryGenesisConfiguration.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryGenesisConfiguration.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryLedgerTip.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryLedgerTip.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryLiveStakeDistribution.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryLiveStakeDistribution.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryNetworkTip.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryNetworkTip.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryProjectedRewards.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryProjectedRewards.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryProposedProtocolParameters.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryProposedProtocolParameters.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryProtocolParameters.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryProtocolParameters.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryRewardAccountSummaries.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryRewardAccountSummaries.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryRewardsProvenance.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryRewardsProvenance.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryStakePools.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryStakePools.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryStartTime.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryStartTime.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/QueryUtxo.py` & `ogmios-1.0.6/src/ogmios/statequery/QueryUtxo.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/statequery/__init__.py` & `ogmios-1.0.6/src/ogmios/statequery/__init__.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/txsubmit/EvaluateTransaction.py` & `ogmios-1.0.6/src/ogmios/txsubmit/EvaluateTransaction.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/src/ogmios/txsubmit/SubmitTransaction.py` & `ogmios-1.0.6/src/ogmios/txsubmit/SubmitTransaction.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/test_datatypes.py` & `ogmios-1.0.6/tests/test_datatypes.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/test_fixtures.py` & `ogmios-1.0.6/tests/ogmios/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/chainsync/test_FindIntersection.py` & `ogmios-1.0.6/tests/ogmios/chainsync/test_FindIntersection.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/chainsync/test_NextBlock.py` & `ogmios-1.0.6/tests/ogmios/chainsync/test_NextBlock.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/mempool/test_HasTransaction.py` & `ogmios-1.0.6/tests/ogmios/mempool/test_HasTransaction.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/mempool/test_MempoolE2E.py` & `ogmios-1.0.6/tests/ogmios/mempool/test_MempoolE2E.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/mempool/test_NextTransaction.py` & `ogmios-1.0.6/tests/ogmios/mempool/test_NextTransaction.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/mempool/test_ReleaseMempool.py` & `ogmios-1.0.6/tests/ogmios/mempool/test_ReleaseMempool.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/mempool/test_SizeOfMempool.py` & `ogmios-1.0.6/tests/ogmios/mempool/test_SizeOfMempool.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_AcquireLedgerState.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_AcquireLedgerState.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_QueryBlockHeight.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_QueryBlockHeight.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_QueryEraSummaries.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_QueryEraSummaries.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_QueryGenesisConfiguration.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_QueryGenesisConfiguration.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_QueryLedgerTip.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_QueryLedgerTip.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_QueryLiveStakeDistribution.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_QueryLiveStakeDistribution.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_QueryNetworkTip.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_QueryNetworkTip.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_QueryProjectedRewards.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_QueryProjectedRewards.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_QueryRewardAccountSummaries.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_QueryRewardAccountSummaries.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_QueryStakePools.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_QueryStakePools.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/statequery/test_QueryUtxo.py` & `ogmios-1.0.6/tests/ogmios/statequery/test_QueryUtxo.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/txsubmit/test_EvaluateTransaction.py` & `ogmios-1.0.6/tests/ogmios/txsubmit/test_EvaluateTransaction.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/ogmios/txsubmit/test_SubmitTransaction.py` & `ogmios-1.0.6/tests/ogmios/txsubmit/test_SubmitTransaction.py`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/tests/test_wallet/generate_keys.sh` & `ogmios-1.0.6/tests/test_wallet/generate_keys.sh`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/LICENSE.txt` & `ogmios-1.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ogmios-1.0.5/README.md` & `ogmios-1.0.6/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 # ogmios-python
 
 [![Pipeline](https://gitlab.com/viperscience/ogmios-python/badges/main/pipeline.svg)](https://gitlab.com/viperscience/ogmios-python/-/pipelines)
 [![Documentation Status](https://readthedocs.org/projects/ogmios-python/badge/?version=latest)](https://ogmios-python.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Version](https://img.shields.io/pypi/v/ogmios.svg)](https://pypi.org/project/ogmios)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ogmios.svg)](https://pypi.org/project/ogmios)
+[![Codecov](https://codecov.io/gitlab/viperscience/ogmios-python/graph/badge.svg?token=7VUVLYR6FP)](https://codecov.io/gitlab/viperscience/ogmios-python)
 [![Catalyst](https://img.shields.io/badge/catalyst-fund10-violet)](https://cardano.ideascale.com/c/idea/105214)
 
 -----
 
 [Ogmios](https://ogmios.dev/) is a lightweight bridge interface for cardano-node. It offers a WebSockets API that enables local clients to speak Ouroboros’ mini-protocols via JSON/RPC. **ogmios-python** is an Ogmios client written in Python designed for ease of use.
 
 -----
 
 **Table of Contents**
 
-- [Installation](#installation)
-- [Quickstart](#quickstart)
-- [License](#license)
+- [ogmios-python](#ogmios-python)
+  - [Installation](#installation)
+  - [Quickstart](#quickstart)
+  - [Documentation](#documentation)
+  - [License](#license)
 
 
 ## Installation
 
 1. Install cardano-node and Ogmios server as described [here](https://ogmios.dev/getting-started/). (Docker installation is recommended.)
 2. Install ogmios-python from [PyPI](https://pypi.org/project/ogmios/) using pip:
```

### Comparing `ogmios-1.0.5/pyproject.toml` & `ogmios-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -179,15 +179,15 @@
 ban-relative-imports = "all"
 
 [tool.ruff.per-file-ignores]
 # Tests can use magic values, assertions, and relative imports
 "tests/**/*" = ["PLR2004", "S101", "TID252"]
 
 [tool.flake8]
-max-line-length = 100
+max-line-length = 120
 
 [tool.coverage.run]
 source_pkgs = ["ogmios", "tests"]
 branch = true
 parallel = true
 omit = [
   "src/ogmios/__about__.py",
```

### Comparing `ogmios-1.0.5/PKG-INFO` & `ogmios-1.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ogmios
-Version: 1.0.5
+Version: 1.0.6
 Summary: Ogmios is a lightweight bridge interface for cardano-node. It offers a WebSockets API that enables local clients to speak Ouroboros' mini-protocols via JSON/RPC. ogmios-python is an Ogmios client written in Python designed for ease of use.
 Project-URL: Documentation, https://ogmios-python.readthedocs.io
 Project-URL: Issues, https://gitlab.com/viperscience/ogmios-python/-/issues
 Project-URL: Source, https://gitlab.com/viperscience/ogmios-python
 Author-email: Willie Marchetto <willie@viperscience.com>, Dylan Crocker <dylan@viperscience.com>
 License-Expression: GPL-3.0-or-later
 License-File: LICENSE.txt
@@ -37,27 +37,30 @@
 
 # ogmios-python
 
 [![Pipeline](https://gitlab.com/viperscience/ogmios-python/badges/main/pipeline.svg)](https://gitlab.com/viperscience/ogmios-python/-/pipelines)
 [![Documentation Status](https://readthedocs.org/projects/ogmios-python/badge/?version=latest)](https://ogmios-python.readthedocs.io/en/latest/?badge=latest)
 [![PyPI - Version](https://img.shields.io/pypi/v/ogmios.svg)](https://pypi.org/project/ogmios)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/ogmios.svg)](https://pypi.org/project/ogmios)
+[![Codecov](https://codecov.io/gitlab/viperscience/ogmios-python/graph/badge.svg?token=7VUVLYR6FP)](https://codecov.io/gitlab/viperscience/ogmios-python)
 [![Catalyst](https://img.shields.io/badge/catalyst-fund10-violet)](https://cardano.ideascale.com/c/idea/105214)
 
 -----
 
 [Ogmios](https://ogmios.dev/) is a lightweight bridge interface for cardano-node. It offers a WebSockets API that enables local clients to speak Ouroboros’ mini-protocols via JSON/RPC. **ogmios-python** is an Ogmios client written in Python designed for ease of use.
 
 -----
 
 **Table of Contents**
 
-- [Installation](#installation)
-- [Quickstart](#quickstart)
-- [License](#license)
+- [ogmios-python](#ogmios-python)
+  - [Installation](#installation)
+  - [Quickstart](#quickstart)
+  - [Documentation](#documentation)
+  - [License](#license)
 
 
 ## Installation
 
 1. Install cardano-node and Ogmios server as described [here](https://ogmios.dev/getting-started/). (Docker installation is recommended.)
 2. Install ogmios-python from [PyPI](https://pypi.org/project/ogmios/) using pip:
```

