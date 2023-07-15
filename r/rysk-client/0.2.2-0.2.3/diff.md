# Comparing `tmp/rysk_client-0.2.2.tar.gz` & `tmp/rysk_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rysk_client-0.2.2.tar", max compression
+gzip compressed data, was "rysk_client-0.2.3.tar", max compression
```

## Comparing `rysk_client-0.2.2.tar` & `rysk_client-0.2.3.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    45006 2023-07-15 13:02:33.149161 rysk_client-0.2.2/README.md
--rw-r--r--   0        0        0      709 2023-07-15 13:02:33.153161 rysk_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/__init__.py
--rw-r--r--   0        0        0     9030 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/cli.py
--rw-r--r--   0        0        0    25070 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/client.py
--rw-r--r--   0        0        0      974 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py
--rw-r--r--   0        0        0    35992 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json
--rw-r--r--   0        0        0    13187 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py
--rw-r--r--   0        0        0      527 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml
--rw-r--r--   0        0        0      971 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py
--rw-r--r--   0        0        0    35311 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json
--rw-r--r--   0        0        0     6580 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py
--rw-r--r--   0        0        0      601 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml
--rw-r--r--   0        0        0      968 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/__init__.py
--rw-r--r--   0        0        0    15813 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json
--rw-r--r--   0        0        0     8845 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/contract.py
--rw-r--r--   0        0        0      509 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/contract.yaml
--rw-r--r--   0        0        0      976 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py
--rw-r--r--   0        0        0    38053 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json
--rw-r--r--   0        0        0    11285 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/contract.py
--rw-r--r--   0        0        0      533 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml
--rw-r--r--   0        0        0      976 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py
--rw-r--r--   0        0        0    42143 2023-07-15 13:02:33.153161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json
--rw-r--r--   0        0        0    13308 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py
--rw-r--r--   0        0        0      533 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml
--rw-r--r--   0        0        0      981 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py
--rw-r--r--   0        0        0    38232 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json
--rw-r--r--   0        0        0    10787 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py
--rw-r--r--   0        0        0      547 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml
--rw-r--r--   0        0        0      965 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/__init__.py
--rw-r--r--   0        0        0    11137 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json
--rw-r--r--   0        0        0     6104 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/contract.py
--rw-r--r--   0        0        0      580 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/contract.yaml
--rw-r--r--   0        0        0      979 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py
--rw-r--r--   0        0        0     2515 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json
--rw-r--r--   0        0        0     4220 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py
--rw-r--r--   0        0        0      541 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml
--rw-r--r--   0        0        0      965 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/__init__.py
--rw-r--r--   0        0        0    15880 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/build/weth.json
--rw-r--r--   0        0        0     6490 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/contract.py
--rw-r--r--   0        0        0      580 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/contract.yaml
--rw-r--r--   0        0        0      488 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/packages/packages.json
--rw-r--r--   0        0        0      690 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/action_type.py
--rw-r--r--   0        0        0      856 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/collateral.py
--rw-r--r--   0        0        0     4875 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/constants.py
--rw-r--r--   0        0        0      212 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/crypto.py
--rw-r--r--   0        0        0      185 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/exceptions.py
--rw-r--r--   0        0        0     8518 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/operation_factory.py
--rw-r--r--   0        0        0      507 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/order.py
--rw-r--r--   0        0        0      182 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/order_side.py
--rw-r--r--   0        0        0     4538 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/pnl_calculator.py
--rw-r--r--   0        0        0      592 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/position.py
--rw-r--r--   0        0        0     1114 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/position_manager.py
--rw-r--r--   0        0        0      193 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/position_side.py
--rw-r--r--   0        0        0     7830 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/rysk_option_market.py
--rw-r--r--   0        0        0     3282 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/subgraph.py
--rw-r--r--   0        0        0     2341 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/src/utils.py
--rw-r--r--   0        0        0    15436 2023-07-15 13:02:33.157161 rysk_client-0.2.2/rysk_client/web3_client.py
--rw-r--r--   0        0        0    45592 1970-01-01 00:00:00.000000 rysk_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    45006 2023-07-15 14:32:08.878401 rysk_client-0.2.3/README.md
+-rw-r--r--   0        0        0      709 2023-07-15 14:32:08.882401 rysk_client-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/__init__.py
+-rw-r--r--   0        0        0     9030 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/cli.py
+-rw-r--r--   0        0        0    25164 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/client.py
+-rw-r--r--   0        0        0      974 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py
+-rw-r--r--   0        0        0    35992 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json
+-rw-r--r--   0        0        0    13187 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py
+-rw-r--r--   0        0        0      527 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml
+-rw-r--r--   0        0        0      971 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py
+-rw-r--r--   0        0        0    35311 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json
+-rw-r--r--   0        0        0     6580 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py
+-rw-r--r--   0        0        0      601 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml
+-rw-r--r--   0        0        0      968 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/o_token/__init__.py
+-rw-r--r--   0        0        0    15813 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json
+-rw-r--r--   0        0        0     8845 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/o_token/contract.py
+-rw-r--r--   0        0        0      509 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/o_token/contract.yaml
+-rw-r--r--   0        0        0      976 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py
+-rw-r--r--   0        0        0    38053 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json
+-rw-r--r--   0        0        0    11285 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/option_exchange/contract.py
+-rw-r--r--   0        0        0      533 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml
+-rw-r--r--   0        0        0      976 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py
+-rw-r--r--   0        0        0    42143 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json
+-rw-r--r--   0        0        0    13308 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py
+-rw-r--r--   0        0        0      533 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml
+-rw-r--r--   0        0        0      981 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py
+-rw-r--r--   0        0        0    38232 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json
+-rw-r--r--   0        0        0    10787 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py
+-rw-r--r--   0        0        0      547 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml
+-rw-r--r--   0        0        0      965 2023-07-15 14:32:08.882401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/usdc/__init__.py
+-rw-r--r--   0        0        0    11137 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json
+-rw-r--r--   0        0        0     6104 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/usdc/contract.py
+-rw-r--r--   0        0        0      580 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/usdc/contract.yaml
+-rw-r--r--   0        0        0      979 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py
+-rw-r--r--   0        0        0     2515 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json
+-rw-r--r--   0        0        0     4220 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py
+-rw-r--r--   0        0        0      541 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml
+-rw-r--r--   0        0        0      965 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/weth/__init__.py
+-rw-r--r--   0        0        0    15880 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/weth/build/weth.json
+-rw-r--r--   0        0        0     6490 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/weth/contract.py
+-rw-r--r--   0        0        0      580 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/weth/contract.yaml
+-rw-r--r--   0        0        0      488 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/packages/packages.json
+-rw-r--r--   0        0        0      690 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/action_type.py
+-rw-r--r--   0        0        0      856 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/collateral.py
+-rw-r--r--   0        0        0     5265 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/constants.py
+-rw-r--r--   0        0        0      212 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/crypto.py
+-rw-r--r--   0        0        0      185 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/exceptions.py
+-rw-r--r--   0        0        0     8518 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/operation_factory.py
+-rw-r--r--   0        0        0      507 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/order.py
+-rw-r--r--   0        0        0      182 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/order_side.py
+-rw-r--r--   0        0        0     4538 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/pnl_calculator.py
+-rw-r--r--   0        0        0      592 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/position.py
+-rw-r--r--   0        0        0     1114 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/position_manager.py
+-rw-r--r--   0        0        0      193 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/position_side.py
+-rw-r--r--   0        0        0     7830 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/rysk_option_market.py
+-rw-r--r--   0        0        0     3253 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/subgraph.py
+-rw-r--r--   0        0        0     2341 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/src/utils.py
+-rw-r--r--   0        0        0    15436 2023-07-15 14:32:08.886401 rysk_client-0.2.3/rysk_client/web3_client.py
+-rw-r--r--   0        0        0    45592 1970-01-01 00:00:00.000000 rysk_client-0.2.3/PKG-INFO
```

### Comparing `rysk_client-0.2.2/README.md` & `rysk_client-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/pyproject.toml` & `rysk_client-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rysk_client"
-version = "0.2.2"
+version = "0.2.3"
 description = ""
 authors = ["8baller <8ball030@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "rysk_client", from = "." },
 ]
```

### Comparing `rysk_client-0.2.2/rysk_client/cli.py` & `rysk_client-0.2.3/rysk_client/cli.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/client.py` & `rysk_client-0.2.3/rysk_client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from dataclasses import dataclass
 from datetime import datetime
 from typing import Any, Dict, List, Optional
 
 import web3
 
 from rysk_client.src.collateral import Collateral
-from rysk_client.src.constants import ARBITRUM_GOERLI, Chain
+from rysk_client.src.constants import (ARBITRUM_GOERLI, CHAINS_TO_SUBGRAPH_URL,
+                                       Chain)
 from rysk_client.src.crypto import EthCrypto
 from rysk_client.src.operation_factory import buy, sell
 from rysk_client.src.order_side import OrderSide
 from rysk_client.src.pnl_calculator import PnlCalculator, Trade
 from rysk_client.src.position_side import PositionSide
 from rysk_client.src.rysk_option_market import OptionChain, RyskOptionMarket
 from rysk_client.src.subgraph import SubgraphClient
@@ -103,15 +104,15 @@
         self._logger = logger or get_logger()
         self.web3_client = Web3Client(
             self._logger,
             self._crypto,
             chain=chain,
             verbose=verbose,
         )
-        self.subgraph_client = SubgraphClient()
+        self.subgraph_client = SubgraphClient(CHAINS_TO_SUBGRAPH_URL[chain])
         self._logger.info(
             f"Rysk client initialized and connected to the blockchain at {self.web3_client.web3.provider}"
         )
         self._verbose = verbose
 
     def _sign_and_sumbit(self, txn, retries=3, backoff=2):
         """
```

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/__init__.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/o_token/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/o_token/contract.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/o_token/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/contract.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/option_exchange/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/__init__.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/usdc/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/contract.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/usdc/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/usdc/contract.yaml` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/usdc/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/__init__.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/weth/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/build/weth.json` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/weth/build/weth.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/contract.py` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/weth/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/packages/eightballer/contracts/weth/contract.yaml` & `rysk_client-0.2.3/rysk_client/packages/eightballer/contracts/weth/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/src/action_type.py` & `rysk_client-0.2.3/rysk_client/src/action_type.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/src/collateral.py` & `rysk_client-0.2.3/rysk_client/src/collateral.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/src/constants.py` & `rysk_client-0.2.3/rysk_client/src/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 """
 This file contains all the constants used in the rysk_client package.
 """
 import os
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Dict
+from typing import Dict, Optional
 
 
 def from_camel_case_to_snake_case(string: str):
     """
     Convert a string from camel case to snake case.
     Note: If the string is all uppercase, it will be converted to lowercase.
     """
     if string.isupper():
         return string.lower()
     return "".join("_" + c.lower() if c.isupper() else c for c in string).lstrip("_")
 
 
 DEFAULT_TIMEOUT = 10
 DEFAULT_ENCODING = "utf-8"
-SUBGRAPH_URL = "https://api.studio.thegraph.com/query/45686/rysk/version/latest"
 NULL_ADDRESS = "0x0000000000000000000000000000000000000000"
 NULL_DATA = "0x0000000000000000000000000000000000000000"
 SUPPORTED_LEVERAGES = [1, 1.5, 2, 3]
 
 CONTRACT_ADDRESSES = {
     "arbitrum": {
         "OpynController": "0x594bD4eC29F7900AE29549c140Ac53b5240d4019",
@@ -75,22 +74,27 @@
     """Chain dataclass."""
 
     name: str
     chain_id: int
     rpc_url: str
     wss_url: str
 
+    def __hash__(self) -> int:
+        """Hash the chain."""
+        return hash(self.chain_id)
+
 
 @dataclass
 class ProtocolDeployment:
     """Protocol deployment dataclass."""
 
     name: str
     contracts: Dict[str, Contract]
     chain: Chain
+    subgraph_url: Optional[str] = None
 
 
 WS_URL = "wss://quaint-billowing-morning.arbitrum-goerli.discover.quiknode.pro/def6c4c783fc626cb8a07d38f845b76b458e6e84"
 ARBITRUM = Chain(
     name="arbitrum",
     chain_id=42161,
     rpc_url="https://arbitrum.public-rpc.com",
@@ -110,14 +114,20 @@
     wss_url="ws://localhost:8545",
 )
 
 
 PROTOCOL_DEPLOYMENTS = {}
 SUPPORTED_CHAINS = [ARBITRUM, ARBITRUM_GOERLI]
 
+
+CHAINS_TO_SUBGRAPH_URL = {
+    ARBITRUM: "https://api.goldsky.com/api/public/project_clhf7zaco0n9j490ce421agn4/subgraphs/arbitrum-one/0.1.17/gn",
+    ARBITRUM_GOERLI: "https://api.goldsky.com/api/public/project_clhf7zaco0n9j490ce421agn4/subgraphs/devey/0.1.17/gn",
+}
+
 for chain in SUPPORTED_CHAINS:
     for name, address in CONTRACT_ADDRESSES[chain.name].items():
         PROTOCOL_DEPLOYMENTS[chain.name] = ProtocolDeployment(
             name=name,
             contracts={
                 from_camel_case_to_snake_case(name): Contract(
                     path=Path(os.path.dirname(__file__))
@@ -129,13 +139,14 @@
                     / "build"
                     / f"{from_camel_case_to_snake_case(name)}.json",
                     address=address,
                 )
                 for name, address in CONTRACT_ADDRESSES[chain.name].items()
             },
             chain=chain,
+            subgraph_url=CHAINS_TO_SUBGRAPH_URL[chain],
         )
 
 
 CHAIN_ID_TO_DEPLOYMENT = {
     deploy.chain.chain_id: deploy for deploy in PROTOCOL_DEPLOYMENTS.values()
 }
```

### Comparing `rysk_client-0.2.2/rysk_client/src/operation_factory.py` & `rysk_client-0.2.3/rysk_client/src/operation_factory.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/src/pnl_calculator.py` & `rysk_client-0.2.3/rysk_client/src/pnl_calculator.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/src/position.py` & `rysk_client-0.2.3/rysk_client/src/position.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/src/position_manager.py` & `rysk_client-0.2.3/rysk_client/src/position_manager.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/src/rysk_option_market.py` & `rysk_client-0.2.3/rysk_client/src/rysk_option_market.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/src/subgraph.py` & `rysk_client-0.2.3/rysk_client/src/subgraph.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import json
 from dataclasses import dataclass
 from typing import Any, Dict, List
 
 import requests
 
-from rysk_client.src.constants import DEFAULT_TIMEOUT, SUBGRAPH_URL
+from rysk_client.src.constants import DEFAULT_TIMEOUT
 
 MARKET_SUBGRAPH_QUERY = """
 {series (
   where: {
     or:[
     {
             isBuyable: true
@@ -117,15 +117,15 @@
 """
 
 
 @dataclass
 class SubgraphClient:
     """Simple client to interact with the Rysk subgraph."""
 
-    url: str = SUBGRAPH_URL
+    url: str
 
     def _query(self, query):
         """Simple function to call a subgraph query."""
         headers = {"Content-Type": "application/json"}
         subgraph_query = {"query": query}
         response = requests.post(
             url=self.url,
```

### Comparing `rysk_client-0.2.2/rysk_client/src/utils.py` & `rysk_client-0.2.3/rysk_client/src/utils.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/rysk_client/web3_client.py` & `rysk_client-0.2.3/rysk_client/web3_client.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.2/PKG-INFO` & `rysk_client-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rysk-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: 
 Author: 8baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

