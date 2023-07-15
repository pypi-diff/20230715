# Comparing `tmp/rysk_client-0.2.4.tar.gz` & `tmp/rysk_client-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rysk_client-0.2.4.tar", max compression
+gzip compressed data, was "rysk_client-0.2.5.tar", max compression
```

## Comparing `rysk_client-0.2.4.tar` & `rysk_client-0.2.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    45006 2023-07-15 16:27:09.260511 rysk_client-0.2.4/README.md
--rw-r--r--   0        0        0      709 2023-07-15 16:27:09.264511 rysk_client-0.2.4/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/__init__.py
--rw-r--r--   0        0        0     9030 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/cli.py
--rw-r--r--   0        0        0    25164 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/client.py
--rw-r--r--   0        0        0      974 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py
--rw-r--r--   0        0        0    35992 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json
--rw-r--r--   0        0        0    13187 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py
--rw-r--r--   0        0        0      527 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml
--rw-r--r--   0        0        0      971 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py
--rw-r--r--   0        0        0    35311 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json
--rw-r--r--   0        0        0     6580 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py
--rw-r--r--   0        0        0      601 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml
--rw-r--r--   0        0        0      968 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/o_token/__init__.py
--rw-r--r--   0        0        0    15813 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json
--rw-r--r--   0        0        0     8845 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/o_token/contract.py
--rw-r--r--   0        0        0      509 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/o_token/contract.yaml
--rw-r--r--   0        0        0      976 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py
--rw-r--r--   0        0        0    38053 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json
--rw-r--r--   0        0        0    11285 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/option_exchange/contract.py
--rw-r--r--   0        0        0      533 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml
--rw-r--r--   0        0        0      976 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py
--rw-r--r--   0        0        0    42143 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json
--rw-r--r--   0        0        0    13308 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py
--rw-r--r--   0        0        0      533 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml
--rw-r--r--   0        0        0      981 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py
--rw-r--r--   0        0        0    38232 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json
--rw-r--r--   0        0        0    10787 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py
--rw-r--r--   0        0        0      547 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml
--rw-r--r--   0        0        0      965 2023-07-15 16:27:09.264511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/usdc/__init__.py
--rw-r--r--   0        0        0    11137 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json
--rw-r--r--   0        0        0     6104 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/usdc/contract.py
--rw-r--r--   0        0        0      580 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/usdc/contract.yaml
--rw-r--r--   0        0        0      979 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py
--rw-r--r--   0        0        0     2515 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json
--rw-r--r--   0        0        0     4220 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py
--rw-r--r--   0        0        0      541 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml
--rw-r--r--   0        0        0      965 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/weth/__init__.py
--rw-r--r--   0        0        0    15880 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/weth/build/weth.json
--rw-r--r--   0        0        0     6490 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/weth/contract.py
--rw-r--r--   0        0        0      580 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/weth/contract.yaml
--rw-r--r--   0        0        0      488 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/packages/packages.json
--rw-r--r--   0        0        0      690 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/action_type.py
--rw-r--r--   0        0        0      856 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/collateral.py
--rw-r--r--   0        0        0     5265 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/constants.py
--rw-r--r--   0        0        0      212 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/crypto.py
--rw-r--r--   0        0        0      185 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/exceptions.py
--rw-r--r--   0        0        0     8518 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/operation_factory.py
--rw-r--r--   0        0        0      507 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/order.py
--rw-r--r--   0        0        0      182 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/order_side.py
--rw-r--r--   0        0        0     4538 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/pnl_calculator.py
--rw-r--r--   0        0        0      592 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/position.py
--rw-r--r--   0        0        0     1114 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/position_manager.py
--rw-r--r--   0        0        0      193 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/position_side.py
--rw-r--r--   0        0        0     7830 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/rysk_option_market.py
--rw-r--r--   0        0        0     3253 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/subgraph.py
--rw-r--r--   0        0        0     2341 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/src/utils.py
--rw-r--r--   0        0        0    15436 2023-07-15 16:27:09.268511 rysk_client-0.2.4/rysk_client/web3_client.py
--rw-r--r--   0        0        0    45592 1970-01-01 00:00:00.000000 rysk_client-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0    45006 2023-07-15 16:27:01.812334 rysk_client-0.2.5/README.md
+-rw-r--r--   0        0        0      709 2023-07-15 16:27:01.816335 rysk_client-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/__init__.py
+-rw-r--r--   0        0        0     9029 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/cli.py
+-rw-r--r--   0        0        0    25164 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/client.py
+-rw-r--r--   0        0        0      974 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py
+-rw-r--r--   0        0        0    35992 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json
+-rw-r--r--   0        0        0    13187 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py
+-rw-r--r--   0        0        0      527 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml
+-rw-r--r--   0        0        0      971 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py
+-rw-r--r--   0        0        0    35311 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json
+-rw-r--r--   0        0        0     6580 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py
+-rw-r--r--   0        0        0      601 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml
+-rw-r--r--   0        0        0      968 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/o_token/__init__.py
+-rw-r--r--   0        0        0    15813 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json
+-rw-r--r--   0        0        0     8845 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/o_token/contract.py
+-rw-r--r--   0        0        0      509 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/o_token/contract.yaml
+-rw-r--r--   0        0        0      976 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py
+-rw-r--r--   0        0        0    38053 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json
+-rw-r--r--   0        0        0    11285 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/option_exchange/contract.py
+-rw-r--r--   0        0        0      533 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml
+-rw-r--r--   0        0        0      976 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py
+-rw-r--r--   0        0        0    42143 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json
+-rw-r--r--   0        0        0    13308 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py
+-rw-r--r--   0        0        0      533 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml
+-rw-r--r--   0        0        0      981 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py
+-rw-r--r--   0        0        0    38232 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json
+-rw-r--r--   0        0        0    10787 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py
+-rw-r--r--   0        0        0      547 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml
+-rw-r--r--   0        0        0      965 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/usdc/__init__.py
+-rw-r--r--   0        0        0    11137 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json
+-rw-r--r--   0        0        0     6104 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/usdc/contract.py
+-rw-r--r--   0        0        0      580 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/usdc/contract.yaml
+-rw-r--r--   0        0        0      979 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py
+-rw-r--r--   0        0        0     2515 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json
+-rw-r--r--   0        0        0     4220 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py
+-rw-r--r--   0        0        0      541 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml
+-rw-r--r--   0        0        0      965 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/weth/__init__.py
+-rw-r--r--   0        0        0    15880 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/weth/build/weth.json
+-rw-r--r--   0        0        0     6490 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/weth/contract.py
+-rw-r--r--   0        0        0      580 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/weth/contract.yaml
+-rw-r--r--   0        0        0      488 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/packages/packages.json
+-rw-r--r--   0        0        0      690 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/action_type.py
+-rw-r--r--   0        0        0      856 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/collateral.py
+-rw-r--r--   0        0        0     5260 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/constants.py
+-rw-r--r--   0        0        0      212 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/crypto.py
+-rw-r--r--   0        0        0      185 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/exceptions.py
+-rw-r--r--   0        0        0     8518 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/operation_factory.py
+-rw-r--r--   0        0        0      507 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/order.py
+-rw-r--r--   0        0        0      182 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/order_side.py
+-rw-r--r--   0        0        0     4538 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/pnl_calculator.py
+-rw-r--r--   0        0        0      592 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/position.py
+-rw-r--r--   0        0        0     1114 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/position_manager.py
+-rw-r--r--   0        0        0      193 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/position_side.py
+-rw-r--r--   0        0        0     7830 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/rysk_option_market.py
+-rw-r--r--   0        0        0     3253 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/subgraph.py
+-rw-r--r--   0        0        0     2341 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/src/utils.py
+-rw-r--r--   0        0        0    15436 2023-07-15 16:27:01.816335 rysk_client-0.2.5/rysk_client/web3_client.py
+-rw-r--r--   0        0        0    45592 1970-01-01 00:00:00.000000 rysk_client-0.2.5/PKG-INFO
```

### Comparing `rysk_client-0.2.4/README.md` & `rysk_client-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/pyproject.toml` & `rysk_client-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rysk_client"
-version = "0.2.4"
+version = "0.2.5"
 description = ""
 authors = ["8baller <8ball030@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "rysk_client", from = "." },
 ]
```

### Comparing `rysk_client-0.2.4/rysk_client/cli.py` & `rysk_client-0.2.5/rysk_client/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     if not hasattr(ctx, "client"):
         auth = {
             "address": os.environ["ETH_ADDRESS"],
             "private_key": os.environ["ETH_PRIVATE_KEY"],
             "logger": ctx.logger,
         }
         ctx.client = RyskClient(**auth)
-        if not ctx.client.web3_client.web3.is_connected():
+        if not ctx.client.web3_client.web3.isConnected():
             raise ConnectionError("Web3 client not connected.")
     return ctx.client
 
 
 @click.group("Rysk client")
 @click.option(
     "--log-level",
```

### Comparing `rysk_client-0.2.4/rysk_client/client.py` & `rysk_client-0.2.5/rysk_client/client.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/beyond_pricer/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/beyond_pricer/build/beyond_pricer.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/beyond_pricer/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/d_h_v_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/d_h_v_lens/build/d_h_v_lens.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/d_h_v_lens/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/o_token/__init__.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/o_token/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/o_token/build/o_token.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/o_token/contract.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/o_token/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/option_exchange/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/option_exchange/build/option_exchange.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/option_exchange/contract.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/option_exchange/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/option_exchange/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_controller/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_controller/build/opyn_controller.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_controller/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_controller/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_option_registry/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_option_registry/build/opyn_option_registry.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/opyn_option_registry/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/usdc/__init__.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/usdc/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/usdc/build/usdc.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/usdc/contract.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/usdc/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/usdc/contract.yaml` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/usdc/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/user_position_lens/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/user_position_lens/build/user_position_lens.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/user_position_lens/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/user_position_lens/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/weth/__init__.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/weth/__init__.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/weth/build/weth.json` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/weth/build/weth.json`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/weth/contract.py` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/weth/contract.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/packages/eightballer/contracts/weth/contract.yaml` & `rysk_client-0.2.5/rysk_client/packages/eightballer/contracts/weth/contract.yaml`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/src/action_type.py` & `rysk_client-0.2.5/rysk_client/src/action_type.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/src/collateral.py` & `rysk_client-0.2.5/rysk_client/src/collateral.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/src/constants.py` & `rysk_client-0.2.5/rysk_client/src/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,16 +4,15 @@
 import os
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Dict, Optional
 
 
 def from_camel_case_to_snake_case(string: str):
-    """
-    Convert a string from camel case to snake case.
+    """Convert a string from camel case to snake case.
     Note: If the string is all uppercase, it will be converted to lowercase.
     """
     if string.isupper():
         return string.lower()
     return "".join("_" + c.lower() if c.isupper() else c for c in string).lstrip("_")
 
 
@@ -98,15 +97,15 @@
     name="arbitrum",
     chain_id=42161,
     rpc_url="https://arbitrum.public-rpc.com",
     wss_url="wss://arb1.arbitrum.io/ws",
 )
 ARBITRUM_GOERLI = Chain(
     name="arbitrum-goerli",
-    chain_id=421611,
+    chain_id=421613,
     rpc_url="https://arbitrum-goerli.rpc.thirdweb.com",
     wss_url=WS_URL,
 )
 
 LOCAL_FORK = Chain(
     name="local-fork",
     chain_id=421611,
```

### Comparing `rysk_client-0.2.4/rysk_client/src/operation_factory.py` & `rysk_client-0.2.5/rysk_client/src/operation_factory.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/src/pnl_calculator.py` & `rysk_client-0.2.5/rysk_client/src/pnl_calculator.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/src/position.py` & `rysk_client-0.2.5/rysk_client/src/position.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/src/position_manager.py` & `rysk_client-0.2.5/rysk_client/src/position_manager.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/src/rysk_option_market.py` & `rysk_client-0.2.5/rysk_client/src/rysk_option_market.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/src/subgraph.py` & `rysk_client-0.2.5/rysk_client/src/subgraph.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/src/utils.py` & `rysk_client-0.2.5/rysk_client/src/utils.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/rysk_client/web3_client.py` & `rysk_client-0.2.5/rysk_client/web3_client.py`

 * *Files identical despite different names*

### Comparing `rysk_client-0.2.4/PKG-INFO` & `rysk_client-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rysk-client
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: 8baller
 Author-email: 8ball030@gmail.com
 Requires-Python: >=3.8,<=3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

