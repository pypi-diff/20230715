# Comparing `tmp/local_candles-0.1.0.tar.gz` & `tmp/local_candles-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "local_candles-0.1.0.tar", max compression
+gzip compressed data, was "local_candles-0.1.1.tar", max compression
```

## Comparing `local_candles-0.1.0.tar` & `local_candles-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      332 2023-06-25 07:04:33.310152 local_candles-0.1.0/README.md
--rw-r--r--   0        0        0     1063 2023-06-25 06:53:20.249618 local_candles-0.1.0/local_candles/__init__.py
--rw-r--r--   0        0        0     3894 2023-06-22 16:57:38.435222 local_candles-0.1.0/local_candles/data.py
--rw-r--r--   0        0        0       54 2023-06-22 15:26:24.816691 local_candles-0.1.0/local_candles/models/__init__.py
--rw-r--r--   0        0        0     1671 2023-06-22 15:25:37.845750 local_candles-0.1.0/local_candles/models/interval.py
--rw-r--r--   0        0        0     1435 2023-06-22 15:25:09.829908 local_candles-0.1.0/local_candles/models/time.py
--rw-r--r--   0        0        0      558 2023-06-22 15:13:17.087278 local_candles-0.1.0/local_candles/sources/__init__.py
--rw-r--r--   0        0        0      355 2023-06-22 15:13:17.094295 local_candles-0.1.0/local_candles/sources/base.py
--rw-r--r--   0        0        0     2305 2023-06-22 15:13:17.086926 local_candles-0.1.0/local_candles/sources/binance_futures_ohlc.py
--rw-r--r--   0        0        0     2320 2023-06-22 15:13:17.087715 local_candles-0.1.0/local_candles/sources/binance_spot_ohlc.py
--rw-r--r--   0        0        0     2630 2023-06-22 15:13:17.086564 local_candles-0.1.0/local_candles/sources/csv_file.py
--rw-r--r--   0        0        0     2342 2023-06-22 15:13:17.093913 local_candles-0.1.0/local_candles/sources/gateio_spot_ohlc.py
--rw-r--r--   0        0        0     2271 2023-06-22 15:13:17.094778 local_candles-0.1.0/local_candles/sources/yahoo_finance_ohlc.py
--rw-r--r--   0        0        0      570 2023-06-22 15:21:16.285899 local_candles-0.1.0/local_candles/utils.py
--rw-r--r--   0        0        0      654 2023-06-25 07:09:16.219872 local_candles-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1101 1970-01-01 00:00:00.000000 local_candles-0.1.0/setup.py
--rw-r--r--   0        0        0     1139 1970-01-01 00:00:00.000000 local_candles-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      667 2023-06-25 07:11:26.007807 local_candles-0.1.1/README.md
+-rw-r--r--   0        0        0     1063 2023-06-25 06:53:20.249618 local_candles-0.1.1/local_candles/__init__.py
+-rw-r--r--   0        0        0     3875 2023-07-15 04:21:29.189728 local_candles-0.1.1/local_candles/data.py
+-rw-r--r--   0        0        0       54 2023-06-22 15:26:24.816691 local_candles-0.1.1/local_candles/models/__init__.py
+-rw-r--r--   0        0        0     1671 2023-06-22 15:25:37.845750 local_candles-0.1.1/local_candles/models/interval.py
+-rw-r--r--   0        0        0     1435 2023-06-22 15:25:09.829908 local_candles-0.1.1/local_candles/models/time.py
+-rw-r--r--   0        0        0      558 2023-06-22 15:13:17.087278 local_candles-0.1.1/local_candles/sources/__init__.py
+-rw-r--r--   0        0        0      355 2023-06-22 15:13:17.094295 local_candles-0.1.1/local_candles/sources/base.py
+-rw-r--r--   0        0        0     2305 2023-06-22 15:13:17.086926 local_candles-0.1.1/local_candles/sources/binance_futures_ohlc.py
+-rw-r--r--   0        0        0     2320 2023-06-22 15:13:17.087715 local_candles-0.1.1/local_candles/sources/binance_spot_ohlc.py
+-rw-r--r--   0        0        0     2630 2023-06-22 15:13:17.086564 local_candles-0.1.1/local_candles/sources/csv_file.py
+-rw-r--r--   0        0        0     2342 2023-06-22 15:13:17.093913 local_candles-0.1.1/local_candles/sources/gateio_spot_ohlc.py
+-rw-r--r--   0        0        0     2271 2023-06-22 15:13:17.094778 local_candles-0.1.1/local_candles/sources/yahoo_finance_ohlc.py
+-rw-r--r--   0        0        0      570 2023-06-22 15:21:16.285899 local_candles-0.1.1/local_candles/utils.py
+-rw-r--r--   0        0        0      654 2023-07-15 04:22:45.098012 local_candles-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 local_candles-0.1.1/setup.py
+-rw-r--r--   0        0        0     1474 1970-01-01 00:00:00.000000 local_candles-0.1.1/PKG-INFO
```

### Comparing `local_candles-0.1.0/local_candles/__init__.py` & `local_candles-0.1.1/local_candles/__init__.py`

 * *Files identical despite different names*

### Comparing `local_candles-0.1.0/local_candles/data.py` & `local_candles-0.1.1/local_candles/data.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,26 +24,27 @@
     def load_df(
         self, source: Source, start_ts: Time, stop_ts: Time, columns: List[str]
     ):
         ts = start_ts
         paths = []
 
         previous_first_ts = None
-        for i in range(20):
+        while True:
             result = self._load_from_cache(prefix=source.slug, ts=ts)
             if result:
                 first_ts, last_ts, p = result
                 completed = True
             else:
                 first_ts, last_ts, p, completed = self._load_from_source(
                     source=source, ts=ts
                 )
-                if first_ts == previous_first_ts:
-                    break
-                previous_first_ts = first_ts
+
+            if first_ts == previous_first_ts:
+                break
+            previous_first_ts = first_ts
 
             paths.append(p)
 
             if not completed:
                 break
 
             if last_ts >= stop_ts:
```

### Comparing `local_candles-0.1.0/local_candles/models/interval.py` & `local_candles-0.1.1/local_candles/models/interval.py`

 * *Files identical despite different names*

### Comparing `local_candles-0.1.0/local_candles/models/time.py` & `local_candles-0.1.1/local_candles/models/time.py`

 * *Files identical despite different names*

### Comparing `local_candles-0.1.0/local_candles/sources/__init__.py` & `local_candles-0.1.1/local_candles/sources/__init__.py`

 * *Files identical despite different names*

### Comparing `local_candles-0.1.0/local_candles/sources/binance_futures_ohlc.py` & `local_candles-0.1.1/local_candles/sources/binance_futures_ohlc.py`

 * *Files identical despite different names*

### Comparing `local_candles-0.1.0/local_candles/sources/binance_spot_ohlc.py` & `local_candles-0.1.1/local_candles/sources/binance_spot_ohlc.py`

 * *Files identical despite different names*

### Comparing `local_candles-0.1.0/local_candles/sources/csv_file.py` & `local_candles-0.1.1/local_candles/sources/csv_file.py`

 * *Files identical despite different names*

### Comparing `local_candles-0.1.0/local_candles/sources/gateio_spot_ohlc.py` & `local_candles-0.1.1/local_candles/sources/gateio_spot_ohlc.py`

 * *Files identical despite different names*

### Comparing `local_candles-0.1.0/local_candles/sources/yahoo_finance_ohlc.py` & `local_candles-0.1.1/local_candles/sources/yahoo_finance_ohlc.py`

 * *Files identical despite different names*

### Comparing `local_candles-0.1.0/local_candles/utils.py` & `local_candles-0.1.1/local_candles/utils.py`

 * *Files identical despite different names*

### Comparing `local_candles-0.1.0/pyproject.toml` & `local_candles-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "local-candles"
-version = "0.1.0"
+version = "0.1.1"
 description = "Candles (ohlc) loaders and cache"
 authors = ["Oleksandr Polieno <polyenoom@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/nanvel/local-candles"
 keywords = ["quant", "trading", "crypto", "cancles", "ohlc", "ohlcv", "dataframe", "pandas"]
 packages = [{include = "local_candles"}]
```

### Comparing `local_candles-0.1.0/setup.py` & `local_candles-0.1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 {'': ['*']}
 
 install_requires = \
 ['pandas>=2.0.2,<3.0.0', 'requests>=2.31.0,<3.0.0']
 
 setup_kwargs = {
     'name': 'local-candles',
-    'version': '0.1.0',
+    'version': '0.1.1',
     'description': 'Candles (ohlc) loaders and cache',
-    'long_description': '# Local candles\n\nUsage example:\n```python\nfrom local_candles import load_candles\n\n\ndef main():\n    df = load_candles(\n        source="binance_futures_ohlc",\n        start_ts="2021-01-01",\n        stop_ts="2021-02-01",\n        interval="1d",\n        symbol="BTCUSDT",\n    )\n\n    print(df)\n\n\nif __name__ == "__main__":\n    main()\n```\n',
+    'long_description': '# Local candles\n\n[![PyPI version](https://badge.fury.io/py/local-candles.svg)](https://badge.fury.io/py/local-candles)\n[![Python Versions](https://img.shields.io/pypi/pyversions/local-candles.svg)](https://pypi.python.org/pypi/local-candles/)\n[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)\n\nUsage example:\n```python\nfrom local_candles import load_candles\n\n\ndef main():\n    df = load_candles(\n        source="binance_futures_ohlc",\n        start_ts="2021-01-01",\n        stop_ts="2021-02-01",\n        interval="1d",\n        symbol="BTCUSDT",\n    )\n\n    print(df)\n\n\nif __name__ == "__main__":\n    main()\n```\n',
     'author': 'Oleksandr Polieno',
     'author_email': 'polyenoom@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/nanvel/local-candles',
     'packages': packages,
     'package_data': package_data,
```

