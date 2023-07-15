# Comparing `tmp/crypto-screening-5.2.1.tar.gz` & `tmp/crypto-screening-5.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-5.2.1.tar", last modified: Sat Jul 15 09:56:17 2023, max compression
+gzip compressed data, was "crypto-screening-5.2.2.tar", last modified: Sat Jul 15 10:26:59 2023, max compression
```

## Comparing `crypto-screening-5.2.1.tar` & `crypto-screening-5.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.993766 crypto-screening-5.2.1/
--rw-rw-rw-   0        0        0       98 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-15 09:56:17.993766 crypto-screening-5.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.2.1/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.2.1/build.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.967653 crypto-screening-5.2.1/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.982750 crypto-screening-5.2.1/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.2.1/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.2.1/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    45470 2023-07-15 01:39:05.000000 crypto-screening-5.2.1/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21227 2023-07-15 01:09:32.000000 crypto-screening-5.2.1/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19348 2023-07-15 01:09:32.000000 crypto-screening-5.2.1/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    14460 2023-07-15 01:09:32.000000 crypto-screening-5.2.1/crypto_screening/collect/orders.py
--rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-5.2.1/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.2.1/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    16881 2023-07-15 09:52:06.000000 crypto-screening-5.2.1/crypto_screening/collect/trades.py
--rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.2.1/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.2.1/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.2.1/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.984749 crypto-screening-5.2.1/crypto_screening/market/
--rw-rw-rw-   0        0        0    19625 2023-07-15 09:29:18.000000 crypto-screening-5.2.1/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.986750 crypto-screening-5.2.1/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-5.2.1/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.2.1/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.2.1/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.2.1/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.992766 crypto-screening-5.2.1/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    36896 2023-07-15 00:16:21.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20288 2023-07-14 23:48:05.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    18063 2023-07-15 00:10:09.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.2.1/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.2.1/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.2.1/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-5.2.1/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.976172 crypto-screening-5.2.1/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.2.1/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.2.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 09:56:17.993766 crypto-screening-5.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-15 09:56:14.000000 crypto-screening-5.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.286264 crypto-screening-5.2.2/
+-rw-rw-rw-   0        0        0       98 2023-07-15 10:26:57.000000 crypto-screening-5.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-15 10:26:59.286264 crypto-screening-5.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.2.2/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.2.2/build.py
+drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.134692 crypto-screening-5.2.2/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.196630 crypto-screening-5.2.2/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.2.2/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.2.2/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    46167 2023-07-15 10:14:05.000000 crypto-screening-5.2.2/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21227 2023-07-15 01:09:32.000000 crypto-screening-5.2.2/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19348 2023-07-15 01:09:32.000000 crypto-screening-5.2.2/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    14460 2023-07-15 01:09:32.000000 crypto-screening-5.2.2/crypto_screening/collect/orders.py
+-rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-5.2.2/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.2.2/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    16881 2023-07-15 09:52:06.000000 crypto-screening-5.2.2/crypto_screening/collect/trades.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.2.2/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.2.2/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.2.2/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.206635 crypto-screening-5.2.2/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19625 2023-07-15 09:29:18.000000 crypto-screening-5.2.2/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.230665 crypto-screening-5.2.2/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-5.2.2/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.2.2/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.2.2/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.2.2/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.285263 crypto-screening-5.2.2/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    36896 2023-07-15 00:16:21.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20288 2023-07-14 23:48:05.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    18063 2023-07-15 00:10:09.000000 crypto-screening-5.2.2/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.2.2/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.2.2/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.2.2/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-5.2.2/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-15 10:26:59.149599 crypto-screening-5.2.2/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-15 10:26:59.000000 crypto-screening-5.2.2/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2023-07-15 10:26:59.000000 crypto-screening-5.2.2/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 10:26:59.000000 crypto-screening-5.2.2/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-15 10:26:59.000000 crypto-screening-5.2.2/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 10:26:59.000000 crypto-screening-5.2.2/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-15 10:26:57.000000 crypto-screening-5.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.2.2/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.2.2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 10:26:59.286264 crypto-screening-5.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-15 10:26:50.000000 crypto-screening-5.2.2/setup.py
```

### Comparing `crypto-screening-5.2.1/PKG-INFO` & `crypto-screening-5.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.2.1
+Version: 5.2.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.2.1/README.md` & `crypto-screening-5.2.2/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/build.py` & `crypto-screening-5.2.2/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/collect/assets.py` & `crypto-screening-5.2.2/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/collect/exchanges.py` & `crypto-screening-5.2.2/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/collect/market.py` & `crypto-screening-5.2.2/crypto_screening/collect/market.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,16 @@
 from crypto_screening.dataset import (
     BIDS, ASKS, BIDS_VOLUME, ASKS_VOLUME, bid_ask_to_ohlcv,
     OPEN, HIGH, LOW, CLOSE, VOLUME, AMOUNT, SIDE, PRICE
 )
 from crypto_screening.market.screeners.base import BaseScreener
 from crypto_screening.market.screeners.orderbook import OrderbookScreener
 from crypto_screening.market.screeners.ohlcv import OHLCVScreener
+from crypto_screening.market.screeners.orders import OrdersScreener
+from crypto_screening.market.screeners.trades import TradesScreener
 from crypto_screening.dataset import dataset_to_json
 from crypto_screening.symbols import symbol_to_parts, parts_to_symbol
 from crypto_screening.collect.screeners import (
     find_screeners, screeners_to_assets_datasets,
     screeners_to_symbols_datasets
 )
 
@@ -1039,25 +1041,35 @@
             screeners_collection.append(screener)
         # end for
     # end for
 
     return screeners_collection
 # end symbols_screeners
 
+
+SCREENER_ATTRIBUTES_MATCHES = {
+    OrderbookScreener: ORDERBOOK_ATTRIBUTES,
+    OHLCVScreener: OHLCV_ATTRIBUTES,
+    OrdersScreener: ORDERS_ATTRIBUTES,
+    TradesScreener: TRADES_ATTRIBUTES
+}
+
 def add_symbols_data_to_screeners(
         screeners: Iterable[BaseScreener],
         data: SymbolsMarketData,
-        adjust: Optional[bool] = True
+        adjust: Optional[bool] = True,
+        force: Optional[bool] = False
 ) -> None:
     """
     Updates the data of the screeners with the symbols data.
 
     :param screeners: The screeners to update.
     :param data: The new data to add to the screeners.
     :param adjust: The value to adjust with screeners that are not found.
+    :param force: The value to force the data into the screeners.
     """
 
     for exchange, symbols in data.items():
         for symbol, rows in symbols.items():
             found_screeners = find_screeners(
                 screeners, exchange=exchange, symbol=symbol
             )
@@ -1074,15 +1086,19 @@
                 for index, row in rows:
                     if (
                         isinstance(screener, OHLCVScreener) and
                         (set(row.keys()) == set(ORDERBOOK_ATTRIBUTES.values()))
                     ):
                         screener.base_market.loc[index] = row
 
-                    else:
+                    elif force or any(
+                        isinstance(screener, base) and
+                        (set(row.keys()) == set(attributes.values()))
+                        for base, attributes in SCREENER_ATTRIBUTES_MATCHES.items()
+                    ):
                         screener.market.loc[index] = row
                     # end if
                 # end for
             # end for
         # end for
     # end for
 # end add_symbols_data_to_screeners
```

### Comparing `crypto-screening-5.2.1/crypto_screening/collect/ohlcv.py` & `crypto-screening-5.2.2/crypto_screening/collect/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/collect/orderbook.py` & `crypto-screening-5.2.2/crypto_screening/collect/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/collect/orders.py` & `crypto-screening-5.2.2/crypto_screening/collect/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/collect/screeners.py` & `crypto-screening-5.2.2/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/collect/symbols.py` & `crypto-screening-5.2.2/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/collect/trades.py` & `crypto-screening-5.2.2/crypto_screening/collect/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/dataset.py` & `crypto-screening-5.2.2/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/interval.py` & `crypto-screening-5.2.2/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/dynamic.py` & `crypto-screening-5.2.2/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/foundation/data.py` & `crypto-screening-5.2.2/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/foundation/protocols.py` & `crypto-screening-5.2.2/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/foundation/state.py` & `crypto-screening-5.2.2/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/foundation/waiting.py` & `crypto-screening-5.2.2/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/screeners/base.py` & `crypto-screening-5.2.2/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/screeners/combined.py` & `crypto-screening-5.2.2/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/screeners/container.py` & `crypto-screening-5.2.2/crypto_screening/market/screeners/container.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-5.2.2/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-5.2.2/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/screeners/orders.py` & `crypto-screening-5.2.2/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/screeners/recorder.py` & `crypto-screening-5.2.2/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/screeners/trades.py` & `crypto-screening-5.2.2/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/market/waiting.py` & `crypto-screening-5.2.2/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/process.py` & `crypto-screening-5.2.2/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/symbols.py` & `crypto-screening-5.2.2/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening/validate.py` & `crypto-screening-5.2.2/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-5.2.2/crypto_screening.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.2.1
+Version: 5.2.2
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.2.1/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-5.2.2/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.1/pyproject.toml` & `crypto-screening-5.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '5.2.1'
+version = '5.2.2'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-5.2.1/setup.py` & `crypto-screening-5.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='crypto-screening',
-        version='5.2.1',
+        version='5.2.2',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

