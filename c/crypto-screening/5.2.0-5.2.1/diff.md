# Comparing `tmp/crypto-screening-5.2.0.tar.gz` & `tmp/crypto-screening-5.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crypto-screening-5.2.0.tar", last modified: Sat Jul 15 09:52:48 2023, max compression
+gzip compressed data, was "crypto-screening-5.2.1.tar", last modified: Sat Jul 15 09:56:17 2023, max compression
```

## Comparing `crypto-screening-5.2.0.tar` & `crypto-screening-5.2.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 09:52:48.309792 crypto-screening-5.2.0/
--rw-rw-rw-   0        0        0       98 2023-07-15 09:52:47.000000 crypto-screening-5.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2059 2023-07-15 09:52:48.309792 crypto-screening-5.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.2.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.2.0/build.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:52:48.280244 crypto-screening-5.2.0/crypto_screening/
-drwxrwxrwx   0        0        0        0 2023-07-15 09:52:48.296281 crypto-screening-5.2.0/crypto_screening/collect/
--rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.2.0/crypto_screening/collect/assets.py
--rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.2.0/crypto_screening/collect/exchanges.py
--rw-rw-rw-   0        0        0    45470 2023-07-15 01:39:05.000000 crypto-screening-5.2.0/crypto_screening/collect/market.py
--rw-rw-rw-   0        0        0    21227 2023-07-15 01:09:32.000000 crypto-screening-5.2.0/crypto_screening/collect/ohlcv.py
--rw-rw-rw-   0        0        0    19348 2023-07-15 01:09:32.000000 crypto-screening-5.2.0/crypto_screening/collect/orderbook.py
--rw-rw-rw-   0        0        0    14460 2023-07-15 01:09:32.000000 crypto-screening-5.2.0/crypto_screening/collect/orders.py
--rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-5.2.0/crypto_screening/collect/screeners.py
--rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.2.0/crypto_screening/collect/symbols.py
--rw-rw-rw-   0        0        0    16881 2023-07-15 09:52:06.000000 crypto-screening-5.2.0/crypto_screening/collect/trades.py
--rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.2.0/crypto_screening/dataset.py
--rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.2.0/crypto_screening/exchanges.py
--rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.2.0/crypto_screening/interval.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:52:48.298788 crypto-screening-5.2.0/crypto_screening/market/
--rw-rw-rw-   0        0        0    19625 2023-07-15 09:29:18.000000 crypto-screening-5.2.0/crypto_screening/market/dynamic.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:52:48.301804 crypto-screening-5.2.0/crypto_screening/market/foundation/
--rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-5.2.0/crypto_screening/market/foundation/data.py
--rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.2.0/crypto_screening/market/foundation/protocols.py
--rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.2.0/crypto_screening/market/foundation/state.py
--rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.2.0/crypto_screening/market/foundation/waiting.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:52:48.308793 crypto-screening-5.2.0/crypto_screening/market/screeners/
--rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.2.0/crypto_screening/market/screeners/__init__.py
--rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-5.2.0/crypto_screening/market/screeners/base.py
--rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.2.0/crypto_screening/market/screeners/combined.py
--rw-rw-rw-   0        0        0    12093 2023-07-15 09:25:40.000000 crypto-screening-5.2.0/crypto_screening/market/screeners/container.py
--rw-rw-rw-   0        0        0    36896 2023-07-15 00:16:21.000000 crypto-screening-5.2.0/crypto_screening/market/screeners/ohlcv.py
--rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.2.0/crypto_screening/market/screeners/orderbook.py
--rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.2.0/crypto_screening/market/screeners/orders.py
--rw-rw-rw-   0        0        0    20288 2023-07-14 23:48:05.000000 crypto-screening-5.2.0/crypto_screening/market/screeners/recorder.py
--rw-rw-rw-   0        0        0    18063 2023-07-15 00:10:09.000000 crypto-screening-5.2.0/crypto_screening/market/screeners/trades.py
--rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.2.0/crypto_screening/market/waiting.py
--rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.2.0/crypto_screening/process.py
--rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.2.0/crypto_screening/symbols.py
--rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-5.2.0/crypto_screening/validate.py
-drwxrwxrwx   0        0        0        0 2023-07-15 09:52:48.289278 crypto-screening-5.2.0/crypto_screening.egg-info/
--rw-rw-rw-   0        0        0     2059 2023-07-15 09:52:48.000000 crypto-screening-5.2.0/crypto_screening.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1443 2023-07-15 09:52:48.000000 crypto-screening-5.2.0/crypto_screening.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 09:52:48.000000 crypto-screening-5.2.0/crypto_screening.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       95 2023-07-15 09:52:48.000000 crypto-screening-5.2.0/crypto_screening.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-07-15 09:52:48.000000 crypto-screening-5.2.0/crypto_screening.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      652 2023-07-15 09:52:47.000000 crypto-screening-5.2.0/pyproject.toml
--rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.2.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-15 09:52:48.309792 crypto-screening-5.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1579 2023-07-15 09:52:41.000000 crypto-screening-5.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.993766 crypto-screening-5.2.1/
+-rw-rw-rw-   0        0        0       98 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2059 2023-07-15 09:56:17.993766 crypto-screening-5.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1238 2023-07-01 07:09:50.000000 crypto-screening-5.2.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-06-23 16:52:27.000000 crypto-screening-5.2.1/build.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.967653 crypto-screening-5.2.1/crypto_screening/
+drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.982750 crypto-screening-5.2.1/crypto_screening/collect/
+-rw-rw-rw-   0        0        0    17727 2023-06-30 14:15:11.000000 crypto-screening-5.2.1/crypto_screening/collect/assets.py
+-rw-rw-rw-   0        0        0     4767 2023-07-10 17:17:46.000000 crypto-screening-5.2.1/crypto_screening/collect/exchanges.py
+-rw-rw-rw-   0        0        0    45470 2023-07-15 01:39:05.000000 crypto-screening-5.2.1/crypto_screening/collect/market.py
+-rw-rw-rw-   0        0        0    21227 2023-07-15 01:09:32.000000 crypto-screening-5.2.1/crypto_screening/collect/ohlcv.py
+-rw-rw-rw-   0        0        0    19348 2023-07-15 01:09:32.000000 crypto-screening-5.2.1/crypto_screening/collect/orderbook.py
+-rw-rw-rw-   0        0        0    14460 2023-07-15 01:09:32.000000 crypto-screening-5.2.1/crypto_screening/collect/orders.py
+-rw-rw-rw-   0        0        0    18206 2023-07-14 12:25:47.000000 crypto-screening-5.2.1/crypto_screening/collect/screeners.py
+-rw-rw-rw-   0        0        0    18977 2023-07-14 12:28:29.000000 crypto-screening-5.2.1/crypto_screening/collect/symbols.py
+-rw-rw-rw-   0        0        0    16881 2023-07-15 09:52:06.000000 crypto-screening-5.2.1/crypto_screening/collect/trades.py
+-rw-rw-rw-   0        0        0    14387 2023-07-14 22:07:04.000000 crypto-screening-5.2.1/crypto_screening/dataset.py
+-rw-rw-rw-   0        0        0      258 2023-06-25 14:21:21.000000 crypto-screening-5.2.1/crypto_screening/exchanges.py
+-rw-rw-rw-   0        0        0     5404 2023-07-14 06:26:34.000000 crypto-screening-5.2.1/crypto_screening/interval.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.984749 crypto-screening-5.2.1/crypto_screening/market/
+-rw-rw-rw-   0        0        0    19625 2023-07-15 09:29:18.000000 crypto-screening-5.2.1/crypto_screening/market/dynamic.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.986750 crypto-screening-5.2.1/crypto_screening/market/foundation/
+-rw-rw-rw-   0        0        0    10765 2023-07-04 21:19:28.000000 crypto-screening-5.2.1/crypto_screening/market/foundation/data.py
+-rw-rw-rw-   0        0        0      891 2023-07-04 21:20:28.000000 crypto-screening-5.2.1/crypto_screening/market/foundation/protocols.py
+-rw-rw-rw-   0        0        0     1330 2023-07-06 12:49:09.000000 crypto-screening-5.2.1/crypto_screening/market/foundation/state.py
+-rw-rw-rw-   0        0        0     6860 2023-07-12 22:15:07.000000 crypto-screening-5.2.1/crypto_screening/market/foundation/waiting.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.992766 crypto-screening-5.2.1/crypto_screening/market/screeners/
+-rw-rw-rw-   0        0        0      461 2023-07-14 23:45:34.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/__init__.py
+-rw-rw-rw-   0        0        0    10966 2023-07-14 07:29:46.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/base.py
+-rw-rw-rw-   0        0        0    12636 2023-07-15 00:35:55.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/combined.py
+-rw-rw-rw-   0        0        0    12093 2023-07-15 09:56:14.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/container.py
+-rw-rw-rw-   0        0        0    36896 2023-07-15 00:16:21.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/ohlcv.py
+-rw-rw-rw-   0        0        0    18524 2023-07-15 00:10:09.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/orderbook.py
+-rw-rw-rw-   0        0        0    18029 2023-07-15 00:10:09.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/orders.py
+-rw-rw-rw-   0        0        0    20288 2023-07-14 23:48:05.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/recorder.py
+-rw-rw-rw-   0        0        0    18063 2023-07-15 00:10:09.000000 crypto-screening-5.2.1/crypto_screening/market/screeners/trades.py
+-rw-rw-rw-   0        0        0     3887 2023-07-12 22:15:36.000000 crypto-screening-5.2.1/crypto_screening/market/waiting.py
+-rw-rw-rw-   0        0        0     2382 2023-06-30 14:15:11.000000 crypto-screening-5.2.1/crypto_screening/process.py
+-rw-rw-rw-   0        0        0     9972 2023-07-06 12:49:43.000000 crypto-screening-5.2.1/crypto_screening/symbols.py
+-rw-rw-rw-   0        0        0     4221 2023-07-14 06:26:34.000000 crypto-screening-5.2.1/crypto_screening/validate.py
+drwxrwxrwx   0        0        0        0 2023-07-15 09:56:17.976172 crypto-screening-5.2.1/crypto_screening.egg-info/
+-rw-rw-rw-   0        0        0     2059 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/crypto_screening.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1443 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/crypto_screening.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/crypto_screening.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       95 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/crypto_screening.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/crypto_screening.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2023-07-15 09:56:17.000000 crypto-screening-5.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0      100 2023-07-13 15:40:31.000000 crypto-screening-5.2.1/requirements-dev.txt
+-rw-rw-rw-   0        0        0       65 2023-07-13 15:40:31.000000 crypto-screening-5.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 09:56:17.993766 crypto-screening-5.2.1/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2023-07-15 09:56:14.000000 crypto-screening-5.2.1/setup.py
```

### Comparing `crypto-screening-5.2.0/PKG-INFO` & `crypto-screening-5.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.2.0
+Version: 5.2.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.2.0/README.md` & `crypto-screening-5.2.1/README.md`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/build.py` & `crypto-screening-5.2.1/build.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/collect/assets.py` & `crypto-screening-5.2.1/crypto_screening/collect/assets.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/collect/exchanges.py` & `crypto-screening-5.2.1/crypto_screening/collect/exchanges.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/collect/market.py` & `crypto-screening-5.2.1/crypto_screening/collect/market.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/collect/ohlcv.py` & `crypto-screening-5.2.1/crypto_screening/collect/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/collect/orderbook.py` & `crypto-screening-5.2.1/crypto_screening/collect/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/collect/orders.py` & `crypto-screening-5.2.1/crypto_screening/collect/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/collect/screeners.py` & `crypto-screening-5.2.1/crypto_screening/collect/screeners.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/collect/symbols.py` & `crypto-screening-5.2.1/crypto_screening/collect/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/collect/trades.py` & `crypto-screening-5.2.1/crypto_screening/collect/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/dataset.py` & `crypto-screening-5.2.1/crypto_screening/dataset.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/interval.py` & `crypto-screening-5.2.1/crypto_screening/interval.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/dynamic.py` & `crypto-screening-5.2.1/crypto_screening/market/dynamic.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/foundation/data.py` & `crypto-screening-5.2.1/crypto_screening/market/foundation/data.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/foundation/protocols.py` & `crypto-screening-5.2.1/crypto_screening/market/foundation/protocols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/foundation/state.py` & `crypto-screening-5.2.1/crypto_screening/market/foundation/state.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/foundation/waiting.py` & `crypto-screening-5.2.1/crypto_screening/market/foundation/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/screeners/base.py` & `crypto-screening-5.2.1/crypto_screening/market/screeners/base.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/screeners/combined.py` & `crypto-screening-5.2.1/crypto_screening/market/screeners/combined.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/screeners/container.py` & `crypto-screening-5.2.1/crypto_screening/market/screeners/container.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,16 +334,16 @@
         :return: The data.
         """
 
         for screener in self.screeners:
             if (
                 (screener.exchange == exchange) and
                 (screener.symbol == symbol) and
-                (screener.interval == interval) and
-                isinstance(screener, OHLCVScreener)
+                isinstance(screener, OHLCVScreener) and
+                (screener.interval == interval)
             ):
                 return screener
             # end if
         # end for
 
         raise ValueError(
             f"OHLCV Screener object for symbol - {symbol} and "
```

### Comparing `crypto-screening-5.2.0/crypto_screening/market/screeners/ohlcv.py` & `crypto-screening-5.2.1/crypto_screening/market/screeners/ohlcv.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/screeners/orderbook.py` & `crypto-screening-5.2.1/crypto_screening/market/screeners/orderbook.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/screeners/orders.py` & `crypto-screening-5.2.1/crypto_screening/market/screeners/orders.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/screeners/recorder.py` & `crypto-screening-5.2.1/crypto_screening/market/screeners/recorder.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/screeners/trades.py` & `crypto-screening-5.2.1/crypto_screening/market/screeners/trades.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/market/waiting.py` & `crypto-screening-5.2.1/crypto_screening/market/waiting.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/process.py` & `crypto-screening-5.2.1/crypto_screening/process.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/symbols.py` & `crypto-screening-5.2.1/crypto_screening/symbols.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening/validate.py` & `crypto-screening-5.2.1/crypto_screening/validate.py`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/crypto_screening.egg-info/PKG-INFO` & `crypto-screening-5.2.1/crypto_screening.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crypto-screening
-Version: 5.2.0
+Version: 5.2.1
 Summary: A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.
 Home-page: https://github.com/Shahaf-F-S/crypto-screening
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `crypto-screening-5.2.0/crypto_screening.egg-info/SOURCES.txt` & `crypto-screening-5.2.1/crypto_screening.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crypto-screening-5.2.0/pyproject.toml` & `crypto-screening-5.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'crypto-screening'
-version = '5.2.0'
+version = '5.2.1'
 description = 'A software for automatically recording real-time crypto exchanges and pairs OHLCV and Orderbook rates.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `crypto-screening-5.2.0/setup.py` & `crypto-screening-5.2.1/setup.py`

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
-        version='5.2.0',
+        version='5.2.1',
         description=(
             "A software for automatically recording "
             "real-time crypto exchanges and pairs "
             "OHLCV and Orderbook rates."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

