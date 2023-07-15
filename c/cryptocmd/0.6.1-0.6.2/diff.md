# Comparing `tmp/cryptocmd-0.6.1.tar.gz` & `tmp/cryptocmd-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptocmd-0.6.1.tar", max compression
+gzip compressed data, was "cryptocmd-0.6.2.tar", max compression
```

## Comparing `cryptocmd-0.6.1.tar` & `cryptocmd-0.6.2.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1511 2022-02-19 21:49:52.868681 cryptocmd-0.6.1/LICENSE
--rw-r--r--   0        0        0     3176 2022-02-19 21:49:52.872681 cryptocmd-0.6.1/README.rst
--rw-r--r--   0        0        0       57 2022-02-19 21:49:52.872681 cryptocmd-0.6.1/cryptocmd/__init__.py
--rw-r--r--   0        0        0       22 2022-02-19 21:49:52.872681 cryptocmd-0.6.1/cryptocmd/__version__.py
--rw-r--r--   0        0        0     8253 2022-02-19 21:49:52.872681 cryptocmd-0.6.1/cryptocmd/core.py
--rw-r--r--   0        0        0     4251 2022-02-19 21:49:52.872681 cryptocmd-0.6.1/cryptocmd/utils.py
--rw-r--r--   0        0        0     1127 2022-02-19 21:49:52.872681 cryptocmd-0.6.1/pyproject.toml
--rw-r--r--   0        0        0     3975 2022-02-19 21:50:10.871198 cryptocmd-0.6.1/setup.py
--rw-r--r--   0        0        0     4184 2022-02-19 21:50:10.871499 cryptocmd-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1511 2023-07-15 10:25:47.778282 cryptocmd-0.6.2/LICENSE
+-rw-r--r--   0        0        0     3886 2023-07-15 10:25:47.778282 cryptocmd-0.6.2/README.rst
+-rw-r--r--   0        0        0       57 2023-07-15 10:25:47.778282 cryptocmd-0.6.2/cryptocmd/__init__.py
+-rw-r--r--   0        0        0       22 2023-07-15 10:25:47.778282 cryptocmd-0.6.2/cryptocmd/__version__.py
+-rw-r--r--   0        0        0     8428 2023-07-15 10:25:47.778282 cryptocmd-0.6.2/cryptocmd/core.py
+-rw-r--r--   0        0        0     4629 2023-07-15 10:25:47.778282 cryptocmd-0.6.2/cryptocmd/utils.py
+-rw-r--r--   0        0        0     1124 2023-07-15 10:25:47.778282 cryptocmd-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0     4891 1970-01-01 00:00:00.000000 cryptocmd-0.6.2/PKG-INFO
```

### Comparing `cryptocmd-0.6.1/LICENSE` & `cryptocmd-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cryptocmd-0.6.1/README.rst` & `cryptocmd-0.6.2/README.rst`

 * *Files 15% similar despite different names*

```diff
@@ -16,14 +16,18 @@
     :target: https://pepy.tech/project/cryptoCMD
     :alt: Downloads
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/ambv/black
     :alt: Code style: black
 
+.. image:: https://img.shields.io/github/sponsors/guptarohit?color=%23FF5733
+    :target: https://github.com/sponsors/guptarohit
+    :alt: GitHub Sponsors
+
 Cryptocurrency historical market price data scraper written in Python.
 
 
 Installation
 ------------
 
 ::
@@ -63,14 +67,36 @@
 
     # export the data as csv file, you can also pass optional `name` parameter
     scraper.export("csv", name="xrp_all_time")
 
     # Pandas dataFrame for the same data
     df = scraper.get_dataframe()
 
+To get data of a cryptocurrency which have same coin code as others
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code:: python
+
+    from cryptocmd import CmcScraper
+
+    # initialise scraper with coin name as well
+    scraper = CmcScraper(coin_code="sol", coin_name="solana")
+
+    # get raw data as list of list
+    headers, data = scraper.get_data()
+
+    # get data in a json format
+    solana_json_data = scraper.get_data("json")
+
+    # export the data as csv file, you can also pass optional `name` parameter
+    scraper.export("csv", name="solana_all_time")
+
+    # Pandas dataFrame for the same data
+    df = scraper.get_dataframe()
+
 To get data of a cryptocurrency for some days
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: python
 
     from cryptocmd import CmcScraper
 
@@ -103,14 +129,10 @@
 Contributing
 ------------
 
 Feel free to make a pull request! :octocat:
 
 If you found this useful, I'd appreciate your consideration in the below. ✨☕
 
-.. image:: https://user-images.githubusercontent.com/7895001/52529389-e2da5280-2d16-11e9-924c-4fe3f309c780.png
+.. image:: https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=rohitgupta&button_colour=5F7FFF&font_colour=ffffff&font_family=Lato&outline_colour=000000&coffee_colour=FFDD00
     :target: https://www.buymeacoffee.com/rohitgupta
     :alt: Buy Me A Coffee
-
-.. image:: https://user-images.githubusercontent.com/7895001/52529390-e8379d00-2d16-11e9-913b-4d09db90403f.png
-    :target: https://www.patreon.com/bePatron?u=14009502
-    :alt: Become a Patron!
```

### Comparing `cryptocmd-0.6.1/cryptocmd/core.py` & `cryptocmd-0.6.2/cryptocmd/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,31 +28,33 @@
         self,
         coin_code,
         start_date=None,
         end_date=None,
         all_time=False,
         order_ascending=False,
         fiat="USD",
+        coin_name=None,
     ):
         """
         :param coin_code: coin code of cryptocurrency e.g. btc
         :param start_date: date since when to scrape data (in the format of dd-mm-yyyy)
         :param end_date: date to which scrape the data (in the format of dd-mm-yyyy)
         :param all_time: 'True' if need data of all time for respective cryptocurrency
         :param order_ascending: data ordered by 'Date' in ascending order (i.e. oldest first).
         :param fiat: fiat code eg. USD, EUR
-
+        :param coin_name: coin name in case of many coins with same code e.g. sol -> solana, solcoin
         """
 
         self.coin_code = coin_code
         self.start_date = start_date
         self.end_date = end_date
         self.all_time = bool(all_time)
         self.order_ascending = order_ascending
         self.fiat = fiat
+        self.coin_name = coin_name
         self.headers = ["Date", "Open", "High", "Low", "Close", "Volume", "Market Cap"]
         self.rows = []
 
         # enable all_time download if start_time or end_time is not given
         if not (self.start_date and self.end_date):
             self.all_time = True
 
@@ -80,15 +82,15 @@
         if self.rows and not forced:
             return
 
         if self.all_time:
             self.start_date, self.end_date = None, None
 
         coin_data = download_coin_data(
-            self.coin_code, self.start_date, self.end_date, self.fiat
+            self.coin_code, self.start_date, self.end_date, self.fiat, self.coin_name
         )
 
         for _row in coin_data["data"]["quotes"]:
 
             _row_quote = list(_row["quote"].values())[0]
             date = datetime.strptime(
                 _row_quote["timestamp"], "%Y-%m-%dT%H:%M:%S.%fZ"
```

### Comparing `cryptocmd-0.6.1/cryptocmd/utils.py` & `cryptocmd-0.6.2/cryptocmd/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -22,30 +22,34 @@
         if hasattr(e, "message"):
             print("Error message (get_url_data) :", e.message)
         else:
             print("Error message (get_url_data) :", e)
         raise e
 
 
-def get_coin_id(coin_code):
+def get_coin_id(coin_code, coin_name):
     """
     This method fetches the name(id) of currency from the given code
     :param coin_code: coin code of a cryptocurrency e.g. btc
+    :param coin_name: coin name in case of many coins with same code e.g. sol -> solana, solcoin
     :return: coin-id for the a cryptocurrency on the coinmarketcap.com
     """
 
     api_url = "https://web-api.coinmarketcap.com/v1/cryptocurrency/map?symbol={coin_code}".format(
         coin_code=coin_code
     )
 
     try:
         json_data = get_url_data(api_url).json()
         error_code = json_data["status"]["error_code"]
         if error_code == 0:
-            return json_data["data"][0]["slug"]
+            if coin_name is None:
+                return json_data["data"][0]["slug"]
+
+            return [data["slug"] for data in json_data["data"] if data["name"].lower() == coin_name.lower()][0]
         if error_code == 400:
             raise InvalidCoinCode(
                 "'{}' coin code is unavailable on coinmarketcap.com".format(coin_code)
             )
         else:
             raise Exception(json_data["status"]["error_message"])
     except Exception as e:
@@ -53,34 +57,35 @@
 
         if hasattr(e, "message"):
             print("Error message:", e.message)
         else:
             print("Error message:", e)
 
 
-def download_coin_data(coin_code, start_date, end_date, fiat):
+def download_coin_data(coin_code, start_date, end_date, fiat, coin_name):
     """
     Download HTML price history for the specified cryptocurrency and time range from CoinMarketCap.
 
     :param coin_code: coin code of a cryptocurrency e.g. btc
     :param start_date: date since when to scrape data (in the format of dd-mm-yyyy)
     :param end_date: date to which scrape the data (in the format of dd-mm-yyyy)
     :param fiat: fiat code eg. USD, EUR
+    :param coin_name: coin name in case of many coins with same code e.g. sol -> solana, solcoin
     :return: returns html of the webpage having historical data of cryptocurrency for certain duration
     """
 
     if start_date is None:
         # default start date on coinmarketcap.com
         start_date = "28-4-2013"
 
     if end_date is None:
         yesterday = datetime.date.today() - datetime.timedelta(1)
         end_date = yesterday.strftime("%d-%m-%Y")
 
-    coin_id = get_coin_id(coin_code)
+    coin_id = get_coin_id(coin_code, coin_name)
 
     # convert the dates to timestamp for the url
     start_date_timestamp = int(
         (
             datetime.datetime.strptime(start_date, "%d-%m-%Y")
             - datetime.timedelta(days=1)
         )
```

### Comparing `cryptocmd-0.6.1/pyproject.toml` & `cryptocmd-0.6.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "cryptocmd"
-version = "0.6.1"
+version = "0.6.2"
 description = "Cryptocurrency historical market price data scrapper."
 authors = ["Rohit Gupta <rohitgtech+git@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/guptarohit/cryptoCMD"
 repository = "https://github.com/guptarohit/cryptoCMD"
 keywords = ["cryptocurrency", "cryptocurrency historical data", "coinmarketcap", "dataset", "historical cryptocurrency prices"]
 
 classifiers = [
     "Development Status :: 4 - Beta",
     "Topic :: Utilities",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "License :: OSI Approved :: BSD License",
 ]
 include = [
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.6.2"
+python = "^3.7"
 requests = "*"
 tablib = "*"
 
 [tool.poetry.dev-dependencies]
-black = "^22.1.0"
+black = "^23.3"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `cryptocmd-0.6.1/PKG-INFO` & `cryptocmd-0.6.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: cryptocmd
-Version: 0.6.1
+Version: 0.6.2
 Summary: Cryptocurrency historical market price data scrapper.
 Home-page: https://github.com/guptarohit/cryptoCMD
 License: BSD-3-Clause
 Keywords: cryptocurrency,cryptocurrency historical data,coinmarketcap,dataset,historical cryptocurrency prices
 Author: Rohit Gupta
 Author-email: rohitgtech+git@gmail.com
-Requires-Python: >=3.6.2,<4.0.0
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Requires-Dist: requests
 Requires-Dist: tablib
 Project-URL: Repository, https://github.com/guptarohit/cryptoCMD
 Description-Content-Type: text/x-rst
 
 .. -*-restructuredtext-*-
@@ -41,14 +41,18 @@
     :target: https://pepy.tech/project/cryptoCMD
     :alt: Downloads
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/ambv/black
     :alt: Code style: black
 
+.. image:: https://img.shields.io/github/sponsors/guptarohit?color=%23FF5733
+    :target: https://github.com/sponsors/guptarohit
+    :alt: GitHub Sponsors
+
 Cryptocurrency historical market price data scraper written in Python.
 
 
 Installation
 ------------
 
 ::
@@ -88,14 +92,36 @@
 
     # export the data as csv file, you can also pass optional `name` parameter
     scraper.export("csv", name="xrp_all_time")
 
     # Pandas dataFrame for the same data
     df = scraper.get_dataframe()
 
+To get data of a cryptocurrency which have same coin code as others
+^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
+
+.. code:: python
+
+    from cryptocmd import CmcScraper
+
+    # initialise scraper with coin name as well
+    scraper = CmcScraper(coin_code="sol", coin_name="solana")
+
+    # get raw data as list of list
+    headers, data = scraper.get_data()
+
+    # get data in a json format
+    solana_json_data = scraper.get_data("json")
+
+    # export the data as csv file, you can also pass optional `name` parameter
+    scraper.export("csv", name="solana_all_time")
+
+    # Pandas dataFrame for the same data
+    df = scraper.get_dataframe()
+
 To get data of a cryptocurrency for some days
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code:: python
 
     from cryptocmd import CmcScraper
 
@@ -128,15 +154,11 @@
 Contributing
 ------------
 
 Feel free to make a pull request! :octocat:
 
 If you found this useful, I'd appreciate your consideration in the below. ✨☕
 
-.. image:: https://user-images.githubusercontent.com/7895001/52529389-e2da5280-2d16-11e9-924c-4fe3f309c780.png
+.. image:: https://img.buymeacoffee.com/button-api/?text=Buy me a coffee&emoji=&slug=rohitgupta&button_colour=5F7FFF&font_colour=ffffff&font_family=Lato&outline_colour=000000&coffee_colour=FFDD00
     :target: https://www.buymeacoffee.com/rohitgupta
     :alt: Buy Me A Coffee
 
-.. image:: https://user-images.githubusercontent.com/7895001/52529390-e8379d00-2d16-11e9-913b-4d09db90403f.png
-    :target: https://www.patreon.com/bePatron?u=14009502
-    :alt: Become a Patron!
-
```

