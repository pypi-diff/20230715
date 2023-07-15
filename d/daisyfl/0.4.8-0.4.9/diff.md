# Comparing `tmp/daisyfl-0.4.8.tar.gz` & `tmp/daisyfl-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "daisyfl-0.4.8.tar", max compression
+gzip compressed data, was "daisyfl-0.4.9.tar", max compression
```

## Comparing `daisyfl-0.4.8.tar` & `daisyfl-0.4.9.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    11358 2023-07-14 13:27:28.582708 daisyfl-0.4.8/LICENSE
--rw-r--r--   0        0        0     1158 2023-07-14 13:27:28.582708 daisyfl-0.4.8/README.md
--rw-r--r--   0        0        0     3661 2023-07-14 13:27:55.562673 daisyfl-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     1093 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/__init__.py
--rw-r--r--   0        0        0     1171 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/__init__.py
--rw-r--r--   0        0        0     9951 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/app.py
--rw-r--r--   0        0        0     3733 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/client.py
--rw-r--r--   0        0        0     1363 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/client_api_handler.py
--rw-r--r--   0        0        0     3780 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/client_operator_manager.py
--rw-r--r--   0        0        0     3367 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/dpfedavg_numpy_client.py
--rw-r--r--   0        0        0      714 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/__init__.py
--rw-r--r--   0        0        0    10038 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/connection.py
--rw-r--r--   0        0        0     6704 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/message_handler.py
--rw-r--r--   0        0        0     5084 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/numpy_client.py
--rw-r--r--   0        0        0     4998 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/trainer.py
--rw-r--r--   0        0        0     1663 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/client/zone_client.py
--rw-r--r--   0        0        0     5644 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/common/__init__.py
--rw-r--r--   0        0        0     1830 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/common/dp.py
--rw-r--r--   0        0        0     3482 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/common/logger.py
--rw-r--r--   0        0        0     1421 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/common/metadata.py
--rw-r--r--   0        0        0     3938 2023-07-14 13:27:28.582708 daisyfl-0.4.8/src/py/daisyfl/common/parameter.py
--rw-r--r--   0        0        0    16903 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/common/serde.py
--rw-r--r--   0        0        0     4044 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/common/typing.py
--rw-r--r--   0        0        0        0 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/__init__.py
--rw-r--r--   0        0        0        0 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base/__init__.py
--rw-r--r--   0        0        0     1162 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base/client_logic.py
--rw-r--r--   0        0        0     5700 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base/server_logic.py
--rw-r--r--   0        0        0        0 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base_async/__init__.py
--rw-r--r--   0        0        0     1162 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base_async/client_logic.py
--rw-r--r--   0        0        0     5383 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/base_async/server_logic.py
--rw-r--r--   0        0        0     1987 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/client_logic.py
--rw-r--r--   0        0        0      381 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/msg.py
--rw-r--r--   0        0        0     5483 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/server_logic.py
--rw-r--r--   0        0        0      961 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
--rw-r--r--   0        0        0     5848 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
--rw-r--r--   0        0        0    12137 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/client_logic.py
--rw-r--r--   0        0        0     1755 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/common.py
--rw-r--r--   0        0        0    10070 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/primitives.py
--rw-r--r--   0        0        0    22268 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/server_logic.py
--rw-r--r--   0        0        0     1456 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/__init__.py
--rw-r--r--   0        0        0     3016 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/aggregate.py
--rw-r--r--   0        0        0     4538 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
--rw-r--r--   0        0        0     5095 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
--rw-r--r--   0        0        0     6134 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
--rw-r--r--   0        0        0     6993 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedadagrad.py
--rw-r--r--   0        0        0     7245 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedadam.py
--rw-r--r--   0        0        0    13054 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedasync.py
--rw-r--r--   0        0        0    12396 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavg.py
--rw-r--r--   0        0        0    10915 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavg_android.py
--rw-r--r--   0        0        0     9115 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavgm.py
--rw-r--r--   0        0        0     5513 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedopt.py
--rw-r--r--   0        0        0     7263 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedyogi.py
--rw-r--r--   0        0        0    10952 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/qfedavg.py
--rw-r--r--   0        0        0     7867 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/strategy/strategy.py
--rw-r--r--   0        0        0      826 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/utils/__init__.py
--rw-r--r--   0        0        0     6979 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/operator/utils/op_tools.py
--rw-r--r--   0        0        0      676 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/proto/__init__.py
--rw-r--r--   0        0        0    70900 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2.py
--rw-r--r--   0        0        0    25816 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2.pyi
--rw-r--r--   0        0        0     2631 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2_grpc.py
--rw-r--r--   0        0        0      781 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2_grpc.pyi
--rw-r--r--   0        0        0     1064 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/__init__.py
--rw-r--r--   0        0        0     5085 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/app.py
--rw-r--r--   0        0        0     7809 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/client_manager.py
--rw-r--r--   0        0        0     2371 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/client_proxy.py
--rw-r--r--   0        0        0      714 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/__init__.py
--rw-r--r--   0        0        0    12768 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
--rw-r--r--   0        0        0     6827 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_bridge.py
--rw-r--r--   0        0        0     4459 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
--rw-r--r--   0        0        0    11290 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_server.py
--rw-r--r--   0        0        0     3626 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/history.py
--rw-r--r--   0        0        0    11871 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/server.py
--rw-r--r--   0        0        0     7341 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/server_api_handler.py
--rw-r--r--   0        0        0     4560 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/server_operator_manager.py
--rw-r--r--   0        0        0    13696 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/server/task_manager.py
--rw-r--r--   0        0        0     1273 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/simulation/__init__.py
--rw-r--r--   0        0        0     7335 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/simulation/app.py
--rw-r--r--   0        0        0      727 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/simulation/ray_transport/__init__.py
--rw-r--r--   0        0        0     4661 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
--rw-r--r--   0        0        0      859 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/utils/__init__.py
--rw-r--r--   0        0        0      121 2023-07-14 13:27:28.586708 daisyfl-0.4.8/src/py/daisyfl/utils/dynamic_loader.py
--rw-r--r--   0        0        0     2765 2023-07-14 13:28:14.933335 daisyfl-0.4.8/setup.py
--rw-r--r--   0        0        0     3286 2023-07-14 13:28:14.933610 daisyfl-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-07-15 03:42:40.119775 daisyfl-0.4.9/LICENSE
+-rw-r--r--   0        0        0     1158 2023-07-15 03:42:40.119775 daisyfl-0.4.9/README.md
+-rw-r--r--   0        0        0     3661 2023-07-15 03:43:16.103695 daisyfl-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1093 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/__init__.py
+-rw-r--r--   0        0        0     1171 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/__init__.py
+-rw-r--r--   0        0        0     9951 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/app.py
+-rw-r--r--   0        0        0     3733 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/client.py
+-rw-r--r--   0        0        0     1363 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/client_api_handler.py
+-rw-r--r--   0        0        0     3780 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/client_operator_manager.py
+-rw-r--r--   0        0        0     3367 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/dpfedavg_numpy_client.py
+-rw-r--r--   0        0        0      714 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/grpc_client/__init__.py
+-rw-r--r--   0        0        0    10038 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/grpc_client/connection.py
+-rw-r--r--   0        0        0     6704 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/grpc_client/message_handler.py
+-rw-r--r--   0        0        0     5084 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/numpy_client.py
+-rw-r--r--   0        0        0     4998 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/trainer.py
+-rw-r--r--   0        0        0     1663 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/client/zone_client.py
+-rw-r--r--   0        0        0     5644 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/common/__init__.py
+-rw-r--r--   0        0        0     1830 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/common/dp.py
+-rw-r--r--   0        0        0     3482 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/common/logger.py
+-rw-r--r--   0        0        0     1421 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/common/metadata.py
+-rw-r--r--   0        0        0     3938 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/common/parameter.py
+-rw-r--r--   0        0        0    16903 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/common/serde.py
+-rw-r--r--   0        0        0     4044 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/common/typing.py
+-rw-r--r--   0        0        0        0 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/base/__init__.py
+-rw-r--r--   0        0        0     1162 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/base/client_logic.py
+-rw-r--r--   0        0        0     5700 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/base/server_logic.py
+-rw-r--r--   0        0        0        0 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/base_async/__init__.py
+-rw-r--r--   0        0        0     1162 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/base_async/client_logic.py
+-rw-r--r--   0        0        0     5383 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/base_async/server_logic.py
+-rw-r--r--   0        0        0     1987 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/msg_demo/client_logic.py
+-rw-r--r--   0        0        0      381 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/msg_demo/msg.py
+-rw-r--r--   0        0        0     5483 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/msg_demo/server_logic.py
+-rw-r--r--   0        0        0      961 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/msg_demo/zone_client_logic.py
+-rw-r--r--   0        0        0     5848 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/msg_demo/zone_server_logic.py
+-rw-r--r--   0        0        0    12137 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/sec_agg/client_logic.py
+-rw-r--r--   0        0        0     1755 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/sec_agg/common.py
+-rw-r--r--   0        0        0    10070 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/sec_agg/primitives.py
+-rw-r--r--   0        0        0    22268 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/sec_agg/server_logic.py
+-rw-r--r--   0        0        0     1456 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/__init__.py
+-rw-r--r--   0        0        0     3016 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/aggregate.py
+-rw-r--r--   0        0        0     4538 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py
+-rw-r--r--   0        0        0     5095 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py
+-rw-r--r--   0        0        0     6134 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py
+-rw-r--r--   0        0        0     6993 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedadagrad.py
+-rw-r--r--   0        0        0     7245 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedadam.py
+-rw-r--r--   0        0        0    13054 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedasync.py
+-rw-r--r--   0        0        0    12396 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedavg.py
+-rw-r--r--   0        0        0    10915 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedavg_android.py
+-rw-r--r--   0        0        0     9115 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedavgm.py
+-rw-r--r--   0        0        0     5513 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedopt.py
+-rw-r--r--   0        0        0     7263 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedyogi.py
+-rw-r--r--   0        0        0    10952 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/qfedavg.py
+-rw-r--r--   0        0        0     7867 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/strategy/strategy.py
+-rw-r--r--   0        0        0      826 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/utils/__init__.py
+-rw-r--r--   0        0        0     6979 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/operator/utils/op_tools.py
+-rw-r--r--   0        0        0      676 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/proto/__init__.py
+-rw-r--r--   0        0        0    70900 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/proto/transport_pb2.py
+-rw-r--r--   0        0        0    25816 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/proto/transport_pb2.pyi
+-rw-r--r--   0        0        0     2631 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/proto/transport_pb2_grpc.py
+-rw-r--r--   0        0        0      781 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/proto/transport_pb2_grpc.pyi
+-rw-r--r--   0        0        0     1064 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/__init__.py
+-rw-r--r--   0        0        0     5085 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/app.py
+-rw-r--r--   0        0        0     7809 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/client_manager.py
+-rw-r--r--   0        0        0     2371 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/client_proxy.py
+-rw-r--r--   0        0        0      714 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/grpc_server/__init__.py
+-rw-r--r--   0        0        0    12768 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/grpc_server/flower_service_servicer.py
+-rw-r--r--   0        0        0     6827 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/grpc_server/grpc_bridge.py
+-rw-r--r--   0        0        0     4459 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py
+-rw-r--r--   0        0        0    11290 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/grpc_server/grpc_server.py
+-rw-r--r--   0        0        0     3626 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/history.py
+-rw-r--r--   0        0        0    11871 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/server.py
+-rw-r--r--   0        0        0     8184 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/server_api_handler.py
+-rw-r--r--   0        0        0     4560 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/server_operator_manager.py
+-rw-r--r--   0        0        0    13696 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/server/task_manager.py
+-rw-r--r--   0        0        0     1273 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/simulation/__init__.py
+-rw-r--r--   0        0        0     7335 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/simulation/app.py
+-rw-r--r--   0        0        0      727 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/simulation/ray_transport/__init__.py
+-rw-r--r--   0        0        0     4661 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py
+-rw-r--r--   0        0        0      859 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/utils/__init__.py
+-rw-r--r--   0        0        0      121 2023-07-15 03:42:40.123775 daisyfl-0.4.9/src/py/daisyfl/utils/dynamic_loader.py
+-rw-r--r--   0        0        0     2765 2023-07-15 03:43:30.131020 daisyfl-0.4.9/setup.py
+-rw-r--r--   0        0        0     3286 2023-07-15 03:43:30.131226 daisyfl-0.4.9/PKG-INFO
```

### Comparing `daisyfl-0.4.8/LICENSE` & `daisyfl-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/README.md` & `daisyfl-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/pyproject.toml` & `daisyfl-0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "daisyfl"
-version = "0.4.8"
+version = "0.4.9"
 description = "Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing"
 license = "Apache-2.0"
 authors = ["tcfwbper <b05208031@ntu.edu.tw>"]
 readme = "README.md"
 homepage = "https://github.com/Intelligent-Systems-Lab/daisy"
 repository = "https://github.com/Intelligent-Systems-Lab/daisy"
 documentation = "https://github.com/Intelligent-Systems-Lab/daisy/tree/main/doc/daisy"
```

### Comparing `daisyfl-0.4.8/src/py/daisyfl/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/app.py` & `daisyfl-0.4.9/src/py/daisyfl/client/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/client.py` & `daisyfl-0.4.9/src/py/daisyfl/client/client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/client_api_handler.py` & `daisyfl-0.4.9/src/py/daisyfl/client/client_api_handler.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/client_operator_manager.py` & `daisyfl-0.4.9/src/py/daisyfl/client/client_operator_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/dpfedavg_numpy_client.py` & `daisyfl-0.4.9/src/py/daisyfl/client/dpfedavg_numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/client/grpc_client/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/connection.py` & `daisyfl-0.4.9/src/py/daisyfl/client/grpc_client/connection.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/grpc_client/message_handler.py` & `daisyfl-0.4.9/src/py/daisyfl/client/grpc_client/message_handler.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/numpy_client.py` & `daisyfl-0.4.9/src/py/daisyfl/client/numpy_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/trainer.py` & `daisyfl-0.4.9/src/py/daisyfl/client/trainer.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/client/zone_client.py` & `daisyfl-0.4.9/src/py/daisyfl/client/zone_client.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/common/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/common/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/common/dp.py` & `daisyfl-0.4.9/src/py/daisyfl/common/dp.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/common/logger.py` & `daisyfl-0.4.9/src/py/daisyfl/common/logger.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/common/metadata.py` & `daisyfl-0.4.9/src/py/daisyfl/common/metadata.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/common/parameter.py` & `daisyfl-0.4.9/src/py/daisyfl/common/parameter.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/common/serde.py` & `daisyfl-0.4.9/src/py/daisyfl/common/serde.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/common/typing.py` & `daisyfl-0.4.9/src/py/daisyfl/common/typing.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/base/client_logic.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/base/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/base/server_logic.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/base/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/base_async/client_logic.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/base_async/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/base_async/server_logic.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/base_async/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/client_logic.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/msg_demo/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/server_logic.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/msg_demo/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/zone_client_logic.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/msg_demo/zone_client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/msg_demo/zone_server_logic.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/msg_demo/zone_server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/client_logic.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/sec_agg/client_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/common.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/sec_agg/common.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/primitives.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/sec_agg/primitives.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/sec_agg/server_logic.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/sec_agg/server_logic.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/aggregate.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/aggregate.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/dpfedavg_adaptive.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/dpfedavg_fixed.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fault_tolerant_fedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedadagrad.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedadagrad.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedadam.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedadam.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedasync.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedasync.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavg.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavg_android.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedavg_android.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedavgm.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedavgm.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedopt.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedopt.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/fedyogi.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/fedyogi.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/qfedavg.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/qfedavg.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/strategy/strategy.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/strategy/strategy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/utils/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/operator/utils/op_tools.py` & `daisyfl-0.4.9/src/py/daisyfl/operator/utils/op_tools.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/proto/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/proto/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2.py` & `daisyfl-0.4.9/src/py/daisyfl/proto/transport_pb2.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2.pyi` & `daisyfl-0.4.9/src/py/daisyfl/proto/transport_pb2.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2_grpc.py` & `daisyfl-0.4.9/src/py/daisyfl/proto/transport_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/proto/transport_pb2_grpc.pyi` & `daisyfl-0.4.9/src/py/daisyfl/proto/transport_pb2_grpc.pyi`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/app.py` & `daisyfl-0.4.9/src/py/daisyfl/server/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/client_manager.py` & `daisyfl-0.4.9/src/py/daisyfl/server/client_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/client_proxy.py` & `daisyfl-0.4.9/src/py/daisyfl/server/client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/server/grpc_server/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/flower_service_servicer.py` & `daisyfl-0.4.9/src/py/daisyfl/server/grpc_server/flower_service_servicer.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_bridge.py` & `daisyfl-0.4.9/src/py/daisyfl/server/grpc_server/grpc_bridge.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py` & `daisyfl-0.4.9/src/py/daisyfl/server/grpc_server/grpc_client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/grpc_server/grpc_server.py` & `daisyfl-0.4.9/src/py/daisyfl/server/grpc_server/grpc_server.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/history.py` & `daisyfl-0.4.9/src/py/daisyfl/server/history.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/server.py` & `daisyfl-0.4.9/src/py/daisyfl/server/server.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/server_api_handler.py` & `daisyfl-0.4.9/src/py/daisyfl/server/server_api_handler.py`

 * *Files 14% similar despite different names*

```diff
@@ -67,14 +67,25 @@
                         )
                         res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
                             "loss_round", "x_axis_of_loss", "counter", labels, mt.history.losses_distributed[-1][0]
                         )
                         res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
                             "loss", "get_loss_of_the_task", "gauge", labels, mt.history.losses_distributed[-1][1]
                         )
+                    if mt.history.metrics_distributed.__contains__("mloss"):
+                        loss_list_global = mt.history.metrics_distributed["mloss"][-1][1] # [lbox, lobj, lcls]
+                        res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
+                            "loss_box_global", "global_loss_box", "gauge", labels, loss_list_global[0]
+                        )
+                        res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
+                            "loss_object_global", "global_loss_object", "gauge", labels, loss_list_global[1]
+                        )
+                        res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
+                            "loss_class_global", "global_loss_class", "gauge", labels, loss_list_global[2]
+                        )
                 # subtask_returns
                 if (mt.subtask_returns.__contains__(PARTICIPATION)):
                     res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
                         "subtask_round", "which_rounds_are_the_subtasks", "counter", labels, mt.subtask_returns[CURRENT_ROUND]
                     )
                     res += "# HELP {0} {1}\n# TYPE {0} {2}\n{0}{3} {4}\n".format(
                         "subtask_returns_selcted", "number_of_clients_which_are_selected", "gauge", labels, mt.subtask_returns[PARTICIPATION][SUBTASK_RETURNS_SELECTED]
```

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/server_operator_manager.py` & `daisyfl-0.4.9/src/py/daisyfl/server/server_operator_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/server/task_manager.py` & `daisyfl-0.4.9/src/py/daisyfl/server/task_manager.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/simulation/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/simulation/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/simulation/app.py` & `daisyfl-0.4.9/src/py/daisyfl/simulation/app.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/simulation/ray_transport/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/simulation/ray_transport/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py` & `daisyfl-0.4.9/src/py/daisyfl/simulation/ray_transport/ray_client_proxy.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/src/py/daisyfl/utils/__init__.py` & `daisyfl-0.4.9/src/py/daisyfl/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `daisyfl-0.4.8/setup.py` & `daisyfl-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 extras_require = \
 {':python_version < "3.8"': ['importlib-metadata>=4.0.0,<5.0.0'],
  'simulation': ['ray[default]>=2.0.0,<2.1.0']}
 
 setup_kwargs = {
     'name': 'daisyfl',
-    'version': '0.4.8',
+    'version': '0.4.9',
     'description': 'Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing',
     'long_description': "# Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing\n\n\n## dev mode (virtual environment)\n### 1. clone the source code\n```\ngit clone https://github.com/Intelligent-Systems-Lab/daisy\n```\n### 2. build up environment\nprepare and activate your virtual environment (python=3.8^)\n```\ncd daisy\n./dev/bootstrap.sh\n```\n### develop<br>\n### setup examples\ndon't overwrite daisyfl dependency in this step.<br>\n```\ncd <example_path>\npip install <pkgs_for_your_example>\n```\n### 5. run examples\n\n## dev mode (docker)\n### 1. clone the source code\n```\ngit clone https://github.com/Intelligent-Systems-Lab/daisy\n```\n### 2. build up environment\n```\ndocker run -it -v <daisy_source_code>:/root/daisy tcfwbper/daisyfl-dev:<version_tag> /bin/bash\n```\n### 3. develop<br>\n### 4. setup examples<br>\ndon't overwrite daisyfl dependency in this step.<br>\n```\ndocker attach <container_id>\n```\n```\ncd <example_path> && conda activate daisy\npip install <pkgs_for_your_example>\n```\n### 5. run examples\n\n## user mode\n### 1. install daisyfl\n```\npip install <daisyfl_version>\n```\n### 2. setup examples\n```\npip install <pkgs_for_your_example>\n```\n### 3. run examples",
     'author': 'tcfwbper',
     'author_email': 'b05208031@ntu.edu.tw',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/Intelligent-Systems-Lab/daisy',
```

### Comparing `daisyfl-0.4.8/PKG-INFO` & `daisyfl-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: daisyfl
-Version: 0.4.8
+Version: 0.4.9
 Summary: Daisy - A Hierarchical Friendly Federated Learning Framework For Edge Computing
 Home-page: https://github.com/Intelligent-Systems-Lab/daisy
 License: Apache-2.0
 Author: tcfwbper
 Author-email: b05208031@ntu.edu.tw
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

