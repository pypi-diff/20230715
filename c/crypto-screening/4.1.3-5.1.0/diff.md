# Comparing `tmp/crypto-screening-4.1.3.tar.gz` & `tmp/crypto-screening-5.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-4.1.3.tar", last modified: Fri Jul 14 15:41:41 2023, max compression
+gzip compressed data, was "crypto-screening-5.1.0.tar", last modified: Sat Jul 15 01:28:39 2023, max compression
```

## Comparing `crypto-screening-4.1.3.tar` & `crypto-screening-5.1.0.tar`

### file list

```diff
@@ -1,46 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.122403 crypto-screening-4.1.3/
--rw-rw-rw-   0        0        0       98 2023-07-14 15:41:40.000000 crypto-screening-4.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-14 15:41:41.122403 crypto-screening-4.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-4.1.3/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-4.1.3/build.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.094403 crypto-screening-4.1.3/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.113403 crypto-screening-4.1.3/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-4.1.3/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-4.1.3/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    45385 2023-07-14 15:39:05.000000 crypto-screening-4.1.3/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21227 2023-07-14 15:39:05.000000 crypto-screening-4.1.3/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19348 2023-07-14 15:39:05.000000 crypto-screening-4.1.3/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-4.1.3/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-4.1.3/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    14173 2023-07-14 15:33:15.000000 crypto-screening-4.1.3/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-4.1.3/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-4.1.3/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.114403 crypto-screening-4.1.3/crypto_screening/market/
--rw-rw-rw-   0        0        0    10937 2023-07-13 18:50:12.000000 crypto-screening-4.1.3/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.117403 crypto-screening-4.1.3/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-4.1.3/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-4.1.3/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-4.1.3/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-4.1.3/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.121403 crypto-screening-4.1.3/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      294 2023-06-30 10:45:52.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0     7037 2023-07-14 07:32:35.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    36128 2023-07-14 08:12:31.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    17662 2023-07-14 08:12:31.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    20526 2023-07-14 07:57:08.000000 crypto-screening-4.1.3/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-4.1.3/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-4.1.3/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-4.1.3/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-4.1.3/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-14 15:41:41.108403 crypto-screening-4.1.3/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-14 15:41:41.000000 crypto-screening-4.1.3/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1239 2023-07-14 15:41:41.000000 crypto-screening-4.1.3/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 15:41:41.000000 crypto-screening-4.1.3/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-14 15:41:41.000000 crypto-screening-4.1.3/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-14 15:41:41.000000 crypto-screening-4.1.3/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-14 15:41:40.000000 crypto-screening-4.1.3/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-4.1.3/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-4.1.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-14 15:41:41.122403 crypto-screening-4.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-14 15:39:05.000000 crypto-screening-4.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:28:39.598916 crypto-screening-5.1.0/
+-rw-rw-rw-   0        0        0       98 2023-07-15 01:28:37.000000 crypto-screening-5.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-15 01:28:39.598916 crypto-screening-5.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.1.0/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.1.0/build.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:28:39.472288 crypto-screening-5.1.0/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-15 01:28:39.516394 crypto-screening-5.1.0/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.1.0/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.1.0/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    45462 2023-07-15 01:09:32.000000 crypto-screening-5.1.0/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21227 2023-07-15 01:09:32.000000 crypto-screening-5.1.0/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19348 2023-07-15 01:09:32.000000 crypto-screening-5.1.0/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    14460 2023-07-15 01:09:32.000000 crypto-screening-5.1.0/crypto_screening/collect/orders.py
+-rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-5.1.0/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.1.0/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    15902 2023-07-15 01:09:59.000000 crypto-screening-5.1.0/crypto_screening/collect/trades.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.1.0/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.1.0/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.1.0/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:28:39.522392 crypto-screening-5.1.0/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19343 2023-07-15 01:27:46.000000 crypto-screening-5.1.0/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:28:39.546410 crypto-screening-5.1.0/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-5.1.0/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.1.0/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.1.0/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.1.0/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:28:39.597917 crypto-screening-5.1.0/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.1.0/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-5.1.0/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.1.0/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    10626 2023-07-15 01:21:59.000000 crypto-screening-5.1.0/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    36896 2023-07-15 00:16:21.000000 crypto-screening-5.1.0/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.1.0/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.1.0/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20288 2023-07-14 23:48:05.000000 crypto-screening-5.1.0/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    18063 2023-07-15 00:10:09.000000 crypto-screening-5.1.0/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.1.0/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.1.0/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.1.0/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-5.1.0/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:28:39.490414 crypto-screening-5.1.0/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-15 01:28:39.000000 crypto-screening-5.1.0/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2023-07-15 01:28:39.000000 crypto-screening-5.1.0/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 01:28:39.000000 crypto-screening-5.1.0/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-15 01:28:39.000000 crypto-screening-5.1.0/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 01:28:39.000000 crypto-screening-5.1.0/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-15 01:28:37.000000 crypto-screening-5.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.1.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.1.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 01:28:39.598916 crypto-screening-5.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-15 01:28:33.000000 crypto-screening-5.1.0/setup.py
```

### Comparing `crypto-screening-4.1.3/PKG-INFO` & `crypto-screening-5.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 4.1.3
+Version: 5.1.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-4.1.3/README.md` & `crypto-screening-5.1.0/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/build.py` & `crypto-screening-5.1.0/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/collect/assets.py` & `crypto-screening-5.1.0/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/collect/exchanges.py` & `crypto-screening-5.1.0/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/collect/market.py` & `crypto-screening-5.1.0/crypto_screening/collect/market.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,37 +11,37 @@
 
 from represent import represent, Modifiers
 
 import numpy as np
 import pandas as pd
 
 from crypto_screening.dataset import (
-    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME,
-    OPEN, HIGH, LOW, CLOSE, VOLUME, bid_ask_to_ohlcv
+    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, bid_ask_to_ohlcv,
+    OPEN, HIGH, LOW, CLOSE, VOLUME, AMOUNT, SIDE, PRICE
 )
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
 from crypto_screening.market.screeners.ohlcv import OHLCVScreener
 from crypto_screening.dataset import dataset_to_json
 from crypto_screening.symbols import symbol_to_parts, parts_to_symbol
 from crypto_screening.collect.screeners import (
     find_screeners, screeners_to_assets_datasets,
     screeners_to_symbols_datasets
 )
 
 __all__ = [
-    "validate_assets_market_state_prices_symbol",
-    "assets_market_price",
-    "is_symbol_in_assets_market_prices",
-    "symbols_market_prices",
-    "symbols_market_price",
-    "assets_market_prices",
-    "validate_symbols_market_state_prices_symbol",
-    "is_exchange_in_market_prices",
-    "is_symbol_in_symbols_market_prices",
+    "validate_assets_market_state_values_symbol",
+    "assets_market_value",
+    "is_symbol_in_assets_market_values",
+    "symbols_market_values",
+    "symbols_market_value",
+    "assets_market_values",
+    "validate_symbols_market_state_values_symbol",
+    "is_exchange_in_market_data",
+    "is_symbol_in_symbols_market_values",
     "symbol_to_assets_market_prices",
     "assets_to_symbol_market_prices",
     "assets_to_symbols_market_datasets",
     "symbols_to_assets_market_datasets",
     "symbols_screeners",
     "symbols_market_datasets_to_symbols_screeners",
     "assets_screeners",
@@ -61,307 +61,311 @@
     "assets_market_data",
     "symbols_market_data",
     "assets_market_state",
     "symbols_market_state",
     "merge_assets_market_states",
     "merge_symbols_market_states",
     "ORDERBOOK_ATTRIBUTES",
-    "OHLCV_ATTRIBUTES",
     "assets_to_symbols_screeners",
-    "symbols_to_assets_screeners"
+    "symbols_to_assets_screeners",
+    "OHLCV_ATTRIBUTES",
+    "ORDERS_ATTRIBUTES",
+    "TRADES_ATTRIBUTES"
 ]
 
-AssetsPrices = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]]
-SymbolsPrices = Dict[str, Dict[str, List[Tuple[dt.datetime, float]]]]
+_V = TypeVar("_V")
+
+AssetsData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, _V]]]]]
+SymbolsData = Dict[str, Dict[str, List[Tuple[dt.datetime, _V]]]]
 
-def is_exchange_in_market_prices(
+def is_exchange_in_market_data(
         exchange: str,
-        prices: Union[AssetsPrices, SymbolsPrices]
+        values: Union[AssetsData, SymbolsData]
 ) -> None:
     """
-    Checks if the exchange is in the prices.
+    Checks if the exchange is in the values.
 
     :param exchange: The exchange name.
-    :param prices: The prices.
+    :param values: The values.
 
     :return: The boolean flag.
     """
 
-    return exchange not in prices
+    return exchange not in values
 # end is_exchange_in_market_prices
 
-def is_symbol_in_assets_market_prices(
+def is_symbol_in_assets_market_values(
         exchange: str,
         symbol: str,
-        prices: AssetsPrices,
+        values: AssetsData,
         separator: Optional[str] = None
 ) -> bool:
     """
-    Checks if the symbol is in the prices' data.
+    Checks if the symbol is in the values' data.
 
     :param exchange: The exchange name.
     :param symbol: The symbol to search.
-    :param prices: The price data to process.
+    :param values: The price data to process.
     :param separator: The separator of the assets.
 
     :return: The validation value.
     """
 
-    if not is_exchange_in_market_prices(exchange=exchange, prices=prices):
+    if not is_exchange_in_market_data(exchange=exchange, values=values):
         return False
     # end if
 
     base, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
-    if base not in prices[exchange]:
+    if base not in values[exchange]:
         return False
     # end if
 
-    if quote not in prices[exchange][base]:
+    if quote not in values[exchange][base]:
         return False
     # end if
 
-    return not np.isnan(prices[exchange][base][quote])
+    return not np.isnan(values[exchange][base][quote])
 # end is_symbol_in_assets_market_prices
 
-def is_symbol_in_symbols_market_prices(
+def is_symbol_in_symbols_market_values(
         exchange: str,
         symbol: str,
-        prices: SymbolsPrices
+        values: SymbolsData
 ) -> bool:
     """
-    Checks if the symbol is in the prices' data.
+    Checks if the symbol is in the values' data.
 
     :param exchange: The exchange name.
     :param symbol: The symbol to search.
-    :param prices: The price data to process.
+    :param values: The price data to process.
 
     :return: The validation value.
     """
 
-    if not is_exchange_in_market_prices(exchange=exchange, prices=prices):
+    if not is_exchange_in_market_data(exchange=exchange, values=values):
         return False
     # end if
 
-    if symbol not in prices[exchange]:
+    if symbol not in values[exchange]:
         return False
     # end if
 
-    return not np.isnan(prices[exchange][symbol])
+    return not np.isnan(values[exchange][symbol])
 # end is_symbol_in_assets_market_prices
 
-def validate_assets_market_state_prices_symbol(
+def validate_assets_market_state_values_symbol(
         exchange: str,
         symbol: str,
-        prices: AssetsPrices,
+        values: AssetsData,
         separator: Optional[str] = None,
         provider: Optional[Any] = None
 ) -> None:
     """
-    Checks if the symbol is in the prices' data.
+    Checks if the symbol is in the values' data.
 
     :param exchange: The exchange name.
     :param symbol: The symbol to search.
     :param separator: The separator of the assets.
-    :param prices: The price data to process.
+    :param values: The price data to process.
     :param provider: The data provider.
 
     :return: The validation value.
     """
 
     base, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
-    if exchange not in prices:
+    if exchange not in values:
         raise ValueError(
-            f"exchange '{exchange}' is not found inside the prices of"
+            f"exchange '{exchange}' is not found inside the values of"
             f"{f' of {provider}' if provider is not None else ''}. "
-            f"Found exchanges for are: {', '.join(prices.keys())}"
+            f"Found exchanges for are: {', '.join(values.keys())}"
         )
     # end if
 
-    if base not in prices[exchange]:
+    if base not in values[exchange]:
         raise ValueError(
-            f"base asset '{base}' is not found in '{exchange}' prices of"
+            f"base asset '{base}' is not found in '{exchange}' values of"
             f"{f' of {provider}' if provider is not None else ''}. "
             f"Found base '{exchange}' assets are: "
-            f"{', '.join(prices[exchange].keys())}"
+            f"{', '.join(values[exchange].keys())}"
         )
     # end if
 
-    if quote not in prices[exchange][base]:
+    if quote not in values[exchange][base]:
         raise ValueError(
             f"quote asset '{quote}' is not found in the quote "
-            f"assets of the '{base}' base asset in the prices"
+            f"assets of the '{base}' base asset in the values"
             f"{f' of {provider}' if provider is not None else ''}. "
             f"Found quote assets for the '{base}' base asset in "
-            f"the prices are: {', '.join(prices[exchange][base].keys())}"
+            f"the values are: {', '.join(values[exchange][base].keys())}"
         )
     # end if
 # end validate_assets_market_state_prices_symbol
 
-def validate_symbols_market_state_prices_symbol(
+def validate_symbols_market_state_values_symbol(
         exchange: str,
         symbol: str,
-        prices: SymbolsPrices,
+        values: SymbolsData,
         provider: Optional[Any] = None
 ) -> None:
     """
-    Checks if the symbol is in the prices' data.
+    Checks if the symbol is in the values' data.
 
     :param exchange: The exchange name.
     :param symbol: The symbol to search.
-    :param prices: The price data to process.
+    :param values: The price data to process.
     :param provider: The data provider.
 
     :return: The validation value.
     """
 
-    if exchange not in prices:
+    if exchange not in values:
         raise ValueError(
-            f"exchange '{exchange}' is not found inside the prices of"
+            f"exchange '{exchange}' is not found inside the values of"
             f"{f' of {provider}' if provider is not None else ''}. "
-            f"Found exchanges for are: {', '.join(prices.keys())}"
+            f"Found exchanges for are: {', '.join(values.keys())}"
         )
     # end if
 
-    if symbol not in prices[exchange]:
+    if symbol not in values[exchange]:
         raise ValueError(
-            f"symbol '{symbol}' is not found in '{exchange}' prices of"
+            f"symbol '{symbol}' is not found in '{exchange}' values of"
             f"{f' of {provider}' if provider is not None else ''}. "
-            f"Found symbols for '{exchange}' prices are: "
-            f"{', '.join(prices[exchange].keys())}"
+            f"Found symbols for '{exchange}' values are: "
+            f"{', '.join(values[exchange].keys())}"
         )
     # end if
 # end validate_symbols_market_state_prices_symbol
 
-def assets_market_price(
+def assets_market_value(
         exchange: str,
         symbol: str,
-        prices: AssetsPrices,
+        values: AssetsData,
         separator: Optional[str] = None,
         provider: Optional[Any] = None
-) -> Tuple[dt.datetime, float]:
+) -> Tuple[dt.datetime, _V]:
     """
-    Checks if the symbol is in the prices' data.
+    Checks if the symbol is in the values' data.
 
     :param exchange: The exchange name.
     :param symbol: The symbol to search.
     :param separator: The separator of the assets.
-    :param prices: The price data to process.
+    :param values: The price data to process.
     :param provider: The data provider.
 
     :return: The validation value.
     """
 
-    validate_assets_market_state_prices_symbol(
-        symbol=symbol, prices=prices, exchange=exchange,
+    validate_assets_market_state_values_symbol(
+        symbol=symbol, values=values, exchange=exchange,
         separator=separator, provider=provider
     )
 
     base, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
-    data = list(prices[exchange][base][quote])
+    data = list(values[exchange][base][quote])
 
-    return data[-1][0], float(data[-1][-1])
+    return data[-1][0], data[-1][-1]
 # end assets_market_price
 
-def symbols_market_price(
+def symbols_market_value(
         exchange: str,
         symbol: str,
-        prices: SymbolsPrices,
+        values: SymbolsData,
         provider: Optional[Any] = None
-) -> Tuple[dt.datetime, float]:
+) -> Tuple[dt.datetime, _V]:
     """
-    Checks if the symbol is in the prices' data.
+    Checks if the symbol is in the values' data.
 
     :param exchange: The exchange name.
     :param symbol: The symbol to search.
-    :param prices: The price data to process.
+    :param values: The price data to process.
     :param provider: The data provider.
 
     :return: The validation value.
     """
 
-    validate_symbols_market_state_prices_symbol(
+    validate_symbols_market_state_values_symbol(
         exchange=exchange, symbol=symbol,
-        prices=prices, provider=provider
+        values=values, provider=provider
     )
 
-    data = list(prices[exchange][symbol])
+    data = list(values[exchange][symbol])
 
-    return data[-1][0], float(data[-1][-1])
+    return data[-1][0], data[-1][-1]
 # end symbols_market_price
 
-def symbols_market_prices(
+def symbols_market_values(
         exchange: str,
         symbol: str,
-        prices: SymbolsPrices,
+        values: SymbolsData,
         provider: Optional[Any] = None
-) -> List[Tuple[dt.datetime, float]]:
+) -> List[Tuple[dt.datetime, _V]]:
     """
-    Checks if the symbol is in the prices' data.
+    Checks if the symbol is in the values' data.
 
     :param exchange: The exchange name.
     :param symbol: The symbol to search.
-    :param prices: The price data to process.
+    :param values: The price data to process.
     :param provider: The data provider.
 
     :return: The validation value.
     """
 
-    validate_symbols_market_state_prices_symbol(
+    validate_symbols_market_state_values_symbol(
         exchange=exchange, symbol=symbol,
-        prices=prices, provider=provider
+        values=values, provider=provider
     )
 
-    return [(time, float(value)) for time, value in prices[exchange][symbol]]
+    return values[exchange][symbol]
 # end symbols_market_prices
 
-def assets_market_prices(
+def assets_market_values(
         exchange: str,
         symbol: str,
-        prices: AssetsPrices,
+        values: AssetsData,
         separator: Optional[str] = None,
         provider: Optional[Any] = None
-) -> List[Tuple[dt.datetime, float]]:
+) -> List[Tuple[dt.datetime, _V]]:
     """
-    Checks if the symbol is in the prices' data.
+    Checks if the symbol is in the values' data.
 
     :param exchange: The exchange name.
     :param symbol: The symbol to search.
     :param separator: The separator of the assets.
-    :param prices: The price data to process.
+    :param values: The price data to process.
     :param provider: The data provider.
 
     :return: The validation value.
     """
 
-    validate_assets_market_state_prices_symbol(
-        symbol=symbol, prices=prices, exchange=exchange,
+    validate_assets_market_state_values_symbol(
+        symbol=symbol, values=values, exchange=exchange,
         separator=separator, provider=provider
     )
 
     base, quote = symbol_to_parts(symbol=symbol, separator=separator)
 
-    return [(time, float(value)) for time, value in prices[exchange][base][quote]]
+    return values[exchange][base][quote]
 # end assets_market_prices
 
 @define(repr=False)
 @represent
 class MarketBase(metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
+    bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
-        The screener objects to collect the prices of the assets.
+        The screener objects to collect the values of the assets.
     """
 
     screeners: Iterable[BaseScreener]
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(excluded=["screeners"])
 
     def __hash__(self) -> int:
@@ -377,15 +381,15 @@
 
 AssetsMarketData = Dict[str, Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]]
 AssetsMarketDatasets = Dict[str, Dict[str, Dict[str, pd.DataFrame]]]
 
 SymbolsMarketData = Dict[str, Dict[str, List[Tuple[dt.datetime, Dict[str, float]]]]]
 SymbolsMarketDatasets = Dict[str, Dict[str, pd.DataFrame]]
 
-def dataset_to_data(dataset: pd.DataFrame) -> List[Tuple[dt.datetime, Dict[str, float]]]:
+def dataset_to_data(dataset: pd.DataFrame) -> List[Tuple[dt.datetime, Dict[str, Any]]]:
     """
     Converts the dataset into the data of the rows.
 
     :param dataset: The dataset.
 
     :return: The data structure.
     """
@@ -475,15 +479,15 @@
 def merge_symbols_market_data(
         *data: SymbolsMarketData, sort: Optional[bool] = True
 ) -> SymbolsMarketData:
     """
     Concatenates the states of the market.
 
     :param data: The states to concatenate.
-    :param sort: The value to sort the prices by the time.
+    :param sort: The value to sort the values by the time.
 
     :return: The states object.
     """
 
     new_data: SymbolsMarketData = {}
 
     for data_packet in data:
@@ -512,15 +516,15 @@
 def merge_assets_market_data(
         *data: AssetsMarketData, sort: Optional[bool] = True
 ) -> AssetsMarketData:
     """
     Concatenates the states of the market.
 
     :param data: The states to concatenate.
-    :param sort: The value to sort the prices by the time.
+    :param sort: The value to sort the values by the time.
 
     :return: The states object.
     """
 
     new_data: AssetsMarketData = {}
 
     for data_packet in data:
@@ -605,26 +609,26 @@
         # end for
     # end for
 
     return symbols_datasets
 # end assets_to_symbols_market_datasets
 
 def assets_to_symbol_market_prices(
-        prices: AssetsPrices, separator: Optional[str] = None
-) -> SymbolsPrices:
+        prices: AssetsData, separator: Optional[str] = None
+) -> SymbolsData:
     """
-    Converts an assets market prices into a symbols market prices.
+    Converts an assets market values into a symbols market values.
 
-    :param prices: The source prices.
+    :param prices: The source values.
     :param separator: The separator for the symbols.
 
-    :return: The result prices.
+    :return: The result values.
     """
 
-    symbols_prices: SymbolsPrices = {}
+    symbols_prices: SymbolsData = {}
 
     for exchange, bases in prices.items():
         for base, quotes in bases.items():
             for quote, data in quotes.items():
                 for time, price in data:
                     (
                         symbols_prices.
@@ -638,26 +642,26 @@
         # end for
     # end for
 
     return symbols_prices
 # end assets_to_symbol_market_prices
 
 def symbol_to_assets_market_prices(
-        prices: SymbolsPrices, separator: Optional[str] = None
-) -> AssetsPrices:
+        prices: SymbolsData, separator: Optional[str] = None
+) -> AssetsData:
     """
-    Converts a symbols market prices into an assets market prices.
+    Converts a symbols market values into an assets market values.
 
-    :param prices: The source prices.
+    :param prices: The source values.
     :param separator: The separator for the symbols.
 
-    :return: The result prices.
+    :return: The result values.
     """
 
-    assets_prices: AssetsPrices = {}
+    assets_prices: AssetsData = {}
 
     for exchange, symbols in prices.items():
         for symbol, data in symbols.items():
             base, quote = symbol_to_parts(symbol, separator=separator)
 
             for time, price in data:
                 (
@@ -737,22 +741,34 @@
 # end assets_to_symbols_market_data
 
 _S = TypeVar("_S", BaseScreener, OrderbookScreener)
 
 AssetsScreeners = Dict[str, Dict[str, Dict[str, Union[BaseScreener, _S]]]]
 
 ORDERBOOK_ATTRIBUTES = {
-    "bids": BIDS, "asks": ASKS,
+    "bids": BIDS,
+    "asks": ASKS,
     "bids_volume": BIDS_VOLUME,
     "asks_volume": ASKS_VOLUME
 }
-
 OHLCV_ATTRIBUTES = {
-    "opens": OPEN, "highs": HIGH, "lows": LOW,
-    "closes": CLOSE, "volumes": VOLUME
+    "open": OPEN,
+    "high": HIGH,
+    "low": LOW,
+    "close": CLOSE,
+    "volume": VOLUME
+}
+ORDERS_ATTRIBUTES = {
+    "bids": BIDS,
+    "asks": ASKS
+}
+TRADES_ATTRIBUTES = {
+    "amount": AMOUNT,
+    "price": PRICE,
+    "side": SIDE
 }
 
 def set_screener_dataset(
         screener: _S,
         dataset: pd.DataFrame,
         clean: Optional[bool] = False,
         replace: Optional[bool] = False
@@ -1113,20 +1129,20 @@
     # end try
 
     return index
 # end index_to_datetime
 
 def assets_market_data(
         columns: Dict[str, str],
-        prices: Optional[Dict[str, AssetsPrices]] = None
+        prices: Optional[Dict[str, AssetsData]] = None
 ) -> AssetsMarketData:
     """
     Returns the structured data of the state.
 
-    :param prices: The prices for the data collection.
+    :param prices: The values for the data collection.
     :param columns: The columns for the data.
 
     :return: The data of the state.
     """
 
     prices = prices or {name: {} for name in columns}
 
@@ -1168,20 +1184,20 @@
     # end for
 
     return new_datasets
 # end assets_market_data
 
 def symbols_market_data(
         columns: Dict[str, str],
-        prices: Optional[Dict[str, SymbolsPrices]] = None
+        prices: Optional[Dict[str, SymbolsData]] = None
 ) -> SymbolsMarketData:
     """
     Returns the structured data of the state.
 
-    :param prices: The prices for the data collection.
+    :param prices: The values for the data collection.
     :param columns: The columns for the data.
 
     :return: The data of the state.
     """
 
     datasets: Dict[str, Dict[str, Dict[dt.datetime, Dict[str, float]]]] = {}
 
@@ -1289,30 +1305,30 @@
 
     return length
 # end adjusted_dataset_length
 
 def assets_market_state(
         columns: Dict[str, str],
         screeners: Iterable[BaseScreener],
-        prices: Optional[Dict[str, AssetsPrices]] = None,
+        prices: Optional[Dict[str, AssetsData]] = None,
         separator: Optional[str] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
-) -> Dict[str, AssetsPrices]:
+) -> Dict[str, AssetsData]:
     """
-    Fetches the prices and relations between the assets.
+    Fetches the values and relations between the assets.
 
-    :param prices: The prices for the data collection.
+    :param prices: The values for the data collection.
     :param columns: The columns for the data.
     :param screeners: The price screeners.
     :param separator: The separator of the assets.
-    :param length: The length of the prices.
+    :param length: The length of the values.
     :param adjust: The value to adjust the length of the sequences.
 
-    :return: The prices of the assets.
+    :return: The values of the assets.
     """
 
     prices = prices or {name: {} for name in columns}
 
     if (length is None) and (not adjust):
         length = minimum_common_dataset_length(
             columns=columns, screeners=screeners
@@ -1356,29 +1372,29 @@
     # end for
 
     return prices
 # end assets_market_state
 
 def symbols_market_state(
         columns: Dict[str, str],
-        prices: Optional[Dict[str, SymbolsPrices]] = None,
+        prices: Optional[Dict[str, SymbolsData]] = None,
         screeners: Optional[Iterable[BaseScreener]] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
-) -> Dict[str, SymbolsPrices]:
+) -> Dict[str, SymbolsData]:
     """
-    Fetches the prices and relations between the assets.
+    Fetches the values and relations between the assets.
 
-    :param prices: The prices for the data collection.
+    :param prices: The values for the data collection.
     :param columns: The columns for the data.
     :param screeners: The price screeners.
-    :param length: The length of the prices.
+    :param length: The length of the values.
     :param adjust: The value to adjust the length of the sequences.
 
-    :return: The prices of the assets.
+    :return: The values of the assets.
     """
 
     prices = prices or {name: {} for name in columns}
 
     if (length is None) and (not adjust):
         length = minimum_common_dataset_length(
             columns=columns, screeners=screeners
@@ -1418,23 +1434,23 @@
     # end for
 
     return prices
 # end symbols_market_state
 
 def merge_assets_market_states(
         *states: MarketBase,
-        prices: Dict[str, AssetsPrices],
+        prices: Dict[str, AssetsData],
         sort: Optional[bool] = True
-) -> Dict[str, AssetsPrices]:
+) -> Dict[str, AssetsData]:
     """
     Concatenates the states of the market.
 
-    :param prices: The prices for the data collection.
+    :param prices: The values for the data collection.
     :param states: The states to concatenate.
-    :param sort: The value to sort the prices by the time.
+    :param sort: The value to sort the values by the time.
 
     :return: The states object.
     """
 
     for state in states:
         for name in prices:
             for exchange, bases in getattr(state, name).items():
@@ -1464,23 +1480,23 @@
     # end if
 
     return prices
 # end merge_assets_market_states
 
 def merge_symbols_market_states(
         *states: MarketBase,
-        prices: Dict[str, SymbolsPrices],
+        prices: Dict[str, SymbolsData],
         sort: Optional[bool] = True
-) -> Dict[str, SymbolsPrices]:
+) -> Dict[str, SymbolsData]:
     """
     Concatenates the states of the market.
 
-    :param prices: The prices for the data collection.
+    :param prices: The values for the data collection.
     :param states: The states to concatenate.
-    :param sort: The value to sort the prices by the time.
+    :param sort: The value to sort the values by the time.
 
     :return: The states object.
     """
 
     for state in states:
         for name in prices:
             for exchange, symbols in getattr(state, name).items():
```

### Comparing `crypto-screening-4.1.3/crypto_screening/collect/ohlcv.py` & `crypto-screening-5.1.0/crypto_screening/collect/ohlcv.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.ohlcv import (
     create_ohlcv_dataframe
 )
 from crypto_screening.collect.market import (
-    MarketBase, assets_market_prices, symbols_market_data,
-    is_symbol_in_assets_market_prices, symbols_market_prices,
-    is_symbol_in_symbols_market_prices, assets_market_data,
+    MarketBase, assets_market_values, symbols_market_data,
+    is_symbol_in_assets_market_values, symbols_market_values,
+    is_symbol_in_symbols_market_values, assets_market_data,
     assets_to_symbol_market_prices, assets_market_state,
     symbol_to_assets_market_prices, symbols_market_state,
     merge_assets_market_states, merge_symbols_market_states,
     OHLCV_ATTRIBUTES
 )
 
 __all__ = [
@@ -44,20 +44,20 @@
 @define(repr=False)
 @represent
 class OHLCVMarketBase(MarketBase, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
+    bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
-        The screener objects to collect the prices of the assets.
+        The screener objects to collect the values of the assets.
     """
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(
         **MarketBase.__modifiers__
     )
     __modifiers__.excluded.extend(["open", "high", "low", "close", "volume"])
 # end OrderbookMarketBase
@@ -68,32 +68,32 @@
 @define(repr=False)
 @represent
 class AssetsOHLCVMarketState(OHLCVMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
+    bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
-        The screener objects to collect the prices of the assets.
+        The screener objects to collect the values of the assets.
 
     - bids:
-        The bids prices of the assets.
+        The bids values of the assets.
 
     - asks:
-        The asks prices of the assets.
+        The asks values of the assets.
 
     - bids_volume:
-        The bids volume prices of the assets.
+        The bids volume values of the assets.
 
     - asks_volume:
-        The asks volume prices of the assets.
+        The asks volume values of the assets.
 
     >>> from crypto_screening.collect.orderbook import AssetsOrderbookMarketState
     >>>
     >>> state = assets_ohlcv_market_state(...)
     """
 
     opens: AssetsPrices
@@ -111,16 +111,16 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.opens,
+        return assets_market_values(
+            exchange=exchange, symbol=symbol, values=self.opens,
             separator=separator, provider=self
         )
     # end bid
 
     def high(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -130,16 +130,16 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.highs,
+        return assets_market_values(
+            exchange=exchange, symbol=symbol, values=self.highs,
             separator=separator, provider=self
         )
     # end ask
 
     def low(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -149,16 +149,16 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.lows,
+        return assets_market_values(
+            exchange=exchange, symbol=symbol, values=self.lows,
             separator=separator, provider=self
         )
     # end bid_volume
 
     def close(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -168,16 +168,16 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.closes,
+        return assets_market_values(
+            exchange=exchange, symbol=symbol, values=self.closes,
             separator=separator, provider=self
         )
     # end ask_volume
 
     def volume(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -187,127 +187,127 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.closes,
+        return assets_market_values(
+            exchange=exchange, symbol=symbol, values=self.closes,
             separator=separator, provider=self
         )
     # end ask_volume
 
     def in_open_prices(
             self,
             exchange: str,
             symbol: str,
             separator: Optional[str] = None
     ) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_assets_market_prices(
+        return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.opens
+            separator=separator, values=self.opens
         )
     # end in_bids_prices
 
     def in_high_prices(
             self,
             exchange: str,
             symbol: str,
             separator: Optional[str] = None
     ) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_assets_market_prices(
+        return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.highs
+            separator=separator, values=self.highs
         )
     # end in_asks_prices
 
     def in_low_prices(
             self,
             exchange: str,
             symbol: str,
             separator: Optional[str] = None
     ) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_assets_market_prices(
+        return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.lows
+            separator=separator, values=self.lows
         )
     # end in_bids_volume_prices
 
     def in_close_prices(
             self,
             exchange: str,
             symbol: str,
             separator: Optional[str] = None
     ) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_assets_market_prices(
+        return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.closes
+            separator=separator, values=self.closes
         )
     # end in_asks_volume_prices
 
     def in_volume_prices(
             self,
             exchange: str,
             symbol: str,
             separator: Optional[str] = None
     ) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_assets_market_prices(
+        return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.volumes
+            separator=separator, values=self.volumes
         )
     # end in_asks_volume_prices
 
     def data(self) -> AssetsMarketData:
         """
         Returns the structured data of the state.
 
@@ -348,22 +348,22 @@
 def assets_ohlcv_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         separator: Optional[str] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> AssetsOHLCVMarketState:
     """
-    Fetches the prices and relations between the assets.
+    Fetches the values and relations between the assets.
 
     :param screeners: The price screeners.
     :param separator: The separator of the assets.
-    :param length: The length of the prices.
+    :param length: The length of the values.
     :param adjust: The value to adjust the length of the sequences.
 
-    :return: The prices of the assets.
+    :return: The values of the assets.
     """
 
     return AssetsOHLCVMarketState(
         screeners=screeners,
         **assets_market_state(
             columns=OHLCV_ATTRIBUTES,
             screeners=screeners, separator=separator,
@@ -378,32 +378,32 @@
 @define(repr=False)
 @represent
 class SymbolsOHLCVMarketState(OHLCVMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
+    bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
-        The screener objects to collect the prices of the assets.
+        The screener objects to collect the values of the assets.
 
     - bids:
-        The bids prices of the assets.
+        The bids values of the assets.
 
     - asks:
-        The asks prices of the assets.
+        The asks values of the assets.
 
     - bids_volume:
-        The bids volume prices of the assets.
+        The bids volume values of the assets.
 
     - asks_volume:
-        The asks volume prices of the assets.
+        The asks volume values of the assets.
 
     >>> from crypto_screening.collect.orderbook import AssetsOrderbookMarketState
     >>>
     >>> state = assets_ohlcv_market_state(...)
     """
 
     opens: SymbolsPrices
@@ -418,156 +418,156 @@
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
 
         :return: The bid price for the symbol.
         """
 
-        return symbols_market_prices(
+        return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            prices=self.opens, provider=self
+            values=self.opens, provider=self
         )
     # end open
 
     def high(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
-        return symbols_market_prices(
+        return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            prices=self.highs, provider=self
+            values=self.highs, provider=self
         )
     # end high
 
     def low(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the bid price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
 
         :return: The bid price for the symbol.
         """
 
-        return symbols_market_prices(
+        return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            prices=self.lows, provider=self
+            values=self.lows, provider=self
         )
     # end low
 
     def close(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
-        return symbols_market_prices(
+        return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            prices=self.closes, provider=self
+            values=self.closes, provider=self
         )
     # end close
 
     def volume(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
-        return symbols_market_prices(
+        return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            prices=self.volumes, provider=self
+            values=self.volumes, provider=self
         )
     # end volume
 
     def in_open_prices(self, exchange: str, symbol: str) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.opens
+        return is_symbol_in_symbols_market_values(
+            exchange=exchange, symbol=symbol, values=self.opens
         )
     # end in_open_prices
 
     def in_high_prices(self, exchange: str, symbol: str) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.highs
+        return is_symbol_in_symbols_market_values(
+            exchange=exchange, symbol=symbol, values=self.highs
         )
     # end in_high_prices
 
     def in_low_prices(self, exchange: str, symbol: str) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.lows
+        return is_symbol_in_symbols_market_values(
+            exchange=exchange, symbol=symbol, values=self.lows
         )
     # end in_low_prices
 
     def in_close_prices(self, exchange: str, symbol: str) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The in_asks_volume_prices value.
         """
 
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.closes
+        return is_symbol_in_symbols_market_values(
+            exchange=exchange, symbol=symbol, values=self.closes
         )
     # end in_close_prices
 
     def in_volume_prices(self, exchange: str, symbol: str) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The in_asks_volume_prices value.
         """
 
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.volumes
+        return is_symbol_in_symbols_market_values(
+            exchange=exchange, symbol=symbol, values=self.volumes
         )
     # end in_volume_prices
 
     def data(self) -> SymbolsMarketData:
         """
         Returns the structured data of the state.
 
@@ -605,21 +605,21 @@
 
 def symbols_ohlcv_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> SymbolsOHLCVMarketState:
     """
-    Fetches the prices and relations between the assets.
+    Fetches the values and relations between the assets.
 
     :param screeners: The price screeners.
-    :param length: The length of the prices.
+    :param length: The length of the values.
     :param adjust: The value to adjust the length of the sequences.
 
-    :return: The prices of the assets.
+    :return: The values of the assets.
     """
 
     return SymbolsOHLCVMarketState(
         screeners=screeners,
         **symbols_market_state(
             columns=OHLCV_ATTRIBUTES, screeners=screeners,
             length=length, adjust=adjust
@@ -630,15 +630,15 @@
 def merge_symbols_ohlcv_market_states(
         *states: SymbolsOHLCVMarketState, sort: Optional[bool] = True
 ) -> SymbolsOHLCVMarketState:
     """
     Concatenates the states of the market.
 
     :param states: The states to concatenate.
-    :param sort: The value to sort the prices by the time.
+    :param sort: The value to sort the values by the time.
 
     :return: The states object.
     """
 
     screeners = []
 
     for state in states:
@@ -656,15 +656,15 @@
 def merge_assets_ohlcv_market_states(
         *states: AssetsOHLCVMarketState, sort: Optional[bool] = True
 ) -> AssetsOHLCVMarketState:
     """
     Concatenates the states of the market.
 
     :param states: The states to concatenate.
-    :param sort: The value to sort the prices by the time.
+    :param sort: The value to sort the values by the time.
 
     :return: The states object.
     """
 
     screeners = []
 
     for state in states:
```

### Comparing `crypto-screening-4.1.3/crypto_screening/collect/orderbook.py` & `crypto-screening-5.1.0/crypto_screening/collect/orderbook.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 import pandas as pd
 
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.orderbook import (
     create_orderbook_dataframe
 )
 from crypto_screening.collect.market import (
-    MarketBase, assets_market_prices, assets_market_data,
-    is_symbol_in_assets_market_prices, symbols_market_prices,
-    is_symbol_in_symbols_market_prices, symbols_market_data,
+    MarketBase, assets_market_values, assets_market_data,
+    is_symbol_in_assets_market_values, symbols_market_values,
+    is_symbol_in_symbols_market_values, symbols_market_data,
     assets_to_symbol_market_prices, assets_market_state,
     symbol_to_assets_market_prices, symbols_market_state,
     merge_assets_market_states, merge_symbols_market_states,
     ORDERBOOK_ATTRIBUTES
 )
 
 __all__ = [
@@ -44,20 +44,20 @@
 @define(repr=False)
 @represent
 class OrderbookMarketBase(MarketBase, metaclass=ABCMeta):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
+    bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
-        The screener objects to collect the prices of the assets.
+        The screener objects to collect the values of the assets.
     """
 
     __modifiers__: ClassVar[Modifiers] = Modifiers(
         **MarketBase.__modifiers__
     )
     __modifiers__.excluded.extend(["bids", "asks", "bids_volume", "asks_volume"])
 # end OrderbookMarketBase
@@ -68,32 +68,32 @@
 @define(repr=False)
 @represent
 class AssetsOrderbookMarketState(OrderbookMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
+    bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
-        The screener objects to collect the prices of the assets.
+        The screener objects to collect the values of the assets.
 
     - bids:
-        The bids prices of the assets.
+        The bids values of the assets.
 
     - asks:
-        The asks prices of the assets.
+        The asks values of the assets.
 
     - bids_volume:
-        The bids volume prices of the assets.
+        The bids volume values of the assets.
 
     - asks_volume:
-        The asks volume prices of the assets.
+        The asks volume values of the assets.
 
     >>> from crypto_screening.collect.orderbook import assets_orderbook_market_state
     >>>
     >>> state = assets_orderbook_market_state(...)
     """
 
     bids: AssetsPrices
@@ -110,16 +110,16 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.bids,
+        return assets_market_values(
+            exchange=exchange, symbol=symbol, values=self.bids,
             separator=separator, provider=self
         )
     # end bid
 
     def ask(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -129,16 +129,16 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.asks,
+        return assets_market_values(
+            exchange=exchange, symbol=symbol, values=self.asks,
             separator=separator, provider=self
         )
     # end ask
 
     def bid_volume(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -148,16 +148,16 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
         :param separator: The separator of the assets.
 
         :return: The bid price for the symbol.
         """
 
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.bids_volume,
+        return assets_market_values(
+            exchange=exchange, symbol=symbol, values=self.bids_volume,
             separator=separator, provider=self
         )
     # end bid_volume
 
     def ask_volume(
             self, exchange: str, symbol: str, separator: Optional[str] = None
     ) -> List[Tuple[dt.datetime, float]]:
@@ -167,105 +167,105 @@
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
         :param separator: The separator of the assets.
 
         :return: The ask price for the symbol.
         """
 
-        return assets_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.asks_volume,
+        return assets_market_values(
+            exchange=exchange, symbol=symbol, values=self.asks_volume,
             separator=separator, provider=self
         )
     # end ask_volume
 
     def in_bids_prices(
             self,
             exchange: str,
             symbol: str,
             separator: Optional[str] = None
     ) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_assets_market_prices(
+        return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.bids
+            separator=separator, values=self.bids
         )
     # end in_bids_prices
 
     def in_asks_prices(
             self,
             exchange: str,
             symbol: str,
             separator: Optional[str] = None
     ) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_assets_market_prices(
+        return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.asks
+            separator=separator, values=self.asks
         )
     # end in_asks_prices
 
     def in_bids_volume_prices(
             self,
             exchange: str,
             symbol: str,
             separator: Optional[str] = None
     ) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_assets_market_prices(
+        return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.bids_volume
+            separator=separator, values=self.bids_volume
         )
     # end in_bids_volume_prices
 
     def in_asks_volume_prices(
             self,
             exchange: str,
             symbol: str,
             separator: Optional[str] = None
     ) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
         :param separator: The separator of the assets.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_assets_market_prices(
+        return is_symbol_in_assets_market_values(
             exchange=exchange, symbol=symbol,
-            separator=separator, prices=self.asks_volume
+            separator=separator, values=self.asks_volume
         )
     # end in_asks_volume_prices
 
     def data(self) -> AssetsMarketData:
         """
         Returns the structured data of the state.
 
@@ -306,22 +306,22 @@
 def assets_orderbook_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         separator: Optional[str] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> AssetsOrderbookMarketState:
     """
-    Fetches the prices and relations between the assets.
+    Fetches the values and relations between the assets.
 
     :param screeners: The price screeners.
     :param separator: The separator of the assets.
-    :param length: The length of the prices.
+    :param length: The length of the values.
     :param adjust: The value to adjust the length of the sequences.
 
-    :return: The prices of the assets.
+    :return: The values of the assets.
     """
 
     return AssetsOrderbookMarketState(
         screeners=screeners,
         **assets_market_state(
             columns=ORDERBOOK_ATTRIBUTES,
             screeners=screeners, separator=separator,
@@ -336,32 +336,32 @@
 @define(repr=False)
 @represent
 class SymbolsOrderbookMarketState(OrderbookMarketBase):
     """
     A class to represent the current market state.
 
     This object contains the state of the market, as Close,
-    bids and asks prices of specific assets, gathered from the network.
+    bids and asks values of specific assets, gathered from the network.
 
     attributes:
 
     - screeners:
-        The screener objects to collect the prices of the assets.
+        The screener objects to collect the values of the assets.
 
     - bids:
-        The bids prices of the assets.
+        The bids values of the assets.
 
     - asks:
-        The asks prices of the assets.
+        The asks values of the assets.
 
     - bids_volume:
-        The bids volume prices of the assets.
+        The bids volume values of the assets.
 
     - asks_volume:
-        The asks volume prices of the assets.
+        The asks volume values of the assets.
 
     >>> from crypto_screening.collect.orderbook import assets_orderbook_market_state
     >>>
     >>> state = assets_orderbook_market_state(...)
     """
 
     bids: SymbolsPrices
@@ -375,125 +375,125 @@
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
 
         :return: The bid price for the symbol.
         """
 
-        return symbols_market_prices(
+        return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            prices=self.bids, provider=self
+            values=self.bids, provider=self
         )
     # end bid
 
     def ask(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
-        return symbols_market_prices(
+        return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            prices=self.asks, provider=self
+            values=self.asks, provider=self
         )
     # end ask
 
     def bid_volume(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the bid price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its bid price.
 
         :return: The bid price for the symbol.
         """
 
-        return symbols_market_prices(
+        return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            prices=self.bids_volume, provider=self
+            values=self.bids_volume, provider=self
         )
     # end bid_volume
 
     def ask_volume(self, exchange: str, symbol: str) -> List[Tuple[dt.datetime, float]]:
         """
         Returns the ask price for the symbol.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to find its ask price.
 
         :return: The ask price for the symbol.
         """
 
-        return symbols_market_prices(
+        return symbols_market_values(
             exchange=exchange, symbol=symbol,
-            prices=self.asks_volume, provider=self
+            values=self.asks_volume, provider=self
         )
     # end ask_volume
 
     def in_bids_prices(self, exchange: str, symbol: str) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.bids
+        return is_symbol_in_symbols_market_values(
+            exchange=exchange, symbol=symbol, values=self.bids
         )
     # end in_bids_prices
 
     def in_asks_prices(self, exchange: str, symbol: str) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.asks
+        return is_symbol_in_symbols_market_values(
+            exchange=exchange, symbol=symbol, values=self.asks
         )
     # end in_asks_prices
 
     def in_bids_volume_prices(self, exchange: str, symbol: str) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The validation value.
         """
 
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.bids_volume
+        return is_symbol_in_symbols_market_values(
+            exchange=exchange, symbol=symbol, values=self.bids_volume
         )
     # end in_bids_volume_prices
 
     def in_asks_volume_prices(self, exchange: str, symbol: str) -> bool:
         """
-        Checks if the symbol is in the prices' data.
+        Checks if the symbol is in the values' data.
 
         :param exchange: The exchange name.
         :param symbol: The symbol to search.
 
         :return: The in_asks_volume_prices value.
         """
 
-        return is_symbol_in_symbols_market_prices(
-            exchange=exchange, symbol=symbol, prices=self.asks_volume
+        return is_symbol_in_symbols_market_values(
+            exchange=exchange, symbol=symbol, values=self.asks_volume
         )
     # end in_asks_prices
 
     def data(self) -> SymbolsMarketData:
         """
         Returns the structured data of the state.
 
@@ -531,21 +531,21 @@
 
 def symbols_orderbook_market_state(
         screeners: Optional[Iterable[BaseScreener]] = None,
         length: Optional[int] = None,
         adjust: Optional[bool] = True
 ) -> SymbolsOrderbookMarketState:
     """
-    Fetches the prices and relations between the assets.
+    Fetches the values and relations between the assets.
 
     :param screeners: The price screeners.
-    :param length: The length of the prices.
+    :param length: The length of the values.
     :param adjust: The value to adjust the length of the sequences.
 
-    :return: The prices of the assets.
+    :return: The values of the assets.
     """
 
     return SymbolsOrderbookMarketState(
         screeners=screeners,
         **symbols_market_state(
             columns=ORDERBOOK_ATTRIBUTES, screeners=screeners,
             length=length, adjust=adjust
@@ -556,15 +556,15 @@
 def merge_symbols_orderbook_market_states(
         *states: SymbolsOrderbookMarketState, sort: Optional[bool] = True
 ) -> SymbolsOrderbookMarketState:
     """
     Concatenates the states of the market.
 
     :param states: The states to concatenate.
-    :param sort: The value to sort the prices by the time.
+    :param sort: The value to sort the values by the time.
 
     :return: The states object.
     """
 
     screeners = []
 
     for state in states:
@@ -582,15 +582,15 @@
 def merge_assets_orderbook_market_states(
         *states: AssetsOrderbookMarketState, sort: Optional[bool] = True
 ) -> AssetsOrderbookMarketState:
     """
     Concatenates the states of the market.
 
     :param states: The states to concatenate.
-    :param sort: The value to sort the prices by the time.
+    :param sort: The value to sort the values by the time.
 
     :return: The states object.
     """
 
     screeners = []
 
     for state in states:
```

### Comparing `crypto-screening-4.1.3/crypto_screening/collect/screeners.py` & `crypto-screening-5.1.0/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/collect/symbols.py` & `crypto-screening-5.1.0/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/dataset.py` & `crypto-screening-5.1.0/crypto_screening/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,34 +43,46 @@
     "CSV_EXTENSION",
     "JSON_EXTENSION",
     "DEFAULT_EXTENSION",
     "BASE_VOLUME",
     "QUOTE_VOLUME",
     "bid_ask_to_ohlcv",
     "create_market_dataframe",
-    "ORDERBOOK_COLUMNS"
+    "ORDERBOOK_COLUMNS",
+    "TRADES_COLUMNS",
+    "PRICE",
+    "SIDE",
+    "ORDERS_COLUMNS",
+    "AMOUNT"
 ]
 
+DATE_TIME = 'DateTime'
+
 OPEN = "Open"
 CLOSE = "Close"
 HIGH = "High"
 LOW = "Low"
 VOLUME = "Volume"
-DATE_TIME = 'DateTime'
 
 BIDS = "Bids"
 ASKS = "Asks"
 BIDS_VOLUME = "Bids Volume"
 ASKS_VOLUME = "Asks Volume"
 BASE_VOLUME = "Base Volume"
 QUOTE_VOLUME = "Quote Volume"
 
+AMOUNT = "Amount"
+PRICE = "Price"
+SIDE = "Side"
+
 OHLC_COLUMNS = (OPEN, HIGH, LOW, CLOSE)
 OHLCV_COLUMNS = (*OHLC_COLUMNS, VOLUME)
 ORDERBOOK_COLUMNS = (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME)
+TRADES_COLUMNS = (AMOUNT, PRICE, SIDE)
+ORDERS_COLUMNS = (BIDS, ASKS)
 
 def row_to_dataset(
         dataset: Union[pd.DataFrame, pd.Series],
         index: Optional[int] = None
 ) -> pd.DataFrame:
     """
     Creates a dataframe from the row.
```

### Comparing `crypto-screening-4.1.3/crypto_screening/interval.py` & `crypto-screening-5.1.0/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/market/dynamic.py` & `crypto-screening-5.1.0/crypto_screening/market/dynamic.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,14 +12,22 @@
     assets_orderbook_market_state, symbols_orderbook_market_state,
     SymbolsOrderbookMarketState, AssetsOrderbookMarketState
 )
 from crypto_screening.collect.ohlcv import (
     assets_ohlcv_market_state, symbols_ohlcv_market_state,
     SymbolsOHLCVMarketState, AssetsOHLCVMarketState
 )
+from crypto_screening.collect.orders import (
+    assets_orders_market_state, symbols_orders_market_state,
+    SymbolsOrdersMarketState, AssetsOrdersMarketState
+)
+from crypto_screening.collect.trades import (
+    assets_trades_market_state, symbols_trades_market_state,
+    SymbolsTradesMarketState, AssetsTradesMarketState
+)
 from crypto_screening.market.screeners.container import ScreenersContainer
 
 __all__ = [
     "DynamicScreener"
 ]
 
 class DynamicScreener(ScreenersContainer):
@@ -111,14 +119,64 @@
         # end try
 
         length = min(length or 0, len(market))
 
         return market.iloc[-length:]
     # end find_orderbook_dataset
 
+    def find_orders_dataset(
+            self,
+            exchange: str,
+            symbol: str,
+            length: Optional[int] = None
+    ) -> pd.DataFrame:
+        """
+        Returns the data by according to the parameters.
+
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+        :param length: The length of the data.
+
+        :return: The data.
+        """
+
+        screener = self.find_orders_screener(
+            exchange=exchange, symbol=symbol
+        )
+
+        length = min(length or 0, len(screener.market))
+
+        return screener.market.iloc[-length:]
+    # end find_orders_dataset
+
+    def find_trades_dataset(
+            self,
+            exchange: str,
+            symbol: str,
+            length: Optional[int] = None
+    ) -> pd.DataFrame:
+        """
+        Returns the data by according to the parameters.
+
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+        :param length: The length of the data.
+
+        :return: The data.
+        """
+
+        screener = self.find_trades_screener(
+            exchange=exchange, symbol=symbol
+        )
+
+        length = min(length or 0, len(screener.market))
+
+        return screener.market.iloc[-length:]
+    # end find_trades_dataset
+
     def find_datasets(
             self,
             exchange: str,
             symbol: str,
             length: Optional[int] = None
     ) -> List[pd.DataFrame]:
         """
@@ -147,27 +205,27 @@
             adjust: Optional[bool] = True,
             bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
     ) -> AssetsOrderbookMarketState:
         """
-        Fetches the prices and relations between the assets.
+        Fetches the values and relations between the assets.
 
-        :param length: The length of the prices.
+        :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
         :param quotes: The quotes of the asset pairs.
         :param excluded: The excluded symbols.
         :param adjust: The value to adjust the invalid exchanges.
         :param separator: The separator of the assets.
         :param included: The symbols to include.
         :param bases: The bases of the asset pairs.
 
-        :return: The prices of the assets.
+        :return: The values of the assets.
         """
 
         screeners = exchanges_symbols_screeners(
             screeners=self.screeners, exchanges=exchanges,
             separator=separator, bases=bases, quotes=quotes,
             included=included, excluded=excluded, adjust=adjust
         )
@@ -186,27 +244,27 @@
             adjust: Optional[bool] = True,
             bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
     ) -> SymbolsOrderbookMarketState:
         """
-        Fetches the prices and relations between the assets.
+        Fetches the values and relations between the assets.
 
-        :param length: The length of the prices.
+        :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
         :param quotes: The quotes of the asset pairs.
         :param excluded: The excluded symbols.
         :param adjust: The value to adjust the invalid exchanges.
         :param separator: The separator of the assets.
         :param included: The symbols to include.
         :param bases: The bases of the asset pairs.
 
-        :return: The prices of the assets.
+        :return: The values of the assets.
         """
 
         screeners = exchanges_symbols_screeners(
             screeners=self.screeners, exchanges=exchanges,
             separator=separator, bases=bases, quotes=quotes,
             included=included, excluded=excluded, adjust=adjust
         )
@@ -224,27 +282,27 @@
             adjust: Optional[bool] = True,
             bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
     ) -> AssetsOHLCVMarketState:
         """
-        Fetches the prices and relations between the assets.
+        Fetches the values and relations between the assets.
 
-        :param length: The length of the prices.
+        :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
         :param quotes: The quotes of the asset pairs.
         :param excluded: The excluded symbols.
         :param adjust: The value to adjust the invalid exchanges.
         :param separator: The separator of the assets.
         :param included: The symbols to include.
         :param bases: The bases of the asset pairs.
 
-        :return: The prices of the assets.
+        :return: The values of the assets.
         """
 
         screeners = exchanges_symbols_screeners(
             screeners=self.screeners, exchanges=exchanges,
             separator=separator, bases=bases, quotes=quotes,
             included=included, excluded=excluded, adjust=adjust
         )
@@ -263,33 +321,187 @@
             adjust: Optional[bool] = True,
             bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
             excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
     ) -> SymbolsOHLCVMarketState:
         """
-        Fetches the prices and relations between the assets.
+        Fetches the values and relations between the assets.
 
-        :param length: The length of the prices.
+        :param length: The length of the values.
         :param adjust: The value to adjust the length of the sequences.
         :param exchanges: The exchanges.
         :param quotes: The quotes of the asset pairs.
         :param excluded: The excluded symbols.
         :param adjust: The value to adjust the invalid exchanges.
         :param separator: The separator of the assets.
         :param included: The symbols to include.
         :param bases: The bases of the asset pairs.
 
-        :return: The prices of the assets.
+        :return: The values of the assets.
         """
 
         screeners = exchanges_symbols_screeners(
             screeners=self.screeners, exchanges=exchanges,
             separator=separator, bases=bases, quotes=quotes,
             included=included, excluded=excluded, adjust=adjust
         )
 
         return symbols_ohlcv_market_state(
             screeners=screeners, length=length, adjust=adjust
         )
     # end symbols_ohlcv_market_state
+
+    def assets_trades_market_state(
+            self,
+            exchanges: Optional[Iterable[str]] = None,
+            separator: Optional[str] = None,
+            length: Optional[int] = None,
+            adjust: Optional[bool] = True,
+            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+    ) -> AssetsTradesMarketState:
+        """
+        Fetches the values and relations between the assets.
+
+        :param length: The length of the values.
+        :param adjust: The value to adjust the length of the sequences.
+        :param exchanges: The exchanges.
+        :param quotes: The quotes of the asset pairs.
+        :param excluded: The excluded symbols.
+        :param adjust: The value to adjust the invalid exchanges.
+        :param separator: The separator of the assets.
+        :param included: The symbols to include.
+        :param bases: The bases of the asset pairs.
+
+        :return: The values of the assets.
+        """
+
+        screeners = exchanges_symbols_screeners(
+            screeners=self.screeners, exchanges=exchanges,
+            separator=separator, bases=bases, quotes=quotes,
+            included=included, excluded=excluded, adjust=adjust
+        )
+
+        return assets_trades_market_state(
+            screeners=screeners, separator=separator,
+            length=length, adjust=adjust
+        )
+    # end assets_trades_market_state
+
+    def symbols_trades_market_state(
+            self,
+            exchanges: Optional[Iterable[str]] = None,
+            separator: Optional[str] = None,
+            length: Optional[int] = None,
+            adjust: Optional[bool] = True,
+            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+    ) -> SymbolsTradesMarketState:
+        """
+        Fetches the values and relations between the assets.
+
+        :param length: The length of the values.
+        :param adjust: The value to adjust the length of the sequences.
+        :param exchanges: The exchanges.
+        :param quotes: The quotes of the asset pairs.
+        :param excluded: The excluded symbols.
+        :param adjust: The value to adjust the invalid exchanges.
+        :param separator: The separator of the assets.
+        :param included: The symbols to include.
+        :param bases: The bases of the asset pairs.
+
+        :return: The values of the assets.
+        """
+
+        screeners = exchanges_symbols_screeners(
+            screeners=self.screeners, exchanges=exchanges,
+            separator=separator, bases=bases, quotes=quotes,
+            included=included, excluded=excluded, adjust=adjust
+        )
+
+        return symbols_trades_market_state(
+            screeners=screeners, length=length, adjust=adjust
+        )
+    # end symbols_trades_market_state
+
+    def assets_orders_market_state(
+            self,
+            exchanges: Optional[Iterable[str]] = None,
+            separator: Optional[str] = None,
+            length: Optional[int] = None,
+            adjust: Optional[bool] = True,
+            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+    ) -> AssetsOrdersMarketState:
+        """
+        Fetches the values and relations between the assets.
+
+        :param length: The length of the values.
+        :param adjust: The value to adjust the length of the sequences.
+        :param exchanges: The exchanges.
+        :param quotes: The quotes of the asset pairs.
+        :param excluded: The excluded symbols.
+        :param adjust: The value to adjust the invalid exchanges.
+        :param separator: The separator of the assets.
+        :param included: The symbols to include.
+        :param bases: The bases of the asset pairs.
+
+        :return: The values of the assets.
+        """
+
+        screeners = exchanges_symbols_screeners(
+            screeners=self.screeners, exchanges=exchanges,
+            separator=separator, bases=bases, quotes=quotes,
+            included=included, excluded=excluded, adjust=adjust
+        )
+
+        return assets_orders_market_state(
+            screeners=screeners, separator=separator,
+            length=length, adjust=adjust
+        )
+    # end assets_orders_market_state
+
+    def symbols_orders_market_state(
+            self,
+            exchanges: Optional[Iterable[str]] = None,
+            separator: Optional[str] = None,
+            length: Optional[int] = None,
+            adjust: Optional[bool] = True,
+            bases: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            quotes: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            included: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None,
+            excluded: Optional[Union[Dict[str, Iterable[str]], Iterable[str]]] = None
+    ) -> SymbolsOrdersMarketState:
+        """
+        Fetches the values and relations between the assets.
+
+        :param length: The length of the values.
+        :param adjust: The value to adjust the length of the sequences.
+        :param exchanges: The exchanges.
+        :param quotes: The quotes of the asset pairs.
+        :param excluded: The excluded symbols.
+        :param adjust: The value to adjust the invalid exchanges.
+        :param separator: The separator of the assets.
+        :param included: The symbols to include.
+        :param bases: The bases of the asset pairs.
+
+        :return: The values of the assets.
+        """
+
+        screeners = exchanges_symbols_screeners(
+            screeners=self.screeners, exchanges=exchanges,
+            separator=separator, bases=bases, quotes=quotes,
+            included=included, excluded=excluded, adjust=adjust
+        )
+
+        return symbols_orders_market_state(
+            screeners=screeners, length=length, adjust=adjust
+        )
+    # end symbols_orders_market_state
 # end DynamicScreener
```

### Comparing `crypto-screening-4.1.3/crypto_screening/market/foundation/data.py` & `crypto-screening-5.1.0/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/market/foundation/protocols.py` & `crypto-screening-5.1.0/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/market/foundation/state.py` & `crypto-screening-5.1.0/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/market/foundation/waiting.py` & `crypto-screening-5.1.0/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/market/screeners/base.py` & `crypto-screening-5.1.0/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/market/screeners/container.py` & `crypto-screening-5.1.0/crypto_screening/market/screeners/container.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 # container.py
 
-from typing import Iterable, List
+from typing import Iterable, List, Type, TypeVar, Optional
 
 from represent import Modifiers
 
 from crypto_screening.market.screeners.recorder import (
     structure_screener_datasets, MarketRecorder
 )
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.ohlcv import OHLCVScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
+from crypto_screening.market.screeners.trades import TradesScreener
+from crypto_screening.market.screeners.orders import OrdersScreener
+
+_S = TypeVar("_S")
 
 class ScreenersContainer(MarketRecorder):
     """
     A class to represent a multi-exchange multi-pairs crypto data screener.
     Using this class enables extracting screener objects and screeners
     data by the exchange name and the symbol of the pair.
 
@@ -46,114 +50,186 @@
         """
 
         super().__init__(market=structure_screener_datasets(screeners=screeners))
 
         self.screeners = screeners
     # end __init__
 
-    def find_screeners(self, exchange: str, symbol: str) -> List[BaseScreener]:
+    def find_screener(
+            self, exchange: str, symbol: str, base: Optional[Type[_S]] = None
+    ) -> _S:
         """
         Returns the data by according to the parameters.
 
+        :param base: The base type of the screener.
         :param exchange: The exchange name.
         :param symbol: The ticker name.
 
         :return: The data.
         """
 
-        if not self.in_market(exchange=exchange, symbol=symbol):
-            raise ValueError(
-                f"Screener object for symbol - {symbol} and "
-                f"exchange - {exchange} cannot be found in {repr(self)}."
-            )
-        # end if
+        for screener in self.screeners:
+            if (
+                (screener.exchange == exchange) and
+                (screener.symbol == symbol) and
+                isinstance(screener, base or BaseScreener)
+            ):
+                return screener
+            # end if
+        # end for
+
+        raise ValueError(
+            f"{base} Screener object for symbol - {symbol} and "
+            f"exchange - {exchange} cannot be found in {repr(self)}."
+        )
+    # end find_orderbook_screener
+
+    def find_screeners(
+            self, exchange: str, symbol: str, base: Optional[Type[_S]] = None
+    ) -> List[_S]:
+        """
+        Returns the data by according to the parameters.
+
+        :param base: The base type of the screener.
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+
+        :return: The data.
+        """
 
         screeners = []
 
         for screener in self.screeners:
-            if (screener.exchange == exchange) and (screener.symbol == symbol):
+            if (
+                (screener.exchange == exchange) and
+                (screener.symbol == symbol) and
+                isinstance(screener, base or BaseScreener)
+            ):
                 screeners.append(screener)
             # end if
         # end for
 
         return screeners
     # end find_screeners
 
-    def orderbook_screener_in_market(self, exchange: str, symbol: str) -> bool:
+    def screener_in_market(
+            self, exchange: str, symbol: str, base: Optional[Type[_S]] = None
+    ) -> bool:
         """
         Returns the data by according to the parameters.
 
+        :param base: The base type of the screener.
         :param exchange: The exchange name.
         :param symbol: The ticker name.
 
         :return: The data.
         """
 
         try:
-            self.find_orderbook_screener(
-                exchange=exchange, symbol=symbol
+            self.find_screener(
+                exchange=exchange, symbol=symbol, base=base
             )
 
             return True
 
         except ValueError:
             return False
+        # end try
+    # end screener_in_market
+
+    def orderbook_screener_in_market(self, exchange: str, symbol: str) -> bool:
+        """
+        Returns the data by according to the parameters.
+
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+
+        :return: The data.
+        """
+
+        return self.screener_in_market(
+            exchange=exchange, symbol=symbol, base=OrderbookScreener
+        )
     # end orderbook_screener_in_market
 
-    def find_orderbook_screener(self, exchange: str, symbol: str) -> OrderbookScreener:
+    def orders_screener_in_market(self, exchange: str, symbol: str) -> bool:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
         :param symbol: The ticker name.
 
         :return: The data.
         """
 
-        for screener in self.screeners:
-            if (
-                (screener.exchange == exchange) and
-                (screener.symbol == symbol) and
-                isinstance(screener, OrderbookScreener)
-            ):
-                return screener
-            # end if
-        # end for
+        return self.screener_in_market(
+            exchange=exchange, symbol=symbol, base=OrdersScreener
+        )
+    # end orders_screener_in_market
 
-        raise ValueError(
-            f"Orderbook Screener object for symbol - {symbol} and "
-            f"exchange - {exchange} cannot be found in {repr(self)}."
+    def find_orderbook_screener(self, exchange: str, symbol: str) -> OrderbookScreener:
+        """
+        Returns the data by according to the parameters.
+
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+
+        :return: The data.
+        """
+
+        return self.find_screener(
+            exchange=exchange, symbol=symbol, base=OrderbookScreener
         )
     # end find_orderbook_screener
 
-    def find_orderbook_screeners(self, exchange: str, symbol: str) -> List[OrderbookScreener]:
+    def find_orders_screener(self, exchange: str, symbol: str) -> OrdersScreener:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
         :param symbol: The ticker name.
 
         :return: The data.
         """
 
-        screeners = []
+        return self.find_screener(
+            exchange=exchange, symbol=symbol, base=OrdersScreener
+        )
+    # end find_orders_screener
 
-        for screener in self.screeners:
-            if (
-                (screener.exchange == exchange) and
-                (screener.symbol == symbol) and
-                isinstance(screener, OrderbookScreener)
-            ):
-                screeners.append(screener)
-            # end if
-        # end for
+    def find_orderbook_screeners(self, exchange: str, symbol: str) -> List[OrderbookScreener]:
+        """
+        Returns the data by according to the parameters.
 
-        return screeners
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+
+        :return: The data.
+        """
+
+        return self.find_screeners(
+            exchange=exchange, symbol=symbol, base=OrderbookScreener
+        )
     # end find_orderbook_screener
 
+    def find_orders_screeners(self, exchange: str, symbol: str) -> List[OrdersScreener]:
+        """
+        Returns the data by according to the parameters.
+
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+
+        :return: The data.
+        """
+
+        return self.find_screeners(
+            exchange=exchange, symbol=symbol, base=OrdersScreener
+        )
+    # end find_orders_screeners
+
     def ohlcv_screener_in_market(
             self, exchange: str, symbol: str, interval: str
     ) -> bool:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
@@ -170,14 +246,29 @@
 
             return True
 
         except ValueError:
             return False
     # end ohlcv_screener_in_market
 
+    def trades_screener_in_market(self, exchange: str, symbol: str) -> bool:
+        """
+        Returns the data by according to the parameters.
+
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+
+        :return: The data.
+        """
+
+        return self.screener_in_market(
+            exchange=exchange, symbol=symbol, base=TradesScreener
+        )
+    # end trades_screener_in_market
+
     def find_ohlcv_screener(
             self, exchange: str, symbol: str, interval: str
     ) -> OHLCVScreener:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
@@ -200,14 +291,29 @@
 
         raise ValueError(
             f"OHLCV Screener object for symbol - {symbol} and "
             f"exchange - {exchange} cannot be found in {repr(self)}."
         )
     # end find_screeners
 
+    def find_trades_screener(self, exchange: str, symbol: str) -> TradesScreener:
+        """
+        Returns the data by according to the parameters.
+
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+
+        :return: The data.
+        """
+
+        return self.find_screener(
+            exchange=exchange, symbol=symbol, base=TradesScreener
+        )
+    # end find_trades_screener
+
     def find_ohlcv_screeners(
             self, exchange: str, symbol: str, interval: str
     ) -> List[OHLCVScreener]:
         """
         Returns the data by according to the parameters.
 
         :param exchange: The exchange name.
@@ -227,9 +333,24 @@
                 isinstance(screener, OHLCVScreener)
             ):
                 screeners.append(screener)
             # end if
         # end for
 
         return screeners
-    # end find_orderbook_screener
+    # end find_ohlcv_screeners
+
+    def find_trades_screeners(self, exchange: str, symbol: str) -> List[TradesScreener]:
+        """
+        Returns the data by according to the parameters.
+
+        :param exchange: The exchange name.
+        :param symbol: The ticker name.
+
+        :return: The data.
+        """
+
+        return self.find_screeners(
+            exchange=exchange, symbol=symbol, base=TradesScreener
+        )
+    # end find_trades_screeners
 # end ScreenersContainer
```

### Comparing `crypto-screening-4.1.3/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-5.1.0/crypto_screening/market/screeners/ohlcv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # ohlcv.py
 
 import datetime as dt
 from typing import (
-    Dict, Optional, Iterable, Any, Union, List
+    Dict, Optional, Iterable, Any, Union, List, Callable
 )
 
 import pandas as pd
 
 from represent import Modifiers
 
 from cryptofeed import FeedHandler
 from cryptofeed.types import OrderBook
+from cryptofeed.defines import L2_BOOK
 
 from crypto_screening.process import find_string_value
 from crypto_screening.interval import interval_to_total_time
 from crypto_screening.dataset import (
     OHLCV_COLUMNS, VOLUME, BIDS, BIDS_VOLUME,
     load_dataset, save_dataset, OHLC_COLUMNS, create_market_dataframe
 )
@@ -196,15 +197,18 @@
         Creates the path to the saving file for the screener object.
 
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
-        return self.dataset_path(location=location)
+        return (
+            self.dataset_path(location=location).
+            replace(".csv", f"-ORDERBOOK.csv")
+        )
     # end orderbook_dataset_path
 
     def save_orderbook_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
         :param location: The saving location of the dataset.
@@ -225,15 +229,15 @@
         :param location: The saving location of the dataset.
 
         :return: The saving path for the dataset.
         """
 
         return (
             self.dataset_path(location=location).
-            replace(".csv", f"-{self.interval}.csv")
+            replace(".csv", f"-OHLCV-{self.interval}.csv")
         )
     # end ohlcv_dataset_path
 
     def save_ohlcv_dataset(self, location: Optional[str] = None) -> None:
         """
         Saves the data of the screener.
 
@@ -577,14 +581,16 @@
             indexes[exchange][symbol][interval] += 1
         # end for
     # end for
 
     return True
 # end record_ohlcv
 
+RecorderParameters = Dict[str, Union[Iterable[str], Dict[str, Callable]]]
+
 class OHLCVMarketRecorder(OrderbookMarketRecorder):
     """
     A class to represent a crypto data feed recorder.
     This object passes the record method to the handler object to record
     the data fetched by the handler.
 
     Parameters:
@@ -666,14 +672,39 @@
 
         :return: The valid data.
         """
 
         return validate_intervals(data=data)
     # end validate_market
 
+    @property
+    def orderbook_market(self) -> Market:
+        """
+        Returns the market to hold the recorder data.
+
+        :return: The market object.
+        """
+
+        return self.market
+    # end orderbook_market
+
+    def parameters(self) -> RecorderParameters:
+        """
+        Returns the order book parameters.
+
+        :return: The order book parameters.
+        """
+
+        return dict(
+            channels=[L2_BOOK],
+            callbacks={L2_BOOK: self.record},
+            max_depth=1
+        )
+    # end parameters
+
     def ohlcv(self, exchange: str, symbol: str, interval: str) -> pd.DataFrame:
         """
         Returns the market data of the symbol from the exchange.
 
         :param exchange: The source name of the exchange.
         :param symbol: The symbol of the pair.
         :param interval: The interval for the dataset.
@@ -812,19 +843,19 @@
 
     - handler:
         The handler object to handle the data feed.
 
     - recorder:
         The recorder object to record the data of the market from the feed.
 
-    >>> from crypto_screening.market.screeners import orderbook_market_screener
+    >>> from crypto_screening.market.screeners import ohlcv_market_screener
     >>>
     >>> structure = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
-    >>> screener = orderbook_market_screener(data=structure)
+    >>> screener = ohlcv_market_screener(data=structure)
     >>> screener.run()
     """
 
     screeners: List[Union[OHLCVScreener, OrderbookScreener]]
     recorder: OHLCVMarketRecorder
 
     COLUMNS = OHLCVMarketRecorder.COLUMNS
```

### Comparing `crypto-screening-4.1.3/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-5.1.0/crypto_screening/market/screeners/orderbook.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,21 +10,20 @@
 from cryptofeed import FeedHandler
 from cryptofeed.types import OrderBook
 from cryptofeed.defines import L2_BOOK
 
 from crypto_screening.symbols import adjust_symbol
 from crypto_screening.process import find_string_value
 from crypto_screening.dataset import (
-    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME,
-    create_market_dataframe
+    BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, save_dataset,
+    create_market_dataframe, ORDERBOOK_COLUMNS, load_dataset
 )
-from crypto_screening.market.screeners.recorder import MarketRecorder
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.recorder import (
-    MarketScreener, structure_screener_datasets
+    MarketScreener, structure_screener_datasets, MarketRecorder
 )
 
 __all__ = [
     "OrderbookMarketScreener",
     "OrderbookMarketRecorder",
     "OrderbookScreener",
     "create_orderbook_market",
@@ -44,15 +43,15 @@
     """
 
     return create_market_dataframe(
         columns=OrderbookMarketRecorder.COLUMNS
     )
 # end create_orderbook_dataframe
 
-def create_orderbook_market(data: Dict[str, Iterable[str]]) -> Dict[str, Dict[str, pd.DataFrame]]:
+def create_orderbook_market(data: Dict[str, Iterable[str]]) -> Market:
     """
     Creates the dataframes of the market data.
 
     :param data: The market data.
 
     :return: The dataframes of the market data.
     """
@@ -89,54 +88,90 @@
 
     - delay:
         The delay to wait between each data fetching.
 
     - market:
         The dataset of the market data as BID/ASK spread.
     """
-# end OrderBookScreener
 
-def validate_orderbook_market(data: Any) -> Market:
-    """
-    Validates the data.
+    @property
+    def orderbook_market(self) -> pd.DataFrame:
+        """
+        Returns the market to hold the recorder data.
+
+        :return: The market object.
+        """
 
-    :param data: The data to validate.
+        return self.market
+    # end orderbook_market
 
-    :return: The valid data.
-    """
+    def orderbook_dataset_path(self, location: Optional[str] = None) -> str:
+        """
+        Creates the path to the saving file for the screener object.
 
-    try:
-        if not isinstance(data, dict):
-            raise ValueError
+        :param location: The saving location of the dataset.
+
+        :return: The saving path for the dataset.
+        """
+
+        return (
+            self.dataset_path(location=location).
+            replace(".csv", f"-ORDERBOOK.csv")
+        )
+    # end orderbook_dataset_path
+
+    def save_orderbook_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        if len(self.orderbook_market) > 0:
+            save_dataset(
+                dataset=self.orderbook_market,
+                path=self.orderbook_dataset_path(location=location)
+            )
         # end if
+    # end save_orderbook_dataset
+
+    def save_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
+
+        self.save_orderbook_dataset(location=location)
+    # end save_dataset
+
+    def load_orderbook_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
+
+        :param location: The saving location of the dataset.
+        """
 
-        for exchange, values in data.items():
-            if not (
-                isinstance(exchange, str) and
-                (
-                    isinstance(values, dict) and
-                    all(
-                        isinstance(symbol, str) and
-                        isinstance(dataset, pd.DataFrame)
-                        for symbol, dataset in values.items()
-                    )
-                )
-            ):
-                raise ValueError
-            # end if
+        data = load_dataset(path=self.orderbook_dataset_path(location=location))
+
+        for index, data in zip(data.index[:], data.loc[:]):
+            self.orderbook_market.loc[index] = data
         # end for
+    # end load_orderbook_dataset
 
-    except (TypeError, ValueError):
-        raise ValueError(
-            f"Data must be of type {Market}, not: {data}."
-        )
-    # end try
+    def load_dataset(self, location: Optional[str] = None) -> None:
+        """
+        Saves the data of the screener.
 
-    return data
-# end validate_orderbook_market
+        :param location: The saving location of the dataset.
+        """
+
+        self.load_orderbook_dataset(location=location)
+    # end load_dataset
+# end OrderbookScreener
 
 def record_orderbook(market: Market, data: OrderBook, timestamp: float) -> bool:
     """
     Records the data from the crypto feed into the dataset.
 
     :param market: The market structure.
     :param data: The data from the exchange.
@@ -194,28 +229,15 @@
     >>> from crypto_screening.market.screeners import orderbook_market_recorder
     >>>
     >>> market = {'binance': ['BTC/USDT'], 'bittrex': ['ETH/USDT']}
     >>>
     >>> recorder = orderbook_market_recorder(data=market)
     """
 
-    COLUMNS = (BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME)
-
-    @staticmethod
-    def validate_market(data: Any) -> Market:
-        """
-        Validates the data.
-
-        :param data: The data to validate.
-
-        :return: The valid data.
-        """
-
-        return validate_orderbook_market(data=data)
-    # end validate_market
+    COLUMNS = ORDERBOOK_COLUMNS
 
     @property
     def orderbook_market(self) -> Market:
         """
         Returns the market to hold the recorder data.
 
         :return: The market object.
```

### Comparing `crypto-screening-4.1.3/crypto_screening/market/screeners/recorder.py` & `crypto-screening-5.1.0/crypto_screening/market/screeners/recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,22 +171,22 @@
     try:
         if not isinstance(data, dict):
             raise ValueError
         # end if
 
         for exchange, values in data.items():
             if not (
-                    isinstance(exchange, str) and
-                    (
-                            isinstance(values, dict) and
-                            all(
-                                isinstance(symbol, str)
-                                for symbol, _ in values.items()
-                            )
+                isinstance(exchange, str) and
+                (
+                    isinstance(values, dict) and
+                    all(
+                        isinstance(symbol, str)
+                        for symbol, _ in values.items()
                     )
+                )
             ):
                 raise ValueError
             # end if
         # end for
 
     except (TypeError, ValueError):
         raise ValueError(
@@ -409,27 +409,31 @@
 
         self.loop: Optional[asyncio.AbstractEventLoop] = None
 
         self._feeds_parameters: Optional[Dict[str, Any]] = None
         self._run_parameters: Optional[Dict[str, Any]] = None
     # end __init__
 
+    def connect_screeners(self) -> None:
+        """Connects the screeners to the recording object."""
+    # end connect_screeners
+
     def structure(self) -> Dict[str, List[str]]:
         """
         Returns the structure of the market data.
 
         :return: The structure of the market.
         """
 
         return self.recorder.structure()
     # end structure
 
     def add_feeds(
             self,
-            data: Dict[str, Iterable[str]],
+            data: Optional[Dict[str, Iterable[str]]] = None,
             fixed: Optional[bool] = True,
             separator: Optional[str] = None,
             amount: Optional[int] = None,
             parameters: Optional[Union[Dict[str, Dict[str, Any]], Dict[str, Any]]] = None
     ) -> None:
         """
         Adds the symbols to the handler for each exchange.
@@ -437,14 +441,18 @@
         :param data: The data of the exchanges and symbols to add.
         :param parameters: The parameters for the exchanges.
         :param fixed: The value for fixed parameters to all exchanges.
         :param amount: The maximum amount of symbols for each feed.
         :param separator: The separator of the assets.
         """
 
+        if data is None:
+            data = self.structure()
+        # end if
+
         self._feeds_parameters = dict(
             data=data, fixed=fixed, separator=separator,
             parameters=parameters
         )
 
         feed_params = self.recorder.parameters()
         feed_params.update(parameters or {})
@@ -485,27 +493,14 @@
         # end if
 
         self.terminate()
         self.refresh_feeds()
         self.run(**self._run_parameters)
     # end rerun
 
-    def orderbook(self, exchange: str, symbol: str) -> pd.DataFrame:
-        """
-        Returns the market data of the symbol from the exchange.
-
-        :param exchange: The source name of the exchange.
-        :param symbol: The symbol of the pair.
-
-        :return: The dataset of the spread data.
-        """
-
-        return self.recorder.orderbook(exchange=exchange, symbol=symbol)
-    # end orderbook
-
     def screening_loop(
             self,
             start: Optional[bool] = True,
             loop: Optional[asyncio.AbstractEventLoop] = None
     ) -> None:
         """
         Runs the process of the price screening.
```

### Comparing `crypto-screening-4.1.3/crypto_screening/market/waiting.py` & `crypto-screening-5.1.0/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/process.py` & `crypto-screening-5.1.0/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/symbols.py` & `crypto-screening-5.1.0/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening/validate.py` & `crypto-screening-5.1.0/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-4.1.3/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-5.1.0/crypto_screening.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 4.1.3
+Version: 5.1.0
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-4.1.3/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-5.1.0/crypto_screening.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -17,21 +17,26 @@
 crypto_screening.egg-info/requires.txt
 crypto_screening.egg-info/top_level.txt
 crypto_screening/collect/assets.py
 crypto_screening/collect/exchanges.py
 crypto_screening/collect/market.py
 crypto_screening/collect/ohlcv.py
 crypto_screening/collect/orderbook.py
+crypto_screening/collect/orders.py
 crypto_screening/collect/screeners.py
 crypto_screening/collect/symbols.py
+crypto_screening/collect/trades.py
 crypto_screening/market/dynamic.py
 crypto_screening/market/waiting.py
 crypto_screening/market/foundation/data.py
 crypto_screening/market/foundation/protocols.py
 crypto_screening/market/foundation/state.py
 crypto_screening/market/foundation/waiting.py
 crypto_screening/market/screeners/__init__.py
 crypto_screening/market/screeners/base.py
+crypto_screening/market/screeners/combined.py
 crypto_screening/market/screeners/container.py
 crypto_screening/market/screeners/ohlcv.py
 crypto_screening/market/screeners/orderbook.py
-crypto_screening/market/screeners/recorder.py
+crypto_screening/market/screeners/orders.py
+crypto_screening/market/screeners/recorder.py
+crypto_screening/market/screeners/trades.py
```

### Comparing `crypto-screening-4.1.3/pyproject.toml` & `crypto-screening-5.1.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '4.1.3'
+version = '5.1.0'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-4.1.3/setup.py` & `crypto-screening-5.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='4.1.3',
+        version='5.1.0',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

