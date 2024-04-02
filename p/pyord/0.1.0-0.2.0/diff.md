# Comparing `tmp/pyord-0.1.0.tar.gz` & `tmp/pyord-0.2.0.tar.gz`

## Comparing `pyord-0.1.0.tar` & `pyord-0.2.0.tar`

### file list

```diff
@@ -1,353 +1,28 @@
--rw-r--r--   0      501       20     2544 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/Cargo.toml
--rw-r--r--   0      501       20       10 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/.dockerignore
--rw-r--r--   0      501       20      147 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/.editorconfig
--rw-r--r--   0      501       20        8 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/.gitattributes
--rw-r--r--   0      501       20     2612 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/.github/workflows/ci.yaml
--rw-r--r--   0      501       20     2021 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/.github/workflows/release.yaml
--rw-r--r--   0      501       20      147 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/.gitignore
--rw-r--r--   0      501       20       44 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/.prettierignore
--rw-r--r--   0      501       20   145258 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/CHANGELOG.md
--rw-r--r--   0      501       20      217 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/CONTRIBUTING
--rw-r--r--   0      501       20    99887 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/Cargo.lock
--rw-r--r--   0      501       20      290 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/Dockerfile
--rw-r--r--   0      501       20     7048 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/LICENSE
--rw-r--r--   0      501       20     9312 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/README.md
--rw-r--r--   0      501       20     1629 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/batch.yaml
--rw-r--r--   0      501       20      403 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/benches/server.rs
--rwxr-xr-x   0      501       20      275 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/bin/benchmark
--rwxr-xr-x   0      501       20      548 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/bin/flamegraph
--rwxr-xr-x   0      501       20      210 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/bin/forbid
--rwxr-xr-x   0      501       20     1124 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/bin/graph
--rwxr-xr-x   0      501       20      304 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/bin/install-bitcoin-core-linux
--rwxr-xr-x   0      501       20      944 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/bin/package
--rw-r--r--   0      501       20    11587 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/bip.mediawiki
--rw-r--r--   0      501       20      667 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/build.rs
--rwxr-xr-x   0      501       20      284 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/contrib/initialize-opendime
--rw-r--r--   0      501       20      540 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/contrib/raw/justfile
--rw-r--r--   0      501       20       52 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/deploy/bitcoin.conf
--rw-r--r--   0      501       20      759 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/deploy/bitcoind.service
--rwxr-xr-x   0      501       20      353 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/deploy/checkout
--rw-r--r--   0      501       20      862 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/deploy/ord.service
--rwxr-xr-x   0      501       20     2739 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/deploy/setup
--rw-r--r--   0      501       20      401 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/book.toml
--rw-r--r--   0      501       20       88 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/language-picker.css
--rw-r--r--   0      501       20   212622 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/ar.po
--rw-r--r--   0      501       20   208989 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/de.po
--rw-r--r--   0      501       20   214102 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/es.po
--rw-r--r--   0      501       20   214258 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/fil.po
--rw-r--r--   0      501       20   225629 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/fr.po
--rw-r--r--   0      501       20   324458 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/hi.po
--rw-r--r--   0      501       20   240562 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/it.po
--rw-r--r--   0      501       20   209411 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/ja.po
--rw-r--r--   0      501       20   234116 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/ko.po
--rw-r--r--   0      501       20   209539 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/pt.po
--rw-r--r--   0      501       20   254417 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/ru.po
--rw-r--r--   0      501       20   204485 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/po/zh.po
--rw-r--r--   0      501       20       88 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/rtl.css
--rw-r--r--   0      501       20     1164 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/SUMMARY.md
--rw-r--r--   0      501       20      893 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/bounties.md
--rw-r--r--   0      501       20      602 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/bounty/0.md
--rw-r--r--   0      501       20      663 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/bounty/1.md
--rw-r--r--   0      501       20      680 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/bounty/2.md
--rw-r--r--   0      501       20     2441 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/bounty/3.md
--rw-r--r--   0      501       20   222987 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/bounty/frequency.tsv
--rw-r--r--   0      501       20     3651 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/contributing.md
--rw-r--r--   0      501       20     1590 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/digital-artifacts.md
--rw-r--r--   0      501       20     1052 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/donate.md
--rw-r--r--   0      501       20    15519 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/faq.md
--rw-r--r--   0      501       20      609 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/batch-inscribing.md
--rw-r--r--   0      501       20   211831 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/sending_01.png
--rw-r--r--   0      501       20   169189 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/sending_02.png
--rw-r--r--   0      501       20   226915 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/sending_03.png
--rw-r--r--   0      501       20   161450 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/sending_04.png
--rw-r--r--   0      501       20   167850 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/sending_05.png
--rw-r--r--   0      501       20   170142 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/sending_06.png
--rw-r--r--   0      501       20   337272 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/troubleshooting_01.png
--rw-r--r--   0      501       20   388671 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/troubleshooting_02.png
--rw-r--r--   0      501       20    82336 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/validating_viewing_01.png
--rw-r--r--   0      501       20    86740 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/validating_viewing_02.png
--rw-r--r--   0      501       20    37389 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/wallet_setup_01.png
--rw-r--r--   0      501       20   177132 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/wallet_setup_02.png
--rw-r--r--   0      501       20   147875 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/wallet_setup_03.png
--rw-r--r--   0      501       20   147048 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/wallet_setup_04.png
--rw-r--r--   0      501       20   150369 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/wallet_setup_05.png
--rw-r--r--   0      501       20   125329 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/wallet_setup_06.png
--rw-r--r--   0      501       20   164680 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/wallet_setup_07.png
--rw-r--r--   0      501       20   147823 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/images/wallet_setup_08.png
--rw-r--r--   0      501       20    11780 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting/sparrow-wallet.md
--rw-r--r--   0      501       20     1091 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/collecting.md
--rw-r--r--   0      501       20     3749 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/explorer.md
--rw-r--r--   0      501       20     1645 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/moderation.md
--rw-r--r--   0      501       20     1475 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/reindexing.md
--rw-r--r--   0      501       20     7810 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/docs/src/guides/sat-hunting.md
--rw-r--r--   0      501       20     1768 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/docs/src/guides/settings.md
--rw-r--r--   0      501       20     1687 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/teleburning.md
--rw-r--r--   0      501       20     3898 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides/testing.md
--rw-r--r--   0      501       20    11705 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/docs/src/guides/wallet.md
--rw-r--r--   0      501       20      182 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/guides.md
--rw-r--r--   0      501       20     1408 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/inscriptions/delegate.md
--rw-r--r--   0      501       20     2306 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/inscriptions/metadata.md
--rw-r--r--   0      501       20     1454 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/inscriptions/pointer.md
--rw-r--r--   0      501       20     2600 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/inscriptions/provenance.md
--rw-r--r--   0      501       20     4924 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/inscriptions/recursion.md
--rw-r--r--   0      501       20     1327 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/inscriptions/rendering.md
--rw-r--r--   0      501       20     6925 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/inscriptions.md
--rw-r--r--   0      501       20     2091 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/introduction.md
--rw-r--r--   0      501       20    10015 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/src/overview.md
--rw-r--r--   0      501       20       24 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/theme/favicon.png
--rw-r--r--   0      501       20       24 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/theme/favicon.svg
--rw-r--r--   0      501       20    19962 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/docs/theme/index.hbs
--rw-r--r--   0      501       20       31 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/examples/alert.html
--rw-r--r--   0      501       20       72 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/examples/external-resources-are-blocked.html
--rw-r--r--   0      501       20    61382 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/examples/h264.mp4
--rw-r--r--   0      501       20       58 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/examples/navigation-to-external-pages-is-blocked.html
--rw-r--r--   0      501       20       57 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/examples/top-navigation-is-blocked.html
--rwxr-xr-x   0      501       20     2570 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/install.sh
--rw-r--r--   0      501       20     5579 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/justfile
--rw-r--r--   0      501       20      249 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/logo-bw.svg
--rw-r--r--   0      501       20      249 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/logo-wb.svg
--rw-r--r--   0      501       20      721 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/ord.yaml
--rwxr-xr-x   0      501       20      819 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/quickstart/macos
--rw-r--r--   0      501       20      128 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/rustfmt.toml
--rw-r--r--   0      501       20      365 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/shell.nix
--rw-r--r--   0      501       20     4287 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/api.rs
--rw-r--r--   0      501       20     1156 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/arguments.rs
--rw-r--r--   0      501       20       29 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/bin/main.rs
--rw-r--r--   0      501       20      701 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/blocktime.rs
--rw-r--r--   0      501       20     3395 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/chain.rs
--rw-r--r--   0      501       20     5094 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/decimal.rs
--rw-r--r--   0      501       20     1604 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/fee_rate.rs
--rw-r--r--   0      501       20    11638 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/index/entry.rs
--rw-r--r--   0      501       20      476 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/index/event.rs
--rw-r--r--   0      501       20     4129 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/index/fetcher.rs
--rw-r--r--   0      501       20     3545 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/index/reorg.rs
--rw-r--r--   0      501       20     1138 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/index/rtx.rs
--rw-r--r--   0      501       20     3924 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/index/testing.rs
--rw-r--r--   0      501       20    17040 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/index/updater/inscription_updater.rs
--rw-r--r--   0      501       20    11874 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/index/updater/rune_updater.rs
--rw-r--r--   0      501       20    24187 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/index/updater.rs
--rw-r--r--   0      501       20   156043 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/index.rs
--rw-r--r--   0      501       20     2386 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/inscriptions/charm.rs
--rw-r--r--   0      501       20    25339 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/inscriptions/envelope.rs
--rw-r--r--   0      501       20    20806 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/inscriptions/inscription.rs
--rw-r--r--   0      501       20     4760 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/inscriptions/inscription_id.rs
--rw-r--r--   0      501       20     7271 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/inscriptions/media.rs
--rw-r--r--   0      501       20     1967 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/inscriptions/tag.rs
--rw-r--r--   0      501       20     2853 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/inscriptions/teleburn.rs
--rw-r--r--   0      501       20      331 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/inscriptions.rs
--rw-r--r--   0      501       20     6703 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/lib.rs
--rw-r--r--   0      501       20     5826 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/object.rs
--rw-r--r--   0      501       20     3494 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/options.rs
--rw-r--r--   0      501       20     6477 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/outgoing.rs
--rw-r--r--   0      501       20     1944 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/representation.rs
--rw-r--r--   0      501       20      153 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/runes/edict.rs
--rw-r--r--   0      501       20      223 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/runes/etching.rs
--rw-r--r--   0      501       20      868 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/runes/flag.rs
--rw-r--r--   0      501       20      177 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/runes/mint.rs
--rw-r--r--   0      501       20     2664 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/runes/pile.rs
--rw-r--r--   0      501       20     8978 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/runes/rune.rs
--rw-r--r--   0      501       20     2559 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/runes/rune_id.rs
--rw-r--r--   0      501       20    35916 2024-03-07 21:49:31.000000 pyord-0.1.0/submodules/ord/src/runes/runestone.rs
--rw-r--r--   0      501       20     3027 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/runes/spaced_rune.rs
--rw-r--r--   0      501       20     1772 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/runes/tag.rs
--rw-r--r--   0      501       20     3121 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/runes/varint.rs
--rw-r--r--   0      501       20   114890 2024-03-07 21:49:31.000000 pyord-0.1.0/submodules/ord/src/runes.rs
--rw-r--r--   0      501       20      314 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/server_config.rs
--rw-r--r--   0      501       20    31019 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/settings.rs
--rw-r--r--   0      501       20      460 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/balances.rs
--rw-r--r--   0      501       20     3354 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/decode.rs
--rw-r--r--   0      501       20     5073 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/subcommand/env.rs
--rw-r--r--   0      501       20      320 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/epochs.rs
--rw-r--r--   0      501       20     1160 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/find.rs
--rw-r--r--   0      501       20      431 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/index/export.rs
--rw-r--r--   0      501       20      999 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/index/info.rs
--rw-r--r--   0      501       20      148 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/index/update.rs
--rw-r--r--   0      501       20      620 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/index.rs
--rw-r--r--   0      501       20     2322 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/list.rs
--rw-r--r--   0      501       20      352 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/parse.rs
--rw-r--r--   0      501       20     1649 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/runes.rs
--rw-r--r--   0      501       20     3208 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/server/accept_encoding.rs
--rw-r--r--   0      501       20      853 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/server/accept_json.rs
--rw-r--r--   0      501       20     2047 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/server/error.rs
--rw-r--r--   0      501       20     1101 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/server/query.rs
--rw-r--r--   0      501       20   150695 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/subcommand/server.rs
--rw-r--r--   0      501       20      108 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/settings.rs
--rw-r--r--   0      501       20      615 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/subsidy.rs
--rw-r--r--   0      501       20      462 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/supply.rs
--rw-r--r--   0      501       20      448 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/teleburn.rs
--rw-r--r--   0      501       20      851 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/traits.rs
--rw-r--r--   0      501       20     1716 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/balance.rs
--rw-r--r--   0      501       20      737 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/cardinals.rs
--rw-r--r--   0      501       20      786 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/create.rs
--rw-r--r--   0      501       20      355 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/dump.rs
--rw-r--r--   0      501       20     3203 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/etch.rs
--rw-r--r--   0      501       20    39220 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/inscribe.rs
--rw-r--r--   0      501       20      966 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/inscriptions.rs
--rw-r--r--   0      501       20      366 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/outputs.rs
--rw-r--r--   0      501       20      339 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/receive.rs
--rw-r--r--   0      501       20     1408 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/restore.rs
--rw-r--r--   0      501       20     7680 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/sats.rs
--rw-r--r--   0      501       20     8698 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/send.rs
--rw-r--r--   0      501       20      725 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet/transactions.rs
--rw-r--r--   0      501       20     2970 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand/wallet.rs
--rw-r--r--   0      501       20     2949 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/subcommand.rs
--rw-r--r--   0      501       20      783 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/tally.rs
--rw-r--r--   0      501       20     2454 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/block.rs
--rw-r--r--   0      501       20     2187 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/blocks.rs
--rw-r--r--   0      501       20     1836 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/children.rs
--rw-r--r--   0      501       20     3334 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/clock.rs
--rw-r--r--   0      501       20     1503 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/collections.rs
--rw-r--r--   0      501       20      717 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/home.rs
--rw-r--r--   0      501       20     1324 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/iframe.rs
--rw-r--r--   0      501       20     1685 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/input.rs
--rw-r--r--   0      501       20    12588 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/inscription.rs
--rw-r--r--   0      501       20     1516 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/inscriptions.rs
--rw-r--r--   0      501       20     2763 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/inscriptions_block.rs
--rw-r--r--   0      501       20     3005 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/metadata.rs
--rw-r--r--   0      501       20     6039 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/output.rs
--rw-r--r--   0      501       20     1123 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/preview.rs
--rw-r--r--   0      501       20      999 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/range.rs
--rw-r--r--   0      501       20       98 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/rare.rs
--rw-r--r--   0      501       20     4652 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/rune.rs
--rw-r--r--   0      501       20     1730 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/rune_balances.rs
--rw-r--r--   0      501       20      693 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/runes.rs
--rw-r--r--   0      501       20     4129 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/sat.rs
--rw-r--r--   0      501       20      638 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/status.rs
--rw-r--r--   0      501       20     2343 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates/transaction.rs
--rw-r--r--   0      501       20     4860 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/templates.rs
--rw-r--r--   0      501       20     3636 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/test.rs
--rw-r--r--   0      501       20    16909 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/wallet/inscribe/batch.rs
--rw-r--r--   0      501       20      682 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/wallet/inscribe/batch_entry.rs
--rw-r--r--   0      501       20     9646 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/wallet/inscribe/batch_file.rs
--rw-r--r--   0      501       20      321 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/wallet/inscribe/mode.rs
--rw-r--r--   0      501       20     1305 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/wallet/inscribe.rs
--rw-r--r--   0      501       20    58521 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/wallet/transaction_builder.rs
--rw-r--r--   0      501       20    17123 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/src/wallet.rs
--rw-r--r--   0      501       20      670 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/book.svg
--rw-r--r--   0      501       20      485 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/clock.svg
--rw-r--r--   0      501       20     1072 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/cubes.svg
--rw-r--r--   0      501       20      632 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/diagram-project.svg
--rw-r--r--   0      501       20     1601 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/discord.svg
--rw-r--r--   0      501       20    13375 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/favicon.png
--rw-r--r--   0      501       20      409 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/favicon.svg
--rw-r--r--   0      501       20      762 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/gem.svg
--rw-r--r--   0      501       20     1611 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/github.svg
--rw-r--r--   0      501       20      820 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/images.svg
--rw-r--r--   0      501       20     3633 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/index.css
--rw-r--r--   0      501       20      774 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/index.js
--rw-r--r--   0      501       20      539 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/magnifying-glass.svg
--rw-r--r--   0      501       20     4630 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/modern-normalize.css
--rw-r--r--   0      501       20      130 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-audio.css
--rw-r--r--   0      501       20      217 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-code.css
--rw-r--r--   0      501       20      631 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-code.js
--rw-r--r--   0      501       20      262 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-font.css
--rw-r--r--   0      501       20      385 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-image.js
--rw-r--r--   0      501       20      133 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-markdown.css
--rw-r--r--   0      501       20      282 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-markdown.js
--rw-r--r--   0      501       20      130 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-pdf.css
--rw-r--r--   0      501       20      662 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-pdf.js
--rw-r--r--   0      501       20      321 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-text.css
--rw-r--r--   0      501       20      476 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-text.js
--rw-r--r--   0      501       20      175 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/static/preview-video.css
--rw-r--r--   0      501       20     1309 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/block.html
--rw-r--r--   0      501       20      570 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/blocks.html
--rw-r--r--   0      501       20      575 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/children.html
--rw-r--r--   0      501       20     6648 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/clock.svg
--rw-r--r--   0      501       20      359 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/collections.html
--rw-r--r--   0      501       20      147 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/home.html
--rw-r--r--   0      501       20      677 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/input.html
--rw-r--r--   0      501       20     3326 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/inscription.html
--rw-r--r--   0      501       20      794 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/inscriptions-block.html
--rw-r--r--   0      501       20      366 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/inscriptions.html
--rw-r--r--   0      501       20     1419 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/output.html
--rw-r--r--   0      501       20     1960 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/page.html
--rw-r--r--   0      501       20      245 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/preview-audio.html
--rw-r--r--   0      501       20      328 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/preview-code.html
--rw-r--r--   0      501       20      362 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/preview-font.html
--rw-r--r--   0      501       20      757 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/preview-image.html
--rw-r--r--   0      501       20      282 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/preview-markdown.html
--rw-r--r--   0      501       20      469 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/preview-model.html
--rw-r--r--   0      501       20      287 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/preview-pdf.html
--rw-r--r--   0      501       20      388 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/preview-text.html
--rw-r--r--   0      501       20      102 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/preview-unknown.html
--rw-r--r--   0      501       20      265 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/preview-video.html
--rw-r--r--   0      501       20      229 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/range.html
--rw-r--r--   0      501       20       75 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/rare.txt
--rw-r--r--   0      501       20      515 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/rune-balances.html
--rw-r--r--   0      501       20     1832 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/rune.html
--rw-r--r--   0      501       20      150 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/runes.html
--rw-r--r--   0      501       20     1251 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/sat.html
--rw-r--r--   0      501       20     1603 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/status.html
--rw-r--r--   0      501       20     1238 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/templates/transaction.html
--rw-r--r--   0      501       20     1964 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/balances.rs
--rw-r--r--   0      501       20     5633 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/tests/command_builder.rs
--rw-r--r--   0      501       20     3565 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/decode.rs
--rw-r--r--   0      501       20     1273 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/epochs.rs
--rw-r--r--   0      501       20    15078 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/etch.rs
--rw-r--r--   0      501       20      577 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/tests/expected.rs
--rw-r--r--   0      501       20     2261 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/find.rs
--rw-r--r--   0      501       20     2544 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/index.rs
--rw-r--r--   0      501       20     2554 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/info.rs
--rw-r--r--   0      501       20    18547 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/json_api.rs
--rw-r--r--   0      501       20     4042 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/tests/lib.rs
--rw-r--r--   0      501       20     1349 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/list.rs
--rw-r--r--   0      501       20      766 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/parse.rs
--rw-r--r--   0      501       20     3770 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/runes.rs
--rw-r--r--   0      501       20    17220 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/tests/server.rs
--rw-r--r--   0      501       20     2935 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/tests/settings.rs
--rw-r--r--   0      501       20     1189 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/subsidy.rs
--rw-r--r--   0      501       20      300 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/supply.rs
--rw-r--r--   0      501       20     4264 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/tests/test_server.rs
--rw-r--r--   0      501       20      903 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/traits.rs
--rw-r--r--   0      501       20      156 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/version.rs
--rw-r--r--   0      501       20     1043 2024-03-07 21:28:36.000000 pyord-0.1.0/submodules/ord/tests/wallet/authentication.rs
--rw-r--r--   0      501       20     4359 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/balance.rs
--rw-r--r--   0      501       20      833 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/cardinals.rs
--rw-r--r--   0      501       20     2807 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/create.rs
--rw-r--r--   0      501       20     2562 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/dump.rs
--rw-r--r--   0      501       20    80924 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/inscribe.rs
--rw-r--r--   0      501       20     4025 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/inscriptions.rs
--rw-r--r--   0      501       20     2262 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/outputs.rs
--rw-r--r--   0      501       20      510 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/receive.rs
--rw-r--r--   0      501       20     6346 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/restore.rs
--rw-r--r--   0      501       20     3161 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/sats.rs
--rw-r--r--   0      501       20    32223 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/send.rs
--rw-r--r--   0      501       20     2473 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet/transactions.rs
--rw-r--r--   0      501       20      194 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/tests/wallet.rs
--rw-r--r--   0      501       20      528 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/crates/ordinals/Cargo.toml
--rw-r--r--   0      501       20      843 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/crates/ordinals/src/decimal_sat.rs
--rw-r--r--   0      501       20     1443 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/crates/ordinals/src/degree.rs
--rw-r--r--   0      501       20      831 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/crates/ordinals/src/deserialize_from_str.rs
--rw-r--r--   0      501       20     6376 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/crates/ordinals/src/epoch.rs
--rw-r--r--   0      501       20     2869 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/crates/ordinals/src/height.rs
--rw-r--r--   0      501       20      840 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/crates/ordinals/src/lib.rs
--rw-r--r--   0      501       20     4637 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/crates/ordinals/src/rarity.rs
--rw-r--r--   0      501       20    21015 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/crates/ordinals/src/sat.rs
--rw-r--r--   0      501       20     4305 2024-03-05 23:01:21.000000 pyord-0.1.0/submodules/ord/crates/ordinals/src/sat_point.rs
--rw-r--r--   0        0        0      419 1970-01-01 00:00:00.000000 pyord-0.1.0/Cargo.toml
--rw-r--r--   0      501       20     2146 2024-03-12 09:08:22.000000 pyord-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0      501       20      686 2024-03-05 22:52:56.000000 pyord-0.1.0/.gitignore
--rw-r--r--   0      501       20       95 2024-03-05 23:01:21.000000 pyord-0.1.0/.gitmodules
--rw-r--r--   0      501       20      127 2024-03-11 12:27:12.000000 pyord-0.1.0/Dockerfile.build
--rw-r--r--   0      501       20     2090 2024-03-11 12:27:12.000000 pyord-0.1.0/Makefile
--rw-r--r--   0      501       20      885 2024-03-11 09:37:15.000000 pyord-0.1.0/README.md
--rw-r--r--   0      501       20    16631 2024-03-07 15:28:26.000000 pyord-0.1.0/generate_stubs.py
--rw-r--r--   0      501       20      834 2024-03-07 21:49:31.000000 pyord-0.1.0/ord.patch
--rw-r--r--   0      501       20     3790 2024-03-11 09:21:36.000000 pyord-0.1.0/pyord.pyi
--rw-r--r--   0      501       20        0 2024-03-07 19:16:59.000000 pyord-0.1.0/python_tests/__init__.py
--rw-r--r--   0      501       20        0 2024-03-07 19:16:59.000000 pyord-0.1.0/python_tests/runes/__init__.py
--rw-r--r--   0      501       20     1126 2024-03-07 19:16:59.000000 pyord-0.1.0/python_tests/runes/test_rune.py
--rw-r--r--   0      501       20      529 2024-03-11 09:19:07.000000 pyord-0.1.0/python_tests/runes/test_rune_id.py
--rw-r--r--   0      501       20     1997 2024-03-11 08:58:08.000000 pyord-0.1.0/python_tests/runes/test_runestone.py
--rw-r--r--   0      501       20      225 2024-03-07 19:16:59.000000 pyord-0.1.0/src/lib.rs
--rw-r--r--   0      501       20      867 2024-03-07 22:18:26.000000 pyord-0.1.0/src/runes/edict.rs
--rw-r--r--   0      501       20     1871 2024-03-07 19:54:36.000000 pyord-0.1.0/src/runes/etching.rs
--rw-r--r--   0      501       20     1269 2024-03-07 19:53:44.000000 pyord-0.1.0/src/runes/mint.rs
--rw-r--r--   0      501       20      983 2024-03-07 19:47:39.000000 pyord-0.1.0/src/runes/rune.rs
--rw-r--r--   0      501       20     1395 2024-03-11 09:21:24.000000 pyord-0.1.0/src/runes/rune_id.rs
--rw-r--r--   0      501       20     3057 2024-03-07 23:41:27.000000 pyord-0.1.0/src/runes/runestone.rs
--rw-r--r--   0      501       20      476 2024-03-11 09:12:58.000000 pyord-0.1.0/src/runes.rs
--rw-r--r--   0      501       20     1633 2024-03-07 23:29:04.000000 pyord-0.1.0/src/utils.rs
--rw-r--r--   0      501       20    93777 2024-03-07 19:16:59.000000 pyord-0.1.0/Cargo.lock
--rw-r--r--   0      501       20      579 2024-03-07 22:24:02.000000 pyord-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1431 1970-01-01 00:00:00.000000 pyord-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      380 1970-01-01 00:00:00.000000 pyord-0.2.0/Cargo.toml
+-rw-r--r--   0      501       20     2146 2024-03-12 09:08:22.000000 pyord-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0      501       20      686 2024-03-05 22:52:56.000000 pyord-0.2.0/.gitignore
+-rw-r--r--   0      501       20        0 2024-04-02 08:34:30.000000 pyord-0.2.0/.gitmodules
+-rw-r--r--   0      501       20      127 2024-03-11 12:27:12.000000 pyord-0.2.0/Dockerfile.build
+-rw-r--r--   0      501       20     1487 2024-04-02 22:59:40.000000 pyord-0.2.0/Makefile
+-rw-r--r--   0      501       20      632 2024-04-02 11:56:30.000000 pyord-0.2.0/README.md
+-rw-r--r--   0      501       20    14777 2024-04-02 22:43:40.000000 pyord-0.2.0/generate_stubs.py
+-rw-r--r--   0      501       20      834 2024-03-07 21:49:31.000000 pyord-0.2.0/ord.patch
+-rw-r--r--   0      501       20     6121 2024-04-02 22:52:33.000000 pyord-0.2.0/pyord.pyi
+-rw-r--r--   0      501       20        0 2024-03-07 19:16:59.000000 pyord-0.2.0/python_tests/__init__.py
+-rw-r--r--   0      501       20        0 2024-03-07 19:16:59.000000 pyord-0.2.0/python_tests/runes/__init__.py
+-rw-r--r--   0      501       20     1122 2024-04-02 18:14:57.000000 pyord-0.2.0/python_tests/runes/test_rune.py
+-rw-r--r--   0      501       20      559 2024-04-02 18:18:31.000000 pyord-0.2.0/python_tests/runes/test_rune_id.py
+-rw-r--r--   0      501       20     3343 2024-04-02 18:31:46.000000 pyord-0.2.0/python_tests/runes/test_runestone.py
+-rw-r--r--   0      501       20     1982 2024-04-02 22:51:16.000000 pyord-0.2.0/src/cenotaph.rs
+-rw-r--r--   0      501       20      992 2024-04-02 12:37:18.000000 pyord-0.2.0/src/edict.rs
+-rw-r--r--   0      501       20     2353 2024-04-02 21:56:32.000000 pyord-0.2.0/src/etching.rs
+-rw-r--r--   0      501       20     1210 2024-04-02 17:53:41.000000 pyord-0.2.0/src/flaw.rs
+-rw-r--r--   0      501       20      640 2024-04-02 22:52:22.000000 pyord-0.2.0/src/lib.rs
+-rw-r--r--   0      501       20      969 2024-04-02 14:49:08.000000 pyord-0.2.0/src/rune.rs
+-rw-r--r--   0      501       20     1622 2024-04-02 22:50:42.000000 pyord-0.2.0/src/rune_id.rs
+-rw-r--r--   0      501       20     3378 2024-04-02 21:56:45.000000 pyord-0.2.0/src/runestone.rs
+-rw-r--r--   0      501       20     2075 2024-04-02 22:51:11.000000 pyord-0.2.0/src/terms.rs
+-rw-r--r--   0      501       20     1633 2024-03-07 23:29:04.000000 pyord-0.2.0/src/utils.rs
+-rw-r--r--   0      501       20    23809 2024-04-02 08:33:48.000000 pyord-0.2.0/Cargo.lock
+-rw-r--r--   0      501       20      579 2024-03-07 22:24:02.000000 pyord-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1178 1970-01-01 00:00:00.000000 pyord-0.2.0/PKG-INFO
```

### Comparing `pyord-0.1.0/.github/workflows/CI.yml` & `pyord-0.2.0/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyord-0.1.0/.gitignore` & `pyord-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyord-0.1.0/README.md` & `pyord-0.2.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -4,23 +4,18 @@
 This project provides Python wrappers for [ord](https://github.com/ordinals/ord) internals.
 
 The project is very much WIP. Currently, only wrappers for structs and functions related to Runes are provided.
 
 The philosophy is to wrap `ord` internal structs as thinly as possible inside pyo3-compatible Rust, and to
 provide sane methods on top of them to enable use in Python.
 
-At the time of writing, patching `ord` is necessary to expose certain structs and functions that are not exposed
-in the public api of `ord`. Make targets `patch-ord` and `update-and-patch-ord` are provided for this.
-
 ## Development
 
 ```bash
 # python3.10 needs to be in PATH
-make init-submodules
-make patch-ord
 make develop  # creates a venv and installs `pyord` inside it
 make test  # test using pytest
 ```
 
 ## Building wheels
 
 ```bash
```

### Comparing `pyord-0.1.0/generate_stubs.py` & `pyord-0.2.0/generate_stubs.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     "__ge__": ([path_to_type("typing", "Any")], path_to_type("bool")),
     "__getattribute__": ([path_to_type("str")], path_to_type("typing", "Any")),
     "__getitem__": ([path_to_type("typing", "Any")], path_to_type("typing", "Any")),
     "__gt__": ([path_to_type("typing", "Any")], path_to_type("bool")),
     "__hash__": ([], path_to_type("int")),
     "__init__": ([], path_to_type("None")),
     "__init_subclass__": None,
+    "__int__": ([], path_to_type("int")),
     "__iter__": ([], path_to_type("typing", "Any")),
     "__le__": ([path_to_type("typing", "Any")], path_to_type("bool")),
     "__len__": ([], path_to_type("int")),
     "__lt__": ([path_to_type("typing", "Any")], path_to_type("bool")),
     "__module__": None,
     "__ne__": ([path_to_type("typing", "Any")], path_to_type("bool")),
     "__new__": None,
@@ -61,76 +62,76 @@
     ),
     "__sizeof__": None,
     "__str__": ([], path_to_type("str")),
     "__subclasshook__": None,
 }
 
 
-def module_stubs(module: Any) -> ast.Module:
-    types_to_import = {"typing"}
+def module_stubs(
+    module: Any,
+    *,
+    types_to_import: frozenset[str] = frozenset(('typing',)),
+) -> ast.Module:
     classes = []
     functions = []
     for member_name, member_value in inspect.getmembers(module):
         element_path = [module.__name__, member_name]
         if member_name.startswith("__"):
             pass
         elif inspect.isclass(member_value):
-            classes.append(class_stubs(member_name, member_value, element_path, types_to_import))
+            classes.append(class_stubs(member_name, member_value, element_path))
         elif inspect.isbuiltin(member_value):
             functions.append(
                 function_stub(
                     member_name,
                     member_value,
                     element_path,
-                    types_to_import,
                     in_class=False,
                 )
             )
         else:
             logging.warning(f"Unsupported root construction {member_name}")
     return ast.Module(
         body=[ast.Import(names=[ast.alias(name=t)]) for t in sorted(types_to_import)] + classes + functions,
         type_ignores=[],
     )
 
 
-def class_stubs(cls_name: str, cls_def: Any, element_path: List[str], types_to_import: Set[str]) -> ast.ClassDef:
+def class_stubs(cls_name: str, cls_def: Any, element_path: List[str]) -> ast.ClassDef:
     attributes: List[ast.AST] = []
     methods: List[ast.AST] = []
     magic_methods: List[ast.AST] = []
     constants: List[ast.AST] = []
     for member_name, member_value in inspect.getmembers(cls_def):
         current_element_path = [*element_path, member_name]
         if member_name == "__init__":
             try:
                 inspect.signature(cls_def)  # we check it actually exists
                 methods = [
                     function_stub(
                         member_name,
                         cls_def,
                         current_element_path,
-                        types_to_import,
                         in_class=True,
                     ),
                     *methods,
                 ]
             except ValueError as e:
                 if "no signature found" not in str(e):
                     raise ValueError(f"Error while parsing signature of {cls_name}.__init_") from e
         elif member_value == OBJECT_MEMBERS.get(member_name) or BUILTINS.get(member_name, ()) is None:
             pass
         elif inspect.isdatadescriptor(member_value):
-            attributes.extend(data_descriptor_stub(member_name, member_value, current_element_path, types_to_import))
+            attributes.extend(data_descriptor_stub(member_name, member_value, current_element_path))
         elif inspect.isroutine(member_value):
             (magic_methods if member_name.startswith("__") else methods).append(
                 function_stub(
                     member_name,
                     member_value,
                     current_element_path,
-                    types_to_import,
                     in_class=True,
                 )
             )
         elif member_name == "__match_args__":
             constants.append(
                 ast.AnnAssign(
                     target=ast.Name(id=member_name, ctx=ast.Store()),
@@ -144,15 +145,15 @@
                 )
             )
         elif member_value is not None:
             constants.append(
                 ast.AnnAssign(
                     target=ast.Name(id=member_name, ctx=ast.Store()),
                     annotation=concatenated_path_to_type(
-                        member_value.__class__.__name__, element_path, types_to_import
+                        member_value.__class__.__name__, element_path
                     ),
                     value=ast.Ellipsis(),
                     simple=1,
                 )
             )
         else:
             logging.warning(f"Unsupported member {member_name} of class {'.'.join(element_path)}")
@@ -169,22 +170,21 @@
     )
 
 
 def data_descriptor_stub(
     data_desc_name: str,
     data_desc_def: Any,
     element_path: List[str],
-    types_to_import: Set[str],
 ) -> Union[Tuple[ast.AnnAssign, ast.Expr], Tuple[ast.AnnAssign]]:
     annotation = None
     doc_comment = None
 
     doc = inspect.getdoc(data_desc_def)
     if doc is not None:
-        annotation = returns_stub(data_desc_name, doc, element_path, types_to_import)
+        annotation = returns_stub(data_desc_name, doc, element_path)
         m = re.findall(r"^ *:return: *(.*) *$", doc, re.MULTILINE)
         if len(m) == 1:
             doc_comment = m[0]
         elif len(m) > 1:
             raise ValueError(
                 f"Multiple return annotations found with :return: in {'.'.join(element_path)} documentation"
             )
@@ -198,15 +198,14 @@
     return (assign, doc_comment) if doc_comment else (assign,)
 
 
 def function_stub(
     fn_name: str,
     fn_def: Any,
     element_path: List[str],
-    types_to_import: Set[str],
     *,
     in_class: bool,
 ) -> ast.FunctionDef:
     body: List[ast.AST] = []
     doc = inspect.getdoc(fn_def)
     if doc is not None:
         doc_comment = build_doc_comment(doc)
@@ -215,28 +214,27 @@
 
     decorator_list = []
     if in_class and hasattr(fn_def, "__self__"):
         decorator_list.append(ast.Name("staticmethod"))
 
     return ast.FunctionDef(
         fn_name,
-        arguments_stub(fn_name, fn_def, doc or "", element_path, types_to_import),
+        arguments_stub(fn_name, fn_def, doc or "", element_path),
         body or [ast.Ellipsis()],
         decorator_list=decorator_list,
-        returns=returns_stub(fn_name, doc, element_path, types_to_import) if doc else None,
+        returns=returns_stub(fn_name, doc, element_path) if doc else None,
         lineno=0,
     )
 
 
 def arguments_stub(
     callable_name: str,
     callable_def: Any,
     doc: str,
     element_path: List[str],
-    types_to_import: Set[str],
 ) -> ast.arguments:
     real_parameters: Mapping[str, inspect.Parameter] = inspect.signature(callable_def).parameters
     if callable_name == "__init__":
         real_parameters = {
             "self": inspect.Parameter("self", inspect.Parameter.POSITIONAL_ONLY),
             **real_parameters,
         }
@@ -250,25 +248,24 @@
         param_names = list(real_parameters.keys())
         if param_names and param_names[0] == "self":
             del param_names[0]
         for name, t in zip(param_names, builtin[0]):
             parsed_param_types[name] = t
 
     # Types from comment
-    for match in re.findall(r"^ *:type *([a-z_]+): ([^\n]*) *$", doc, re.MULTILINE):
+    for match in re.findall(r"^ *:type *([a-zA-Z_][a-zA-Z0-9_]*): ([^\n]*) *$", doc, re.MULTILINE):
         if match[0] not in real_parameters:
             raise ValueError(
                 f"The parameter {match[0]} of {'.'.join(element_path)} "
                 "is defined in the documentation but not in the function signature"
             )
         type = match[1]
-        if type.endswith(", optional"):
+        if is_optional_type(type):
             optional_params.add(match[0])
-            type = type[:-10]
-        parsed_param_types[match[0]] = convert_type_from_doc(type, element_path, types_to_import)
+        parsed_param_types[match[0]] = convert_type_from_doc(type, element_path)
 
     # we parse the parameters
     posonlyargs = []
     args = []
     vararg = None
     kwonlyargs = []
     kw_defaults = []
@@ -281,19 +278,20 @@
                 "has no type definition in the function documentation"
             )
         param_ast = ast.arg(arg=param.name, annotation=parsed_param_types.get(param.name))
 
         default_ast = None
         if param.default != param.empty:
             default_ast = ast.Constant(param.default)
-            if param.name not in optional_params:
-                raise ValueError(
-                    f"Parameter {param.name} of {'.'.join(element_path)} "
-                    "is optional according to the type but not flagged as such in the doc"
-                )
+            # This makes no sense!
+            # if param.name not in optional_params:
+            #     raise ValueError(
+            #         f"Parameter {param.name} of {'.'.join(element_path)} "
+            #         "is optional according to the type but not flagged as such in the doc"
+            #     )
         elif param.name in optional_params:
             raise ValueError(
                 f"Parameter {param.name} of {'.'.join(element_path)} "
                 "is optional according to the documentation but has no default value"
             )
 
         if param.kind == param.POSITIONAL_ONLY:
@@ -317,102 +315,55 @@
         kwonlyargs=kwonlyargs,
         kw_defaults=kw_defaults,
         defaults=defaults,
         kwarg=kwarg,
     )
 
 
-def returns_stub(callable_name: str, doc: str, element_path: List[str], types_to_import: Set[str]) -> Optional[ast.AST]:
+def returns_stub(callable_name: str, doc: str, element_path: List[str]) -> Optional[ast.AST]:
     m = re.findall(r"^ *:rtype: *([^\n]*) *$", doc, re.MULTILINE)
     if len(m) == 0:
         builtin = BUILTINS.get(callable_name)
         if isinstance(builtin, tuple) and builtin[1] is not None:
             return builtin[1]
         raise ValueError(
             f"The return type of {'.'.join(element_path)} "
             "has no type definition using :rtype: in the function documentation"
         )
     if len(m) > 1:
         raise ValueError(f"Multiple return type annotations found with :rtype: for {'.'.join(element_path)}")
-    return convert_type_from_doc(m[0], element_path, types_to_import)
+    return convert_type_from_doc(m[0], element_path)
 
 
-def convert_type_from_doc(type_str: str, element_path: List[str], types_to_import: Set[str]) -> ast.AST:
+def convert_type_from_doc(type_str: str, element_path: List[str]) -> ast.AST:
     type_str = type_str.strip()
-    return parse_type_to_ast(type_str, element_path, types_to_import)
+    return parse_type_to_ast(type_str, element_path)
 
 
-def parse_type_to_ast(type_str: str, element_path: List[str], types_to_import: Set[str]) -> ast.AST:
-    # let's tokenize
-    tokens = []
-    current_token = ""
-    for c in type_str:
-        if "a" <= c <= "z" or "A" <= c <= "Z" or c == ".":
-            current_token += c
-        else:
-            if current_token:
-                tokens.append(current_token)
-            current_token = ""
-            if c != " ":
-                tokens.append(c)
-    if current_token:
-        tokens.append(current_token)
-
-    # let's first parse nested parenthesis
-    stack: List[List[Any]] = [[]]
-    for token in tokens:
-        if token == "[":
-            children: List[str] = []
-            stack[-1].append(children)
-            stack.append(children)
-        elif token == "]":
-            stack.pop()
-        else:
-            stack[-1].append(token)
-
-    # then it's easy
-    def parse_sequence(sequence: List[Any]) -> ast.AST:
-        # we split based on "or"
-        or_groups: List[List[str]] = [[]]
-        for e in sequence:
-            if e == "or":
-                or_groups.append([])
-            else:
-                or_groups[-1].append(e)
-        if any(not g for g in or_groups):
-            raise ValueError(f"Not able to parse type '{type_str}' used by {'.'.join(element_path)}")
-
-        new_elements: List[ast.AST] = []
-        for group in or_groups:
-            if len(group) == 1 and isinstance(group[0], str):
-                new_elements.append(concatenated_path_to_type(group[0], element_path, types_to_import))
-            elif len(group) == 2 and isinstance(group[0], str) and isinstance(group[1], list):
-                new_elements.append(
-                    ast.Subscript(
-                        value=concatenated_path_to_type(group[0], element_path, types_to_import),
-                        slice=parse_sequence(group[1]),
-                        ctx=ast.Load(),
-                    )
-                )
-            else:
-                raise ValueError(f"Not able to parse type '{type_str}' used by {'.'.join(element_path)}")
-        return reduce(lambda left, right: ast.BinOp(left=left, op=ast.BitOr(), right=right), new_elements)
+def parse_type_to_ast(type_str: str, element_path: List[str]) -> ast.AST:
+    try:
+        parsed = ast.parse(type_str, mode="eval").body
+    except SyntaxError as e:
+        raise ValueError(f"Not able to parse type '{type_str}' used by {'.'.join(element_path)}") from e
+    if isinstance(parsed, ast.Attribute):
+        pass
+    return parsed
 
-    return parse_sequence(stack[0])
 
-
-def concatenated_path_to_type(path: str, element_path: List[str], types_to_import: Set[str]) -> ast.AST:
+def concatenated_path_to_type(path: str, element_path: List[str]) -> ast.AST:
     parts = path.split(".")
     if any(not p for p in parts):
         raise ValueError(f"Not able to parse type '{path}' used by {'.'.join(element_path)}")
-    if len(parts) > 1:
-        types_to_import.add(".".join(parts[:-1]))
     return path_to_type(*parts)
 
 
+def is_optional_type(type_str: str) -> bool:
+    return type_str.startswith('typing.Optional')
+
+
 def build_doc_comment(doc: str) -> Optional[ast.Expr]:
     lines = [line.strip() for line in doc.split("\n")]
     clean_lines = []
     for line in lines:
         if line.startswith((":type", ":rtype")):
             continue
         clean_lines.append(line)
@@ -429,12 +380,23 @@
     parser.add_argument("module_name", help="Name of the Python module for which generate stubs")
     parser.add_argument(
         "out",
         help="Name of the Python stub file to write to",
         type=argparse.FileType("wt"),
     )
     parser.add_argument("--ruff", help="Formats the generated stubs using Ruff", action="store_true")
+    parser.add_argument(
+        "--imports",
+        type=lambda s: frozenset(i.strip() for i in s.split(',') if i.strip()),
+        help="Comma-separated list of modules to import at the start of the stubs file",
+        default=frozenset(('typing',)),
+    )
     args = parser.parse_args()
-    stub_content = ast.unparse(module_stubs(importlib.import_module(args.module_name)))
+    stub_content = ast.unparse(
+        module_stubs(
+            importlib.import_module(args.module_name),
+            types_to_import=args.imports,
+        ),
+    )
     args.out.write(stub_content)
     if args.ruff:
         format_with_ruff(args.out.name)
```

### Comparing `pyord-0.1.0/ord.patch` & `pyord-0.2.0/ord.patch`

 * *Files identical despite different names*

### Comparing `pyord-0.1.0/pyord.pyi` & `pyord-0.2.0/pyord.pyi`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,144 @@
 import typing
 
 @typing.final
+class Cenotaph:
+    """Cenotaph"""
+    etching: typing.Optional[Rune]
+    flaws: list[Flaw]
+    is_cenotaph: bool
+    mint: typing.Optional[RuneId]
+
+    def __init__(self, /, flaws: list[Flaw], etching: typing.Optional[Rune]=None, mint: typing.Optional[RuneId]=None) -> None:
+        """Cenotaph"""
+
+    def __eq__(self, value: typing.Any, /) -> bool:
+        """Return self==value."""
+
+    def __ge__(self, value: typing.Any, /) -> bool:
+        """Return self>=value."""
+
+    def __gt__(self, value: typing.Any, /) -> bool:
+        """Return self>value."""
+
+    def __le__(self, value: typing.Any, /) -> bool:
+        """Return self<=value."""
+
+    def __lt__(self, value: typing.Any, /) -> bool:
+        """Return self<value."""
+
+    def __ne__(self, value: typing.Any, /) -> bool:
+        """Return self!=value."""
+
+    def __repr__(self, /) -> str:
+        """Return repr(self)."""
+
+@typing.final
 class Edict:
     amount: int
-    id: int
+    id: RuneId
     output: int
 
-    def __init__(self, /, id: int, amount: int, output: int) -> None:...
+    def __init__(self, /, id: RuneId, amount: int, output: int) -> None:...
 
     def __repr__(self, /) -> str:
         """Return repr(self)."""
 
 @typing.final
 class Etching:
-    divisibility: int
-    mint: typing.Optional[Mint]
+    divisibility: typing.Optional[int]
+    premine: typing.Optional[int]
     rune: typing.Optional[Rune]
     spacers: int
     symbol: typing.Optional[str]
+    terms: typing.Optional[Terms]
 
-    def __init__(self, /, divisibility: int, spacers: int, mint: typing.Optional[Mint]=None, rune: typing.Optional[Rune]=None, symbol: typing.Optional[str]=None) -> None:...
+    def __init__(self, /, divisibility: typing.Optional[int]=None, premine: typing.Optional[int]=None, rune: typing.Optional[Rune]=None, spacers: typing.Optional[int]=None, symbol: typing.Optional[str]=None, terms: typing.Optional[Terms]=None) -> None:...
 
     def __repr__(self, /) -> str:
         """Return repr(self)."""
 
 @typing.final
-class Mint:
-    deadline: typing.Optional[int]
-    limit: typing.Optional[int]
-    term: typing.Optional[int]
+class Flaw:
+    """A Flaw in a Runestone that makes it a Cenotaph
+:param n: Flaw as integer"""
+    flag: int
+    reason: str
+
+    def __init__(self, /, n: int) -> None:
+        """A Flaw in a Runestone that makes it a Cenotaph
+:param n: Flaw as integer"""
+
+    @staticmethod
+    def all() -> list[Flaw]:...
 
-    def __init__(self, /, deadline: typing.Optional[int]=None, limit: typing.Optional[int]=None, term: typing.Optional[int]=None) -> None:...
+    def __eq__(self, value: typing.Any, /) -> bool:
+        """Return self==value."""
+
+    def __ge__(self, value: typing.Any, /) -> bool:
+        """Return self>=value."""
+
+    def __gt__(self, value: typing.Any, /) -> bool:
+        """Return self>value."""
+
+    def __int__(self, /) -> int:
+        """int(self)"""
+
+    def __le__(self, value: typing.Any, /) -> bool:
+        """Return self<=value."""
+
+    def __lt__(self, value: typing.Any, /) -> bool:
+        """Return self<value."""
+
+    def __ne__(self, value: typing.Any, /) -> bool:
+        """Return self!=value."""
 
     def __repr__(self, /) -> str:
         """Return repr(self)."""
 
 @typing.final
 class Rune:
     """Rune
-:param num: The rune number"""
+:param n: The rune number"""
+    n: int
     name: str
-    num: int
 
-    def __init__(self, /, num: int) -> None:
+    def __init__(self, /, n: int) -> None:
         """Rune
-:param num: The rune number"""
+:param n: The rune number"""
 
     @staticmethod
     def from_str(s: str) -> Rune:
         """convert the string representation of the rune to a rune
 :param s: the string representation of the rune"""
 
     def __repr__(self, /) -> str:
         """Return repr(self)."""
 
 @typing.final
 class RuneId:
     """RuneId
-:param height: Etching block height
-:param index: Etching transaction index"""
-    height: int
-    index: int
-    num: int
-    'number suitable for use as Edict id'
+:param block: Etching block height
+:param tx: Etching transaction index"""
+    block: int
+    tx: int
 
-    def __init__(self, /, height: int, index: int) -> None:
+    def __init__(self, /, block: int, tx: int) -> None:
         """RuneId
-:param height: Etching block height
-:param index: Etching transaction index"""
+:param block: Etching block height
+:param tx: Etching transaction index"""
+
+    def delta(self, /, next: RuneId) -> typing.Optional[typing.Tuple[int, int]]:...
 
     @staticmethod
-    def from_num(num: int) -> RuneId:
-        """Parse the RuneId from a number usable as Edict id"""
+    def from_str(s: str) -> RuneId:
+        """Parse the RuneId from a string "block:tx"
+:param s: block height and tx separated by a colon"""
+
+    def next(self, /, block: int, tx: int) -> typing.Optional[RuneId]:...
 
     def __eq__(self, value: typing.Any, /) -> bool:
         """Return self==value."""
 
     def __ge__(self, value: typing.Any, /) -> bool:
         """Return self>=value."""
 
@@ -93,29 +156,29 @@
 
     def __repr__(self, /) -> str:
         """Return repr(self)."""
 
 @typing.final
 class Runestone:
     """Runestone"""
-    burn: bool
-    claim: typing.Optional[int]
-    default_output: typing.Optional[int]
     edicts: typing.List[Edict]
     etching: typing.Optional[Etching]
+    is_cenotaph: bool
+    mint: typing.Optional[RuneId]
+    pointer: typing.Optional[int]
 
-    def __init__(self, /, burn: bool=False, edicts: typing.Iterable[Edict]=(), claim: typing.Optional[int]=None, default_output: typing.Optional[int]=None, etching: typing.Optional[Etching]=None) -> None:
+    def __init__(self, /, edicts: typing.Optional[typing.Iterable[Edict]]=None, etching: typing.Optional[Etching]=None, mint: typing.Optional[RuneId]=None, pointer: typing.Optional[int]=None) -> None:
         """Runestone"""
 
     @staticmethod
-    def from_hex_tx(hex_tx: str) -> typing.Optional[Runestone]:
-        """Return a Runestone from a Bitcoin transaction, or None if the transaction contains no
-Runestone"""
+    def decipher_hex(hex_tx: str) -> typing.Union[Runestone, Cenotaph, None]:
+        """Return a Runestone or Cenotaph from a Bitcoin transaction, or None if the transaction
+contains no Runestone"""
 
-    def script_pubkey(self, /) -> bytes:
+    def encipher(self, /) -> bytes:
         """get the scriptPubKey of the Runestone"""
 
     def __eq__(self, value: typing.Any, /) -> bool:
         """Return self==value."""
 
     def __ge__(self, value: typing.Any, /) -> bool:
         """Return self>=value."""
@@ -129,8 +192,20 @@
     def __lt__(self, value: typing.Any, /) -> bool:
         """Return self<value."""
 
     def __ne__(self, value: typing.Any, /) -> bool:
         """Return self!=value."""
 
     def __repr__(self, /) -> str:
+        """Return repr(self)."""
+
+@typing.final
+class Terms:
+    amount: typing.Optional[int]
+    cap: typing.Optional[int]
+    height: tuple[typing.Optional[int], typing.Optional[int]]
+    offset: tuple[typing.Optional[int], typing.Optional[int]]
+
+    def __init__(self, /, amount: typing.Optional[int]=None, cap: typing.Optional[int]=None, height: tuple[typing.Optional[int], typing.Optional[int]]=..., offset: tuple[typing.Optional[int], typing.Optional[int]]=...) -> None:...
+
+    def __repr__(self, /) -> str:
         """Return repr(self)."""
```

### Comparing `pyord-0.1.0/python_tests/runes/test_rune.py` & `pyord-0.2.0/python_tests/runes/test_rune.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,16 +41,16 @@
         (U128_MAX - 1, "BCGDENLQRQWDSLRUGSNLBTMFIJAU"),
         (U128_MAX, "BCGDENLQRQWDSLRUGSNLBTMFIJAV"),
     ]
 )
 def test_round_trip(n: int, s: str):
     a = pyord.Rune(n)
     assert a.name == s
-    assert a.num == n
+    assert a.n == n
     b = pyord.Rune.from_str(s)
     assert b.name == s
-    assert b.num == n
+    assert b.n == n
     if n != U128_MAX:
         assert a != pyord.Rune(n + 1)
     if n != 0:
         assert a != pyord.Rune(n - 1)
```

### Comparing `pyord-0.1.0/src/runes/edict.rs` & `pyord-0.2.0/src/edict.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 use pyo3::prelude::*;
 
-use ord::runes::Edict;
+use ordinals::Edict;
+use super::rune_id::PyRuneId;
 
-/// :type id: int
+/// :type id: RuneId
 /// :type amount: int
 /// :type output: int
 #[pyclass(name="Edict")]
 #[derive(Debug, PartialEq, Copy, Clone)]
 pub struct PyEdict(pub Edict);
 
 
 #[pymethods]
 impl PyEdict {
     #[new]
     pub fn new(
-        id: u128,
+        id: PyRuneId,
         amount: u128,
-        output: u128,
+        output: u32,
     ) -> Self {
         PyEdict(Edict {
-            id,
+            id: id.0,
             amount,
             output,
         })
     }
 
     pub fn __repr__(&self) -> String {
-        format!("Edict(id={}, amount={}, output={})", self.id(), self.amount(), self.output())
+        format!(
+            "Edict(id={}, amount={}, output={})",
+            self.id().__repr__(),
+            self.amount(),
+            self.output()
+        )
     }
 
-    /// :rtype: int
+    /// :rtype: RuneId
     #[getter]
-    pub fn id(&self) -> u128 {
-        self.0.id
+    pub fn id(&self) -> PyRuneId {
+        PyRuneId(self.0.id)
     }
 
     /// :rtype: int
     #[getter]
     pub fn amount(&self) -> u128 {
         self.0.amount
     }
 
     /// :rtype: int
     #[getter]
-    pub fn output(&self) -> u128 {
+    pub fn output(&self) -> u32 {
         self.0.output
     }
 }
```

### Comparing `pyord-0.1.0/src/runes/etching.rs` & `pyord-0.2.0/src/etching.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,75 +1,85 @@
 use pyo3::prelude::*;
-use ord::runes::Etching;
+use ordinals::Etching;
 
-use super::mint::PyMint;
+use super::terms::PyTerms;
 use super::rune::PyRune;
 
-/// :type divisibility: int
-/// :type mint: typing.Optional[Mint], optional
-/// :type rune: typing.Optional[Rune], optional
-/// :type spacers: int
-/// :type symbol: typing.Optional[str], optional
+/// :type divisibility: typing.Optional[int]
+/// :type premine: typing.Optional[int]
+/// :type rune: typing.Optional[Rune]
+/// :type spacers: typing.Optional[int]
+/// :type symbol: typing.Optional[str]
+/// :type terms: typing.Optional[Terms]
 #[pyclass(name="Etching")]
 #[derive(Debug, PartialEq, Copy, Clone)]
 pub struct PyEtching(pub Etching);
 
 #[pymethods]
 impl PyEtching {
     #[new]
     pub fn new(
-        divisibility: u8,
-        spacers: u32,
-        mint: Option<PyMint>,
+        divisibility: Option<u8>,
+        premine: Option<u128>,
         rune: Option<PyRune>,
+        spacers: Option<u32>,
         symbol: Option<char>,
+        terms: Option<PyTerms>,
     ) -> Self {
         Self(Etching {
             divisibility,
-            mint: mint.map(|m| m.0),
+            premine,
             rune: rune.map(|r| r.0),
             spacers,
             symbol,
+            terms: terms.map(|m| m.0),
         })
     }
 
     pub fn __repr__(&self) -> String {
         format!(
-            "Etching(divisibility={}, mint={}, rune={}, spacers={}, symbol={})",
-            self.divisibility(),
-            self.mint().map(|m| m.__repr__()).unwrap_or("None".to_string()),
+            "Etching(divisibility={}, premine={}, rune={}, spacers={}, symbol={}, terms={})",
+            self.divisibility().map(|i| i.to_string()).unwrap_or("None".to_string()),
+            self.premine().map(|i| i.to_string()).unwrap_or("None".to_string()),
             self.rune().map(|r| r.__repr__()).unwrap_or("None".to_string()),
-            self.spacers(),
+            self.spacers().map(|i| i.to_string()).unwrap_or("None".to_string()),
             self.symbol().map(|s| format!("'{}'", s.to_string())).unwrap_or("None".to_string()),
+            self.terms().map(|m| m.__repr__()).unwrap_or("None".to_string()),
         )
     }
 
-    /// :rtype: int
+    /// :rtype: typing.Optional[int]
     #[getter]
-    pub fn divisibility(&self) -> u8 {
+    pub fn divisibility(&self) -> Option<u8> {
         self.0.divisibility
     }
 
-    /// :rtype: typing.Optional[Mint]
+    /// :rtype: typing.Optional[int]
     #[getter]
-    pub fn mint(&self) -> Option<PyMint> {
-        self.0.mint.map(|m| PyMint(m))
+    pub fn premine(&self) -> Option<u128> {
+        self.0.premine
     }
 
     /// :rtype: typing.Optional[Rune]
     #[getter]
     pub fn rune(&self) -> Option<PyRune> {
         self.0.rune.map(|r| PyRune(r))
     }
 
     /// :rtype: int
     #[getter]
-    pub fn spacers(&self) -> u32 {
+    pub fn spacers(&self) -> Option<u32> {
         self.0.spacers
     }
 
     /// :rtype: typing.Optional[str]
     #[getter]
     pub fn symbol(&self) -> Option<char> {
         self.0.symbol
     }
+
+    /// :rtype: typing.Optional[Terms]
+    #[getter]
+    pub fn terms(&self) -> Option<PyTerms> {
+        self.0.terms.map(|m| PyTerms(m))
+    }
 }
```

### Comparing `pyord-0.1.0/src/runes/rune.rs` & `pyord-0.2.0/src/rune.rs`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 use pyo3::prelude::*;
 
-use ord::runes::Rune;
+use ordinals::Rune;
 
 /// Rune
-/// :param num: The rune number
-/// :type num: int
+/// :param n: The rune number
+/// :type n: int
 #[pyclass(name="Rune")]
 #[derive(Debug, PartialEq, Copy, Clone, PartialOrd, Ord, Eq)]
 pub struct PyRune(pub Rune);
 
 
 #[pymethods]
 impl PyRune {
     #[new]
-    pub fn new(num: u128) -> Self {
-        PyRune(Rune(num))
+    pub fn new(n: u128) -> Self {
+        PyRune(Rune(n))
     }
 
     /// the number (id) of the rune
     /// :rtype: int
     #[getter]
-    pub fn num(&self) -> u128 {
+    pub fn n(&self) -> u128 {
         self.0 .0
     }
 
-    /// the name of the rune as string
+    /// the name of the rune as a string
     /// :rtype: str
     #[getter]
     pub fn name(&self) -> String {
         self.0.to_string()
     }
 
     pub fn __repr__(&self) -> String {
-        format!("Rune(num={}, name='{}')", self.num(), self.name())
+        format!("Rune(n={}, name='{}')", self.n(), self.name())
     }
 
     /// convert the string representation of the rune to a rune
     /// :param s: the string representation of the rune
     /// :type s: str
     /// :rtype: Rune
     #[staticmethod]
```

### Comparing `pyord-0.1.0/src/runes/runestone.rs` & `pyord-0.2.0/src/runestone.rs`

 * *Files 15% similar despite different names*

```diff
@@ -1,106 +1,113 @@
 use pyo3::prelude::*;
 use pyo3::types::PyBytes;
 
-use ord::runes::Runestone;
+use ordinals::Artifact;
+use ordinals::Runestone;
 
 use crate::utils::hex_to_bitcoin_tx;
 
 use super::edict::PyEdict;
 use super::etching::PyEtching;
+use super::rune_id::PyRuneId;
+use super::cenotaph::PyCenotaph;
 
 /// Runestone
-/// :type burn: bool, optional
-/// :type claim: typing.Optional[int], optional
-/// :type default_output: typing.Optional[int], optional
-/// :type edicts: typing.Iterable[Edict], optional
-/// :type etching: typing.Optional[Etching], optional
+/// :type edicts: typing.Optional[typing.Iterable[Edict]]
+/// :type etching: typing.Optional[Etching]
+/// :type mint: typing.Optional[RuneId]
+/// :type pointer: typing.Optional[int]
 #[pyclass(name="Runestone")]
 #[derive(Debug, PartialEq)]
 pub struct PyRunestone(pub Runestone);
 
 
 #[pymethods]
 impl PyRunestone {
     #[new]
-    #[pyo3(text_signature = "(burn=False, edicts=(), claim=None, default_output=None, etching=None)")]
+    #[pyo3(signature = (edicts=None, etching=None, mint=None, pointer=None))]
     pub fn new(
-        burn: Option<bool>,
         edicts: Option<Vec<PyEdict>>,
-        claim: Option<u128>,
-        default_output: Option<u32>,
         etching: Option<PyEtching>,
+        mint: Option<PyRuneId>,
+        pointer: Option<u32>,
     ) -> Self {
         PyRunestone(Runestone {
-            burn: burn.unwrap_or(false),
-            claim,
-            default_output,
             edicts: edicts.unwrap_or_default().into_iter().map(|e| e.0).collect(),
             etching: etching.map(|e| e.0),
+            mint: mint.map(|m| m.0),
+            pointer,
         })
     }
 
-    /// Return a Runestone from a Bitcoin transaction, or None if the transaction contains no
-    /// Runestone
+    /// Return a Runestone or Cenotaph from a Bitcoin transaction, or None if the transaction
+    /// contains no Runestone
     /// :type hex_tx: str
-    /// :rtype: typing.Optional[Runestone]
+    /// :rtype: typing.Union[Runestone, Cenotaph, None]
     #[staticmethod]
-    pub fn from_hex_tx(hex_tx: &str) -> PyResult<Option<Self>> {
+    pub fn decipher_hex(py: Python, hex_tx: &str) -> PyResult<Option<PyObject>> {
         let tx = hex_to_bitcoin_tx(hex_tx)?;
-        Ok(Runestone::from_transaction(&tx).map(|r| PyRunestone(r)))
+        let result = Runestone::decipher(&tx);
+        match result {
+            None => Ok(None),
+            Some(artifact) => match artifact {
+                Artifact::Cenotaph(cenotaph) => Ok(Some(PyCenotaph(cenotaph).into_py(py))),
+                Artifact::Runestone(runestone) => Ok(Some(PyRunestone(runestone).into_py(py))),
+            },
+        }
     }
 
     /// get the scriptPubKey of the Runestone
     /// :rtype: bytes
-    pub fn script_pubkey(&self, py: Python) -> PyObject {
+    pub fn encipher(&self, py: Python) -> PyObject {
         let buffer = self.0.encipher().into_bytes();
         // TODO: check that this doesn't leak memory
         PyBytes::new(py, &buffer).into()
     }
 
     pub fn __repr__(&self) -> String {
         format!(
-            "Runestone(burn={}, claim={}, default_output={}, edicts={})",
-            self.burn(),
-            self.claim().map(|d| d.to_string()).unwrap_or("None".to_string()),
-            self.default_output().map(|d| d.to_string()).unwrap_or("None".to_string()),
+            "Runestone(edicts={}, etching={}, mint={}, pointer={})",
             format!(
                 "[{}]",
                 self.edicts().iter().map(|e| e.__repr__()).collect::<Vec<String>>().join(", ")
             ),
+            self.etching().map(|e| e.__repr__()).unwrap_or("None".to_string()),
+            self.mint().map(|m| m.__repr__()).unwrap_or("None".to_string()),
+            self.pointer().map(|i| i.to_string()).unwrap_or("None".to_string()),
         )
     }
 
     pub fn __eq__(&self, other: &PyRunestone) -> bool {
         self.0 == other.0
     }
 
-    /// :rtype: bool
+    /// :rtype: typing.Optional[Etching]
     #[getter]
-    pub fn burn(&self) -> bool {
-        self.0.burn
+    pub fn etching(&self) -> Option<PyEtching> {
+        self.0.etching.map(|e| PyEtching(e))
     }
 
-    /// :rtype: typing.Optional[int]
+    /// :rtype: typing.List[Edict]
     #[getter]
-    pub fn claim(&self) -> Option<u128> {
-        self.0.claim
+    pub fn edicts(&self) -> Vec<PyEdict> {
+        self.0.edicts.iter().map(|e| PyEdict(*e)).collect()
     }
 
-    /// :rtype: typing.Optional[int]
+    /// :rtype: typing.Optional[RuneId]
     #[getter]
-    pub fn default_output(&self) -> Option<u32> {
-        self.0.default_output
+    pub fn mint(&self) -> Option<PyRuneId> {
+        self.0.mint.map(|m| PyRuneId(m))
     }
 
-    /// :rtype: typing.List[Edict]
+    /// :rtype: typing.Optional[int]
     #[getter]
-    pub fn edicts(&self) -> Vec<PyEdict> {
-        self.0.edicts.iter().map(|e| PyEdict(*e)).collect()
+    pub fn pointer(&self) -> Option<u32> {
+        self.0.pointer
     }
 
-    /// :rtype: typing.Optional[Etching]
+    /// :rtype: bool
     #[getter]
-    pub fn etching(&self) -> Option<PyEtching> {
-        self.0.etching.map(|e| PyEtching(e))
+    pub fn is_cenotaph(&self) -> bool {
+        false
     }
 }
```

### Comparing `pyord-0.1.0/src/utils.rs` & `pyord-0.2.0/src/utils.rs`

 * *Files identical despite different names*

### Comparing `pyord-0.1.0/pyproject.toml` & `pyord-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyord-0.1.0/PKG-INFO` & `pyord-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyord
-Version: 0.1.0
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: python-bitcointx ; extra == 'dev'
 Requires-Dist: ipython ; extra == 'dev'
 Requires-Dist: ipdb ; extra == 'dev'
 Requires-Dist: pytest ; extra == 'dev'
@@ -19,23 +19,18 @@
 This project provides Python wrappers for [ord](https://github.com/ordinals/ord) internals.
 
 The project is very much WIP. Currently, only wrappers for structs and functions related to Runes are provided.
 
 The philosophy is to wrap `ord` internal structs as thinly as possible inside pyo3-compatible Rust, and to
 provide sane methods on top of them to enable use in Python.
 
-At the time of writing, patching `ord` is necessary to expose certain structs and functions that are not exposed
-in the public api of `ord`. Make targets `patch-ord` and `update-and-patch-ord` are provided for this.
-
 ## Development
 
 ```bash
 # python3.10 needs to be in PATH
-make init-submodules
-make patch-ord
 make develop  # creates a venv and installs `pyord` inside it
 make test  # test using pytest
 ```
 
 ## Building wheels
 
 ```bash
```

