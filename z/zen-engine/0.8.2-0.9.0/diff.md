# Comparing `tmp/zen_engine-0.8.2.tar.gz` & `tmp/zen_engine-0.9.0.tar.gz`

## Comparing `zen_engine-0.8.2.tar` & `zen_engine-0.9.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 zen_engine-0.8.2/local_dependencies/zen-expression/Cargo.toml
--rw-r--r--   0     1001      123     2347 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/README.md
--rw-r--r--   0     1001      123      625 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/benches/isolate.rs
--rw-r--r--   0     1001      123    93335 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/benches/lexer.rs
--rw-r--r--   0     1001      123    93602 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/benches/standard.rs
--rw-r--r--   0     1001      123      867 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/benches/unary.rs
--rw-r--r--   0     1001      123      970 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/ast.rs
--rw-r--r--   0     1001      123    19250 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/compiler.rs
--rw-r--r--   0     1001      123     1479 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/helpers.rs
--rw-r--r--   0     1001      123     6816 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/isolate.rs
--rw-r--r--   0     1001      123      783 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/codes.rs
--rw-r--r--   0     1001      123     2035 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/cursor.rs
--rw-r--r--   0     1001      123      404 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/error.rs
--rw-r--r--   0     1001      123     6339 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/lexer.rs
--rw-r--r--   0     1001      123       88 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/mod.rs
--rw-r--r--   0     1001      123      273 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/token.rs
--rw-r--r--   0     1001      123      203 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/lib.rs
--rw-r--r--   0     1001      123     4010 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/opcodes.rs
--rw-r--r--   0     1001      123      922 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/definitions.rs
--rw-r--r--   0     1001      123      638 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/error.rs
--rw-r--r--   0     1001      123     5318 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/iter.rs
--rw-r--r--   0     1001      123      131 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/mod.rs
--rw-r--r--   0     1001      123     4286 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/standard/constants.rs
--rw-r--r--   0     1001      123    14053 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/standard/mod.rs
--rw-r--r--   0     1001      123     2604 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/unary/constants.rs
--rw-r--r--   0     1001      123     9905 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/unary/mod.rs
--rw-r--r--   0     1001      123    51034 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/src/vm.rs
--rw-r--r--   0     1001      123    23163 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/tests/isolate.rs
--rw-r--r--   0     1001      123    11822 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/tests/lexer.rs
--rw-r--r--   0     1001      123     9097 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/tests/standard.rs
--rw-r--r--   0     1001      123     5185 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-expression/tests/unary.rs
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.8.2/local_dependencies/zen-engine/Cargo.toml
--rw-r--r--   0     1001      123     4305 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/README.md
--rw-r--r--   0     1001      123     1558 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/benches/engine.rs
--rw-r--r--   0     1001      123     2031 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/decision.rs
--rw-r--r--   0     1001      123     2605 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/engine.rs
--rw-r--r--   0     1001      123     2222 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/error.rs
--rw-r--r--   0     1001      123     1651 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/decision.rs
--rw-r--r--   0     1001      123     2136 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/expression/mod.rs
--rw-r--r--   0     1001      123     1097 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/mod.rs
--rw-r--r--   0     1001      123     3046 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/script.rs
--rw-r--r--   0     1001      123     6485 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
--rw-r--r--   0     1001      123      528 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
--rw-r--r--   0     1001      123     1747 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/vm.rs
--rw-r--r--   0     1001      123    11347 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/graph.rs
--rw-r--r--   0     1001      123      115 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/mod.rs
--rw-r--r--   0     1001      123      745 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/node.rs
--rw-r--r--   0     1001      123      807 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/table/mod.rs
--rw-r--r--   0     1001      123     5632 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/table/zen.rs
--rw-r--r--   0     1001      123     4796 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/lib.rs
--rw-r--r--   0     1001      123      715 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/closure.rs
--rw-r--r--   0     1001      123     2449 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/filesystem.rs
--rw-r--r--   0     1001      123     1245 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/memory.rs
--rw-r--r--   0     1001      123      892 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/mod.rs
--rw-r--r--   0     1001      123      466 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/noop.rs
--rw-r--r--   0     1001      123     3160 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/model/mod.rs
--rw-r--r--   0     1001      123     9076 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/util/json_map.rs
--rw-r--r--   0     1001      123       25 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/src/util/mod.rs
--rw-r--r--   0     1001      123     2081 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/tests/decision.rs
--rw-r--r--   0     1001      123     4759 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/tests/engine.rs
--rw-r--r--   0     1001      123     1381 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/tests/model.rs
--rw-r--r--   0     1001      123      884 2023-07-27 20:02:57.000000 zen_engine-0.8.2/local_dependencies/zen-engine/tests/support/mod.rs
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.8.2/Cargo.toml
--rw-r--r--   0     1001      123      135 2023-07-27 20:02:57.000000 zen_engine-0.8.2/.bumpversion.cfg
--rw-r--r--   0     1001      123      691 2023-07-27 20:02:57.000000 zen_engine-0.8.2/.gitignore
--rw-r--r--   0     1001      123     1057 2023-07-27 20:02:57.000000 zen_engine-0.8.2/LICENSE
--rw-r--r--   0     1001      123     5965 2023-07-27 20:02:57.000000 zen_engine-0.8.2/README.md
--rw-r--r--   0     1001      123     1578 2023-07-27 20:02:57.000000 zen_engine-0.8.2/index.py
--rw-r--r--   0     1001      123      966 2023-07-27 20:02:57.000000 zen_engine-0.8.2/pyproject.toml
--rw-r--r--   0     1001      123     1517 2023-07-27 20:02:57.000000 zen_engine-0.8.2/src/decision.rs
--rw-r--r--   0     1001      123     3100 2023-07-27 20:02:57.000000 zen_engine-0.8.2/src/engine.rs
--rw-r--r--   0     1001      123      335 2023-07-27 20:02:57.000000 zen_engine-0.8.2/src/lib.rs
--rw-r--r--   0     1001      123     1188 2023-07-27 20:02:57.000000 zen_engine-0.8.2/src/loader.rs
--rw-r--r--   0     1001      123     1122 2023-07-27 20:02:57.000000 zen_engine-0.8.2/src/value.rs
--rw-r--r--   0     1001      123    48279 2023-07-27 20:03:04.000000 zen_engine-0.8.2/Cargo.lock
--rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 zen_engine-0.9.0/local_dependencies/zen-expression/Cargo.toml
+-rw-r--r--   0     1001      123     2347 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/README.md
+-rw-r--r--   0     1001      123      625 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/benches/isolate.rs
+-rw-r--r--   0     1001      123    93335 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/benches/lexer.rs
+-rw-r--r--   0     1001      123    93602 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/benches/standard.rs
+-rw-r--r--   0     1001      123      867 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/benches/unary.rs
+-rw-r--r--   0     1001      123      970 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/ast.rs
+-rw-r--r--   0     1001      123    19259 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/compiler.rs
+-rw-r--r--   0     1001      123     1479 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/helpers.rs
+-rw-r--r--   0     1001      123     6816 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/isolate.rs
+-rw-r--r--   0     1001      123      783 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/lexer/codes.rs
+-rw-r--r--   0     1001      123     2035 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/lexer/cursor.rs
+-rw-r--r--   0     1001      123      404 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/lexer/error.rs
+-rw-r--r--   0     1001      123     6339 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/lexer/lexer.rs
+-rw-r--r--   0     1001      123       88 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/lexer/mod.rs
+-rw-r--r--   0     1001      123      273 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/lexer/token.rs
+-rw-r--r--   0     1001      123      203 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/lib.rs
+-rw-r--r--   0     1001      123     3985 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/opcodes.rs
+-rw-r--r--   0     1001      123      922 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/definitions.rs
+-rw-r--r--   0     1001      123      638 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/error.rs
+-rw-r--r--   0     1001      123     5318 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/iter.rs
+-rw-r--r--   0     1001      123      131 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/mod.rs
+-rw-r--r--   0     1001      123     4338 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/standard/constants.rs
+-rw-r--r--   0     1001      123    14379 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/standard/mod.rs
+-rw-r--r--   0     1001      123     2652 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/unary/constants.rs
+-rw-r--r--   0     1001      123     9905 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/unary/mod.rs
+-rw-r--r--   0     1001      123    50614 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/src/vm.rs
+-rw-r--r--   0     1001      123    23628 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/tests/isolate.rs
+-rw-r--r--   0     1001      123    11822 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/tests/lexer.rs
+-rw-r--r--   0     1001      123     9146 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/tests/standard.rs
+-rw-r--r--   0     1001      123     5206 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-expression/tests/unary.rs
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.9.0/local_dependencies/zen-engine/Cargo.toml
+-rw-r--r--   0     1001      123     4305 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/README.md
+-rw-r--r--   0     1001      123     1558 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/benches/engine.rs
+-rw-r--r--   0     1001      123     2031 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/decision.rs
+-rw-r--r--   0     1001      123     2605 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/engine.rs
+-rw-r--r--   0     1001      123     2222 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/error.rs
+-rw-r--r--   0     1001      123     1651 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/decision.rs
+-rw-r--r--   0     1001      123     2136 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/expression/mod.rs
+-rw-r--r--   0     1001      123     1097 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/function/mod.rs
+-rw-r--r--   0     1001      123     3046 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/function/script.rs
+-rw-r--r--   0     1001      123     6485 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
+-rw-r--r--   0     1001      123      528 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
+-rw-r--r--   0     1001      123     1747 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/function/vm.rs
+-rw-r--r--   0     1001      123    11347 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/graph.rs
+-rw-r--r--   0     1001      123      115 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/mod.rs
+-rw-r--r--   0     1001      123      745 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/node.rs
+-rw-r--r--   0     1001      123      807 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/table/mod.rs
+-rw-r--r--   0     1001      123     5632 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/table/zen.rs
+-rw-r--r--   0     1001      123     4796 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/lib.rs
+-rw-r--r--   0     1001      123      715 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/loader/closure.rs
+-rw-r--r--   0     1001      123     2449 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/loader/filesystem.rs
+-rw-r--r--   0     1001      123     1245 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/loader/memory.rs
+-rw-r--r--   0     1001      123      892 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/loader/mod.rs
+-rw-r--r--   0     1001      123      466 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/loader/noop.rs
+-rw-r--r--   0     1001      123     3160 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/model/mod.rs
+-rw-r--r--   0     1001      123     9076 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/util/json_map.rs
+-rw-r--r--   0     1001      123       25 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/src/util/mod.rs
+-rw-r--r--   0     1001      123     2081 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/tests/decision.rs
+-rw-r--r--   0     1001      123     4759 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/tests/engine.rs
+-rw-r--r--   0     1001      123     1381 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/tests/model.rs
+-rw-r--r--   0     1001      123      884 2023-07-28 11:38:10.000000 zen_engine-0.9.0/local_dependencies/zen-engine/tests/support/mod.rs
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.9.0/Cargo.toml
+-rw-r--r--   0     1001      123      135 2023-07-28 11:38:10.000000 zen_engine-0.9.0/.bumpversion.cfg
+-rw-r--r--   0     1001      123      691 2023-07-28 11:38:10.000000 zen_engine-0.9.0/.gitignore
+-rw-r--r--   0     1001      123     1057 2023-07-28 11:38:10.000000 zen_engine-0.9.0/LICENSE
+-rw-r--r--   0     1001      123     5965 2023-07-28 11:38:10.000000 zen_engine-0.9.0/README.md
+-rw-r--r--   0     1001      123     1578 2023-07-28 11:38:10.000000 zen_engine-0.9.0/index.py
+-rw-r--r--   0     1001      123      966 2023-07-28 11:38:10.000000 zen_engine-0.9.0/pyproject.toml
+-rw-r--r--   0     1001      123     1517 2023-07-28 11:38:10.000000 zen_engine-0.9.0/src/decision.rs
+-rw-r--r--   0     1001      123     3100 2023-07-28 11:38:10.000000 zen_engine-0.9.0/src/engine.rs
+-rw-r--r--   0     1001      123      335 2023-07-28 11:38:10.000000 zen_engine-0.9.0/src/lib.rs
+-rw-r--r--   0     1001      123     1188 2023-07-28 11:38:10.000000 zen_engine-0.9.0/src/loader.rs
+-rw-r--r--   0     1001      123     1122 2023-07-28 11:38:10.000000 zen_engine-0.9.0/src/value.rs
+-rw-r--r--   0     1001      123    48279 2023-07-28 11:38:15.000000 zen_engine-0.9.0/Cargo.lock
+-rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.9.0/PKG-INFO
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/Cargo.toml` & `zen_engine-0.9.0/local_dependencies/zen-expression/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 authors = ["GoRules Team <bot@gorules.io>"]
 description = "Zen Expression Language"
 name = "zen-expression"
 license = "MIT"
-version = "0.7.1"
+version = "0.8.0"
 edition = "2021"
 repository = "https://github.com/gorules/zen.git"
 
 
 [dependencies]
 ahash = "0.8.3"
 bumpalo = "3.13.0"
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/README.md` & `zen_engine-0.9.0/local_dependencies/zen-expression/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/benches/isolate.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/benches/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/benches/lexer.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/benches/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/benches/standard.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/benches/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/benches/unary.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/benches/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/ast.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/ast.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/compiler.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/compiler.rs`

 * *Files 0% similar despite different names*

```diff
@@ -384,15 +384,15 @@
                     Ok(self.emit(Opcode::Round))
                 }
                 "rand" => {
                     self.compile_argument(name, arguments, 0)?;
                     Ok(self.emit(Opcode::Random))
                 }
                 "dayOfWeek" | "dayOfMonth" | "dayOfYear" | "weekOfMonth" | "weekOfYear"
-                | "monthOfYear" | "seasonOfYear" | "monthString" | "weekdayString" => {
+                | "monthOfYear" | "seasonOfYear" | "monthString" | "weekdayString" | "year" => {
                     self.compile_argument(name, arguments, 0)?;
                     Ok(self.emit(Opcode::DateManipulation(name)))
                 }
                 "all" => {
                     self.compile_argument(name, arguments, 0)?;
                     self.emit(Opcode::Begin);
                     let mut loop_break: usize = 0;
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/helpers.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/isolate.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/codes.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/lexer/codes.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/cursor.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/lexer/cursor.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/lexer/lexer.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/lexer/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/opcodes.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/opcodes.rs`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
 
 #[derive(Debug)]
 pub enum Opcode<'a> {
     Push(Variable<'a>),
     Pop,
     Rot,
     Fetch,
-    FetchField(&'a str),
     FetchEnv(&'a str),
     Negate,
     Not,
     Equal,
     Jump(usize),
     JumpIfTrue(usize),
     JumpIfFalse(usize),
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/definitions.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/definitions.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/error.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/iter.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/iter.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/standard/constants.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/standard/constants.rs`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
         "median" => BuiltIn { arity: Arity::Single },
         "mode" => BuiltIn { arity: Arity::Single },
 
         "floor" => BuiltIn { arity: Arity::Single },
         "ceil" => BuiltIn { arity: Arity::Single },
         "round" => BuiltIn { arity: Arity::Single },
 
+        "year" => BuiltIn { arity: Arity::Single },
         "dayOfWeek" => BuiltIn { arity: Arity::Single },
         "dayOfMonth" => BuiltIn { arity: Arity::Single },
         "dayOfYear" => BuiltIn { arity: Arity::Single },
         "weekOfMonth" => BuiltIn { arity: Arity::Single },
         "weekOfYear" => BuiltIn { arity: Arity::Single },
         "monthOfYear" => BuiltIn { arity: Arity::Single },
         "seasonOfYear" => BuiltIn { arity: Arity::Single },
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/standard/mod.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/standard/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 use std::cell::Cell;
 
 use bumpalo::Bump;
 
 use crate::ast::Node;
 use crate::lexer::token::{Token, TokenKind};
 use crate::parser::definitions::{Arity, Associativity};
-use crate::parser::error::ParserError::{MemoryFailure, UnexpectedToken, UnknownBuiltIn};
+use crate::parser::error::ParserError::{
+    FailedToParse, MemoryFailure, UnexpectedToken, UnknownBuiltIn,
+};
 use crate::parser::error::ParserResult;
 use crate::parser::iter::ParserIterator;
 use crate::parser::standard::constants::{BINARY_OPERATORS, BUILT_INS, UNARY_OPERATORS};
 
 mod constants;
 
+#[derive(Debug)]
 pub struct StandardParser<'a, 'b>
 where
     'b: 'a,
 {
     iterator: ParserIterator<'a, 'b>,
     bump: &'b Bump,
     depth: Cell<u8>,
@@ -30,15 +33,23 @@
             iterator: ParserIterator::try_new(tokens, bump)?,
             bump,
             depth: Cell::new(0),
         })
     }
 
     pub fn parse(&self) -> ParserResult<&'b Node<'b>> {
-        self.parse_expression(0)
+        let result = self.parse_expression(0)?;
+        if !self.iterator.is_done() {
+            let token = self.iterator.current();
+            return Err(FailedToParse {
+                message: format!("Unterminated token {} on {:?}", token.value, token.span),
+            });
+        }
+
+        return Ok(result);
     }
 
     fn parse_expression(&self, precedence: u8) -> ParserResult<&'b Node<'b>> {
         let mut node_left = self.parse_primary()?;
         let mut token = self.iterator.current();
 
         while !self.iterator.is_done() {
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/unary/constants.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/unary/constants.rs`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     "floor" => BuiltIn { arity: Arity::Single },
     "ceil" => BuiltIn { arity: Arity::Single },
     "round" => BuiltIn { arity: Arity::Single },
 
     "flatten" => BuiltIn { arity: Arity::Single },
 
+    "year" => BuiltIn { arity: Arity::Single },
     "dayOfWeek" => BuiltIn { arity: Arity::Single },
     "dayOfMonth" => BuiltIn { arity: Arity::Single },
     "dayOfYear" => BuiltIn { arity: Arity::Single },
     "weekOfMonth" => BuiltIn { arity: Arity::Single },
     "weekOfYear" => BuiltIn { arity: Arity::Single },
     "monthOfYear" => BuiltIn { arity: Arity::Single },
     "seasonOfYear" => BuiltIn { arity: Arity::Single },
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/parser/unary/mod.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/parser/unary/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/src/vm.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/src/vm.rs`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,16 @@
 use thiserror::Error;
 
 use crate::helpers::{date_time, time};
 use crate::opcodes::Variable::{Array, Bool, Int, Interval, Null, Number, Object, String};
 use crate::opcodes::{Opcode, Variable};
 use crate::vm::VMError::{OpcodeErr, OpcodeOutOfBounds, ParseDateTimeErr, StackOutOfBounds};
 
+const NULL_VAR: &'static Variable = &Null;
+
 #[derive(Debug, Error)]
 pub enum VMError {
     #[error("Unsupported opcode type")]
     OpcodeErr {
         opcode: std::string::String,
         message: std::string::String,
     },
@@ -110,62 +112,29 @@
                 }
                 Opcode::Fetch => {
                     let b = self.pop()?;
                     let a = self.pop()?;
 
                     match (a, b) {
                         (Object(o), String(s)) => {
-                            self.push_ref(o.get(*s).ok_or_else(|| OpcodeErr {
-                                opcode: "Fetch".into(),
-                                message: "Undefined object key".into(),
-                            })?);
+                            self.push_ref(o.get(*s).unwrap_or(&NULL_VAR));
                         }
                         (Array(arr), Number(n)) => self.push_ref(
                             arr.get(n.to_usize().ok_or_else(|| OpcodeErr {
                                 opcode: "Fetch".into(),
                                 message: "Failed to convert to usize".into(),
                             })?)
-                            .ok_or_else(|| OpcodeErr {
-                                opcode: "Fetch".into(),
-                                message: "Undefined array index".into(),
-                            })?,
+                            .unwrap_or(&NULL_VAR),
                         ),
-                        _ => {
-                            return Err(OpcodeErr {
-                                opcode: "Fetch".into(),
-                                message: "Unsupported types".into(),
-                            })
-                        }
-                    }
-                }
-                Opcode::FetchField(f) => {
-                    let a = self.pop()?;
-                    match a {
-                        Object(o) => {
-                            self.push_ref(o.get(*f).ok_or_else(|| OpcodeErr {
-                                opcode: "FetchField".into(),
-                                message: "Undefined object key".into(),
-                            })?);
-                        }
-                        _ => {
-                            return Err(OpcodeErr {
-                                opcode: "FetchField".into(),
-                                message: "Unsupported type".into(),
-                            })
-                        }
+                        _ => self.push_ref(&NULL_VAR),
                     }
                 }
                 Opcode::FetchEnv(f) => match env {
-                    Object(o) => {
-                        self.push_ref(o.get(*f).ok_or_else(|| OpcodeErr {
-                            opcode: "FetchEnv".into(),
-                            message: "Undefined object key".into(),
-                        })?);
-                    }
-                    Null => self.push(Null),
+                    Object(o) => self.push_ref(o.get(*f).unwrap_or(&NULL_VAR)),
+                    Null => self.push_ref(NULL_VAR),
                     _ => {
                         return Err(OpcodeErr {
                             opcode: "FetchEnv".into(),
                             message: "Unsupported type".into(),
                         })
                     }
                 },
@@ -208,18 +177,15 @@
                         (String(a), String(b)) => {
                             self.stack.push(self.bump.alloc(Bool(a == b)));
                         }
                         (Null, Null) => {
                             self.stack.push(self.bump.alloc(Bool(true)));
                         }
                         _ => {
-                            return Err(OpcodeErr {
-                                opcode: "Equal".into(),
-                                message: "Unsupported type".into(),
-                            })
+                            self.stack.push(self.bump.alloc(Bool(false)));
                         }
                     }
                 }
                 Opcode::Jump(j) => self.ip += j,
                 Opcode::JumpIfTrue(j) => {
                     let a = self.stack.last().ok_or_else(|| OpcodeErr {
                         opcode: "JumpIfTrue".into(),
@@ -344,14 +310,22 @@
                             let is_in = arr.iter().any(|b| match b {
                                 Bool(b) => a == b,
                                 _ => false,
                             });
 
                             self.stack.push(self.bump.alloc(Bool(is_in)));
                         }
+                        (Null, Array(arr)) => {
+                            let is_in = arr.iter().any(|b| match b {
+                                Null => true,
+                                _ => false,
+                            });
+
+                            self.stack.push(self.bump.alloc(Bool(is_in)));
+                        }
                         _ => {
                             return Err(OpcodeErr {
                                 opcode: "In".into(),
                                 message: "Unsupported type".into(),
                             })
                         }
                     }
@@ -881,14 +855,15 @@
                         }
                         _ => match a {
                             Array(arr) => {
                                 let is_in = arr.iter().any(|a| match (a, b) {
                                     (Number(a), Number(b)) => a == b,
                                     (String(a), String(b)) => a == b,
                                     (Bool(a), Bool(b)) => a == b,
+                                    (Null, Null) => true,
                                     _ => false,
                                 });
 
                                 self.stack.push(self.bump.alloc(Bool(is_in)));
                             }
                             _ => {
                                 return Err(OpcodeErr {
@@ -1001,14 +976,15 @@
                                 opcode: "DateManipulation".into(),
                                 message: "Unsupported type".into(),
                             })
                         }
                     };
 
                     let var = match *operation {
+                        "year" => Number(time.year().into()),
                         "dayOfWeek" => Number(time.weekday().number_from_monday().into()),
                         "dayOfMonth" => Number(time.day().into()),
                         "dayOfYear" => Number(time.ordinal().into()),
                         "weekOfYear" => Number(time.iso_week().week().into()),
                         "monthOfYear" => Number(time.month().into()),
                         "monthString" => {
                             String(self.bump.alloc_str(&time.format("%b").to_string()))
@@ -1132,28 +1108,36 @@
                             .alloc(Array(self.bump.alloc_slice_copy(flat_arr.as_slice()))),
                     )
                 }
                 Opcode::ParseDateTime => {
                     let a = self.pop()?;
                     let ts = match a {
                         String(a) => date_time(a)?.timestamp(),
+                        Number(a) => a.to_i64().ok_or_else(|| OpcodeErr {
+                            opcode: "ParseDateTime".into(),
+                            message: "Number overflow".into(),
+                        })?,
                         _ => {
                             return Err(OpcodeErr {
                                 opcode: "ParseDateTime".into(),
                                 message: "Unsupported type".into(),
                             })
                         }
                     };
 
                     self.stack.push(self.bump.alloc(Number(ts.into())))
                 }
                 Opcode::ParseTime => {
                     let a = self.pop()?;
                     let ts = match a {
                         String(a) => time(a)?.num_seconds_from_midnight(),
+                        Number(a) => a.to_u32().ok_or_else(|| OpcodeErr {
+                            opcode: "ParseTime".into(),
+                            message: "Number overflow".into(),
+                        })?,
                         _ => {
                             return Err(OpcodeErr {
                                 opcode: "ParseTime".into(),
                                 message: "Unsupported type".into(),
                             })
                         }
                     };
@@ -1164,14 +1148,18 @@
 
                     let dur = match a {
                         String(a) => humantime::parse_duration(a)
                             .map_err(|_| ParseDateTimeErr {
                                 timestamp: a.to_string(),
                             })?
                             .as_secs(),
+                        Number(n) => n.to_u64().ok_or_else(|| OpcodeErr {
+                            opcode: "ParseDuration".into(),
+                            message: "Number overflow".into(),
+                        })?,
                         _ => {
                             return Err(OpcodeErr {
                                 opcode: "ParseDuration".into(),
                                 message: "Unsupported type".into(),
                             })
                         }
                     };
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/tests/isolate.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/tests/isolate.rs`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,26 @@
 
 #[test]
 fn isolate_standard_test() {
     let tests = Vec::from([
         TestEnv {
             env: json!({
                 "hello": "Hello, ",
-                "world": "world!"
+                "world": "world!",
             }),
-            cases: Vec::from([TestCase {
-                expr: "hello + world",
-                result: json!("Hello, world!"),
-            }]),
+            cases: Vec::from([
+                TestCase {
+                    expr: "hello + world",
+                    result: json!("Hello, world!"),
+                },
+                TestCase {
+                    expr: "hello.nested.null.test",
+                    result: json!(null),
+                },
+            ]),
         },
         TestEnv {
             env: json!({
                 "a": 3,
                 "b": 6,
                 "c": 1
             }),
@@ -325,14 +331,22 @@
                     expr: r#"monthString("2022-11-14")"#,
                     result: json!("Nov"),
                 },
                 TestCase {
                     expr: r#"weekdayString(date("2022-11-14"))"#,
                     result: json!("Mon"),
                 },
+                TestCase {
+                    expr: r#"year("2022-01-01")"#,
+                    result: json!(2022),
+                },
+                TestCase {
+                    expr: r#"year(date("2022-01-01"))"#,
+                    result: json!(2022),
+                },
             ]),
         },
         TestEnv {
             env: json!({}),
             cases: Vec::from([
                 TestCase {
                     expr: r#"sum([1, 2, 3])"#,
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/tests/lexer.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/tests/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/tests/standard.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/tests/standard.rs`

 * *Files 1% similar despite different names*

```diff
@@ -294,15 +294,15 @@
 
         bump.reset();
     }
 }
 
 #[test]
 fn failure_tests() {
-    let tests: Vec<&str> = Vec::from(["a + b ++"]);
+    let tests: Vec<&str> = Vec::from(["a + b ++", "null.nested.property", "false.nested.property"]);
 
     let lexer = Lexer::new();
     let mut bump = Bump::new();
 
     for test in tests {
         let t_res = lexer.tokenize(test).unwrap();
         let tokens = t_res.borrow();
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-expression/tests/unary.rs` & `zen_engine-0.9.0/local_dependencies/zen-expression/tests/unary.rs`

 * *Files 1% similar despite different names*

```diff
@@ -152,15 +152,15 @@
 
         bump.reset();
     }
 }
 
 #[test]
 fn failure_tests() {
-    let tests: Vec<&str> = Vec::from(["a + b ++", "a +++ b +--= fa"]);
+    let tests: Vec<&str> = Vec::from(["a + b ++", "a +++ b +--= fa", "null.a", "false.b"]);
 
     let lexer = Lexer::new();
     let mut bump = Bump::new();
 
     for test in tests {
         let t_res = lexer.tokenize(test).unwrap();
         let tokens = t_res.borrow();
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/Cargo.toml` & `zen_engine-0.9.0/local_dependencies/zen-engine/Cargo.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 authors = ["GoRules Team <bot@gorules.io>"]
 description = "Business rules engine"
 name = "zen-engine"
 license = "MIT"
-version = "0.7.1"
+version = "0.8.0"
 edition = "2021"
 repository = "https://github.com/gorules/zen.git"
 
 [lib]
 doctest = false
 
 [dependencies]
@@ -18,15 +18,15 @@
 bincode = { version = "2.0.0-rc.3", optional = true }
 serde_json = { version = "1.0.96", features = ["arbitrary_precision"] }
 serde = { version = "1.0.163", features = ["derive"] }
 serde_v8 = { version = "0.103.0" }
 once_cell = { version = "1.17.2" }
 futures = "0.3.28"
 v8 = { version = "0.74.0" }
-zen-expression = { path = "../zen-expression", version = "0.7.1" }
+zen-expression = { path = "../zen-expression", version = "0.8.0" }
 
 [features]
 bincode = ["dep:bincode"]
 
 [[bench]]
 harness = false
 name = "engine"
```

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/README.md` & `zen_engine-0.9.0/local_dependencies/zen-engine/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/benches/engine.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/benches/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/decision.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/engine.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/error.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/decision.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/expression/mod.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/expression/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/mod.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/function/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/script.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/function/script.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/scripts/internals.js` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/function/vm.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/function/vm.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/graph.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/graph.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/node.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/node.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/table/mod.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/table/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/handler/table/zen.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/handler/table/zen.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/lib.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/closure.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/loader/closure.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/filesystem.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/loader/filesystem.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/memory.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/loader/memory.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/loader/mod.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/loader/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/model/mod.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/model/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/src/util/json_map.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/src/util/json_map.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/tests/decision.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/tests/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/tests/engine.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/tests/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/tests/model.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/tests/model.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/local_dependencies/zen-engine/tests/support/mod.rs` & `zen_engine-0.9.0/local_dependencies/zen-engine/tests/support/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/.gitignore` & `zen_engine-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/LICENSE` & `zen_engine-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/README.md` & `zen_engine-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/index.py` & `zen_engine-0.9.0/index.py`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/pyproject.toml` & `zen_engine-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/src/decision.rs` & `zen_engine-0.9.0/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/src/engine.rs` & `zen_engine-0.9.0/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/src/loader.rs` & `zen_engine-0.9.0/src/loader.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/src/value.rs` & `zen_engine-0.9.0/src/value.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.8.2/Cargo.lock` & `zen_engine-0.9.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1846,15 +1846,15 @@
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
 name = "zen-engine"
-version = "0.7.1"
+version = "0.8.0"
 dependencies = [
  "anyhow",
  "async-recursion",
  "async-trait",
  "bincode",
  "criterion",
  "futures",
@@ -1866,15 +1866,15 @@
  "tokio",
  "v8",
  "zen-expression",
 ]
 
 [[package]]
 name = "zen-expression"
-version = "0.7.1"
+version = "0.8.0"
 dependencies = [
  "ahash 0.8.3",
  "bumpalo",
  "chrono",
  "criterion",
  "fastrand",
  "hashbrown 0.13.2",
@@ -1899,15 +1899,15 @@
  "napi-derive",
  "serde_json",
  "zen-engine",
 ]
 
 [[package]]
 name = "zen-python"
-version = "0.8.2"
+version = "0.9.0"
 dependencies = [
  "anyhow",
  "async-trait",
  "futures",
  "pyo3",
  "pythonize",
  "serde",
```

### Comparing `zen_engine-0.8.2/PKG-INFO` & `zen_engine-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-engine
-Version: 0.8.2
+Version: 0.9.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: bumpver; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
```

