# Comparing `tmp/zen_engine-0.7.0.tar.gz` & `tmp/zen_engine-0.8.0.tar.gz`

## Comparing `zen_engine-0.7.0.tar` & `zen_engine-0.8.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 zen_engine-0.7.0/local_dependencies/zen-expression/Cargo.toml
--rw-r--r--   0     1001      123     2347 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/README.md
--rw-r--r--   0     1001      123      625 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/benches/isolate.rs
--rw-r--r--   0     1001      123    93335 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/benches/lexer.rs
--rw-r--r--   0     1001      123    93602 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/benches/standard.rs
--rw-r--r--   0     1001      123      867 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/benches/unary.rs
--rw-r--r--   0     1001      123      970 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/ast.rs
--rw-r--r--   0     1001      123    19250 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/compiler.rs
--rw-r--r--   0     1001      123     1479 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/helpers.rs
--rw-r--r--   0     1001      123     6819 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/isolate.rs
--rw-r--r--   0     1001      123      769 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/codes.rs
--rw-r--r--   0     1001      123     2035 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/cursor.rs
--rw-r--r--   0     1001      123      404 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/error.rs
--rw-r--r--   0     1001      123     6311 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/lexer.rs
--rw-r--r--   0     1001      123       88 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/mod.rs
--rw-r--r--   0     1001      123      273 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/token.rs
--rw-r--r--   0     1001      123      203 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/lib.rs
--rw-r--r--   0     1001      123     4010 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/opcodes.rs
--rw-r--r--   0     1001      123      922 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/definitions.rs
--rw-r--r--   0     1001      123      638 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/error.rs
--rw-r--r--   0     1001      123     5318 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/iter.rs
--rw-r--r--   0     1001      123      131 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/mod.rs
--rw-r--r--   0     1001      123     4286 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/standard/constants.rs
--rw-r--r--   0     1001      123    14060 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/standard/mod.rs
--rw-r--r--   0     1001      123     2604 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/unary/constants.rs
--rw-r--r--   0     1001      123     9905 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/unary/mod.rs
--rw-r--r--   0     1001      123    51034 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/src/vm.rs
--rw-r--r--   0     1001      123    22433 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/tests/isolate.rs
--rw-r--r--   0     1001      123    11822 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/tests/lexer.rs
--rw-r--r--   0     1001      123     9097 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/tests/standard.rs
--rw-r--r--   0     1001      123     5185 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-expression/tests/unary.rs
--rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.7.0/local_dependencies/zen-engine/Cargo.toml
--rw-r--r--   0     1001      123     4305 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/README.md
--rw-r--r--   0     1001      123     1558 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/benches/engine.rs
--rw-r--r--   0     1001      123     2031 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/decision.rs
--rw-r--r--   0     1001      123     2605 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/engine.rs
--rw-r--r--   0     1001      123      972 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/error.rs
--rw-r--r--   0     1001      123     1651 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/decision.rs
--rw-r--r--   0     1001      123     2136 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/expression/mod.rs
--rw-r--r--   0     1001      123     1097 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/mod.rs
--rw-r--r--   0     1001      123     3046 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/script.rs
--rw-r--r--   0     1001      123     6485 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
--rw-r--r--   0     1001      123      528 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
--rw-r--r--   0     1001      123     1747 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/vm.rs
--rw-r--r--   0     1001      123    11347 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/graph.rs
--rw-r--r--   0     1001      123      115 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/mod.rs
--rw-r--r--   0     1001      123      745 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/node.rs
--rw-r--r--   0     1001      123      807 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/table/mod.rs
--rw-r--r--   0     1001      123     4940 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/table/zen.rs
--rw-r--r--   0     1001      123     4796 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/lib.rs
--rw-r--r--   0     1001      123      715 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/closure.rs
--rw-r--r--   0     1001      123     2449 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/filesystem.rs
--rw-r--r--   0     1001      123     1245 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/memory.rs
--rw-r--r--   0     1001      123      892 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/mod.rs
--rw-r--r--   0     1001      123      466 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/noop.rs
--rw-r--r--   0     1001      123     3152 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/model/mod.rs
--rw-r--r--   0     1001      123     9076 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/util/json_map.rs
--rw-r--r--   0     1001      123       25 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/src/util/mod.rs
--rw-r--r--   0     1001      123     2081 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/tests/decision.rs
--rw-r--r--   0     1001      123     4759 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/tests/engine.rs
--rw-r--r--   0     1001      123     1381 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/tests/model.rs
--rw-r--r--   0     1001      123      884 2023-07-13 09:18:18.000000 zen_engine-0.7.0/local_dependencies/zen-engine/tests/support/mod.rs
--rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.7.0/Cargo.toml
--rw-r--r--   0     1001      123      135 2023-07-13 09:18:18.000000 zen_engine-0.7.0/.bumpversion.cfg
--rw-r--r--   0     1001      123      691 2023-07-13 09:18:18.000000 zen_engine-0.7.0/.gitignore
--rw-r--r--   0     1001      123     1057 2023-07-13 09:18:18.000000 zen_engine-0.7.0/LICENSE
--rw-r--r--   0     1001      123     5965 2023-07-13 09:18:18.000000 zen_engine-0.7.0/README.md
--rw-r--r--   0     1001      123     1578 2023-07-13 09:18:18.000000 zen_engine-0.7.0/index.py
--rw-r--r--   0     1001      123      966 2023-07-13 09:18:18.000000 zen_engine-0.7.0/pyproject.toml
--rw-r--r--   0     1001      123     1429 2023-07-13 09:18:18.000000 zen_engine-0.7.0/src/decision.rs
--rw-r--r--   0     1001      123     3012 2023-07-13 09:18:18.000000 zen_engine-0.7.0/src/engine.rs
--rw-r--r--   0     1001      123      335 2023-07-13 09:18:18.000000 zen_engine-0.7.0/src/lib.rs
--rw-r--r--   0     1001      123     1188 2023-07-13 09:18:18.000000 zen_engine-0.7.0/src/loader.rs
--rw-r--r--   0     1001      123     1122 2023-07-13 09:18:18.000000 zen_engine-0.7.0/src/value.rs
--rw-r--r--   0     1001      123    48278 2023-07-13 09:18:27.000000 zen_engine-0.7.0/Cargo.lock
--rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0      841 1970-01-01 00:00:00.000000 zen_engine-0.8.0/local_dependencies/zen-expression/Cargo.toml
+-rw-r--r--   0     1001      123     2347 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/README.md
+-rw-r--r--   0     1001      123      625 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/benches/isolate.rs
+-rw-r--r--   0     1001      123    93335 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/benches/lexer.rs
+-rw-r--r--   0     1001      123    93602 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/benches/standard.rs
+-rw-r--r--   0     1001      123      867 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/benches/unary.rs
+-rw-r--r--   0     1001      123      970 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/ast.rs
+-rw-r--r--   0     1001      123    19250 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/compiler.rs
+-rw-r--r--   0     1001      123     1479 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/helpers.rs
+-rw-r--r--   0     1001      123     6816 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/isolate.rs
+-rw-r--r--   0     1001      123      783 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/codes.rs
+-rw-r--r--   0     1001      123     2035 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/cursor.rs
+-rw-r--r--   0     1001      123      404 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/error.rs
+-rw-r--r--   0     1001      123     6339 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/lexer.rs
+-rw-r--r--   0     1001      123       88 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/mod.rs
+-rw-r--r--   0     1001      123      273 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/token.rs
+-rw-r--r--   0     1001      123      203 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/lib.rs
+-rw-r--r--   0     1001      123     4010 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/opcodes.rs
+-rw-r--r--   0     1001      123      922 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/definitions.rs
+-rw-r--r--   0     1001      123      638 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/error.rs
+-rw-r--r--   0     1001      123     5318 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/iter.rs
+-rw-r--r--   0     1001      123      131 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/mod.rs
+-rw-r--r--   0     1001      123     4286 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/standard/constants.rs
+-rw-r--r--   0     1001      123    14060 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/standard/mod.rs
+-rw-r--r--   0     1001      123     2604 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/unary/constants.rs
+-rw-r--r--   0     1001      123     9905 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/unary/mod.rs
+-rw-r--r--   0     1001      123    51034 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/src/vm.rs
+-rw-r--r--   0     1001      123    22433 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/tests/isolate.rs
+-rw-r--r--   0     1001      123    11822 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/tests/lexer.rs
+-rw-r--r--   0     1001      123     9097 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/tests/standard.rs
+-rw-r--r--   0     1001      123     5185 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-expression/tests/unary.rs
+-rw-r--r--   0        0        0      786 1970-01-01 00:00:00.000000 zen_engine-0.8.0/local_dependencies/zen-engine/Cargo.toml
+-rw-r--r--   0     1001      123     4305 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/README.md
+-rw-r--r--   0     1001      123     1558 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/benches/engine.rs
+-rw-r--r--   0     1001      123     2031 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/decision.rs
+-rw-r--r--   0     1001      123     2605 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/engine.rs
+-rw-r--r--   0     1001      123      972 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/error.rs
+-rw-r--r--   0     1001      123     1651 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/decision.rs
+-rw-r--r--   0     1001      123     2136 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/expression/mod.rs
+-rw-r--r--   0     1001      123     1097 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/mod.rs
+-rw-r--r--   0     1001      123     3046 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/script.rs
+-rw-r--r--   0     1001      123     6485 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js
+-rw-r--r--   0     1001      123      528 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js
+-rw-r--r--   0     1001      123     1747 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/vm.rs
+-rw-r--r--   0     1001      123    11347 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/graph.rs
+-rw-r--r--   0     1001      123      115 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/mod.rs
+-rw-r--r--   0     1001      123      745 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/node.rs
+-rw-r--r--   0     1001      123      807 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/table/mod.rs
+-rw-r--r--   0     1001      123     5478 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/table/zen.rs
+-rw-r--r--   0     1001      123     4796 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/lib.rs
+-rw-r--r--   0     1001      123      715 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/closure.rs
+-rw-r--r--   0     1001      123     2449 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/filesystem.rs
+-rw-r--r--   0     1001      123     1245 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/memory.rs
+-rw-r--r--   0     1001      123      892 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/mod.rs
+-rw-r--r--   0     1001      123      466 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/noop.rs
+-rw-r--r--   0     1001      123     3160 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/model/mod.rs
+-rw-r--r--   0     1001      123     9076 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/util/json_map.rs
+-rw-r--r--   0     1001      123       25 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/src/util/mod.rs
+-rw-r--r--   0     1001      123     2081 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/tests/decision.rs
+-rw-r--r--   0     1001      123     4759 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/tests/engine.rs
+-rw-r--r--   0     1001      123     1381 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/tests/model.rs
+-rw-r--r--   0     1001      123      884 2023-07-14 23:19:34.000000 zen_engine-0.8.0/local_dependencies/zen-engine/tests/support/mod.rs
+-rw-r--r--   0        0        0      396 1970-01-01 00:00:00.000000 zen_engine-0.8.0/Cargo.toml
+-rw-r--r--   0     1001      123      135 2023-07-14 23:19:34.000000 zen_engine-0.8.0/.bumpversion.cfg
+-rw-r--r--   0     1001      123      691 2023-07-14 23:19:34.000000 zen_engine-0.8.0/.gitignore
+-rw-r--r--   0     1001      123     1057 2023-07-14 23:19:34.000000 zen_engine-0.8.0/LICENSE
+-rw-r--r--   0     1001      123     5965 2023-07-14 23:19:34.000000 zen_engine-0.8.0/README.md
+-rw-r--r--   0     1001      123     1578 2023-07-14 23:19:34.000000 zen_engine-0.8.0/index.py
+-rw-r--r--   0     1001      123      966 2023-07-14 23:19:34.000000 zen_engine-0.8.0/pyproject.toml
+-rw-r--r--   0     1001      123     1429 2023-07-14 23:19:34.000000 zen_engine-0.8.0/src/decision.rs
+-rw-r--r--   0     1001      123     3012 2023-07-14 23:19:34.000000 zen_engine-0.8.0/src/engine.rs
+-rw-r--r--   0     1001      123      335 2023-07-14 23:19:34.000000 zen_engine-0.8.0/src/lib.rs
+-rw-r--r--   0     1001      123     1188 2023-07-14 23:19:34.000000 zen_engine-0.8.0/src/loader.rs
+-rw-r--r--   0     1001      123     1122 2023-07-14 23:19:34.000000 zen_engine-0.8.0/src/value.rs
+-rw-r--r--   0     1001      123    48278 2023-07-14 23:19:41.000000 zen_engine-0.8.0/Cargo.lock
+-rw-r--r--   0        0        0     6813 1970-01-01 00:00:00.000000 zen_engine-0.8.0/PKG-INFO
```

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/Cargo.toml` & `zen_engine-0.8.0/local_dependencies/zen-expression/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 authors = ["GoRules Team <bot@gorules.io>"]
 description = "Zen Expression Language"
 name = "zen-expression"
 license = "MIT"
-version = "0.5.2"
+version = "0.7.0"
 edition = "2021"
 repository = "https://github.com/gorules/zen.git"
 
 
 [dependencies]
 ahash = "0.8.3"
 bumpalo = "3.13.0"
```

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/README.md` & `zen_engine-0.8.0/local_dependencies/zen-expression/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/benches/isolate.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/benches/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/benches/lexer.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/benches/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/benches/standard.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/benches/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/benches/unary.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/benches/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/ast.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/ast.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/compiler.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/compiler.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/helpers.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/helpers.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/isolate.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/isolate.rs`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         if let Variable::Object(obj) = env {
             obj.insert("$", value);
         }
 
         Ok(())
     }
 
-    pub fn get_reference(&self, reference: &'a str) -> Option<Value> {
+    pub fn get_reference(&self, reference: &str) -> Option<Value> {
         let refs = self.references.borrow();
         let var = refs.get(reference)?;
 
         (*var).try_into().ok()
     }
 
     pub fn run_standard(&self, source: &'a str) -> Result<Value, IsolateError> {
```

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/codes.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/codes.rs`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #[macro_export]
 macro_rules! is_token_type {
     ($str: expr, "space") => {
-        matches!($str, ' ')
+        matches!($str, ' ' | '\n' | '\t')
     };
     ($str: expr, "quote") => {
         matches!($str, '\'' | '"')
     };
     ($str: expr, "digit") => {
         matches!($str, '0'..='9')
     };
```

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/cursor.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/cursor.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/lexer/lexer.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/lexer/lexer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
             tokens,
         }
     }
 
     pub fn scan(&self) -> VoidResult {
         while let Some((i, s)) = self.cursor.peek() {
             match s {
-                ' ' => {
+                _ if is_token_type!(s, "space") => {
                     self.cursor.next();
                     Ok(())
                 }
                 _ if is_token_type!(s, "quote") => self.string(),
                 _ if is_token_type!(s, "digit") => self.number(),
                 _ if is_token_type!(s, "bracket") => self.bracket(),
                 _ if is_token_type!(s, "cmp_operator") => self.operator(),
```

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/opcodes.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/opcodes.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/definitions.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/definitions.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/error.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/iter.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/iter.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/standard/constants.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/standard/constants.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/standard/mod.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/standard/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/unary/constants.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/unary/constants.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/parser/unary/mod.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/parser/unary/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/src/vm.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/src/vm.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/tests/isolate.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/tests/isolate.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/tests/lexer.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/tests/lexer.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/tests/standard.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/tests/standard.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-expression/tests/unary.rs` & `zen_engine-0.8.0/local_dependencies/zen-expression/tests/unary.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/Cargo.toml` & `zen_engine-0.8.0/local_dependencies/zen-engine/Cargo.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [package]
 authors = ["GoRules Team <bot@gorules.io>"]
 description = "Business rules engine"
 name = "zen-engine"
 license = "MIT"
-version = "0.5.2"
+version = "0.7.0"
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
-zen-expression = { path = "../zen-expression", version = "0.5.2" }
+zen-expression = { path = "../zen-expression", version = "0.7.0" }
 
 [features]
 bincode = ["dep:bincode"]
 
 [[bench]]
 harness = false
 name = "engine"
```

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/README.md` & `zen_engine-0.8.0/local_dependencies/zen-engine/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/benches/engine.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/benches/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/decision.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/engine.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/error.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/error.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/decision.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/expression/mod.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/expression/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/mod.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/script.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/script.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/scripts/dayjs.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/scripts/internals.js`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/function/vm.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/function/vm.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/graph.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/graph.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/node.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/node.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/table/mod.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/table/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/handler/table/zen.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/handler/table/zen.rs`

 * *Files 8% similar despite different names*

```diff
@@ -93,15 +93,25 @@
         let rule = content.rules.get(index)?;
         for input in &content.inputs {
             let rule_value = rule.get(input.id.as_str())?;
             if rule_value.is_empty() {
                 continue;
             }
 
-            self.isolate.set_reference(input.field.as_str()).ok()?;
+            let Some(input_field) = &input.field else {
+                let result = self.isolate.run_standard(rule_value.as_str()).ok()?;
+                let is_ok = result.as_bool().unwrap_or(false);
+                if !is_ok {
+                    return None;
+                }
+
+                continue;
+            };
+
+            self.isolate.set_reference(input_field.as_str()).ok()?;
             let result = self.isolate.run_unary(rule_value.as_str()).ok()?;
 
             let is_ok = result.as_bool().unwrap_or(false);
             if !is_ok {
                 return None;
             }
         }
@@ -133,19 +143,24 @@
 
         let mut expressions: HashMap<String, String> = Default::default();
         let mut reference_map: HashMap<String, Value> = Default::default();
         expressions.insert("_id".to_string(), rule_id.clone());
 
         for input in &content.inputs {
             let rule_value = rule.get(input.id.as_str())?;
-            expressions.insert(input.field.clone(), rule_value.clone());
+            let mut input_identifier = input.id.clone();
+            if let Some(input_field) = &input.field {
+                input_identifier = format!("{input_field}[{input_identifier}]");
+            }
 
-            if let Some(reference) = self.isolate.get_reference(input.field.as_str()) {
-                reference_map.insert(input.field.clone(), reference);
+            if let Some(reference) = self.isolate.get_reference(input_identifier.as_str()) {
+                reference_map.insert(input_identifier.clone(), reference);
             }
+
+            expressions.insert(input_identifier, rule_value.clone());
         }
 
         Some(RowResult {
             output: outputs,
             rule: Some(expressions),
             reference_map: Some(reference_map),
             index,
```

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/lib.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/lib.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/closure.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/closure.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/filesystem.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/filesystem.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/memory.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/memory.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/loader/mod.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/loader/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/model/mod.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/model/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
 #[cfg_attr(feature = "bincode", derive(Encode, Decode))]
 #[serde(rename_all = "camelCase")]
 pub struct DecisionTableInputField {
     pub id: String,
     pub name: String,
-    pub field: String,
+    pub field: Option<String>,
 }
 
 #[derive(Clone, Debug, PartialEq, Deserialize, Serialize)]
 #[cfg_attr(feature = "bincode", derive(Encode, Decode))]
 #[serde(rename_all = "camelCase")]
 pub struct DecisionTableOutputField {
     pub id: String,
```

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/src/util/json_map.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/src/util/json_map.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/tests/decision.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/tests/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/tests/engine.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/tests/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/tests/model.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/tests/model.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/local_dependencies/zen-engine/tests/support/mod.rs` & `zen_engine-0.8.0/local_dependencies/zen-engine/tests/support/mod.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/.gitignore` & `zen_engine-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/LICENSE` & `zen_engine-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/README.md` & `zen_engine-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/index.py` & `zen_engine-0.8.0/index.py`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/pyproject.toml` & `zen_engine-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/src/decision.rs` & `zen_engine-0.8.0/src/decision.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/src/engine.rs` & `zen_engine-0.8.0/src/engine.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/src/loader.rs` & `zen_engine-0.8.0/src/loader.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/src/value.rs` & `zen_engine-0.8.0/src/value.rs`

 * *Files identical despite different names*

### Comparing `zen_engine-0.7.0/Cargo.lock` & `zen_engine-0.8.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -317,26 +317,26 @@
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "4.3.11"
+version = "4.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1640e5cc7fb47dbb8338fd471b105e7ed6c3cb2aeb00c2e067127ffd3764a05d"
+checksum = "3eab9e8ceb9afdade1ab3f0fd8dbce5b1b2f468ad653baf10e771781b2b67b73"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.11"
+version = "4.3.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "98c59138d527eeaf9b53f35a77fcc1fad9d883116070c63d5de1c7dc7b00c72b"
+checksum = "9f2763db829349bf00cfc06251268865ed4363b93a943174f638daf3ecdba2cd"
 dependencies = [
  "anstyle",
  "clap_lex",
 ]
 
 [[package]]
 name = "clap_lex"
@@ -1846,15 +1846,15 @@
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
 name = "zen-engine"
-version = "0.5.2"
+version = "0.7.0"
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
-version = "0.5.2"
+version = "0.7.0"
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
-version = "0.7.0"
+version = "0.8.0"
 dependencies = [
  "anyhow",
  "async-trait",
  "futures",
  "pyo3",
  "pythonize",
  "serde",
```

### Comparing `zen_engine-0.7.0/PKG-INFO` & `zen_engine-0.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zen-engine
-Version: 0.7.0
+Version: 0.8.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: black; extra == 'dev'
 Requires-Dist: bumpver; extra == 'dev'
 Requires-Dist: isort; extra == 'dev'
 Requires-Dist: pip-tools; extra == 'dev'
```

