# Comparing `tmp/apit212-0.0.7.tar.gz` & `tmp/apit212-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apit212-0.0.7.tar", last modified: Wed Jul  5 20:06:11 2023, max compression
+gzip compressed data, was "apit212-0.0.8.tar", last modified: Sat Jul 15 00:10:54 2023, max compression
```

## Comparing `apit212-0.0.7.tar` & `apit212-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-05 20:06:11.455014 apit212-0.0.7/
--rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-0.0.7/LICENSE
--rw-rw-rw-   0        0        0     7008 2023-07-05 20:06:11.451244 apit212-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     6241 2023-07-05 18:57:42.000000 apit212-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-05 20:06:11.390904 apit212-0.0.7/apit212/
--rw-rw-rw-   0        0        0    17830 2023-07-05 20:04:42.000000 apit212-0.0.7/apit212/Apit212.py
--rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-0.0.7/apit212/__init__.py
--rw-rw-rw-   0        0        0     1250 2023-07-05 19:45:15.000000 apit212-0.0.7/apit212/apitconstant.py
--rw-rw-rw-   0        0        0     4884 2023-07-05 19:45:17.000000 apit212-0.0.7/apit212/cfdScrape.py
-drwxrwxrwx   0        0        0        0 2023-07-05 20:06:11.451244 apit212-0.0.7/apit212.egg-info/
--rw-rw-rw-   0        0        0     7008 2023-07-05 20:06:11.000000 apit212-0.0.7/apit212.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-07-05 20:06:11.000000 apit212-0.0.7/apit212.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-05 20:06:11.000000 apit212-0.0.7/apit212.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-05 20:06:11.000000 apit212-0.0.7/apit212.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-05 20:06:11.000000 apit212-0.0.7/apit212.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      839 2023-07-05 20:05:22.000000 apit212-0.0.7/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-05 20:06:11.455014 apit212-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      898 2023-07-05 20:05:28.000000 apit212-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 00:10:54.541528 apit212-0.0.8/
+-rw-rw-rw-   0        0        0     1083 2023-07-05 18:54:25.000000 apit212-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0     7148 2023-07-15 00:10:54.539496 apit212-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     6381 2023-07-15 00:10:04.000000 apit212-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 00:10:54.424049 apit212-0.0.8/apit212/
+-rw-rw-rw-   0        0        0    18278 2023-07-15 00:05:08.000000 apit212-0.0.8/apit212/Apit212.py
+-rw-rw-rw-   0        0        0       98 2023-07-05 18:54:13.000000 apit212-0.0.8/apit212/__init__.py
+-rw-rw-rw-   0        0        0     1250 2023-07-05 19:45:15.000000 apit212-0.0.8/apit212/apitconstant.py
+-rw-rw-rw-   0        0        0     4884 2023-07-05 19:45:17.000000 apit212-0.0.8/apit212/cfdScrape.py
+drwxrwxrwx   0        0        0        0 2023-07-15 00:10:54.533977 apit212-0.0.8/apit212.egg-info/
+-rw-rw-rw-   0        0        0     7148 2023-07-15 00:10:54.000000 apit212-0.0.8/apit212.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-07-15 00:10:54.000000 apit212-0.0.8/apit212.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 00:10:54.000000 apit212-0.0.8/apit212.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-15 00:10:54.000000 apit212-0.0.8/apit212.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-15 00:10:54.000000 apit212-0.0.8/apit212.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      839 2023-07-15 00:05:35.000000 apit212-0.0.8/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 00:10:54.541528 apit212-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      898 2023-07-15 00:05:45.000000 apit212-0.0.8/setup.py
```

### Comparing `apit212-0.0.7/LICENSE` & `apit212-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `apit212-0.0.7/PKG-INFO` & `apit212-0.0.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: apit212
-Version: 0.0.7
-Summary: Unofficial trading212 API
-Home-page: https://github.com/Flock92/aPit212
-Author: Flock92
-Author-email: Flock92 <stuwe_3000@outlook.com>
-Maintainer-email: Flock92 <stuwe_3000@outlook.com>
-License: MIT
-Project-URL: Homepage, https://github.com/Flock92/apit212
-Project-URL: Bug Tracker, https://github.com/Flock92/apit212/issues
-Keywords: trading,trading212,api,trade,flock92
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Classifier: Development Status :: 4 - Beta
-Requires: requests
-Requires: selenium
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # **Apit212**
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212 Please note that either myself or trading212 take responsibility for the use of this API.
 I will continue to work on this project and would appriciate any feedback. 
 
 ## Requirments
 
@@ -239,14 +217,22 @@
 ```py
 
 cancel_order = client.cancel_order(order_id)
 
 
 ```
 
+You can also use the *cancel_all_orders* to cancel all pending limits orders.
+
+```py
+
+cancel_all = client.cancel_all_orders()
+
+```
+
 ### Close Position
 The *cancel_position* function will submit a request to cancel a open position.
 
 ```py
 
 
 cancel_position = client.close_position(position_id=market_order, quantity=market_order, current_price=current_price)
```

### Comparing `apit212-0.0.7/README.md` & `apit212-0.0.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: apit212
+Version: 0.0.8
+Summary: Unofficial trading212 API
+Home-page: https://github.com/Flock92/aPit212
+Author: Flock92
+Author-email: Flock92 <stuwe_3000@outlook.com>
+Maintainer-email: Flock92 <stuwe_3000@outlook.com>
+License: MIT
+Project-URL: Homepage, https://github.com/Flock92/apit212
+Project-URL: Bug Tracker, https://github.com/Flock92/apit212/issues
+Keywords: trading,trading212,api,trade,flock92
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Development Status :: 4 - Beta
+Requires: requests
+Requires: selenium
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # **Apit212**
 
 This is a Pyhton based API using selenium and requests to get insformation from the broker trading 212 Please note that either myself or trading212 take responsibility for the use of this API.
 I will continue to work on this project and would appriciate any feedback. 
 
 ## Requirments
 
@@ -217,14 +239,22 @@
 ```py
 
 cancel_order = client.cancel_order(order_id)
 
 
 ```
 
+You can also use the *cancel_all_orders* to cancel all pending limits orders.
+
+```py
+
+cancel_all = client.cancel_all_orders()
+
+```
+
 ### Close Position
 The *cancel_position* function will submit a request to cancel a open position.
 
 ```py
 
 
 cancel_position = client.close_position(position_id=market_order, quantity=market_order, current_price=current_price)
```

### Comparing `apit212-0.0.7/apit212/Apit212.py` & `apit212-0.0.8/apit212/Apit212.py`

 * *Files 4% similar despite different names*

```diff
@@ -261,14 +261,26 @@
         'quantity': 110.0, 'maxBuy': None, 'maxSell': None, 'maxOpenBuy': None, 'maxOpenSell': None, 'swap': -16.11,
         'frontend': 'WC4', 'pplAdjustment': None, 'autoInvestQuantity': None, 'fxPpl': None}
         """
         payload = {'positionId': f'{order_id}'}
         r = requests.delete(url=f"{self.url}/rest/v2/pending-orders/entry/{order_id}",
                             headers=self.headers, data=json.dumps(payload))
         return r.json()
+    
+    # CANCEL ALL PENDING ORDERS
+    def cancel_all_orders(self) -> dict:
+        """"""
+        payload = []
+        data = requests.post(url=f"{self.url}/rest/trading/v1/accounts/summary",
+                             headers=self.headers, data=json.dumps(payload))
+
+        r = requests.delete(url=f"{self.url}/rest/v2/pending-orders/cancel",
+                            headers=self.headers, data=data)
+
+        return r.json()
 
     # CANCEL ORDER
     def close_position(self, position_id, quantity, current_price) -> dict:
         """
         close open positions
         :param position_id:
         :param quantity:
```

### Comparing `apit212-0.0.7/apit212/apitconstant.py` & `apit212-0.0.8/apit212/apitconstant.py`

 * *Files identical despite different names*

### Comparing `apit212-0.0.7/apit212/cfdScrape.py` & `apit212-0.0.8/apit212/cfdScrape.py`

 * *Files identical despite different names*

### Comparing `apit212-0.0.7/apit212.egg-info/PKG-INFO` & `apit212-0.0.8/apit212.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apit212
-Version: 0.0.7
+Version: 0.0.8
 Summary: Unofficial trading212 API
 Home-page: https://github.com/Flock92/aPit212
 Author: Flock92
 Author-email: Flock92 <stuwe_3000@outlook.com>
 Maintainer-email: Flock92 <stuwe_3000@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Flock92/apit212
@@ -239,14 +239,22 @@
 ```py
 
 cancel_order = client.cancel_order(order_id)
 
 
 ```
 
+You can also use the *cancel_all_orders* to cancel all pending limits orders.
+
+```py
+
+cancel_all = client.cancel_all_orders()
+
+```
+
 ### Close Position
 The *cancel_position* function will submit a request to cancel a open position.
 
 ```py
 
 
 cancel_position = client.close_position(position_id=market_order, quantity=market_order, current_price=current_price)
```

### Comparing `apit212-0.0.7/pyproject.toml` & `apit212-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "apit212"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
 { name= "Flock92", email= "stuwe_3000@outlook.com" },
 ]
 
 maintainers = [
   {name = "Flock92", email = "stuwe_3000@outlook.com"}
 ]
```

### Comparing `apit212-0.0.7/setup.py` & `apit212-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 long_description = """This is an unofficial API use to interact with the trading212 platform. It is still currently in
                    it's testing stages I created this API to challenge myself and also start creating a portfolio of
                    work that i can showcase to employers"""
 
 setup(
     name="apit212",
-    version="0.0.7",
+    version="0.0.8",
     packages=find_packages(),
     requires=[
         'requests',
         'selenium',
     ],
     author="Flock92",
     author_email="stuwe_3000@outlook.com",
```

