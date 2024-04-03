# Comparing `tmp/chrs-0.3.0a4.tar.gz` & `tmp/chrs-0.3.1.tar.gz`

## Comparing `chrs-0.3.0a4.tar` & `chrs-0.3.1.tar`

### file list

```diff
@@ -1,92 +1,92 @@
--rw-r--r--   0     1001      127     1865 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/Cargo.toml
--rw-r--r--   0     1001      127      432 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/README.md
--rw-r--r--   0     1001      127     2428 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/account.rs
--rw-r--r--   0     1001      127      235 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/client/access.rs
--rw-r--r--   0     1001      127     3304 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/client/anon.rs
--rw-r--r--   0     1001      127     8130 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/client/authed.rs
--rw-r--r--   0     1001      127     2685 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/client/base.rs
--rw-r--r--   0     1001      127     3288 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/client/either.rs
--rw-r--r--   0     1001      127     3595 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/client/filebrowser.rs
--rw-r--r--   0     1001      127      193 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/client.rs
--rw-r--r--   0     1001      127     2919 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/errors.rs
--rw-r--r--   0     1001      127      614 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/lib.rs
--rw-r--r--   0     1001      127     8647 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/models/data.rs
--rw-r--r--   0     1001      127     2224 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/models/file.rs
--rw-r--r--   0     1001      127     4237 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/models/linked.rs
--rw-r--r--   0     1001      127     2083 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/models/live/downloadable.rs
--rw-r--r--   0     1001      127     2789 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/models/live/feed.rs
--rw-r--r--   0     1001      127     1521 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/models/live/pipeline.rs
--rw-r--r--   0     1001      127     1403 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/models/live/plugin.rs
--rw-r--r--   0     1001      127     1469 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/models/live/plugininstance.rs
--rw-r--r--   0     1001      127      244 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/models/live.rs
--rw-r--r--   0     1001      127      750 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/models.rs
--rw-r--r--   0     1001      127     4141 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/pipeline.rs
--rw-r--r--   0     1001      127      963 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/requests.rs
--rw-r--r--   0     1001      127     1986 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/search/query.rs
--rw-r--r--   0     1001      127    10656 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/search/search.rs
--rw-r--r--   0     1001      127     5740 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/search/searches.rs
--rw-r--r--   0     1001      127      228 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/search.rs
--rw-r--r--   0     1001      127     1684 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/types/cube_url.rs
--rw-r--r--   0     1001      127     3108 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/types/enums.rs
--rw-r--r--   0     1001      127     1621 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/types/ids.rs
--rw-r--r--   0     1001      127     1051 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/types/strings.rs
--rw-r--r--   0     1001      127      532 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/types/urls.rs
--rw-r--r--   0     1001      127      207 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/src/types.rs
--rw-r--r--   0     1001      127     6433 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/tests/data/sample_files/a_folder/pikachu_testpass.txt
--rw-r--r--   0     1001      127       13 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/tests/data/sample_files/a_folder/simple.txt
--rw-r--r--   0     1001      127     3418 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/tests/data/sample_files/logo_chris.png
--rw-r--r--   0     1001      127      163 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/tests/helpers/mod.rs
--rw-r--r--   0     1001      127     5449 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/tests/test_logged_in.rs
--rw-r--r--   0     1001      127     5137 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chris/tests/test_public.rs
--rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 chrs-0.3.0a4/chrs/Cargo.toml
--rw-r--r--   0     1001      127      625 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/README.md
--rw-r--r--   0     1001      127    12585 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/arg/given_data_node.rs
--rw-r--r--   0     1001      127    13476 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/arg/given_plugin_instance.rs
--rw-r--r--   0     1001      127    11228 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/arg/runnable.rs
--rw-r--r--   0     1001      127      831 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/arg/runnable_parser.rs
--rw-r--r--   0     1001      127      215 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/arg.rs
--rw-r--r--   0     1001      127      924 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/cd.rs
--rw-r--r--   0     1001      127     9489 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/credentials.rs
--rw-r--r--   0     1001      127     4765 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/describe.rs
--rw-r--r--   0     1001      127    11589 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/download.rs
--rw-r--r--   0     1001      127      168 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/error_messages.rs
--rw-r--r--   0     1001      127      547 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/file_transfer/bytes_bar.rs
--rw-r--r--   0     1001      127      210 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/file_transfer/error.rs
--rw-r--r--   0     1001      127     2739 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/file_transfer/multi_progress.rs
--rw-r--r--   0     1001      127      226 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/file_transfer.rs
--rw-r--r--   0     1001      127     1296 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/files/channel.rs
--rw-r--r--   0     1001      127    25319 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/files/decoder.rs
--rw-r--r--   0     1001      127      101 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/files.rs
--rw-r--r--   0     1001      127     3706 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/list.rs
--rw-r--r--   0     1001      127      481 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/login/cd.rs
--rw-r--r--   0     1001      127     3131 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/login/cmd.rs
--rw-r--r--   0     1001      127     2033 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/login/prompt.rs
--rw-r--r--   0     1001      127    15642 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/login/state.rs
--rw-r--r--   0     1001      127     6888 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/login/store.rs
--rw-r--r--   0     1001      127     3267 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/login/switch.rs
--rw-r--r--   0     1001      127     1985 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/login/ui.rs
--rw-r--r--   0     1001      127      123 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/login.rs
--rw-r--r--   0     1001      127      548 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/logs.rs
--rw-r--r--   0     1001      127     1856 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/ls/cmd.rs
--rw-r--r--   0     1001      127      408 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/ls/options.rs
--rw-r--r--   0     1001      127     3983 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/ls/plain.rs
--rw-r--r--   0     1001      127      257 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/ls/tree.rs
--rw-r--r--   0     1001      127       64 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/ls.rs
--rw-r--r--   0     1001      127     6165 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/main.rs
--rw-r--r--   0     1001      127     8770 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/plugin_clap.rs
--rw-r--r--   0     1001      127    24169 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/run.rs
--rw-r--r--   0     1001      127     1683 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/search.rs
--rw-r--r--   0     1001      127      230 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/shlex.rs
--rw-r--r--   0     1001      127     1617 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/status/cmd.rs
--rw-r--r--   0     1001      127     2579 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/status/feed.rs
--rw-r--r--   0     1001      127     2945 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/status/find_branch.rs
--rw-r--r--   0     1001      127     6079 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/status/print_branch.rs
--rw-r--r--   0     1001      127       58 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/status.rs
--rw-r--r--   0     1001      127      471 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/unicode.rs
--rw-r--r--   0     1001      127    13417 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/upload.rs
--rw-r--r--   0     1001      127      666 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/src/whoami.rs
--rw-r--r--   0     1001      127    51985 2024-03-12 05:28:41.000000 chrs-0.3.0a4/chrs/test_data/cube_chrisproject_org_feed_45_plugininstances_results.json
--rw-r--r--   0     1001      127    93948 2024-03-12 05:28:41.000000 chrs-0.3.0a4/Cargo.lock
--rw-r--r--   0        0        0      171 1970-01-01 00:00:00.000000 chrs-0.3.0a4/Cargo.toml
--rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 chrs-0.3.0a4/pyproject.toml
--rw-r--r--   0        0        0     1350 1970-01-01 00:00:00.000000 chrs-0.3.0a4/PKG-INFO
+-rw-r--r--   0     1001      127     1869 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/Cargo.toml
+-rw-r--r--   0     1001      127      432 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/README.md
+-rw-r--r--   0     1001      127     2428 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/account.rs
+-rw-r--r--   0     1001      127      235 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/client/access.rs
+-rw-r--r--   0     1001      127     3304 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/client/anon.rs
+-rw-r--r--   0     1001      127     8296 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/client/authed.rs
+-rw-r--r--   0     1001      127     2685 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/client/base.rs
+-rw-r--r--   0     1001      127     3288 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/client/either.rs
+-rw-r--r--   0     1001      127     3595 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/client/filebrowser.rs
+-rw-r--r--   0     1001      127      193 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/client.rs
+-rw-r--r--   0     1001      127     2919 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/errors.rs
+-rw-r--r--   0     1001      127      614 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/lib.rs
+-rw-r--r--   0     1001      127     8647 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/models/data.rs
+-rw-r--r--   0     1001      127     3861 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/models/file.rs
+-rw-r--r--   0     1001      127     4237 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/models/linked.rs
+-rw-r--r--   0     1001      127     2083 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/models/live/downloadable.rs
+-rw-r--r--   0     1001      127     2789 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/models/live/feed.rs
+-rw-r--r--   0     1001      127     1521 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/models/live/pipeline.rs
+-rw-r--r--   0     1001      127     1403 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/models/live/plugin.rs
+-rw-r--r--   0     1001      127     1469 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/models/live/plugininstance.rs
+-rw-r--r--   0     1001      127      244 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/models/live.rs
+-rw-r--r--   0     1001      127      750 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/models.rs
+-rw-r--r--   0     1001      127     4141 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/pipeline.rs
+-rw-r--r--   0     1001      127      963 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/requests.rs
+-rw-r--r--   0     1001      127     1986 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/search/query.rs
+-rw-r--r--   0     1001      127    10662 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/search/search.rs
+-rw-r--r--   0     1001      127     8910 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/search/searches.rs
+-rw-r--r--   0     1001      127      228 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/search.rs
+-rw-r--r--   0     1001      127     1684 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/types/cube_url.rs
+-rw-r--r--   0     1001      127     3108 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/types/enums.rs
+-rw-r--r--   0     1001      127     1757 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/types/ids.rs
+-rw-r--r--   0     1001      127     1051 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/types/strings.rs
+-rw-r--r--   0     1001      127      532 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/types/urls.rs
+-rw-r--r--   0     1001      127      207 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/src/types.rs
+-rw-r--r--   0     1001      127     6433 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/tests/data/sample_files/a_folder/pikachu_testpass.txt
+-rw-r--r--   0     1001      127       13 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/tests/data/sample_files/a_folder/simple.txt
+-rw-r--r--   0     1001      127     3418 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/tests/data/sample_files/logo_chris.png
+-rw-r--r--   0     1001      127      163 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/tests/helpers/mod.rs
+-rw-r--r--   0     1001      127     5451 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/tests/test_logged_in.rs
+-rw-r--r--   0     1001      127     5137 2024-04-03 17:32:28.000000 chrs-0.3.1/chris/tests/test_public.rs
+-rw-r--r--   0        0        0     1801 1970-01-01 00:00:00.000000 chrs-0.3.1/chrs/Cargo.toml
+-rw-r--r--   0     1001      127      625 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/README.md
+-rw-r--r--   0     1001      127    12585 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/arg/given_data_node.rs
+-rw-r--r--   0     1001      127    13476 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/arg/given_plugin_instance.rs
+-rw-r--r--   0     1001      127    11228 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/arg/runnable.rs
+-rw-r--r--   0     1001      127      831 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/arg/runnable_parser.rs
+-rw-r--r--   0     1001      127      215 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/arg.rs
+-rw-r--r--   0     1001      127      924 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/cd.rs
+-rw-r--r--   0     1001      127     9596 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/credentials.rs
+-rw-r--r--   0     1001      127     4765 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/describe.rs
+-rw-r--r--   0     1001      127    11583 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/download.rs
+-rw-r--r--   0     1001      127      168 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/error_messages.rs
+-rw-r--r--   0     1001      127      547 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/file_transfer/bytes_bar.rs
+-rw-r--r--   0     1001      127      210 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/file_transfer/error.rs
+-rw-r--r--   0     1001      127     2739 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/file_transfer/multi_progress.rs
+-rw-r--r--   0     1001      127      226 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/file_transfer.rs
+-rw-r--r--   0     1001      127     1296 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/files/channel.rs
+-rw-r--r--   0     1001      127    25319 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/files/decoder.rs
+-rw-r--r--   0     1001      127      101 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/files.rs
+-rw-r--r--   0     1001      127     3706 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/list.rs
+-rw-r--r--   0     1001      127      481 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/login/cd.rs
+-rw-r--r--   0     1001      127     3131 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/login/cmd.rs
+-rw-r--r--   0     1001      127     2033 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/login/prompt.rs
+-rw-r--r--   0     1001      127    15798 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/login/state.rs
+-rw-r--r--   0     1001      127     7112 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/login/store.rs
+-rw-r--r--   0     1001      127     3267 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/login/switch.rs
+-rw-r--r--   0     1001      127     1985 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/login/ui.rs
+-rw-r--r--   0     1001      127      123 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/login.rs
+-rw-r--r--   0     1001      127      548 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/logs.rs
+-rw-r--r--   0     1001      127     1856 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/ls/cmd.rs
+-rw-r--r--   0     1001      127      408 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/ls/options.rs
+-rw-r--r--   0     1001      127     3983 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/ls/plain.rs
+-rw-r--r--   0     1001      127      257 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/ls/tree.rs
+-rw-r--r--   0     1001      127       64 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/ls.rs
+-rw-r--r--   0     1001      127     6482 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/main.rs
+-rw-r--r--   0     1001      127     8770 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/plugin_clap.rs
+-rw-r--r--   0     1001      127    24568 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/run.rs
+-rw-r--r--   0     1001      127     1683 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/search.rs
+-rw-r--r--   0     1001      127      230 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/shlex.rs
+-rw-r--r--   0     1001      127     1617 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/status/cmd.rs
+-rw-r--r--   0     1001      127     2579 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/status/feed.rs
+-rw-r--r--   0     1001      127     2945 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/status/find_branch.rs
+-rw-r--r--   0     1001      127     6079 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/status/print_branch.rs
+-rw-r--r--   0     1001      127       58 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/status.rs
+-rw-r--r--   0     1001      127      471 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/unicode.rs
+-rw-r--r--   0     1001      127    14619 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/upload.rs
+-rw-r--r--   0     1001      127      666 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/src/whoami.rs
+-rw-r--r--   0     1001      127    51985 2024-04-03 17:32:28.000000 chrs-0.3.1/chrs/test_data/cube_chrisproject_org_feed_45_plugininstances_results.json
+-rw-r--r--   0     1001      127    93948 2024-04-03 17:32:28.000000 chrs-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0      218 1970-01-01 00:00:00.000000 chrs-0.3.1/Cargo.toml
+-rw-r--r--   0        0        0      453 1970-01-01 00:00:00.000000 chrs-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1348 1970-01-01 00:00:00.000000 chrs-0.3.1/PKG-INFO
```

### Comparing `chrs-0.3.0a4/chris/Cargo.toml` & `chrs-0.3.1/chris/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "chris"
-version = "0.4.0"
+version = "0.5.0-a.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 description = "ChRIS client library"
 readme = "README.md"
 repository = "https://github.com/FNNDSC/chrs"
 license = "MIT"
```

### Comparing `chrs-0.3.0a4/chris/src/account.rs` & `chrs-0.3.1/chris/src/account.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/client/anon.rs` & `chrs-0.3.1/chris/src/client/anon.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/client/authed.rs` & `chrs-0.3.1/chris/src/client/authed.rs`

 * *Files 4% similar despite different names*

```diff
@@ -162,18 +162,24 @@
     }
 
     /// Search for feed files
     pub fn files(&self) -> FilesSearchBuilder<A> {
         self.query(&self.links.files)
     }
 
+    /// Search for workflows
     pub fn workflows(&self) -> WorkflowSearchBuilder<A> {
         self.query(&self.links.workflows)
     }
 
+    /// Search for PACSFiles
+    pub fn pacsfiles(&self) -> PacsFilesSearchBuilder<A> {
+        self.query(&self.links.pacsfiles)
+    }
+
     // ==================================================
     //                 FILES UPLOAD
     // ==================================================
 
     /// Create a _ChRIS_ uploadedfile from a stream of bytes.
     ///
     /// [`ChrisClient::upload_stream`] is a lower-level function called by
```

### Comparing `chrs-0.3.0a4/chris/src/client/base.rs` & `chrs-0.3.1/chris/src/client/base.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/client/either.rs` & `chrs-0.3.1/chris/src/client/either.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/client/filebrowser.rs` & `chrs-0.3.1/chris/src/client/filebrowser.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/errors.rs` & `chrs-0.3.1/chris/src/errors.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/lib.rs` & `chrs-0.3.1/chris/src/lib.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/models/data.rs` & `chrs-0.3.1/chris/src/models/data.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/models/linked.rs` & `chrs-0.3.1/chris/src/models/linked.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/models/live/downloadable.rs` & `chrs-0.3.1/chris/src/models/live/downloadable.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/models/live/feed.rs` & `chrs-0.3.1/chris/src/models/live/feed.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/models/live/pipeline.rs` & `chrs-0.3.1/chris/src/models/live/pipeline.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/models/live/plugin.rs` & `chrs-0.3.1/chris/src/models/live/plugin.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/models/live/plugininstance.rs` & `chrs-0.3.1/chris/src/models/live/plugininstance.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/models.rs` & `chrs-0.3.1/chris/src/models.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/pipeline.rs` & `chrs-0.3.1/chris/src/pipeline.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/requests.rs` & `chrs-0.3.1/chris/src/requests.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/search/query.rs` & `chrs-0.3.1/chris/src/search/query.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/search/search.rs` & `chrs-0.3.1/chris/src/search/search.rs`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             query: self.query,
             phantom: Default::default(),
             is_search: self.is_search,
         }
     }
 
     /// See [Search::get_count]
-    async fn get_count(&self) -> Result<u32, CubeError> {
+    async fn get_count(&self) -> Result<usize, CubeError> {
         let res = self.get_search().query(&LIMIT_ONE).send().await?;
         let data: HasCount = check(res).await?.json().await?;
         Ok(data.count)
     }
 
     /// See [Search::get_first]
     async fn get_first(&self) -> Result<Option<LinkedModel<R, A>>, CubeError> {
@@ -205,15 +205,15 @@
         Self {
             max_items: Some(max),
             ..self
         }
     }
 
     /// Get the count of items in this collection.
-    pub async fn get_count(&self) -> Result<u32, CubeError> {
+    pub async fn get_count(&self) -> Result<usize, CubeError> {
         if let Some(search) = &self.actual {
             search.get_count().await
         } else {
             Ok(0)
         }
     }
 
@@ -345,9 +345,9 @@
     limit: 1,
     offset: 0,
 };
 
 /// A HTTP JSON response which has a count field.
 #[derive(Deserialize)]
 struct HasCount {
-    count: u32,
+    count: usize,
 }
```

### Comparing `chrs-0.3.0a4/chris/src/types/cube_url.rs` & `chrs-0.3.1/chris/src/types/cube_url.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/types/enums.rs` & `chrs-0.3.1/chris/src/types/enums.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/types/ids.rs` & `chrs-0.3.1/chris/src/types/ids.rs`

 * *Files 1% similar despite different names*

```diff
@@ -40,7 +40,11 @@
 /// Compute resource ID
 #[derive(Copy, Clone, Shrinkwrap, Serialize, Deserialize, Debug, Hash, Eq, PartialEq)]
 pub struct ComputeResourceId(pub u32);
 
 /// Feed file ID
 #[derive(Copy, Clone, Shrinkwrap, Serialize, Deserialize, Debug, Hash, Eq, PartialEq)]
 pub struct FeedFileId(pub u32);
+
+/// PACSFile ID
+#[derive(Copy, Clone, Shrinkwrap, Serialize, Deserialize, Debug, Hash, Eq, PartialEq)]
+pub struct PacsFileId(pub u32);
```

### Comparing `chrs-0.3.0a4/chris/src/types/strings.rs` & `chrs-0.3.1/chris/src/types/strings.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/src/types/urls.rs` & `chrs-0.3.1/chris/src/types/urls.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/tests/data/sample_files/a_folder/pikachu_testpass.txt` & `chrs-0.3.1/chris/tests/data/sample_files/a_folder/pikachu_testpass.txt`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/tests/data/sample_files/logo_chris.png` & `chrs-0.3.1/chris/tests/data/sample_files/logo_chris.png`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chris/tests/test_logged_in.rs` & `chrs-0.3.1/chris/tests/test_logged_in.rs`

 * *Files 1% similar despite different names*

```diff
@@ -158,15 +158,15 @@
     let note_content: String = fake::faker::company::en::CatchPhase().fake();
     let lazy_note = changed_feed.note();
     let changed_note = lazy_note.set("Description", &note_content).await?;
     assert_eq!(changed_note.object.content, note_content);
     Ok(())
 }
 
-async fn count_feeds_with_name(client: &ChrisClient, name: &str) -> u32 {
+async fn count_feeds_with_name(client: &ChrisClient, name: &str) -> usize {
     client
         .feeds()
         .name_exact(name)
         .search()
         .get_count()
         .await
         .unwrap()
```

### Comparing `chrs-0.3.0a4/chris/tests/test_public.rs` & `chrs-0.3.1/chris/tests/test_public.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/Cargo.toml` & `chrs-0.3.1/chrs/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "chrs"
-version = "0.3.0-a.4"
+version = "0.3.1"
 authors = ["Jennings Zhang <jennings.zhang@childrens.harvard.edu>", "FNNDSC <dev@babyMRI.org>"]
 
 edition = "2021"
 
 readme = "README.md"
 description = "CLI ChRIS client"
 repository = "https://github.com/FNNDSC/chrs"
@@ -12,15 +12,15 @@
 documentation = "https://chrisproject.org/docs/chrs"
 license = "MIT"
 categories = ["command-line-utilities", "science"]
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [dependencies]
-chris = { path = "../chris", version = "0.4.0", features = ["rustls"], default-features = false }
+chris = { path = "../chris", version = "0.5.0-a.1", features = ["rustls"], default-features = false }
 clap = { version = "4.1.1", features = ["derive", "string"] }
 keyring = "2.3.2"
 thiserror = "1.0.30"
 tokio = { version = "1.17.0", features = ["full"] }
 tokio-util = { version = "0.7.1", features = [ "io" ] }
 futures = "0.3.21"
 async-stream = "0.3.3"
```

### Comparing `chrs-0.3.0a4/chrs/README.md` & `chrs-0.3.1/chrs/README.md`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/arg/given_data_node.rs` & `chrs-0.3.1/chrs/src/arg/given_data_node.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/arg/given_plugin_instance.rs` & `chrs-0.3.1/chrs/src/arg/given_plugin_instance.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/arg/runnable.rs` & `chrs-0.3.1/chrs/src/arg/runnable.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/arg/runnable_parser.rs` & `chrs-0.3.1/chrs/src/arg/runnable_parser.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/cd.rs` & `chrs-0.3.1/chrs/src/cd.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/credentials.rs` & `chrs-0.3.1/chrs/src/credentials.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-use color_eyre::eyre;
 use color_eyre::eyre::{eyre, Context};
 use color_eyre::owo_colors::OwoColorize;
+use color_eyre::{eyre, Section};
 use reqwest_middleware::Middleware;
 use reqwest_retry::{
     policies::ExponentialBackoff, RetryTransientMiddleware, Retryable, RetryableStrategy,
 };
 use std::path::PathBuf;
 
 use chris::reqwest::Response;
@@ -190,24 +190,27 @@
             .connect()
             .await
     } else {
         ChrisClient::build(cube_url.clone(), username.clone(), token)?
             .connect()
             .await
     };
-    result.map(EitherClient::LoggedIn).wrap_err_with(|| {
-        format!(
-            "Could not log in. The saved token might have expired, please run {}",
+    result
+        .map(EitherClient::LoggedIn)
+        .wrap_err("Could not log in. The authorization token might have expired.")
+        .with_suggestion(|| {
             format!(
-                "chrs logout --cube \"{}\" --username \"{}\"",
-                &cube_url, &username
+                "Try logging out.\n\n\t{}",
+                format!(
+                    "chrs logout --cube \"{}\" --username \"{}\"",
+                    &cube_url, &username
+                )
+                .bold()
             )
-            .bold()
-        )
-    })
+        })
 }
 
 fn handle_error(error: chris::reqwest::Error, url: &CubeUrl) -> eyre::Error {
     if let Some(code) = error.status() {
         if code == chris::reqwest::StatusCode::UNAUTHORIZED {
             eyre::Error::msg("Incorrect login")
         } else {
```

### Comparing `chrs-0.3.0a4/chrs/src/describe.rs` & `chrs-0.3.1/chrs/src/describe.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/download.rs` & `chrs-0.3.1/chrs/src/download.rs`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         .await?;
     let src = args
         .src
         .clone()
         .or_else(|| old.map(|id| id.into()))
         .ok_or_else(|| eyre!("Missing operand"))?;
     let (files, dst, rel) = get_files_search(&client, src, old, args.dst.clone()).await?;
-    let size = download_files(client, files, args, dst, dbg!(rel)).await?;
+    let size = download_files(client, files, args, dst, rel).await?;
     eprintln!("Downloaded: {}", HumanBytes(size));
     Ok(())
 }
 
 type Files = Search<BasicFileResponse, RoAccess>;
 
 /// Main implementation
```

### Comparing `chrs-0.3.0a4/chrs/src/file_transfer/bytes_bar.rs` & `chrs-0.3.1/chrs/src/file_transfer/bytes_bar.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/file_transfer/multi_progress.rs` & `chrs-0.3.1/chrs/src/file_transfer/multi_progress.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/files/channel.rs` & `chrs-0.3.1/chrs/src/files/channel.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/files/decoder.rs` & `chrs-0.3.1/chrs/src/files/decoder.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/list.rs` & `chrs-0.3.1/chrs/src/list.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/login/cmd.rs` & `chrs-0.3.1/chrs/src/login/cmd.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/login/prompt.rs` & `chrs-0.3.1/chrs/src/login/prompt.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/login/state.rs` & `chrs-0.3.1/chrs/src/login/state.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 use crate::login::store::{Backend, CubeState, SavedCubeState};
 use chris::types::{CubeUrl, PluginInstanceId, Username};
 use color_eyre::eyre::{Result, WrapErr};
 use color_eyre::owo_colors::OwoColorize;
+use color_eyre::Section;
 use serde::{Deserialize, Serialize};
 use std::path::Path;
 
 const SERVICE: &str = "org.chrisproject.chrs";
 const APP_NAME: &str = "chrs";
 
 /// The application state is a list of user sessions represented by [SavedCubeState].
@@ -109,15 +110,22 @@
     /// Load config from file.
     pub fn load<P: AsRef<Path>>(config_path: Option<P>) -> Result<Self> {
         let result = if let Some(path) = config_path {
             confy::load_path(path)
         } else {
             confy::load(APP_NAME, None)
         };
-        result.wrap_err_with(|| format!("Could not load config file. If chrs was upgraded from an old version, please run `{}`", "rm -rf ~/.config/chrs".bold()))
+        result
+            .wrap_err("Could not load config file. ")
+            .with_suggestion(|| {
+                format!(
+                    "If chrs was upgraded from an old version, please run `{}`",
+                    "rm -rf ~/.config/chrs".bold()
+                )
+            })
     }
 
     /// Write config to file.
     pub fn save<P: AsRef<Path>>(&self, config_path: Option<P>) -> Result<()> {
         let result = if let Some(path) = config_path {
             confy::store_path(path, self)
         } else {
```

### Comparing `chrs-0.3.0a4/chrs/src/login/store.rs` & `chrs-0.3.1/chrs/src/login/store.rs`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 //! When saved to keyring, the token is identified by a string in the form
 //! "<CUBEUsername>@<CUBEAddress>"
 
 use crate::login::ui::UiUrl;
 use chris::types::{CubeUrl, PluginInstanceId, Username};
 use color_eyre::eyre::{Result, WrapErr};
 use color_eyre::owo_colors::OwoColorize;
+use color_eyre::Section;
 use serde::{Deserialize, Serialize};
 
 /// Supported mechanisms for storing secrets.
 pub enum Backend {
     ClearText,
     Keyring,
 }
@@ -78,24 +79,28 @@
     /// token is saved to the keyring.
     pub fn into_saved(self, backend: Backend, service: &str) -> Result<SavedCubeState> {
         let token: StoredToken = if let Some(token) = &self.token {
             match backend {
                 Backend::ClearText => StoredToken::Text(token.to_string()),
                 Backend::Keyring => {
                     let entry = keyring::Entry::new(service, &self.to_keyring_username())?;
-                    entry.set_password(token).wrap_err_with(|| {
-                        format!(
-                            "Could not save token to keyring. Please try again with: `{}`",
+                    entry
+                        .set_password(token)
+                        .wrap_err("Could not save token to keyring.")
+                        .with_suggestion(|| {
                             format!(
-                                "chrs login --cube={} --username={} --token={}",
-                                &self.cube, &self.username, token
+                                "Try using the {} option. \n\n\t{}",
+                                "--no-keyring".bold(),
+                                format!(
+                                    "chrs login --cube={} --username={} --token={} --no-keyring",
+                                    &self.cube, &self.username, token
+                                )
+                                .bold()
                             )
-                            .bold()
-                        )
-                    })?;
+                        })?;
                     StoredToken::Keyring
                 }
             }
         } else {
             StoredToken::None
         };
         let saved = SavedCubeState {
```

### Comparing `chrs-0.3.0a4/chrs/src/login/switch.rs` & `chrs-0.3.1/chrs/src/login/switch.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/login/ui.rs` & `chrs-0.3.1/chrs/src/login/ui.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/logs.rs` & `chrs-0.3.1/chrs/src/logs.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/ls/cmd.rs` & `chrs-0.3.1/chrs/src/ls/cmd.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/ls/plain.rs` & `chrs-0.3.1/chrs/src/ls/plain.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/main.rs` & `chrs-0.3.1/chrs/src/main.rs`

 * *Files 6% similar despite different names*

```diff
@@ -178,15 +178,22 @@
     //         files: Vec<PathBuf>,
     //     },
     //
 }
 
 #[tokio::main]
 async fn main() -> color_eyre::eyre::Result<()> {
+    #[cfg(debug_assertions)]
     color_eyre::install()?;
+    #[cfg(not(debug_assertions))]
+    color_eyre::config::HookBuilder::default()
+        // .issue_url(concat!(env!("CARGO_PKG_REPOSITORY"), "/issues/new"))
+        // .add_issue_metadata("version", env!("CARGO_PKG_VERSION"))
+        .display_location_section(false)
+        .install()?;
 
     let args: Cli = Cli::parse();
     let credentials = Credentials {
         cube_url: args.cube,
         username: args.username,
         password: args.password,
         token: args.token,
```

### Comparing `chrs-0.3.0a4/chrs/src/plugin_clap.rs` & `chrs-0.3.1/chrs/src/plugin_clap.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/run.rs` & `chrs-0.3.1/chrs/src/run.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+use std::borrow::Cow;
 use std::collections::HashMap;
+use std::fmt::Display;
 
 use clap::Parser;
 use color_eyre::eyre::{eyre, OptionExt, WrapErr};
 use color_eyre::owo_colors::OwoColorize;
 use color_eyre::{eyre, eyre::bail};
 use futures::{StreamExt, TryStreamExt};
 use itertools::Itertools;
+use tokio::try_join;
 
 use chris::errors::CubeError;
 use chris::types::{ComputeResourceName, PluginInstanceId, PluginParameterValue};
 use chris::{
     BaseChrisClient, ChrisClient, EitherClient, PipelineRw, PluginInstanceResponse,
     PluginInstanceRw, PluginRw,
 };
@@ -95,19 +98,21 @@
 
 async fn run(
     client: &ChrisClient,
     old: Option<PluginInstanceId>,
     ui: Option<UiUrl>,
     args: RunArgs,
 ) -> eyre::Result<Option<PluginInstanceId>> {
-    let runnable = args
-        .plugin_or_pipeline
-        .clone()
-        .resolve_using(client)
-        .await?;
+    let (title_is_unique, runnable) = try_join!(
+        check_title(client, old, args.title.as_deref(), args.force),
+        args.plugin_or_pipeline.clone().resolve_using(client)
+    )?;
+    if let Some(error) = title_is_unique {
+        bail!("{}", error);
+    }
     let plinst = match runnable {
         Runnable::Plugin(p) => run_plugin(client, p, old, args).await,
         Runnable::Pipeline(p) => run_pipeline(client, p, old, args).await,
     }?;
     if let (Some(ui), Some(plinst)) = (ui, plinst.as_ref()) {
         let feed = plinst.feed().get().await?;
         let feed_ui_url = ui.feed_url_of(&feed.object);
@@ -121,17 +126,14 @@
     plugin: PluginRw,
     old: Option<PluginInstanceId>,
     args: RunArgs,
 ) -> eyre::Result<Option<PluginInstanceRw>> {
     let (params, incoming) = clap_serialize_params(&plugin, &args.parameters).await?;
     let previous = get_input(client, old, incoming, args.threads).await?;
     let previous_id = previous.as_ref().map(|previous| previous.object.id.0);
-    if !args.force {
-        check_title(client, previous.as_ref(), args.title.as_deref()).await?;
-    }
     if args.dry_run {
         eprintln!("Input: plugininstance/{:?}", previous_id);
         Ok(None)
     } else {
         create_plugin_instance(&plugin, params, previous_id, args)
             .await
             .map(Some)
@@ -144,17 +146,14 @@
     old: Option<PluginInstanceId>,
     args: RunArgs,
 ) -> eyre::Result<Option<PluginInstanceRw>> {
     let inputs: Vec<GivenDataNode> = args.parameters.into_iter().map(|p| p.into()).collect();
     let prev = get_input(client, old, inputs, args.threads)
         .await?
         .ok_or_eyre("Missing operand")?;
-    if !args.force {
-        check_title(client, Some(&prev), args.title.as_deref()).await?;
-    }
     let workflow = pipeline
         .create_workflow(prev.object.id, args.title.as_deref())
         .await?;
     // get the "last" plugin instance created by the workflow. Assumes CUBE returns the plugin instances in order.
     workflow
         .plugin_instances()
         .get_first()
@@ -225,54 +224,63 @@
                 PluginParameterValue::Integer(v as i64),
             )
         }),
     ];
     optional_resources.into_iter().flatten()
 }
 
-/// Raise error if:
-///
-/// - title is None
-/// - if has previous, title is not unique in the feed
-/// - if no previous, title is not a unique feed name
 async fn check_title(
     client: &ChrisClient,
-    previous: Option<&PluginInstanceRw>,
+    old: Option<PluginInstanceId>,
     title: Option<&str>,
-) -> eyre::Result<()> {
+    force: bool,
+) -> eyre::Result<Option<TitleUniqueness>> {
+    if force {
+        return Ok(None);
+    }
     if let Some(title) = title {
-        if let Some(plinst) = previous {
-            if title_is_not_unique(client, &plinst.object, title).await? {
-                bail!(
-                    "Title is not unique within the feed. {}",
-                    "You can bypass this check using --force".dimmed()
-                );
+        if let Some(id) = old {
+            if title_is_not_unique(client, id, title).await? {
+                return Ok(Some(TitleUniqueness::NotUniqueWithinFeed));
             }
         } else if feed_name_is_not_unique(client, title).await? {
-            bail!(
-                "Title is not a unique feed name. {}",
-                "You can bypass this check using --force".dimmed()
-            );
+            return Ok(Some(TitleUniqueness::NotUniqueFeedName));
         }
     } else {
-        bail!(
-            "Please provide a value for {}. {}",
-            "--title".bold(),
-            "You can bypass this check using --force".dimmed()
-        )
+        return Ok(Some(TitleUniqueness::NoTitle));
     };
-    Ok(())
+    Ok(None)
+}
+
+enum TitleUniqueness {
+    NotUniqueWithinFeed,
+    NotUniqueFeedName,
+    NoTitle,
+}
+
+impl Display for TitleUniqueness {
+    fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
+        let hint = "You can bypass this check using --force";
+        let msg = match self {
+            TitleUniqueness::NotUniqueWithinFeed => {
+                Cow::Borrowed("Title is not unique within feed.")
+            }
+            TitleUniqueness::NotUniqueFeedName => Cow::Borrowed("Title is not a unique feed name."),
+            TitleUniqueness::NoTitle => Cow::Owned(format!("A {} is required.", "--title".bold())),
+        };
+        write!(f, "{} {}", msg, hint.dimmed())
+    }
 }
 
 async fn title_is_not_unique(
     client: &ChrisClient,
-    plinst: &PluginInstanceResponse,
+    plinst: PluginInstanceId,
     title: &str,
 ) -> Result<bool, CubeError> {
-    let feed_id = plinst.feed_id;
+    let feed_id = client.get_plugin_instance(plinst).await?.object.feed_id;
     let query = client
         .plugin_instances()
         .feed_id(feed_id)
         .title(title.to_string());
     let search = query.search();
     search.get_count().await.map(|count| count > 0)
 }
@@ -380,16 +388,16 @@
     use std::path::PathBuf;
 
     use fake::Fake;
     use futures::TryStreamExt;
     use rstest::*;
     use tempfile::TempDir;
 
-    use chris::Account;
     use chris::types::{CubeUrl, Username};
+    use chris::Account;
 
     use crate::credentials::NO_ARGS;
     use crate::login::state::ChrsSessions;
     use crate::login::store::{SavedCubeState, StoredToken};
 
     use super::*;
 
@@ -450,15 +458,17 @@
     async fn test_gives_warning_for_no_title(credentials: &Credentials) {
         if let Err(error) = run_command(
             credentials.clone(),
             create_args(None, "pl-mri10yr06mo01da_normal", &[]),
         )
         .await
         {
-            assert!(error.to_string().contains("Please provide a value for"))
+            assert!(error
+                .to_string()
+                .contains(TitleUniqueness::NoTitle.to_string().as_str()))
         } else {
             panic!("Expected an error to happen because no title was given.")
         }
     }
 
     #[rstest]
     #[tokio::test(flavor = "multi_thread")]
@@ -538,15 +548,15 @@
                 &[&feed_by_name],
             ),
         )
         .await;
         if let Err(error) = third_run_fail {
             assert!(error
                 .to_string()
-                .contains("Title is not unique within the feed."));
+                .contains(TitleUniqueness::NotUniqueWithinFeed.to_string().as_str()));
         } else {
             panic!("Expected an error message about non-unique plugin instance title.");
         }
         let third_title = uuid_name("third title");
         run_command(
             credentials.clone(),
             create_args_mem(
```

### Comparing `chrs-0.3.0a4/chrs/src/search.rs` & `chrs-0.3.1/chrs/src/search.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/status/cmd.rs` & `chrs-0.3.1/chrs/src/status/cmd.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/status/feed.rs` & `chrs-0.3.1/chrs/src/status/feed.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/status/find_branch.rs` & `chrs-0.3.1/chrs/src/status/find_branch.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/status/print_branch.rs` & `chrs-0.3.1/chrs/src/status/print_branch.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/src/upload.rs` & `chrs-0.3.1/chrs/src/upload.rs`

 * *Files 6% similar despite different names*

```diff
@@ -62,14 +62,15 @@
     old: Option<PluginInstanceId>,
     ui: Option<UiUrl>,
     args: UploadArgs,
     config_path: Option<PathBuf>,
 ) -> eyre::Result<()> {
     let threads = args.threads;
     let input_paths = args.paths.clone();
+    let title = args.feed.clone();
     let get_cube_info = async {
         let (current_feed, previous_id) =
             find_existing_feed(&client, old, args.feed.as_deref()).await?;
         let plugins = find_plugins(&client, previous_id.is_some(), &args).await?;
         Ok::<_, eyre::Error>((current_feed, previous_id, plugins))
     };
 
@@ -78,18 +79,27 @@
         discover_files(input_paths).map_err(eyre::Error::new)
     )?;
 
     let upload_path = upload_all(&client, files, threads).await?;
     let plinsts = run_plugins(plugins, previous_id, upload_path).await?;
 
     let feed = if let Some(feed) = current_feed {
+        // added to an already existing feed
         Some(feed)
     } else if let Some(plinst) = plinsts.last() {
-        Some(plinst.feed().get().await?)
+        // created a new feed, need to set feed name
+        let feed = plinst.feed().get().await?;
+        let named_feed = if let Some(title) = title {
+            feed.set_name(&title).await?
+        } else {
+            feed
+        };
+        Some(named_feed)
     } else {
+        // nothing happened
         None
     };
     if let Some(feed) = feed {
         if let Some(note) = args.note {
             feed.note().set("Description", note).await?;
         }
         if let Some(ui) = ui {
@@ -208,17 +218,15 @@
     tx: UnboundedSender<FileTransferEvent>,
 ) -> Result<(), chris::errors::FileIOError> {
     let file_name = file
         .path
         .file_name()
         .unwrap_or(file.path.as_str())
         .to_string();
-    let rel = pathdiff::diff_utf8_paths(&file.path, &file.src)
-        .map(|p| p.to_string())
-        .unwrap_or_else(|| file.path.to_string());
+    let rel = file.to_relative();
     let upload_name = format!("{}/{}", base, rel);
     let content_length = fs_err::tokio::metadata(&file.path).await?.len();
     let open_file = fs_err::tokio::File::open(&file.path).await?;
     let chunk_tx = tx.clone();
     let stream = FramedRead::new(open_file, BytesCodec::new()).map_ok(move |chunk| {
         chunk_tx
             .send(FileTransferEvent::Chunk {
@@ -320,14 +328,29 @@
 struct DiscoveredFile {
     /// The path to the file
     path: Utf8PathBuf,
     /// Positional argument path which this file was discovered under
     src: Utf8PathBuf,
 }
 
+impl DiscoveredFile {
+    fn to_relative(&self) -> String {
+        if self.path == self.src {
+            self.path
+                .file_name()
+                .unwrap_or(self.path.as_str())
+                .to_string()
+        } else {
+            pathdiff::diff_utf8_paths(&self.path, &self.src)
+                .map(|p| p.to_string())
+                .unwrap_or_else(|| self.path.to_string())
+        }
+    }
+}
+
 /// Collect all files in a set of paths.
 async fn discover_files(paths: Vec<Utf8PathBuf>) -> Result<Vec<DiscoveredFile>, std::io::Error> {
     let either_file_or_dir: Vec<(std::fs::Metadata, Utf8PathBuf)> = futures::stream::iter(paths)
         .map(|p| async move { fs_err::tokio::metadata(&p).await.map(|m| (m, p)) })
         .map(Ok::<_, std::io::Error>)
         .try_buffer_unordered(100)
         .try_collect()
@@ -414,7 +437,31 @@
             .get_only()
             .await
             .wrap_err_with(|| "pl-unstack-folders@1.0.0 not found")?;
         plugins.push(second_plugin);
     }
     Ok(plugins)
 }
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+    use rstest::*;
+
+    #[rstest]
+    #[case("a", "a", "a")]
+    #[case("a/b", "a/b", "b")]
+    #[case("a", "a/b", "b")]
+    #[case("a", "a/b/c", "b/c")]
+    fn test_discovered_file_to_relative(
+        #[case] src: &str,
+        #[case] path: &str,
+        #[case] expected: &str,
+    ) {
+        let discovered = DiscoveredFile {
+            path: Utf8PathBuf::from(path),
+            src: Utf8PathBuf::from(src),
+        };
+        let actual = discovered.to_relative();
+        assert_eq!(&actual, expected);
+    }
+}
```

### Comparing `chrs-0.3.0a4/chrs/src/whoami.rs` & `chrs-0.3.1/chrs/src/whoami.rs`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/chrs/test_data/cube_chrisproject_org_feed_45_plugininstances_results.json` & `chrs-0.3.1/chrs/test_data/cube_chrisproject_org_feed_45_plugininstances_results.json`

 * *Files identical despite different names*

### Comparing `chrs-0.3.0a4/Cargo.lock` & `chrs-0.3.1/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -527,15 +527,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chris"
-version = "0.4.0"
+version = "0.5.0-a.1"
 dependencies = [
  "aliri_braid",
  "anyhow",
  "async-std",
  "async-stream",
  "async-trait",
  "bytes",
@@ -578,15 +578,15 @@
  "num-traits",
  "serde",
  "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "chrs"
-version = "0.3.0-a.4"
+version = "0.3.1"
 dependencies = [
  "aliri_braid",
  "async-recursion",
  "async-stream",
  "async-walkdir",
  "camino",
  "chris",
```

### Comparing `chrs-0.3.0a4/PKG-INFO` & `chrs-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: chrs
-Version: 0.3.0a4
+Version: 0.3.1
 Classifier: Programming Language :: Rust
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Summary: CLI ChRIS client
 Home-Page: https://chrisproject.org
```

