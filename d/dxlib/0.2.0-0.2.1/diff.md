# Comparing `tmp/dxlib-0.2.0.tar.gz` & `tmp/dxlib-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxlib-0.2.0.tar", last modified: Sat Jul 15 07:42:08 2023, max compression
+gzip compressed data, was "dxlib-0.2.1.tar", last modified: Sat Jul 15 08:03:30 2023, max compression
```

## Comparing `dxlib-0.2.0.tar` & `dxlib-0.2.1.tar`

### file list

```diff
@@ -1,30 +1,41 @@
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.768211 dxlib-0.2.0/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-07-15 07:42:08.765200 dxlib-0.2.0/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      526 2023-04-20 14:34:27.000000 dxlib-0.2.0/README.md
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.358830 dxlib-0.2.0/dxlib/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       19 2023-07-15 07:24:40.000000 dxlib-0.2.0/dxlib/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.636952 dxlib-0.2.0/dxlib/api/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       76 2023-07-15 05:54:39.000000 dxlib-0.2.0/dxlib/api/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1345 2023-07-15 07:08:40.000000 dxlib-0.2.0/dxlib/api/__main__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1343 2023-07-15 05:57:39.000000 dxlib-0.2.0/dxlib/api/alphavantage.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      569 2023-07-15 03:43:22.000000 dxlib-0.2.0/dxlib/api/logger.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      315 2023-07-15 04:34:42.000000 dxlib-0.2.0/dxlib/api/terminal.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1857 2023-07-15 04:12:02.000000 dxlib-0.2.0/dxlib/api/utils.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1448 2023-07-14 03:22:23.000000 dxlib-0.2.0/dxlib/app.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.676041 dxlib-0.2.0/dxlib/db/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.2.0/dxlib/db/__init__.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.746335 dxlib-0.2.0/dxlib/db/sql/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.0/dxlib/db/sql/__init__.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      153 2023-06-30 10:10:39.000000 dxlib-0.2.0/dxlib/db/sql/create.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      761 2023-06-30 10:14:21.000000 dxlib-0.2.0/dxlib/db/sql/queries.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4361 2023-07-14 00:49:31.000000 dxlib-0.2.0/dxlib/db/utils.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      404 2023-04-20 14:41:16.000000 dxlib-0.2.0/dxlib/euler_method.py
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      274 2023-04-20 14:39:35.000000 dxlib-0.2.0/dxlib/finite_differences.py
-drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:42:08.484872 dxlib-0.2.0/dxlib.egg-info/
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1262 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/PKG-INFO
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      485 2023-07-15 07:42:08.000000 dxlib-0.2.0/dxlib.egg-info/SOURCES.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/dependency_links.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      119 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/requires.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 07:42:07.000000 dxlib-0.2.0/dxlib.egg-info/top_level.txt
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 07:42:08.768211 dxlib-0.2.0/setup.cfg
--rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:28:39.000000 dxlib-0.2.0/setup.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.506143 dxlib-0.2.1/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 08:03:30.503141 dxlib-0.2.1/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      981 2023-07-15 07:58:15.000000 dxlib-0.2.1/README.md
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:29.868367 dxlib-0.2.1/dxlib/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       95 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.079595 dxlib-0.2.1/dxlib/api/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       73 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/api/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1304 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/api/alphavantage.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:44.000000 dxlib-0.2.1/dxlib/api/logger.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:49:34.000000 dxlib-0.2.1/dxlib/api/terminal.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.152861 dxlib-0.2.1/dxlib/core/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:09.000000 dxlib-0.2.1/dxlib/core/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      387 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/core/euler_method.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      262 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/core/finite_differences.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.201993 dxlib-0.2.1/dxlib/data/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       21 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/data/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1805 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/data/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.250433 dxlib-0.2.1/dxlib/db/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-13 23:57:17.000000 dxlib-0.2.1/dxlib/db/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.339354 dxlib-0.2.1/dxlib/db/sql/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-06-30 10:14:59.000000 dxlib-0.2.1/dxlib/db/sql/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      148 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/db/sql/create.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      730 2023-07-15 07:58:04.000000 dxlib-0.2.1/dxlib/db/sql/queries.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     4241 2023-07-15 07:58:05.000000 dxlib-0.2.1/dxlib/db/utils.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.413000 dxlib-0.2.1/dxlib/models/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:31.000000 dxlib-0.2.1/dxlib/models/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       86 2023-07-15 07:58:05.000000 dxlib-0.2.1/dxlib/models/options.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-04-28 17:50:38.000000 dxlib-0.2.1/dxlib/models/pricing.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.435020 dxlib-0.2.1/dxlib/research/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:50:59.000000 dxlib-0.2.1/dxlib/research/__init__.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:30.481295 dxlib-0.2.1/dxlib/simulation/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 07:51:15.000000 dxlib-0.2.1/dxlib/simulation/__init__.py
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     7903 2023-07-15 07:58:05.000000 dxlib-0.2.1/dxlib/simulation/backtesting.py
+drwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        0 2023-07-15 08:03:29.979701 dxlib-0.2.1/dxlib.egg-info/
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1716 2023-07-15 08:03:29.000000 dxlib-0.2.1/dxlib.egg-info/PKG-INFO
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      668 2023-07-15 08:03:29.000000 dxlib-0.2.1/dxlib.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        1 2023-07-15 08:03:29.000000 dxlib-0.2.1/dxlib.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)      106 2023-07-15 08:03:29.000000 dxlib-0.2.1/dxlib.egg-info/requires.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)        6 2023-07-15 08:03:29.000000 dxlib-0.2.1/dxlib.egg-info/top_level.txt
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)       38 2023-07-15 08:03:30.507144 dxlib-0.2.1/setup.cfg
+-rwxrwxrwx   0 rzimmerdev  (1000) rzimmerdev  (1000)     1328 2023-07-15 07:44:19.000000 dxlib-0.2.1/setup.py
```

### Comparing `dxlib-0.2.0/PKG-INFO` & `dxlib-0.2.1/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -27,22 +27,43 @@
 ## Installation
 
 `pip install dxlib`
 
 
 ## Quickstart
 
+### Research Module
 ```
 from dxlib import finite_differences
 
 import numpy
 import matplotlib.pyplot
 
 x = np.arange(-3, 3, h)
 y = np.tanh(x)
 
 dy = finite_differences(x, y)
 ```
 
+### Simulation Module
+
+
+### API Module
+
+```
+from dxlib.api import AlphaVantageAPI as av
+
+print("Realtime exchange rates from the last 5 minutes:")
+
+alpha_vantage = av("<api_key>")
+for i in range(5):
+  currencies_to_query = ['JPY', 'EUR', 'GBP', 'CAD', 'AUD']
+  exchange_rates_df = api.fetch_currency_exchange_rates(currencies_to_query)
+  print(terminal, exchange_rates_df)
+  time.sleep(60)
+```
+
+### Data Module
+
 A visual graph of the finite differences should be plotted,
 and the numerical values for the differentiation at the point x
-returned.
+returned.
```

### Comparing `dxlib-0.2.0/dxlib/api/alphavantage.py` & `dxlib-0.2.1/dxlib/api/alphavantage.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import requests
-import pandas
-
-
-class AlphaVantageAPI:
-    def __init__(self, api_key):
-        self.api_key = api_key
-        self.base_url = 'https://www.alphavantage.co/query?'
-
-    def fetch_quote(self, symbol):
-        url = f'{self.base_url}function=GLOBAL_QUOTE&symbol={symbol}&apikey={self.api_key}'
-        response = requests.get(url)
-        data = response.json()
-        return data['Global Quote']
-
-    def fetch_currency_exchange_rates(self, currencies):
-        exchange_rates = []
-
-        for currency in currencies:
-            params = {
-                'function': 'CURRENCY_EXCHANGE_RATE',
-                'from_currency': 'USD',
-                'to_currency': currency,
-                'apikey': self.api_key
-            }
-
-            response = requests.get(self.base_url, params=params)
-            data = response.json()
-
-            try:
-                exchange_rate_data = data['Realtime Currency Exchange Rate']
-                exchange_rates.append({
-                    'Currency': currency,
-                    'Exchange Rate': exchange_rate_data['5. Exchange Rate'],
-                    'Last Refreshed': exchange_rate_data['6. Last Refreshed']
-                })
-            except KeyError:
-                print(data)
-        return pandas.DataFrame(exchange_rates)
+import requests
+import pandas
+
+
+class AlphaVantageAPI:
+    def __init__(self, api_key):
+        self.api_key = api_key
+        self.base_url = 'https://www.alphavantage.co/query?'
+
+    def fetch_quote(self, symbol):
+        url = f'{self.base_url}function=GLOBAL_QUOTE&symbol={symbol}&apikey={self.api_key}'
+        response = requests.get(url)
+        data = response.json()
+        return data['Global Quote']
+
+    def fetch_currency_exchange_rates(self, currencies):
+        exchange_rates = []
+
+        for currency in currencies:
+            params = {
+                'function': 'CURRENCY_EXCHANGE_RATE',
+                'from_currency': 'USD',
+                'to_currency': currency,
+                'apikey': self.api_key
+            }
+
+            response = requests.get(self.base_url, params=params)
+            data = response.json()
+
+            try:
+                exchange_rate_data = data['Realtime Currency Exchange Rate']
+                exchange_rates.append({
+                    'Currency': currency,
+                    'Exchange Rate': exchange_rate_data['5. Exchange Rate'],
+                    'Last Refreshed': exchange_rate_data['6. Last Refreshed']
+                })
+            except KeyError:
+                print(data)
+        return pandas.DataFrame(exchange_rates)
```

### Comparing `dxlib-0.2.0/dxlib/api/utils.py` & `dxlib-0.2.1/dxlib/data/utils.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,52 @@
-import csv
-import pandas
-
-
-def append_to_csv(data, csv_file='stock_data.csv'):
-    if isinstance(data, list):
-        try:
-            with open(csv_file, 'r') as file:
-                is_empty = len(file.readline().strip()) == 0
-        except FileNotFoundError:
-            is_empty = True
-
-        with open(csv_file, 'a', newline='') as file:
-            writer = csv.writer(file)
-            if is_empty:
-                if isinstance(data[0], (list, tuple)):
-                    writer.writerows(data)
-                else:
-                    writer.writerow(data)
-            else:
-                if isinstance(data[0], (list, tuple)):
-                    for item in data:
-                        writer.writerow(item)
-                else:
-                    writer.writerow(data)
-
-    elif isinstance(data, dict):
-        fieldnames = list(data.keys())
-
-        try:
-            with open(csv_file, 'r') as file:
-                reader = csv.DictReader(file)
-                existing_fieldnames = reader.fieldnames
-        except FileNotFoundError:
-            existing_fieldnames = []
-
-        if existing_fieldnames:
-            ordered_data = [data[field] for field in existing_fieldnames]
-        else:
-            ordered_data = list(data.values())
-
-        with open(csv_file, 'a', newline='') as file:
-            writer = csv.DictWriter(file, fieldnames=fieldnames)
-            if not existing_fieldnames:
-                writer.writeheader()
-            writer.writerow({field: value for field, value in zip(existing_fieldnames, ordered_data)})
-
-    elif isinstance(data, pandas.DataFrame):
-        data.to_csv(csv_file, mode='a', header=False, index=False)
-
-    else:
-        raise ValueError("Unsupported data type. Only lists, dictionaries, and pandas DataFrames are supported.")
+import csv
+import pandas
+
+
+def append_to_csv(data, csv_file='stock_data.csv'):
+    if isinstance(data, list):
+        try:
+            with open(csv_file, 'r') as file:
+                is_empty = len(file.readline().strip()) == 0
+        except FileNotFoundError:
+            is_empty = True
+
+        with open(csv_file, 'a', newline='') as file:
+            writer = csv.writer(file)
+            if is_empty:
+                if isinstance(data[0], (list, tuple)):
+                    writer.writerows(data)
+                else:
+                    writer.writerow(data)
+            else:
+                if isinstance(data[0], (list, tuple)):
+                    for item in data:
+                        writer.writerow(item)
+                else:
+                    writer.writerow(data)
+
+    elif isinstance(data, dict):
+        fieldnames = list(data.keys())
+
+        try:
+            with open(csv_file, 'r') as file:
+                reader = csv.DictReader(file)
+                existing_fieldnames = reader.fieldnames
+        except FileNotFoundError:
+            existing_fieldnames = []
+
+        if existing_fieldnames:
+            ordered_data = [data[field] for field in existing_fieldnames]
+        else:
+            ordered_data = list(data.values())
+
+        with open(csv_file, 'a', newline='') as file:
+            writer = csv.DictWriter(file, fieldnames=fieldnames)
+            if not existing_fieldnames:
+                writer.writeheader()
+            writer.writerow({field: value for field, value in zip(existing_fieldnames, ordered_data)})
+
+    elif isinstance(data, pandas.DataFrame):
+        data.to_csv(csv_file, mode='a', header=False, index=False)
+
+    else:
+        raise ValueError("Unsupported data type. Only lists, dictionaries, and pandas DataFrames are supported.")
```

### Comparing `dxlib-0.2.0/dxlib/db/sql/queries.py` & `dxlib-0.2.1/dxlib/db/sql/queries.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-def GET_TABLES():
-    return """
-    SELECT table_name FROM user_tables;
-    """
-
-def GET_USERS():
-    return """
-    SELECT P.NOME FROM PESSOA P 
-    JOIN  
-    (SELECT A.CPF FROM ALUNO A WHERE NOT EXISTS (
-        (SELECT M.NOME, M.CURSO FROM MISSAO M
-            WHERE M.CURSO = 'Informatica1')
-            MINUS
-            (SELECT F.MISSAO, F.CURSO FROM FAZ F
-            WHERE F.ALUNO = A.CPF)
-        )
-    ) 
-    X ON P.CPF = X.CPF
-    """
-
-
-def GET_MISSIONS():
-    return """
-    SELECT P.NOME, F.CURSO, MISSOES_FEITAS FROM PESSOA P 
-    JOIN 
-    (SELECT A.CPF, F.CURSO, COUNT(*) AS MISSOES_FEITAS FROM ALUNO A
-        JOIN FAZ F ON (F.ALUNO = A.CPF)
-        GROUP BY A.CPF, F.CURSO 
-    ) 
-    ON P.CPF = A.CPF
-    """
+def GET_TABLES():
+    return """
+    SELECT table_name FROM user_tables;
+    """
+
+def GET_USERS():
+    return """
+    SELECT P.NOME FROM PESSOA P 
+    JOIN  
+    (SELECT A.CPF FROM ALUNO A WHERE NOT EXISTS (
+        (SELECT M.NOME, M.CURSO FROM MISSAO M
+            WHERE M.CURSO = 'Informatica1')
+            MINUS
+            (SELECT F.MISSAO, F.CURSO FROM FAZ F
+            WHERE F.ALUNO = A.CPF)
+        )
+    ) 
+    X ON P.CPF = X.CPF
+    """
+
+
+def GET_MISSIONS():
+    return """
+    SELECT P.NOME, F.CURSO, MISSOES_FEITAS FROM PESSOA P 
+    JOIN 
+    (SELECT A.CPF, F.CURSO, COUNT(*) AS MISSOES_FEITAS FROM ALUNO A
+        JOIN FAZ F ON (F.ALUNO = A.CPF)
+        GROUP BY A.CPF, F.CURSO 
+    ) 
+    ON P.CPF = A.CPF
+    """
```

### Comparing `dxlib-0.2.0/dxlib/db/utils.py` & `dxlib-0.2.1/dxlib/db/utils.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,120 +1,120 @@
-from pymongo import MongoClient
-
-
-class DatabaseManager:
-    connection = None
-
-    def connect(self, host, port):
-        if not self.connection:
-            self.connection = MongoClient(host, port)
-
-    def create(self, command, cursor=None):
-        if not self.connection:
-            raise ConnectionError("Connect to DB!")
-        with cursor if cursor else self.connection.cursor() as cursor:
-            cursor.execute(command.value)
-
-    def get(self, command, cursor=None):
-        if not self.connection:
-            raise ConnectionError("Connect to DB!")
-        with cursor if cursor else self.connection.cursor() as cursor:
-            return list(cursor.execute(command.value))
-
-    def create_schema(self):
-        with open("sql/create_schema.sql") as file:
-            sql = file.read()
-
-        create = sql.split(";")
-        print(create)
-        print(self.connection)
-
-
-class Menu:
-    def __init__(self, name, identifier, paths: list = None, calls: list[dict] = None,
-                 text="Selecione uma opção para continuar:"):
-        self.name = name
-        self.identifier = identifier
-        self.paths = [] if not paths else paths
-        self.calls = [] if not calls else calls
-        self.text = text
-
-    def select(self, index):
-        if index < 0:
-            raise IndexError("Invalid option")
-        else:
-            return self.paths[index]
-
-    def call(self, index, *args, **kwargs):
-        if index >= len(self.calls):
-            raise IndexError("Invalid option")
-        else:
-            return self.calls[index]["method"](*args, **kwargs)
-
-
-class Navigation:
-    terminal = None
-
-    def __init__(self, starting_menu: Menu, terminal):
-        self.current_menu = starting_menu
-        self.previous_menus = []
-        self.terminal = terminal
-
-    def display(self, output=None):
-        self.terminal.clear()
-        self.terminal.header(f"Menu: { self.current_menu.name}\n")
-
-        if self.previous_menus:
-            self.terminal.print(f"0 - Return. \n")
-
-        for idx, path in enumerate(self.current_menu.paths):
-            self.terminal.print(f"{idx + 1} - {path.identifier}")
-
-        for idx, call in enumerate(self.current_menu.calls):
-            self.terminal.print(f"{len(self.current_menu.paths) + idx + 1} - {call['name']}")
-
-        self.terminal.print(f"{len(self.current_menu.paths) + len(self.current_menu.calls) + 1} - Exit \n")
-
-        if output:
-            self.terminal.log(json=output)
-
-    def listen(self):
-        while True:
-            option = int(self.terminal.get_input(self.current_menu.text + "\n"))
-
-            if option == (len(self.current_menu.paths) + len(self.current_menu.calls)) + 1:
-                raise SystemExit
-
-            if option == 0 and self.previous_menus:
-                self.current_menu = self.previous_menus.pop()
-                break
-
-            option -= 1
-
-            try:
-                if option < len(self.current_menu.paths):
-                    selected_menu = self.current_menu.select(option)
-                    self.enter_menu(selected_menu)
-                    break
-
-                else:
-                    try:
-                        call = self.current_menu.calls[option - len(self.current_menu.paths)]
-                        args = call.get("args", None)
-
-                        if args:
-                            args = self.terminal.get_input(f"Required parameters: {args}\n")
-                            output = self.current_menu.call(option - len(self.current_menu.paths), args.split(" "))
-                        else:
-                            output = self.current_menu.call(option - len(self.current_menu.paths))
-                        return output
-                    except ValueError as params:
-                        self.terminal.print(f"For the selected option {option}, provide the following params: {params}")
-
-            except IndexError:
-                self.terminal.print("Invalid option, please select a number between 0 e {}".format(
-                    len(self.current_menu.paths) + len(self.current_menu.calls) + 1
-                ))
-
-    def enter_menu(self, menu):
-        self.previous_menus.append(self.current_menu)
-        self.current_menu = menu
+from pymongo import MongoClient
+
+
+class DatabaseManager:
+    connection = None
+
+    def connect(self, host, port):
+        if not self.connection:
+            self.connection = MongoClient(host, port)
+
+    def create(self, command, cursor=None):
+        if not self.connection:
+            raise ConnectionError("Connect to DB!")
+        with cursor if cursor else self.connection.cursor() as cursor:
+            cursor.execute(command.value)
+
+    def get(self, command, cursor=None):
+        if not self.connection:
+            raise ConnectionError("Connect to DB!")
+        with cursor if cursor else self.connection.cursor() as cursor:
+            return list(cursor.execute(command.value))
+
+    def create_schema(self):
+        with open("sql/create_schema.sql") as file:
+            sql = file.read()
+
+        create = sql.split(";")
+        print(create)
+        print(self.connection)
+
+
+class Menu:
+    def __init__(self, name, identifier, paths: list = None, calls: list[dict] = None,
+                 text="Selecione uma opção para continuar:"):
+        self.name = name
+        self.identifier = identifier
+        self.paths = [] if not paths else paths
+        self.calls = [] if not calls else calls
+        self.text = text
+
+    def select(self, index):
+        if index < 0:
+            raise IndexError("Invalid option")
+        else:
+            return self.paths[index]
+
+    def call(self, index, *args, **kwargs):
+        if index >= len(self.calls):
+            raise IndexError("Invalid option")
+        else:
+            return self.calls[index]["method"](*args, **kwargs)
+
+
+class Navigation:
+    terminal = None
+
+    def __init__(self, starting_menu: Menu, terminal):
+        self.current_menu = starting_menu
+        self.previous_menus = []
+        self.terminal = terminal
+
+    def display(self, output=None):
+        self.terminal.clear()
+        self.terminal.header(f"Menu: { self.current_menu.name}\n")
+
+        if self.previous_menus:
+            self.terminal.print(f"0 - Return. \n")
+
+        for idx, path in enumerate(self.current_menu.paths):
+            self.terminal.print(f"{idx + 1} - {path.identifier}")
+
+        for idx, call in enumerate(self.current_menu.calls):
+            self.terminal.print(f"{len(self.current_menu.paths) + idx + 1} - {call['name']}")
+
+        self.terminal.print(f"{len(self.current_menu.paths) + len(self.current_menu.calls) + 1} - Exit \n")
+
+        if output:
+            self.terminal.log(json=output)
+
+    def listen(self):
+        while True:
+            option = int(self.terminal.get_input(self.current_menu.text + "\n"))
+
+            if option == (len(self.current_menu.paths) + len(self.current_menu.calls)) + 1:
+                raise SystemExit
+
+            if option == 0 and self.previous_menus:
+                self.current_menu = self.previous_menus.pop()
+                break
+
+            option -= 1
+
+            try:
+                if option < len(self.current_menu.paths):
+                    selected_menu = self.current_menu.select(option)
+                    self.enter_menu(selected_menu)
+                    break
+
+                else:
+                    try:
+                        call = self.current_menu.calls[option - len(self.current_menu.paths)]
+                        args = call.get("args", None)
+
+                        if args:
+                            args = self.terminal.get_input(f"Required parameters: {args}\n")
+                            output = self.current_menu.call(option - len(self.current_menu.paths), args.split(" "))
+                        else:
+                            output = self.current_menu.call(option - len(self.current_menu.paths))
+                        return output
+                    except ValueError as params:
+                        self.terminal.print(f"For the selected option {option}, provide the following params: {params}")
+
+            except IndexError:
+                self.terminal.print("Invalid option, please select a number between 0 e {}".format(
+                    len(self.current_menu.paths) + len(self.current_menu.calls) + 1
+                ))
+
+    def enter_menu(self, menu):
+        self.previous_menus.append(self.current_menu)
+        self.current_menu = menu
```

### Comparing `dxlib-0.2.0/dxlib.egg-info/PKG-INFO` & `dxlib-0.2.1/dxlib.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxlib
-Version: 0.2.0
+Version: 0.2.1
 Summary: Quantitative Methods for Finance
 Home-page: https://github.com/delphos-quant/dxlib
 Author: Rafael Zimmer
 Author-email: rzimmerde@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -27,22 +27,43 @@
 ## Installation
 
 `pip install dxlib`
 
 
 ## Quickstart
 
+### Research Module
 ```
 from dxlib import finite_differences
 
 import numpy
 import matplotlib.pyplot
 
 x = np.arange(-3, 3, h)
 y = np.tanh(x)
 
 dy = finite_differences(x, y)
 ```
 
+### Simulation Module
+
+
+### API Module
+
+```
+from dxlib.api import AlphaVantageAPI as av
+
+print("Realtime exchange rates from the last 5 minutes:")
+
+alpha_vantage = av("<api_key>")
+for i in range(5):
+  currencies_to_query = ['JPY', 'EUR', 'GBP', 'CAD', 'AUD']
+  exchange_rates_df = api.fetch_currency_exchange_rates(currencies_to_query)
+  print(terminal, exchange_rates_df)
+  time.sleep(60)
+```
+
+### Data Module
+
 A visual graph of the finite differences should be plotted,
 and the numerical values for the differentiation at the point x
-returned.
+returned.
```

### Comparing `dxlib-0.2.0/setup.py` & `dxlib-0.2.1/setup.py`

 * *Files identical despite different names*

