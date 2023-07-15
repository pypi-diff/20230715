# Comparing `tmp/colossalai-nightly-2023.7.15.tar.gz` & `tmp/colossalai-nightly-2023.7.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colossalai-nightly-2023.7.15.tar", last modified: Sat Jul 15 00:17:29 2023, max compression
+gzip compressed data, was "colossalai-nightly-2023.7.8.tar", last modified: Sat Jul  8 00:17:20 2023, max compression
```

## Comparing `colossalai-nightly-2023.7.15.tar` & `colossalai-nightly-2023.7.8.tar`

### file list

```diff
@@ -1,955 +1,955 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.225348 colossalai-nightly-2023.7.15/
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25400 2023-07-15 00:17:29.225348 colossalai-nightly-2023.7.15/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.093349 colossalai-nightly-2023.7.15/colossalai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.093349 colossalai-nightly-2023.7.15/colossalai/_C/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.093349 colossalai-nightly-2023.7.15/colossalai/_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.093349 colossalai-nightly-2023.7.15/colossalai/_analyzer/_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/_subclasses/_meta_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/_subclasses/_monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/_subclasses/flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/_subclasses/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.097349 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/graph_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/node_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.097349 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/passes/graph_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/passes/shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/symbolic_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.097349 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.097349 colossalai-nightly-2023.7.15/colossalai/amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/amp_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.097349 colossalai-nightly-2023.7.15/colossalai/amp/apex_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/apex_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/apex_amp/apex_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.097349 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/_fp16_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.097349 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/grad_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/grad_scaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.101349 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/mixed_precision_mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/mixed_precision_mixin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/naive_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.101349 colossalai-nightly-2023.7.15/colossalai/amp/torch_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/torch_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/torch_amp/_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/amp/torch_amp/torch_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.101349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.101349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/build_c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.101349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.105349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.105349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/base_offload_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/mem_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/training_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.109349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/comm_metainfo_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/runtime_apply_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/runtime_preparation_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.109349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/pipeline_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/pipeline_shard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.109349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.113349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.117349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.117349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.117349 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/sharding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.117349 colossalai-nightly-2023.7.15/colossalai/booster/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/booster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.121349 colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/fp16_apex.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/fp16_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/fp16_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/fp8.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/mixed_precision_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.121349 colossalai-nightly-2023.7.15/colossalai/booster/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/plugin/dp_plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/plugin/gemini_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/plugin/low_level_zero_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/plugin/torch_ddp_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/booster/plugin/torch_fsdp_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.121349 colossalai-nightly-2023.7.15/colossalai/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.121349 colossalai-nightly-2023.7.15/colossalai/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/checkpoint_io/checkpoint_io_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/checkpoint_io/general_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/checkpoint_io/index_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    22100 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/checkpoint_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.121349 colossalai-nightly-2023.7.15/colossalai/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.121349 colossalai-nightly-2023.7.15/colossalai/cli/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/benchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.121349 colossalai-nightly-2023.7.15/colossalai/cli/check/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/check/check_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.125349 colossalai-nightly-2023.7.15/colossalai/cli/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/launcher/hostinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/launcher/multinode_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cli/launcher/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.125349 colossalai-nightly-2023.7.15/colossalai/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cluster/device_mesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cluster/dist_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/cluster/process_group_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.125349 colossalai-nightly-2023.7.15/colossalai/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/communication/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/communication/p2p.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/communication/p2p_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/communication/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.125349 colossalai-nightly-2023.7.15/colossalai/context/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/moe_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/parallel_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/parallel_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.129349 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/process_group_initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.129349 colossalai-nightly-2023.7.15/colossalai/context/random/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/random/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/random/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/context/singleton_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.129349 colossalai-nightly-2023.7.15/colossalai/device/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/device/alpha_beta_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/device/calc_pipeline_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/device/device_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.129349 colossalai-nightly-2023.7.15/colossalai/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/_base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.129349 colossalai-nightly-2023.7.15/colossalai/engine/gradient_accumulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/gradient_accumulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.129349 colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_base_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_moe_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_zero_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.133349 colossalai-nightly-2023.7.15/colossalai/engine/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/schedule/_base_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/schedule/_non_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/schedule/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/engine/schedule/_pipeline_schedule_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.133349 colossalai-nightly-2023.7.15/colossalai/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/_meta_regist_12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/_meta_regist_13.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.133349 colossalai-nightly-2023.7.15/colossalai/fx/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/codegen/activation_checkpoint_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/graph_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.133349 colossalai-nightly-2023.7.15/colossalai/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/passes/adding_split_node_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/passes/concrete_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/passes/passes_for_gpt2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/passes/shard_1d_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/passes/split_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/passes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.133349 colossalai-nightly-2023.7.15/colossalai/fx/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.137349 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.137349 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.141349 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/memory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/opcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/profiler/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.141349 colossalai-nightly-2023.7.15/colossalai/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/_meta_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/_symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/_tracer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.141349 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.141349 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.141349 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.141349 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.145349 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.145349 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/fx/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.145349 colossalai-nightly-2023.7.15/colossalai/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/interface/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/interface/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.145349 colossalai-nightly-2023.7.15/colossalai/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.149349 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.153349 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.157349 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
--rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.157349 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
--rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/scaled_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.157349 colossalai-nightly-2023.7.15/colossalai/kernel/jit/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/jit/bias_dropout_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/jit/bias_gelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/jit/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.161349 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.161349 colossalai-nightly-2023.7.15/colossalai/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23592 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/lazy/lazy_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.161349 colossalai-nightly-2023.7.15/colossalai/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.161349 colossalai-nightly-2023.7.15/colossalai/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.165349 colossalai-nightly-2023.7.15/colossalai/nn/_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/element_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/embedding_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/_ops/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.165349 colossalai-nightly-2023.7.15/colossalai/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/base_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.165349 colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.165349 colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.165349 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_1d/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_1d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_1d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_1d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.165349 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2d/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.169349 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2p5d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2p5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2p5d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2p5d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2p5d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.169349 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_3d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_3d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_3d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_3d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_3d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.169349 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_sequence/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_sequence/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_sequence/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.169349 colossalai-nightly-2023.7.15/colossalai/nn/layer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.169349 colossalai-nightly-2023.7.15/colossalai/nn/layer/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/vanilla/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.169349 colossalai-nightly-2023.7.15/colossalai/nn/layer/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/layer/wrapper/pipeline_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.169349 colossalai-nightly-2023.7.15/colossalai/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/loss/loss_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/loss/loss_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/loss/loss_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/loss/loss_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/loss/loss_moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.173349 colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/delayed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/onecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.173349 colossalai-nightly-2023.7.15/colossalai/nn/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/metric/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/metric/accuracy_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/metric/accuracy_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/metric/accuracy_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.173349 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/colossalai_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/fused_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/fused_lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/fused_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/hybrid_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/optimizer/nvme_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.173349 colossalai-nightly-2023.7.15/colossalai/nn/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.173349 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.177348 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/copyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/colo_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/nn/parallel/reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.177348 colossalai-nightly-2023.7.15/colossalai/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/layer_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.177348 colossalai-nightly-2023.7.15/colossalai/pipeline/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.177348 colossalai-nightly-2023.7.15/colossalai/pipeline/middleware/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/middleware/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/middleware/adaptor/fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/middleware/topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/pipelinable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/pipeline_process_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.177348 colossalai-nightly-2023.7.15/colossalai/pipeline/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59170 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/rpc/_pipeline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/rpc/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.177348 colossalai-nightly-2023.7.15/colossalai/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.177348 colossalai-nightly-2023.7.15/colossalai/shardformer/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.181349 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/parallel_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/qkv_fused_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/layer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.181349 colossalai-nightly-2023.7.15/colossalai/shardformer/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/modeling/bloom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.181349 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/autopolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/basepolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/policies/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.181349 colossalai-nightly-2023.7.15/colossalai/shardformer/shard/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/shard/shard_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/shard/sharder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/shardformer/shard/shardformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.185349 colossalai-nightly-2023.7.15/colossalai/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/colo_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/colo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21790 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/compute_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.185349 colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    24565 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/layout_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/dist_spec_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/distspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/op_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/param_op_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/process_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    36486 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/shape_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/tensor_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.189349 colossalai-nightly-2023.7.15/colossalai/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/testing/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/testing/pytest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/testing/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.189349 colossalai-nightly-2023.7.15/colossalai/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/trainer/_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.189349 colossalai-nightly-2023.7.15/colossalai/trainer/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/trainer/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_commons_.py
--rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_log_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_metric_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.189349 colossalai-nightly-2023.7.15/colossalai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/activation_checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.189349 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint/module_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.193349 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.193349 colossalai-nightly-2023.7.15/colossalai/utils/data_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/data_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/data_sampler/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/data_sampler/data_parallel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.193349 colossalai-nightly-2023.7.15/colossalai/utils/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.193349 colossalai-nightly-2023.7.15/colossalai/utils/multi_tensor_apply/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/multi_tensor_apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.193349 colossalai-nightly-2023.7.15/colossalai/utils/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/profiler/extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.193349 colossalai-nightly-2023.7.15/colossalai/utils/profiler/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/profiler/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/profiler/legacy/comm_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/profiler/legacy/pcie_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/profiler/legacy/prof_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/profiler/stateful_tensor_mem_extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.193349 colossalai-nightly-2023.7.15/colossalai/utils/rank_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/rank_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/rank_recorder/rank_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.193349 colossalai-nightly-2023.7.15/colossalai/utils/tensor_detector/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/tensor_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/tensor_detector/tensor_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.193349 colossalai-nightly-2023.7.15/colossalai/zero/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.197348 colossalai-nightly-2023.7.15/colossalai/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.197348 colossalai-nightly-2023.7.15/colossalai/zero/gemini/chunk/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/chunk/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/chunk/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/chunk/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/chunk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/colo_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    37822 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/gemini_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/gemini_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/gemini_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    29879 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/gemini_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.197348 colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/memory_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/gemini/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.197348 colossalai-nightly-2023.7.15/colossalai/zero/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.201348 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/gemini_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.201348 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/ophooks/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/ophooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/ophooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.201348 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/paramhooks/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/paramhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/stateful_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/tensor_placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.201348 colossalai-nightly-2023.7.15/colossalai/zero/legacy/init_ctx/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/init_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/init_ctx/init_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.201348 colossalai-nightly-2023.7.15/colossalai/zero/legacy/shard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/shard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/shard_utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.201348 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/zero_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.201348 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_optim/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.201348 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_param/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_param/sharded_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_param/sharded_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.205348 colossalai-nightly-2023.7.15/colossalai/zero/low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/low_level/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.205348 colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/base_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/bucket_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/gradient_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    26595 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/low_level/low_level_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/colossalai/zero/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.205348 colossalai-nightly-2023.7.15/colossalai_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25400 2023-07-15 00:17:28.000000 colossalai-nightly-2023.7.15/colossalai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39364 2023-07-15 00:17:29.000000 colossalai-nightly-2023.7.15/colossalai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 00:17:28.000000 colossalai-nightly-2023.7.15/colossalai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-15 00:17:28.000000 colossalai-nightly-2023.7.15/colossalai_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-15 00:17:28.000000 colossalai-nightly-2023.7.15/colossalai_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-15 00:17:28.000000 colossalai-nightly-2023.7.15/colossalai_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.209348 colossalai-nightly-2023.7.15/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.209348 colossalai-nightly-2023.7.15/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 00:17:29.225348 colossalai-nightly-2023.7.15/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.093349 colossalai-nightly-2023.7.15/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.209348 colossalai-nightly-2023.7.15/tests/components_to_test/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/hanging_param_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/inline_op_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/nested_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/repeated_computed_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/simple_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.209348 colossalai-nightly-2023.7.15/tests/components_to_test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/utils/dummy_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/components_to_test/utils/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.209348 colossalai-nightly-2023.7.15/tests/kit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.209348 colossalai-nightly-2023.7.15/tests/kit/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.209348 colossalai-nightly-2023.7.15/tests/kit/model_zoo/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/diffusers/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.213348 colossalai-nightly-2023.7.15/tests/kit/model_zoo/timm/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/timm/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.213348 colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchaudio/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchaudio/torchaudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.213348 colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchrec/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchrec/torchrec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.213348 colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchvision/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.213348 colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/t5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.213348 colossalai-nightly-2023.7.15/tests/test_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.217348 colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/test_bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/test_mod_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/test_nested_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/test_shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/test_symbolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.217348 colossalai-nightly-2023.7.15/tests/test_analyzer/test_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_subclasses/test_aten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_subclasses/test_flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_analyzer/test_subclasses/test_meta_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.217348 colossalai-nightly-2023.7.15/tests/test_auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.217348 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_pass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_pass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.217348 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.217348 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.221348 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.225348 colossalai-nightly-2023.7.15/tests/test_shardformer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:29.225348 colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/tests/test_shardformer/test_with_torch_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 00:17:16.000000 colossalai-nightly-2023.7.15/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_C/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_meta_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/graph_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/node_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/graph_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/symbolic_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/amp_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/apex_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_fp16_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/naive_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/torch_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/build_c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/base_offload_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/mem_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/training_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/comm_metainfo_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_apply_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_preparation_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/pipeline_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/pipeline_shard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.938463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/sharding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/booster/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/booster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_apex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/mixed_precision_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/booster/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/dp_plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/gemini_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/low_level_zero_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_ddp_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_fsdp_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/checkpoint_io_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/general_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/index_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22100 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/cli/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/check/check_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/cli/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/hostinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/multinode_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/device_mesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/dist_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/process_group_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/p2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/p2p_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/moe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/parallel_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/parallel_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/process_group_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/context/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/random/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/random/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/singleton_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/alpha_beta_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/calc_pipeline_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/device_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/_base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_base_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_moe_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_zero_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/engine/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_base_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_non_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_13.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/codegen/activation_checkpoint_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/graph_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/adding_split_node_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/concrete_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/passes_for_gpt2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/shard_1d_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/split_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/memory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/opcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/_meta_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/_symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/_tracer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/interface/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/interface/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.970465 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.970465 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/layer_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/scaled_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/kernel/jit/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_dropout_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_gelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23592 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/lazy/lazy_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/element_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/base_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/pipeline_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/delayed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/colossalai_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/hybrid_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/nvme_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/copyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/colo_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/layer_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/pipelinable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/pipeline_process_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59170 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/shardformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/parallel_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/qkv_fused_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/bloom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/autopolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/basepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/shard_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/sharder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/shardformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/colo_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/colo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21790 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/compute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24565 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/dist_spec_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/distspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/op_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/param_op_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36486 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/shape_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/tensor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/pytest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_commons_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_log_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_metric_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/activation_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/module_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/convertor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/data_parallel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/comm_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/pcie_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/prof_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/stateful_tensor_mem_extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/rank_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/tensor_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/zero/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/colo_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37822 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29879 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/gemini_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/init_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/zero_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/base_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/bucket_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/gradient_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26595 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/low_level_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39364 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.922461 colossalai-nightly-2023.7.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/components_to_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/hanging_param_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/inline_op_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/nested_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/repeated_computed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/simple_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/components_to_test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/utils/dummy_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/utils/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/torchaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/torchrec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/t5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_mod_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_nested_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_symbolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_aten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_meta_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.022470 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.022470 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/tests/test_shardformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_with_torch_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/version.txt
```

### Comparing `colossalai-nightly-2023.7.15/LICENSE` & `colossalai-nightly-2023.7.8/LICENSE`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/PKG-INFO` & `colossalai-nightly-2023.7.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.7.15
+Version: 2023.7.8
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.7.15 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.7.8 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
```

### Comparing `colossalai-nightly-2023.7.15/README.md` & `colossalai-nightly-2023.7.8/README.md`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/_subclasses/_meta_registration.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_meta_registration.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/_subclasses/_monkey_patch.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/_subclasses/flop_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/_subclasses/meta_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/codegen.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/graph_module.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/node_util.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/node_util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/passes/graph_profile.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/graph_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/passes/shape_prop.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/symbolic_profile.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/bias_addition.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/custom_leaf_module.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/custom_leaf_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/proxy.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/symbolic_trace.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/_analyzer/fx/tracer/tracer.py` & `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/apex_amp/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/apex_amp/apex_amp.py` & `colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/apex_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/_fp16_optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/mixed_precision_mixin/base.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/naive_amp/naive_amp.py` & `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/naive_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/torch_amp/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/torch_amp/_grad_scaler.py` & `colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/amp/torch_amp/torch_amp.py` & `colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/torch_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/checkpoint/operation.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/meta_registry/where.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/where.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/registry.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/meta_profiler/shard_metainfo.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/shard_metainfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/amp_optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/amp_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/base_offload_module.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/base_offload_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/mem_optimize.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/mem_optimize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/region.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/region_manager.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/runtime.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/runtime.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/solver.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/training_simulator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/training_simulator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/offload/util.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/comm_metainfo_pass.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/comm_metainfo_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/meta_info_prop.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/runtime_apply_pass.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_apply_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/passes/runtime_preparation_pass.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_preparation_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/constants.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/initialize.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/registry.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/options.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/options.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/sharding_strategy.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/sharding_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/solver/solver.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/broadcast.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/factory.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/factory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/misc.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/misc.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/reshape.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/auto_parallel/tensor_shard/utils/sharding.py` & `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/sharding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/accelerator.py` & `colossalai-nightly-2023.7.8/colossalai/booster/accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/booster.py` & `colossalai-nightly-2023.7.8/colossalai/booster/booster.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/fp16_apex.py` & `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_apex.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/fp16_naive.py` & `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_naive.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/fp16_torch.py` & `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/mixed_precision/mixed_precision_base.py` & `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/mixed_precision_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/plugin/dp_plugin_base.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/dp_plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/plugin/gemini_plugin.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/gemini_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/plugin/low_level_zero_plugin.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/low_level_zero_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/plugin/plugin_base.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/plugin/torch_ddp_plugin.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_ddp_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/booster/plugin/torch_fsdp_plugin.py` & `colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_fsdp_plugin.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/builder/builder.py` & `colossalai-nightly-2023.7.8/colossalai/builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/checkpoint_io/checkpoint_io_base.py` & `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/checkpoint_io_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/checkpoint_io/general_checkpoint_io.py` & `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/general_checkpoint_io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/checkpoint_io/index_file.py` & `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/index_file.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/checkpoint_io/utils.py` & `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cli/benchmark/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/cli/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cli/benchmark/benchmark.py` & `colossalai-nightly-2023.7.8/colossalai/cli/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cli/benchmark/utils.py` & `colossalai-nightly-2023.7.8/colossalai/cli/benchmark/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cli/check/check_installation.py` & `colossalai-nightly-2023.7.8/colossalai/cli/check/check_installation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cli/launcher/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/cli/launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cli/launcher/hostinfo.py` & `colossalai-nightly-2023.7.8/colossalai/cli/launcher/hostinfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cli/launcher/multinode_runner.py` & `colossalai-nightly-2023.7.8/colossalai/cli/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cli/launcher/run.py` & `colossalai-nightly-2023.7.8/colossalai/cli/launcher/run.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cluster/device_mesh_manager.py` & `colossalai-nightly-2023.7.8/colossalai/cluster/device_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cluster/dist_coordinator.py` & `colossalai-nightly-2023.7.8/colossalai/cluster/dist_coordinator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/cluster/process_group_manager.py` & `colossalai-nightly-2023.7.8/colossalai/cluster/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/communication/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/communication/collective.py` & `colossalai-nightly-2023.7.8/colossalai/communication/collective.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/communication/p2p.py` & `colossalai-nightly-2023.7.8/colossalai/communication/p2p.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/communication/p2p_v2.py` & `colossalai-nightly-2023.7.8/colossalai/communication/p2p_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/communication/ring.py` & `colossalai-nightly-2023.7.8/colossalai/communication/ring.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/communication/utils.py` & `colossalai-nightly-2023.7.8/colossalai/communication/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/constants.py` & `colossalai-nightly-2023.7.8/colossalai/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/config.py` & `colossalai-nightly-2023.7.8/colossalai/context/config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/moe_context.py` & `colossalai-nightly-2023.7.8/colossalai/context/moe_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/parallel_context.py` & `colossalai-nightly-2023.7.8/colossalai/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/parallel_mode.py` & `colossalai-nightly-2023.7.8/colossalai/context/parallel_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_1d.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_2d.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_2p5d.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_3d.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_data.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_data.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_model.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_pipeline.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_pipeline.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_sequence.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_sequence.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/initializer_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/process_group_initializer/process_group_initializer.py` & `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/random/_helper.py` & `colossalai-nightly-2023.7.8/colossalai/context/random/_helper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/random/seed_manager.py` & `colossalai-nightly-2023.7.8/colossalai/context/random/seed_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/context/singleton_meta.py` & `colossalai-nightly-2023.7.8/colossalai/context/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/device/alpha_beta_profiler.py` & `colossalai-nightly-2023.7.8/colossalai/device/alpha_beta_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/device/calc_pipeline_strategy.py` & `colossalai-nightly-2023.7.8/colossalai/device/calc_pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/device/device_mesh.py` & `colossalai-nightly-2023.7.8/colossalai/device/device_mesh.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/_base_engine.py` & `colossalai-nightly-2023.7.8/colossalai/engine/_base_engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/gradient_accumulation/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/gradient_accumulation/_gradient_accumulation.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/_gradient_accumulation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_base_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_base_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_moe_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_moe_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/_zero_gradient_handler.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_zero_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/gradient_handler/utils.py` & `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/schedule/_base_schedule.py` & `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_base_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/schedule/_non_pipeline_schedule.py` & `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_non_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/schedule/_pipeline_schedule.py` & `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/engine/schedule/_pipeline_schedule_v2.py` & `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/_compatibility.py` & `colossalai-nightly-2023.7.8/colossalai/fx/_compatibility.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/_meta_regist_12.py` & `colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_12.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/_meta_regist_13.py` & `colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_13.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/codegen/activation_checkpoint_codegen.py` & `colossalai-nightly-2023.7.8/colossalai/fx/codegen/activation_checkpoint_codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/graph_module.py` & `colossalai-nightly-2023.7.8/colossalai/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/passes/adding_split_node_pass.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/adding_split_node_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/passes/concrete_info_prop.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/concrete_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/passes/meta_info_prop.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/passes/passes_for_gpt2_test.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/passes_for_gpt2_test.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/passes/shard_1d_pass.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/shard_1d_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/passes/split_module.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/split_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/passes/utils.py` & `colossalai-nightly-2023.7.8/colossalai/fx/passes/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/constants.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/dataflow.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/constants.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/activation_function.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/pooling.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/activation_function.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/attention.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/convolution.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/pooling.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/profiler_module/rnn.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/registry.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/experimental/shard_utils.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/memory_utils.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/memory_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/opcount.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/opcount.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/profiler.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/shard_utils.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/profiler/tensor.py` & `colossalai-nightly-2023.7.8/colossalai/fx/profiler/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/proxy.py` & `colossalai-nightly-2023.7.8/colossalai/fx/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/_meta_trace.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/_meta_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/_symbolic_trace.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/_symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/_tracer_utils.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/_tracer_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/experimental.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/experimental.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/convolution.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/convolution.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/pooling.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/meta_patch/patched_module/rnn.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/registry.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/fx/tracer/tracer.py` & `colossalai-nightly-2023.7.8/colossalai/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/global_variables.py` & `colossalai-nightly-2023.7.8/colossalai/global_variables.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/initialize.py` & `colossalai-nightly-2023.7.8/colossalai/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/interface/model.py` & `colossalai-nightly-2023.7.8/colossalai/interface/model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/interface/optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/interface/optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/cpu_adam.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/context.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/context.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/csrc/type_shim.h` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/type_shim.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/flash_attention.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/flash_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/layer_norm.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/layer_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/multihead_attention.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/cuda_native/scaled_softmax.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/scaled_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/jit/bias_dropout_add.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_dropout_add.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/jit/bias_gelu.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_gelu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/jit/option.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/jit/option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/builder.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/cpu_adam.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/fused_optim.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/layernorm.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/moe.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/kernel/op_builder/utils.py` & `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/lazy/lazy_init.py` & `colossalai-nightly-2023.7.8/colossalai/lazy/lazy_init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/logging/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/logging/logger.py` & `colossalai-nightly-2023.7.8/colossalai/logging/logger.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/_ops/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/_ops/addmm.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/_ops/batch_norm.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/batch_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/_ops/element_wise.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/element_wise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/_ops/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/_ops/embedding_bag.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding_bag.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/_ops/layernorm.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/_ops/linear.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/_ops/loss.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/_ops/view.py` & `colossalai-nightly-2023.7.8/colossalai/nn/_ops/view.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/init.py` & `colossalai-nightly-2023.7.8/colossalai/nn/init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/base_layer.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/base_layer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/dropout.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/linear.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/colossalai_layer/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/checkpoint.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/experts.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/experts.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/routers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/routers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/moe/utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_1d/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_1d/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_1d/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2d/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2d/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2d/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2p5d/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2p5d/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_2p5d/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_3d/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_3d/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_3d/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_sequence/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/parallel_sequence/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/utils/common.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/vanilla/layers.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/layer/wrapper/pipeline_wrapper.py` & `colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/loss/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/loss/loss_1d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/loss/loss_2d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/loss/loss_2p5d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/loss/loss_3d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/loss/loss_moe.py` & `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/cosine.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/delayed.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/delayed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/linear.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/multistep.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/multistep.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/onecycle.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/onecycle.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/poly.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/poly.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/lr_scheduler/torch.py` & `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/metric/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/metric/accuracy_2d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/metric/accuracy_2p5d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/metric/accuracy_3d.py` & `colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/optimizer/colossalai_optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/colossalai_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/optimizer/cpu_adam.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/optimizer/fused_adam.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/optimizer/fused_lamb.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/optimizer/fused_sgd.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/optimizer/hybrid_adam.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/hybrid_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/optimizer/lamb.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/optimizer/lars.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/optimizer/nvme_optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/nvme_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/data_parallel.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/copyer.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/copyer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/colo_module.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/colo_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/linear.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/layers/module_utils.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/module_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/nn/parallel/reducer.py` & `colossalai-nightly-2023.7.8/colossalai/nn/parallel/reducer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/pipeline/layer_spec.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/layer_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/pipeline/middleware/adaptor/fx.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/fx.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/pipeline/middleware/topo.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/topo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/pipeline/pipelinable.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/pipelinable.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/pipeline/pipeline_process_group.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/pipeline_process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/pipeline/rpc/_pipeline_base.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/pipeline/rpc/_pipeline_schedule.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/pipeline/rpc/utils.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/pipeline/utils.py` & `colossalai-nightly-2023.7.8/colossalai/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/registry/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/registry/registry.py` & `colossalai-nightly-2023.7.8/colossalai/registry/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/layer/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/layer/_operation.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/layer/dropout.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/layer/embedding.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/layer/linear.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/layer/loss.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/layer/normalization.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/layer/parallel_module.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/parallel_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/layer/qkv_fused_linear.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/qkv_fused_linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/layer/utils.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/modeling/bloom.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/policies/autopolicy.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/autopolicy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/policies/basepolicy.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/basepolicy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/policies/bert.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/policies/bloom.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/policies/gpt2.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/policies/llama.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/policies/opt.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/policies/t5.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/policies/vit.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/vit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/shard/shard_config.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/shard/shard_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/shard/sharder.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/shard/sharder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/shardformer/shard/shardformer.py` & `colossalai-nightly-2023.7.8/colossalai/shardformer/shard/shardformer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/colo_parameter.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/colo_parameter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/colo_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/colo_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/comm_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/compute_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/compute_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/api.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/api.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/comm_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/layout.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/layout_converter.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout_converter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/sharding_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/d_tensor/utils.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/dist_spec_mgr.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/dist_spec_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/distspec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/distspec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/op_wrapper.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/op_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/param_op_hook.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/param_op_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/process_group.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/shape_consistency.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/shape_consistency.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/sharding_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/tensor_spec.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/tensor_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/tensor/utils.py` & `colossalai-nightly-2023.7.8/colossalai/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/testing/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/testing/comparison.py` & `colossalai-nightly-2023.7.8/colossalai/testing/comparison.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/testing/pytest_wrapper.py` & `colossalai-nightly-2023.7.8/colossalai/testing/pytest_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/testing/random.py` & `colossalai-nightly-2023.7.8/colossalai/testing/random.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/testing/utils.py` & `colossalai-nightly-2023.7.8/colossalai/testing/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/trainer/_trainer.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/_trainer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/trainer/hooks/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_base_hook.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_base_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_checkpoint_hook.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_log_hook.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_log_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_lr_scheduler_hook.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/trainer/hooks/_metric_hook.py` & `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_metric_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/activation_checkpoint.py` & `colossalai-nightly-2023.7.8/colossalai/utils/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpoint/module_checkpoint.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/module_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpoint/utils.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/backend.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/backend.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/convertor.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/convertor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/distributed.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/distributed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/io.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/io.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/meta.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/reader.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/reader.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/utils.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpoint_io/writer.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/writer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/checkpointing.py` & `colossalai-nightly-2023.7.8/colossalai/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/common.py` & `colossalai-nightly-2023.7.8/colossalai/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/cuda.py` & `colossalai-nightly-2023.7.8/colossalai/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/data_sampler/data_parallel_sampler.py` & `colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/data_parallel_sampler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/memory.py` & `colossalai-nightly-2023.7.8/colossalai/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/model/utils.py` & `colossalai-nightly-2023.7.8/colossalai/utils/model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/moe.py` & `colossalai-nightly-2023.7.8/colossalai/utils/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py` & `colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/profiler/legacy/comm_profiler.py` & `colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/comm_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/profiler/legacy/pcie_profiler.py` & `colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/pcie_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/profiler/legacy/prof_utils.py` & `colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/prof_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/profiler/profiler.py` & `colossalai-nightly-2023.7.8/colossalai/utils/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/profiler/stateful_tensor_mem_extention.py` & `colossalai-nightly-2023.7.8/colossalai/utils/profiler/stateful_tensor_mem_extention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/rank_recorder/rank_recorder.py` & `colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/rank_recorder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/tensor_detector/tensor_detector.py` & `colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/tensor_detector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/utils/timer.py` & `colossalai-nightly-2023.7.8/colossalai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/zero/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/chunk/chunk.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/chunk.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/chunk/manager.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/chunk/search_utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/search_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/chunk/utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/colo_init_context.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/colo_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/gemini_ddp.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/gemini_hook.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/gemini_mgr.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/gemini_optimizer.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/memory_monitor.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/memory_stats.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_stats.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/memstats_collector.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/param_runtime_order.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/param_runtime_order.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/memory_tracer/utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/placement_policy.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/gemini/utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/gemini/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/__init__.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/gemini_context.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/gemini_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/ophooks/utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/stateful_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/tensor_placement_policy.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/gemini/tensor_utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/init_ctx/init_context.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/shard_utils/base_shard_strategy.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/base_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/shard_utils/commons.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/commons.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/reduce_scatter.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/sharded_model_v2.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/sharded_model_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_model/zero_hook.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/zero_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_param/sharded_param.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_param.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/legacy/sharded_param/sharded_tensor.py` & `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/low_level/_utils.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/bucket_store.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/bucket_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/gradient_store.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/gradient_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/parameter_store.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/parameter_store.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/low_level/bookkeeping/tensor_bucket.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/tensor_bucket.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/low_level/low_level_optim.py` & `colossalai-nightly-2023.7.8/colossalai/zero/low_level/low_level_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai/zero/wrapper.py` & `colossalai-nightly-2023.7.8/colossalai/zero/wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/colossalai_nightly.egg-info/PKG-INFO` & `colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.7.15
+Version: 2023.7.8
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.7.15 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.7.8 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
```

### Comparing `colossalai-nightly-2023.7.15/colossalai_nightly.egg-info/SOURCES.txt` & `colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/op_builder/__init__.py` & `colossalai-nightly-2023.7.8/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/op_builder/builder.py` & `colossalai-nightly-2023.7.8/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/op_builder/cpu_adam.py` & `colossalai-nightly-2023.7.8/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/op_builder/fused_optim.py` & `colossalai-nightly-2023.7.8/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/op_builder/layernorm.py` & `colossalai-nightly-2023.7.8/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/op_builder/moe.py` & `colossalai-nightly-2023.7.8/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.7.8/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.7.8/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.7.8/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/op_builder/utils.py` & `colossalai-nightly-2023.7.8/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/requirements/requirements-test.txt` & `colossalai-nightly-2023.7.8/requirements/requirements-test.txt`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/setup.py` & `colossalai-nightly-2023.7.8/setup.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/albert.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/beit.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/beit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/bert.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/gpt2.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/hanging_param_model.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/hanging_param_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/inline_op_model.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/inline_op_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/nested_model.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/nested_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/registry.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/repeated_computed_layers.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/repeated_computed_layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/resnet.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/resnet.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/simple_net.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/simple_net.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/components_to_test/utils/executor.py` & `colossalai-nightly-2023.7.8/tests/components_to_test/utils/executor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/diffusers/diffusers.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/diffusers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/registry.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/timm/timm.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/timm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchaudio/torchaudio.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/torchaudio.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchrec/torchrec.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/torchrec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/torchvision/torchvision.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/torchvision.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/albert.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/bert.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/bloom.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/gpt.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/gpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/llama.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/opt.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/kit/model_zoo/transformers/t5.py` & `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/test_bias_addition.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/test_mod_dir.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_mod_dir.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/test_nested_ckpt.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_nested_ckpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/test_shape_prop.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/test_symbolic_profile.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_analyzer/test_fx/zoo.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/zoo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_analyzer/test_subclasses/test_aten.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_aten.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_analyzer/test_subclasses/test_flop_tensor.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_analyzer/test_subclasses/test_meta_mode.py` & `colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_meta_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_pass/test_node_converting_pass.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_node_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py` & `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/_utils.py` & `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_bert.py` & `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_bloom.py` & `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_gpt2.py` & `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_llama.py` & `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_opt.py` & `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_t5.py` & `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_shardformer/test_model/test_shard_vit.py` & `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_vit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.15/tests/test_shardformer/test_with_torch_ddp.py` & `colossalai-nightly-2023.7.8/tests/test_shardformer/test_with_torch_ddp.py`

 * *Files identical despite different names*

