# Comparing `tmp/prompt_graph_sdk-0.1.6.tar.gz` & `tmp/prompt_graph_sdk-0.1.7.tar.gz`

## Comparing `prompt_graph_sdk-0.1.6.tar` & `prompt_graph_sdk-0.1.7.tar`

### file list

```diff
@@ -1,103 +1,103 @@
--rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/Cargo.toml
--rw-r--r--   0      501       20        7 2023-06-06 19:00:40.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/.gitignore
--rw-r--r--   0      501       20      176 2023-06-07 21:19:03.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/.idea/.gitignore
--rw-r--r--   0      501       20      372 2023-06-09 01:28:56.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/.idea/modules.xml
--rw-r--r--   0      501       20      480 2023-06-09 01:28:56.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/.idea/prompt-graph-local-exec.iml
--rw-r--r--   0      501       20      186 2023-06-07 21:23:07.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/.idea/vcs.xml
--rw-r--r--   0      501       20    17896 2023-06-07 23:17:18.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/Cargo.lock
--rw-r--r--   0      501       20      930 2023-06-16 08:56:04.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/Dockerfile
--rw-r--r--   0      501       20      186 2023-06-14 07:11:37.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/README.md
--rw-r--r--   0      501       20       67 2023-07-05 18:45:30.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/build.rs
--rw-r--r--   0      501       20      436 2023-07-05 18:08:57.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/package.json
--rw-r--r--   0      501       20     3198 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/branches.rs
--rw-r--r--   0      501       20     3543 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/changes.rs
--rw-r--r--   0      501       20     3365 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/executing_nodes.rs
--rw-r--r--   0      501       20     3897 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/graph_mutations.rs
--rw-r--r--   0      501       20     2630 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/input_proposals_and_responses.rs
--rw-r--r--   0      501       20     4820 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/mod.rs
--rw-r--r--   0      501       20    28985 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/parquet_serialization.rs
--rw-r--r--   0      501       20     1647 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/playback.rs
--rw-r--r--   0      501       20     6495 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/state_path_storage.rs
--rw-r--r--   0      501       20    31979 2023-07-14 01:29:45.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/executor.rs
--rw-r--r--   0      501       20     2194 2023-07-12 19:22:06.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/initialize_nodes/mod.rs
--rw-r--r--   0      501       20       15 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/integrations/mod.rs
--rw-r--r--   0      501       20     1312 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/integrations/openai/batch.rs
--rw-r--r--   0      501       20       33 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/integrations/openai/mod.rs
--rw-r--r--   0      501       20     5757 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/integrations/openai/streaming.rs
--rw-r--r--   0      501       20     4540 2023-07-14 05:19:55.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/lib.rs
--rw-r--r--   0      501       20      253 2023-07-14 23:11:02.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/main.rs
--rw-r--r--   0      501       20      143 2023-07-12 23:10:14.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/mod.rs
--rw-r--r--   0      501       20     2919 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/deno.rs
--rw-r--r--   0      501       20       75 2023-06-29 02:56:18.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/mod.rs
--rw-r--r--   0      501       20     2735 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/node.rs
--rw-r--r--   0      501       20     2290 2023-06-29 02:50:28.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/starlark.rs
--rw-r--r--   0      501       20        9 2023-06-14 18:44:30.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_component/mod.rs
--rw-r--r--   0      501       20      189 2023-06-16 08:43:59.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_component/node.rs
--rw-r--r--   0      501       20     1255 2023-07-12 23:10:14.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_join.rs
--rw-r--r--   0      501       20       13 2023-07-07 23:11:46.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_loader/mod.rs
--rw-r--r--   0      501       20     3455 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_loader/node.rs
--rw-r--r--   0      501       20      976 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_map.rs
--rw-r--r--   0      501       20     2701 2023-07-14 01:13:46.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_memory/in_memory.rs
--rw-r--r--   0      501       20       32 2023-07-14 01:13:46.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_memory/mod.rs
--rw-r--r--   0      501       20    12541 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_memory/node.rs
--rw-r--r--   0      501       20       13 2023-06-14 07:25:43.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_prompt/mod.rs
--rw-r--r--   0      501       20     1611 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_prompt/node.rs
--rw-r--r--   0      501       20    14878 2023-07-14 23:29:22.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/tonic_runtime.rs
--rw-r--r--   0      501       20     4627 2023-07-07 23:11:46.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/tests/data/files_and_dirs.zip
--rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/Cargo.toml
--rw-r--r--   0      501       20        7 2023-06-06 19:00:40.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/.gitignore
--rw-r--r--   0      501       20      176 2023-06-07 21:19:31.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/.idea/.gitignore
--rw-r--r--   0      501       20      348 2023-06-09 01:28:56.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/.idea/modules.xml
--rw-r--r--   0      501       20      480 2023-06-09 01:28:56.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/.idea/prompt-graph-core.iml
--rw-r--r--   0      501       20      247 2023-06-09 18:13:45.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/.idea/vcs.xml
--rw-r--r--   0      501       20      376 2023-06-16 09:32:15.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/README.md
--rw-r--r--   0      501       20      193 2023-07-14 23:56:33.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/build.rs
--rw-r--r--   0      501       20      176 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/.idea/.gitignore
--rw-r--r--   0      501       20      172 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/.idea/misc.xml
--rw-r--r--   0      501       20      270 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/.idea/modules.xml
--rw-r--r--   0      501       20      336 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/.idea/protobufs.iml
--rw-r--r--   0      501       20      183 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/.idea/vcs.xml
--rw-r--r--   0      501       20       83 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/DSLWrapper.proto
--rw-r--r--   0      501       20    10027 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/DSL_v1.proto
--rw-r--r--   0      501       20     1366 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/TypeDef_v1.proto
--rw-r--r--   0      501       20      176 2023-07-15 01:12:03.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/protobufs/.idea/.gitignore
--rw-r--r--   0      501       20      172 2023-07-15 01:12:03.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/protobufs/.idea/misc.xml
--rw-r--r--   0      501       20      270 2023-07-15 01:12:03.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/protobufs/.idea/modules.xml
--rw-r--r--   0      501       20      336 2023-07-15 01:12:03.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/protobufs/.idea/protobufs.iml
--rw-r--r--   0      501       20      183 2023-07-15 01:12:03.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/protobufs/.idea/vcs.xml
--rw-r--r--   0      501       20       83 2023-07-15 01:12:03.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/protobufs/DSLWrapper.proto
--rw-r--r--   0      501       20    10027 2023-07-15 01:12:03.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/protobufs/DSL_v1.proto
--rw-r--r--   0      501       20     1366 2023-07-15 01:12:03.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/protobufs/TypeDef_v1.proto
--rw-r--r--   0      501       20    29405 2023-07-14 01:13:46.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/build_runtime_graph/graph_parse.rs
--rw-r--r--   0      501       20       20 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/build_runtime_graph/mod.rs
--rw-r--r--   0      501       20    10348 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/execution_router.rs
--rw-r--r--   0      501       20     2502 2023-07-14 02:30:00.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/execution_router_wasm.rs
--rw-r--r--   0      501       20    12033 2023-07-14 02:29:37.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/graph_definition.rs
--rw-r--r--   0      501       20     2247 2023-07-14 02:50:22.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/lib.rs
--rw-r--r--   0      501       20       37 2023-06-14 08:37:54.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/proto2.rs
--rw-r--r--   0      501       20     9727 2023-07-12 17:39:12.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/templates.rs
--rw-r--r--   0      501       20     1047 2023-06-14 20:23:24.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/utils/impl_serialize_file.rs
--rw-r--r--   0      501       20      951 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/utils/mod.rs
--rw-r--r--   0      501       20      327 2023-07-14 02:30:18.000000 prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/utils/wasm_error.rs
--rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 prompt_graph_sdk-0.1.6/Cargo.toml
--rw-r--r--   0      501       20      156 2023-07-14 02:35:41.000000 prompt_graph_sdk-0.1.6/build.rs
--rw-r--r--   0      501       20       61 2023-06-16 00:14:00.000000 prompt_graph_sdk-0.1.6/node_test.js
--rw-r--r--   0      501       20      416 2023-07-05 18:09:02.000000 prompt_graph_sdk-0.1.6/package.json
--rw-r--r--   0      501       20      111 2023-07-15 01:12:01.000000 prompt_graph_sdk-0.1.6/pyproject.toml
--rw-r--r--   0      501       20       33 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/scripts/generate_python.sh
--rw-r--r--   0      501       20     3284 2023-07-14 02:36:00.000000 prompt_graph_sdk-0.1.6/src/lib.rs
--rw-r--r--   0      501       20       45 2023-07-12 23:10:14.000000 prompt_graph_sdk-0.1.6/src/main.rs
--rw-r--r--   0      501       20      100 2023-06-16 17:36:43.000000 prompt_graph_sdk-0.1.6/src/translations/mod.rs
--rw-r--r--   0      501       20      256 2023-06-16 06:42:56.000000 prompt_graph_sdk-0.1.6/src/translations/nodejs.rs
--rw-r--r--   0      501       20    35133 2023-07-15 00:14:35.000000 prompt_graph_sdk-0.1.6/src/translations/python.rs
--rw-r--r--   0      501       20     5056 2023-07-14 02:35:16.000000 prompt_graph_sdk-0.1.6/src/translations/rust.rs
--rw-r--r--   0      501       20       43 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/src/translations/wasm.rs
--rw-r--r--   0      501       20      176 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/tests/python/.idea/.gitignore
--rw-r--r--   0      501       20      174 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/tests/python/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0      501       20      185 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/tests/python/.idea/misc.xml
--rw-r--r--   0      501       20      264 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/tests/python/.idea/modules.xml
--rw-r--r--   0      501       20      284 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/tests/python/.idea/python.iml
--rw-r--r--   0      501       20      192 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/tests/python/.idea/vcs.xml
--rw-r--r--   0      501       20      108 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.6/tests/python/test.py
--rw-r--r--   0      501       20   143261 2023-07-15 01:12:03.000000 prompt_graph_sdk-0.1.6/Cargo.lock
--rw-r--r--   0        0        0       60 1970-01-01 00:00:00.000000 prompt_graph_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1234 1970-01-01 00:00:00.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/Cargo.toml
+-rw-r--r--   0      501       20        7 2023-06-06 19:00:40.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/.gitignore
+-rw-r--r--   0      501       20      176 2023-06-07 21:19:31.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/.idea/.gitignore
+-rw-r--r--   0      501       20      348 2023-06-09 01:28:56.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/.idea/modules.xml
+-rw-r--r--   0      501       20      480 2023-06-09 01:28:56.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/.idea/prompt-graph-core.iml
+-rw-r--r--   0      501       20      247 2023-06-09 18:13:45.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/.idea/vcs.xml
+-rw-r--r--   0      501       20      376 2023-06-16 09:32:15.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/README.md
+-rw-r--r--   0      501       20      193 2023-07-14 23:56:33.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/build.rs
+-rw-r--r--   0      501       20      176 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/.idea/.gitignore
+-rw-r--r--   0      501       20      172 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/.idea/misc.xml
+-rw-r--r--   0      501       20      270 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/.idea/modules.xml
+-rw-r--r--   0      501       20      336 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/.idea/protobufs.iml
+-rw-r--r--   0      501       20      183 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/.idea/vcs.xml
+-rw-r--r--   0      501       20       83 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/DSLWrapper.proto
+-rw-r--r--   0      501       20    10027 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/DSL_v1.proto
+-rw-r--r--   0      501       20     1366 2023-07-14 23:57:32.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/TypeDef_v1.proto
+-rw-r--r--   0      501       20      176 2023-07-15 01:49:28.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/protobufs/.idea/.gitignore
+-rw-r--r--   0      501       20      172 2023-07-15 01:49:28.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/protobufs/.idea/misc.xml
+-rw-r--r--   0      501       20      270 2023-07-15 01:49:28.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/protobufs/.idea/modules.xml
+-rw-r--r--   0      501       20      336 2023-07-15 01:49:28.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/protobufs/.idea/protobufs.iml
+-rw-r--r--   0      501       20      183 2023-07-15 01:49:28.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/protobufs/.idea/vcs.xml
+-rw-r--r--   0      501       20       83 2023-07-15 01:49:28.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/protobufs/DSLWrapper.proto
+-rw-r--r--   0      501       20    10027 2023-07-15 01:49:28.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/protobufs/DSL_v1.proto
+-rw-r--r--   0      501       20     1366 2023-07-15 01:49:28.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/protobufs/TypeDef_v1.proto
+-rw-r--r--   0      501       20    29405 2023-07-14 01:13:46.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/build_runtime_graph/graph_parse.rs
+-rw-r--r--   0      501       20       20 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/build_runtime_graph/mod.rs
+-rw-r--r--   0      501       20    10291 2023-07-15 01:48:53.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/execution_router.rs
+-rw-r--r--   0      501       20     2502 2023-07-14 02:30:00.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/execution_router_wasm.rs
+-rw-r--r--   0      501       20    12033 2023-07-14 02:29:37.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/graph_definition.rs
+-rw-r--r--   0      501       20     2247 2023-07-14 02:50:22.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/lib.rs
+-rw-r--r--   0      501       20       37 2023-06-14 08:37:54.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/proto2.rs
+-rw-r--r--   0      501       20     9727 2023-07-12 17:39:12.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/templates.rs
+-rw-r--r--   0      501       20     1047 2023-06-14 20:23:24.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/utils/impl_serialize_file.rs
+-rw-r--r--   0      501       20      951 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/utils/mod.rs
+-rw-r--r--   0      501       20      327 2023-07-14 02:30:18.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/utils/wasm_error.rs
+-rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/Cargo.toml
+-rw-r--r--   0      501       20        7 2023-06-06 19:00:40.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/.gitignore
+-rw-r--r--   0      501       20      176 2023-06-07 21:19:03.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/.idea/.gitignore
+-rw-r--r--   0      501       20      372 2023-06-09 01:28:56.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/.idea/modules.xml
+-rw-r--r--   0      501       20      480 2023-06-09 01:28:56.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/.idea/prompt-graph-local-exec.iml
+-rw-r--r--   0      501       20      186 2023-06-07 21:23:07.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/.idea/vcs.xml
+-rw-r--r--   0      501       20    17896 2023-06-07 23:17:18.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/Cargo.lock
+-rw-r--r--   0      501       20      930 2023-06-16 08:56:04.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/Dockerfile
+-rw-r--r--   0      501       20      186 2023-06-14 07:11:37.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/README.md
+-rw-r--r--   0      501       20       67 2023-07-05 18:45:30.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/build.rs
+-rw-r--r--   0      501       20      436 2023-07-05 18:08:57.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/package.json
+-rw-r--r--   0      501       20     3198 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/branches.rs
+-rw-r--r--   0      501       20     3543 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/changes.rs
+-rw-r--r--   0      501       20     3365 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/executing_nodes.rs
+-rw-r--r--   0      501       20     3897 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/graph_mutations.rs
+-rw-r--r--   0      501       20     2630 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/input_proposals_and_responses.rs
+-rw-r--r--   0      501       20     4820 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/mod.rs
+-rw-r--r--   0      501       20    28959 2023-07-15 01:48:43.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/parquet_serialization.rs
+-rw-r--r--   0      501       20     1647 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/playback.rs
+-rw-r--r--   0      501       20     6495 2023-07-11 22:38:52.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/state_path_storage.rs
+-rw-r--r--   0      501       20    31904 2023-07-15 01:48:58.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/executor.rs
+-rw-r--r--   0      501       20     2194 2023-07-12 19:22:06.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/initialize_nodes/mod.rs
+-rw-r--r--   0      501       20       15 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/integrations/mod.rs
+-rw-r--r--   0      501       20     1312 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/integrations/openai/batch.rs
+-rw-r--r--   0      501       20       33 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/integrations/openai/mod.rs
+-rw-r--r--   0      501       20     5757 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/integrations/openai/streaming.rs
+-rw-r--r--   0      501       20     4540 2023-07-14 05:19:55.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/lib.rs
+-rw-r--r--   0      501       20      253 2023-07-14 23:11:02.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/main.rs
+-rw-r--r--   0      501       20      143 2023-07-12 23:10:14.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/mod.rs
+-rw-r--r--   0      501       20     2887 2023-07-15 01:48:49.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/deno.rs
+-rw-r--r--   0      501       20       75 2023-06-29 02:56:18.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/mod.rs
+-rw-r--r--   0      501       20     2735 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/node.rs
+-rw-r--r--   0      501       20     2290 2023-06-29 02:50:28.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/starlark.rs
+-rw-r--r--   0      501       20        9 2023-06-14 18:44:30.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_component/mod.rs
+-rw-r--r--   0      501       20      189 2023-06-16 08:43:59.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_component/node.rs
+-rw-r--r--   0      501       20     1255 2023-07-12 23:10:14.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_join.rs
+-rw-r--r--   0      501       20       13 2023-07-07 23:11:46.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_loader/mod.rs
+-rw-r--r--   0      501       20     3518 2023-07-15 01:49:15.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_loader/node.rs
+-rw-r--r--   0      501       20      976 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_map.rs
+-rw-r--r--   0      501       20     2701 2023-07-14 01:13:46.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_memory/in_memory.rs
+-rw-r--r--   0      501       20       32 2023-07-14 01:13:46.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_memory/mod.rs
+-rw-r--r--   0      501       20    12541 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_memory/node.rs
+-rw-r--r--   0      501       20       13 2023-06-14 07:25:43.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_prompt/mod.rs
+-rw-r--r--   0      501       20     1611 2023-07-13 11:33:42.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_prompt/node.rs
+-rw-r--r--   0      501       20    14878 2023-07-14 23:29:22.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/tonic_runtime.rs
+-rw-r--r--   0      501       20     4627 2023-07-07 23:11:46.000000 prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/tests/data/files_and_dirs.zip
+-rw-r--r--   0        0        0     1452 1970-01-01 00:00:00.000000 prompt_graph_sdk-0.1.7/Cargo.toml
+-rw-r--r--   0      501       20      156 2023-07-14 02:35:41.000000 prompt_graph_sdk-0.1.7/build.rs
+-rw-r--r--   0      501       20       61 2023-06-16 00:14:00.000000 prompt_graph_sdk-0.1.7/node_test.js
+-rw-r--r--   0      501       20      416 2023-07-05 18:09:02.000000 prompt_graph_sdk-0.1.7/package.json
+-rw-r--r--   0      501       20      111 2023-07-15 01:12:01.000000 prompt_graph_sdk-0.1.7/pyproject.toml
+-rw-r--r--   0      501       20       33 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/scripts/generate_python.sh
+-rw-r--r--   0      501       20     3284 2023-07-14 02:36:00.000000 prompt_graph_sdk-0.1.7/src/lib.rs
+-rw-r--r--   0      501       20       45 2023-07-12 23:10:14.000000 prompt_graph_sdk-0.1.7/src/main.rs
+-rw-r--r--   0      501       20      100 2023-06-16 17:36:43.000000 prompt_graph_sdk-0.1.7/src/translations/mod.rs
+-rw-r--r--   0      501       20      256 2023-06-16 06:42:56.000000 prompt_graph_sdk-0.1.7/src/translations/nodejs.rs
+-rw-r--r--   0      501       20    35177 2023-07-15 01:29:15.000000 prompt_graph_sdk-0.1.7/src/translations/python.rs
+-rw-r--r--   0      501       20     5056 2023-07-14 02:35:16.000000 prompt_graph_sdk-0.1.7/src/translations/rust.rs
+-rw-r--r--   0      501       20       43 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/src/translations/wasm.rs
+-rw-r--r--   0      501       20      176 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/tests/python/.idea/.gitignore
+-rw-r--r--   0      501       20      174 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/tests/python/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0      501       20      185 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/tests/python/.idea/misc.xml
+-rw-r--r--   0      501       20      264 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/tests/python/.idea/modules.xml
+-rw-r--r--   0      501       20      284 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/tests/python/.idea/python.iml
+-rw-r--r--   0      501       20      192 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/tests/python/.idea/vcs.xml
+-rw-r--r--   0      501       20      108 2023-07-07 19:49:23.000000 prompt_graph_sdk-0.1.7/tests/python/test.py
+-rw-r--r--   0      501       20   143261 2023-07-15 01:49:29.000000 prompt_graph_sdk-0.1.7/Cargo.lock
+-rw-r--r--   0        0        0       60 1970-01-01 00:00:00.000000 prompt_graph_sdk-0.1.7/PKG-INFO
```

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/Cargo.toml` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/Cargo.toml`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/Cargo.lock` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/Cargo.lock`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/Dockerfile` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/Dockerfile`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/branches.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/branches.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/changes.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/changes.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/executing_nodes.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/executing_nodes.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/graph_mutations.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/graph_mutations.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/input_proposals_and_responses.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/input_proposals_and_responses.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/mod.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/mod.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/parquet_serialization.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/parquet_serialization.rs`

 * *Files 0% similar despite different names*

```diff
@@ -388,15 +388,14 @@
         let mut array_proposal_counter = UInt64Builder::with_capacity(input_responses.len());
         let mut array_branch = UInt64Builder::with_capacity(input_responses.len());
         let mut array_path = ListBuilder::with_capacity(StringBuilder::new(), input_responses.len());
         let mut array_value = BinaryBuilder::with_capacity(input_responses.len(), MAX_GRAPHQL_QUERY_SIZE_BYTES);
 
         for input_response in input_responses {
             for c in input_response.changes {
-                dbg!(&c);
                 array_id.append_value(input_response.id.clone());
                 array_proposal_counter.append_value(input_response.proposal_counter);
                 array_branch.append_value(input_response.branch);
                 array_path.append_value(c.path.unwrap().address.into_iter().map(|x| Some(x)));
                 array_value.append_value(c.value.unwrap().encode_to_vec());
             }
         }
```

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/playback.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/playback.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/db_operations/state_path_storage.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/db_operations/state_path_storage.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/executor.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/executor.rs`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,14 @@
             .change_values_used_in_execution
             .iter()
             .map(|p| p.monotonic_counter).collect();
 
         // let change_set = &node_will_execute
         //     .change_values_used_in_execution.iter().map(|x| x.change_value.as_ref().unwrap().clone()).collect();
 
-        dbg!(&name);
         let output_namespaces = self.clean_definition_graph.node_to_output_tables.get(name).unwrap().clone();
 
         let filled_values = match (item.core.as_ref().unwrap(), item.item.as_ref().unwrap()) {
             (c, item::Item::Map(n)) => {
                 node_map::execute_node_map(&node_will_execute, n, &output_namespaces)
             }
             (c, item::Item::NodeCode(n)) => {
@@ -598,15 +597,14 @@
         };
         debug_scan_all_state_counters(&executor.tree,0 );
         insert_pending_graph_mutation(&executor.tree, 0, mutation_file);
         executor.progress_mutations().await;
         executor.progress_changes().await;
         let v: Vec<_> = scan_all_pending_changes(&executor.tree).collect();
         debug_scan_all_state_counters(&executor.tree,0 );
-        dbg!(&v);
         assert_eq!(v.len(), 1);
         assert_eq!(v[0].filled_values[0].value.as_ref().unwrap().val.as_ref().unwrap(), &Val::String("hello world".to_string()));
         // TODO: on introduction of a new node, it should be evaluated based on existing state at that frame
     }
 
 
     // TODO: validate pause functionality - no changes should be processed while paused
@@ -677,24 +675,22 @@
         play_execution_at_frame(&executor.tree, 0);
 
         // TODO: validate that the branch is created and that the node is re-run on the branch
         // TODO: we should now see that previous change get evaluated in _both_ branches
         // TODO: and we should see changes created for both
 
         let v: Vec<_> = scan_all_pending_changes(&executor.tree).collect();
-        dbg!(&v);
         assert_eq!(v.len(), 1);
         assert_eq!(v[0].source_node, "code_node_test".to_string());
         assert_eq!(v[0].monotonic_counter, 1);
         assert_eq!(v[0].branch, 0);
 
         // This progress_changes should evaluate each of the branches
         executor.progress_changes().await;
         let v: Vec<_> = scan_all_pending_changes(&executor.tree).collect();
-        dbg!(&v);
         assert_eq!(v.len(), 2);
         assert_eq!(v[0].source_node, "code_node_test_dep".to_string());
         assert_eq!(v[1].source_node, "code_node_test_dep".to_string());
         assert_eq!(v[0].branch, 0);
         assert_eq!(v[1].branch, 1);
         assert_eq!(v[0].monotonic_counter, 2);
         assert_eq!(v[1].monotonic_counter, 2);
```

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/initialize_nodes/mod.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/initialize_nodes/mod.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/integrations/openai/batch.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/integrations/openai/batch.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/integrations/openai/streaming.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/integrations/openai/streaming.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/lib.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/deno.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/deno.rs`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
         c.source_code.clone()
     };
 
     let wrapped_source_code = format!(r#"(function main() {{
         {}
     }})();"#, source_code);
 
-    dbg!(&wrapped_source_code);
     let mut runtime = JsRuntime::new(
         RuntimeOptions::default(),
     );
     // TODO: the script receives the arguments as a json payload "#state"
     let result = runtime.execute_script(
         "main.js",
         FastString::Owned(wrapped_source_code.into_boxed_str()),
```

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/node.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/node.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/starlark.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_code/starlark.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_join.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_join.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_loader/node.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_loader/node.rs`

 * *Files 5% similar despite different names*

```diff
@@ -72,19 +72,20 @@
 
         let nwe = NodeWillExecute {
             source_node: "".to_string(),
             change_values_used_in_execution: vec![],
             matched_query_index: 0
         };
 
-        dbg!(execute_node_loader(&nwe, &&PromptGraphNodeLoader {
-            load_from: Some(LoadFrom::ZipfileBytes(buffer)),
-        }, &ItemCore {
-            name: "test".to_string(),
-            ..Default::default()
-        },
-
-            &HashSet::from(["".to_string()])
-        ).unwrap());
+        // TODO: assert this
+        // dbg!(execute_node_loader(&nwe, &&PromptGraphNodeLoader {
+        //     load_from: Some(LoadFrom::ZipfileBytes(buffer)),
+        // }, &ItemCore {
+        //     name: "test".to_string(),
+        //     ..Default::default()
+        // },
+        //
+        //     &HashSet::from(["".to_string()])
+        // ).unwrap());
         Ok(())
     }
 }
```

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_map.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_map.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_memory/in_memory.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_memory/in_memory.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_memory/node.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_memory/node.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_prompt/node.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/runtime_nodes/node_prompt/node.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/src/tonic_runtime.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/src/tonic_runtime.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-exec/tests/data/files_and_dirs.zip` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-exec/tests/data/files_and_dirs.zip`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/Cargo.toml` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/DSL_v1.proto` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/DSL_v1.proto`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/TypeDef_v1.proto` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/TypeDef_v1.proto`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/protobufs/DSL_v1.proto` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/protobufs/DSL_v1.proto`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/protobufs/protobufs/TypeDef_v1.proto` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/protobufs/protobufs/TypeDef_v1.proto`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/build_runtime_graph/graph_parse.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/build_runtime_graph/graph_parse.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/execution_router.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/execution_router.rs`

 * *Files 1% similar despite different names*

```diff
@@ -15,22 +15,20 @@
     state: &impl ExecutionState,
     paths_to_satisfy: &Vec<Vec<String>>
 ) -> Option<Vec<WrappedChangeValue>> {
     // for each of the matched nodes, we need to evaluate the query against the current state
     // check if the updated state object is satisfying all necessary paths for this query
     let mut satisfied_paths = vec![];
 
-    dbg!(&paths_to_satisfy);
     for path in paths_to_satisfy {
         if let Some(change_value) = state.get_value(path.join(":").as_bytes()) {
             satisfied_paths.push(change_value.clone());
         }
     }
 
-    dbg!(&satisfied_paths);
     if satisfied_paths.len() != paths_to_satisfy.len() { return None }
 
     Some(satisfied_paths.into_iter().map(|(counter, v)| WrappedChangeValue {
         monotonic_counter: counter,
         change_value: Some(v),
     }).collect())
 }
```

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/execution_router_wasm.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/execution_router_wasm.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/graph_definition.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/graph_definition.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/lib.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/templates.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/templates.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/utils/impl_serialize_file.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/utils/impl_serialize_file.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/local_dependencies/prompt-graph-core/src/utils/mod.rs` & `prompt_graph_sdk-0.1.7/local_dependencies/prompt-graph-core/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/Cargo.toml` & `prompt_graph_sdk-0.1.7/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "prompt-graph-sdk"
-version = "0.1.6"
+version = "0.1.7"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "prompt_graph_sdk"
 crate-type = ["cdylib", "lib"]
 bench = false
```

### Comparing `prompt_graph_sdk-0.1.6/src/lib.rs` & `prompt_graph_sdk-0.1.7/src/lib.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/src/translations/python.rs` & `prompt_graph_sdk-0.1.7/src/translations/python.rs`

 * *Files 0% similar despite different names*

```diff
@@ -305,14 +305,15 @@
         dict.set_item("branch", branch).unwrap();
         dict.set_item("counter", counter).unwrap();
         if let Some(node) = node {
             dict.set_item("node_name", &node.source_node).unwrap();
             dict.set_item("type_name", &custom_node_type_name).unwrap();
 
             let event_dict = PyDict::new(py);
+            // TODO: this needs to be fixed
             for change in &node.change_values_used_in_execution {
                 if let Some(v) = &change.change_value {
                     match v {
                         ChangeValue { path: Some(path), value: Some(value), .. } => {
                             add_to_dict(
                                 py,
                                 &path.address,
```

### Comparing `prompt_graph_sdk-0.1.6/src/translations/rust.rs` & `prompt_graph_sdk-0.1.7/src/translations/rust.rs`

 * *Files identical despite different names*

### Comparing `prompt_graph_sdk-0.1.6/Cargo.lock` & `prompt_graph_sdk-0.1.7/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -3518,15 +3518,15 @@
  "twox-hash",
  "ulid",
  "zip",
 ]
 
 [[package]]
 name = "prompt-graph-sdk"
-version = "0.1.6"
+version = "0.1.7"
 dependencies = [
  "anyhow",
  "env_logger 0.10.0",
  "futures 0.3.28",
  "handlebars",
  "indoc",
  "log",
```

