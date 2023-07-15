# Comparing `tmp/LolzteamApi-1.0.18.tar.gz` & `tmp/LolzteamApi-1.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LolzteamApi-1.0.18.tar", last modified: Mon Jul 10 05:30:26 2023, max compression
+gzip compressed data, was "LolzteamApi-1.0.19.tar", last modified: Sat Jul 15 08:25:01 2023, max compression
```

## Comparing `LolzteamApi-1.0.18.tar` & `LolzteamApi-1.0.19.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 05:30:26.608044 LolzteamApi-1.0.18/
--rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.18/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-10 05:30:26.602043 LolzteamApi-1.0.18/LolzteamApi/
--rw-rw-rw-   0        0        0   167776 2023-07-10 05:28:40.000000 LolzteamApi-1.0.18/LolzteamApi/LolzteamApi.py
--rw-rw-rw-   0        0        0       36 2023-07-10 00:23:41.000000 LolzteamApi-1.0.18/LolzteamApi/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-10 05:30:26.606045 LolzteamApi-1.0.18/LolzteamApi.egg-info/
--rw-rw-rw-   0        0        0     2261 2023-07-10 05:30:26.000000 LolzteamApi-1.0.18/LolzteamApi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-07-10 05:30:26.000000 LolzteamApi-1.0.18/LolzteamApi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 05:30:26.000000 LolzteamApi-1.0.18/LolzteamApi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-07-10 05:30:26.000000 LolzteamApi-1.0.18/LolzteamApi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-10 05:30:26.000000 LolzteamApi-1.0.18/LolzteamApi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2261 2023-07-10 05:30:26.607045 LolzteamApi-1.0.18/PKG-INFO
--rw-rw-rw-   0        0        0     1860 2023-07-10 01:19:44.000000 LolzteamApi-1.0.18/README.md
--rw-rw-rw-   0        0        0       42 2023-07-10 05:30:26.608044 LolzteamApi-1.0.18/setup.cfg
--rw-rw-rw-   0        0        0      694 2023-07-10 01:23:22.000000 LolzteamApi-1.0.18/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:25:01.957109 LolzteamApi-1.0.19/
+-rw-rw-rw-   0        0        0     1089 2023-07-08 18:11:39.000000 LolzteamApi-1.0.19/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-15 08:25:01.950106 LolzteamApi-1.0.19/LolzteamApi/
+-rw-rw-rw-   0        0        0   175980 2023-07-15 08:15:04.000000 LolzteamApi-1.0.19/LolzteamApi/LolzteamApi.py
+-rw-rw-rw-   0        0        0       43 2023-07-15 08:07:56.000000 LolzteamApi-1.0.19/LolzteamApi/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 08:25:01.955105 LolzteamApi-1.0.19/LolzteamApi.egg-info/
+-rw-rw-rw-   0        0        0     2262 2023-07-15 08:25:01.000000 LolzteamApi-1.0.19/LolzteamApi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-07-15 08:25:01.000000 LolzteamApi-1.0.19/LolzteamApi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 08:25:01.000000 LolzteamApi-1.0.19/LolzteamApi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-07-15 08:25:01.000000 LolzteamApi-1.0.19/LolzteamApi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-07-15 08:25:01.000000 LolzteamApi-1.0.19/LolzteamApi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2262 2023-07-15 08:25:01.956106 LolzteamApi-1.0.19/PKG-INFO
+-rw-rw-rw-   0        0        0     1860 2023-07-10 01:19:44.000000 LolzteamApi-1.0.19/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 08:25:01.958106 LolzteamApi-1.0.19/setup.cfg
+-rw-rw-rw-   0        0        0      695 2023-07-15 08:10:04.000000 LolzteamApi-1.0.19/setup.py
```

### Comparing `LolzteamApi-1.0.18/LICENSE` & `LolzteamApi-1.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.18/LolzteamApi/LolzteamApi.py` & `LolzteamApi-1.0.19/LolzteamApi/LolzteamApi.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,26 +2,107 @@
 import time
 import json
 
 from importlib.metadata import version
 from bs4 import BeautifulSoup
 
 
+class Types:
+    class Proxy:  # LolzteamApi init
+        socks5 = "SOCKS5"
+        socks4 = "SOCKS4"
+        http = "HTTP"
+        https = "HTTPS"
+
+    class Market:
+        class Operation_types:
+            income = "income"
+            cost = "cost"
+            refilled_balance = "refilled_balance"
+            withdrawal_balance = "withdrawal_balance"
+            paid_item = "paid_item"
+            sold_item = "sold_item"
+            money_transfer = "money_transfer"
+            receiving_money = "receiving_money"
+            internal_purchase = "internal_purchase"
+            claim_hold = "claim_hold"
+
+        class Length:
+            hour = "hour"
+            day = "day"
+            week = "week"
+            month = "month"
+            year = "year"
+
+        class Currency:
+            cny = "cny"
+            usd = "usd"
+            rub = "rub"
+            eur = "eur"
+            uah = "uah"
+            kzt = "kzt"
+            byn = "byn"
+            gbp = "gbp"
+
+        class Item_origin:
+            brute = "brute"
+            stealer = "stealer"
+            fishing = "fishing"
+            autoreg = "autoreg"
+            personal = "personal"
+            resale = "resale"
+            retrieve = "retrieve"
+
+        class Guarantee:
+            half_day = -1
+            day = 0
+            three_days = 1
+
+    class Forum:
+        class Contests:
+            class Length:
+                minutes = "minutes"
+                hours = "hours"
+                days = "days"
+
+            class Upgrade_prizes:
+                supreme = 1
+                legend = 6
+                antipublic = 12
+                uniq = 14
+                photo_leaks = 17
+                auto_participation = 19
+
+
 class LolzteamApi:
-    def __init__(self, token: str, bypass_429: bool = True, language: str = "RU", disable_update_check: bool = False):
+    def __init__(self, token: str, bypass_429: bool = True, language: str = "RU", disable_update_check: bool = False,
+                 proxy_type: str = None, proxy: str = None):
         """
         :param token: Your token. You can get in there -> https://zelenka.guru/account/api
         :param bypass_429: Bypass status code 429 by sleep
         :param language: Language for your api responses. Pass "en" if you want to get responses in english or pass "ru" if you want to get responses in russian.
         :param disable_update_check: Pass True if you don't want to see annoying update message
+        :param proxy_type: Your proxy type. You can use types ( Types.Proxy.socks5 or socks4,https,http )
+        :param proxy: Proxy string. Example -> ip:port or login:password@ip:port
         """
 
         if not disable_update_check:
             self.__check_for_new_version()
 
+        if proxy_type is not None:
+            proxy_type = proxy_type.upper()
+            if proxy_type in ["HTTPS", "HTTP", "SOCKS4", "SOCKS5"]:
+                self.__proxy_type = proxy_type
+                self.__proxy = proxy
+            else:
+                raise Exception(f"Proxy type has invalid value. It can be only https,http,socks4 or socks5")
+        else:
+            self.__proxy = None
+            self.__proxy_type = None
+
         self.__token = token
         self.__headers = {'Authorization': f"bearer {self.__token}"}
 
         self.__bypass_429 = bypass_429
         self.__auto_delay_time = time.time() - 3
         self.__locale = language
         self.__token_user_id = self.__set_user_id
@@ -32,31 +113,62 @@
     def send_request(self, method: str, url: str, params: dict = None, data=None, files=None):
         method = method.upper()
         LolzteamApi.__auto_delay(self)
 
         if params is None:
             params = {}
         params["locale"] = self.__locale
+        proxies = {}
+        if self.__proxy_type is not None:
+            match self.__proxy_type:
+                case "HTTP":
+                    proxies = {
+                        "http": f"http://{self.__proxy}",
+                        "https": f"http://{self.__proxy}"
+                    }
+                case "HTTPS":
+                    proxies = {
+                        "http": f"http://{self.__proxy}",
+                        "https": f"https://{self.__proxy}"
+                    }
+                case "SOCKS4":
+                    proxies = {
+                        "http": f"socks4://{self.__proxy}",
+                        "https": f"socks4://{self.__proxy}"
+                    }
+                case "SOCKS5":
+                    proxies = {
+                        "http": f"socks5://{self.__proxy}",
+                        "https": f"socks5://{self.__proxy}"
+                    }
+                case _:
+                    raise Exception(
+                        f"Proxy type has invalid value. It can be only https,http,socks4 or socks5")  # How tf you get that error?
         match method:
             case "GET":
-                response = requests.get(url=url, params=params, data=data, files=files, headers=self.__headers)
+                response = requests.get(url=url, params=params, data=data, files=files, headers=self.__headers,
+                                        proxies=proxies)
             case "POST":
-                response = requests.post(url=url, params=params, data=data, files=files, headers=self.__headers)
+                response = requests.post(url=url, params=params, data=data, files=files, headers=self.__headers,
+                                         proxies=proxies)
             case "PUT":
-                response = requests.put(url=url, params=params, data=data, files=files, headers=self.__headers)
+                response = requests.put(url=url, params=params, data=data, files=files, headers=self.__headers,
+                                        proxies=proxies)
             case "DELETE":
-                response = requests.delete(url=url, params=params, data=data, files=files, headers=self.__headers)
+                response = requests.delete(url=url, params=params, data=data, files=files, headers=self.__headers,
+                                           proxies=proxies)
             case _:
-                response = {"error": "Создатель либы где-то проебался. Отпиши @AS7RID в тг, он починит"}
+                raise Exception(f"Invalid requests method. Contact @AS7RID")
         self.__auto_delay_time = time.time()
         try:
             return response.json()
         except requests.exceptions.JSONDecodeError:
             return response.text
 
+    # noinspection PyTypeChecker
     def __set_user_id(self):
         url = "https://api.lzt.market/me"
         response = LolzteamApi.send_request(self=self, method="GET", url=url)
         try:
             return response["user"]["user_id"]
         except KeyError:
             return None
@@ -92,14 +204,32 @@
             print()
 
     def change_token(self, new_token: str):
         self.__token = new_token
         self.__token_user_id = self.__set_user_id()
         self.__headers = {'Authorization': f"bearer {self.__token}"}
 
+    def change_proxy(self, proxy_type: str = None, proxy: str = None):
+        """
+        Delete or change your proxy
+
+        Skip proxy_type and proxy if you want to delete it
+
+        :param proxy_type: Your proxy type. You can use types ( Types.Proxy.socks5 or socks4,https,http )
+        :param proxy: Proxy string. Example -> ip:port or login:password@ip:port
+        """
+        if proxy_type is not None:
+            if proxy_type in ["HTTPS", "HTTP", "SOCKS4", "SOCKS5"]:
+                self.__proxy_type = proxy_type
+            else:
+                raise Exception(f"Proxy type has invalid value. It can be only https,http,socks4 or socks5")
+        else:
+            self.__proxy_type = None
+        self.__proxy = proxy
+
     class __Forum:
         def __init__(self, api_self):
             self.__api = api_self  # Passing main self to sub all classes
 
             #  Sections definitions
             self.categories = self.__Categories(self.__api)
             self.forums = self.__Forums(self.__api)
@@ -2377,16 +2507,17 @@
                     "allow_accept_accounts": allow_accept_accounts,
                     "hide_favourites": hide_favourites,
                     "vk_ua": vk_ua
                 }
                 return LolzteamApi.send_request(self=self.__api, method="PUT", url=url, params=params)
 
             # Copy of __List.owned
-            def owned(self, user_id: int = None, category_id: int = None, pmin: int = None, pmax: int = None,
-                      title: str = None):
+            def owned(self, user_id: int = None, page: int = None, category_id: int = None, pmin: int = None,
+                      pmax: int = None,
+                      title: str = None, search_params: dict = None):
                 """
                 GET https://api.lzt.market/user/user_id/items
 
                 Displays a list of owned accounts.
 
                 Category id-names list:
 
@@ -2437,39 +2568,46 @@
                 26 - spotify - Spotify
 
                 27 - war-thunder - War Thunder
 
                 Required scopes: market
 
                 :param user_id: ID of user.
+                :param page: Page
                 :param category_id: Accounts category
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
+                :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
+
                 if user_id is None:  # Tweak
                     if type(self.__token_user_id) is not int:
                         self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
-                url = f"https://api.lzt.market/user/{user_id}/items"
                 params = {
                     "user_id": user_id,
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
-                    "title": title
+                    "title": title,
+                    "page": page
                 }
+                if search_params is not None:
+                    for key, value in search_params.items():
+                        params[str(key)] = value
+                url = f"https://api.lzt.market/user/{user_id}/items"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             # Copy of __List.purchased
-            def purchased(self, user_id: int = None, category_id: int = None, pmin: int = None, pmax: int = None,
-                          title: str = None):
+            def purchased(self, user_id: int = None, page: int = None, category_id: int = None, pmin: int = None,
+                          pmax: int = None, title: str = None, search_params: dict = None):
                 """
                 GET https://api.lzt.market/user/user_id/orders
 
                 Displays a list of purchased accounts.
 
                 Category id-names list:
 
@@ -2520,74 +2658,88 @@
                 26 - spotify - Spotify
 
                 27 - war-thunder - War Thunder
 
                 Required scopes: market
 
                 :param user_id: ID of user.
+                :param page: Page
                 :param category_id: Accounts category
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
+                :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
 
                 if user_id is None:  # Tweak
                     if type(self.__token_user_id) is not int:
                         self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 params = {
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
-                    "title": title
+                    "title": title,
+                    "page": page
                 }
+                if search_params is not None:
+                    for key, value in search_params.items():
+                        params[str(key)] = value
                 url = f"https://api.lzt.market/user/{user_id}/orders"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             # Copy of __List.favorite
-            def favorite(self, page: int = None):
+            def favorite(self, page: int = None, search_params: dict = None):
                 """
                 GET https://api.lzt.market/fave
 
                 Displays a list of favourites accounts.
 
                 Required scopes: market
 
                 :param page: The number of the page to display results from
+                :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
                 url = "https://api.lzt.market/fave"
                 params = {
                     "page": page
                 }
+                if search_params is not None:
+                    for key, value in search_params.items():
+                        params[str(key)] = value
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             # Copy of __List.viewed
-            def viewed(self, page: int = None):
+            def viewed(self, page: int = None, search_params: dict = None):
                 """
                 GET https://api.lzt.market/viewed
 
                 Displays a list of viewed accounts.
 
                 Required scopes: market
 
                 :param page: The number of the page to display results from
+                :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
                 url = "https://api.lzt.market/viewed"
                 params = {
                     "page": page
                 }
+                if search_params is not None:
+                    for key, value in search_params.items():
+                        params[str(key)] = value
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
         class __List:
             def __init__(self, api_self, token_user_id):
                 self.__api = api_self
                 self.__token_user_id = token_user_id
 
@@ -2613,15 +2765,15 @@
                     params = {
                         "top_queries": top_queries
                     }
                     return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
                 def get(self, category_name: str, pmin: int = None, pmax: int = None, title: str = None,
                         parse_sticky_items: bool = None, parse_same_items: bool = None, games: list[int] or int = None,
-                        page: int = None):
+                        page: int = None, search_params: dict = None):
                     """
                     GET https://api.lzt.market/categoryName
 
                     Displays a list of accounts in a specific category according to your parameters.
 
                     Category id-names list:
 
@@ -2679,28 +2831,32 @@
                     :param pmin: Minimal price of account (Inclusive)
                     :param pmax: Maximum price of account (Inclusive)
                     :param title: The word or words contained in the account title
                     :param parse_sticky_items: If true, API will return stickied accounts in results
                     :param parse_same_items: If true, API will return account history in results
                     :param games: The ID of a game found on the account
                     :param page: The number of the page to display results from
-
+                    :param search_params: Search params for your request. Example {"origin":"autoreg"} will return only "autoreg" accounts
                     :return: json server response
 
                     """
+                    category_name = category_name.lower()
                     url = f"https://api.lzt.market/{category_name}"
                     params = {
                         "pmin": pmin,
                         "pmax": pmax,
                         "title": title,
                         "parse_sticky_items": parse_sticky_items,
                         "parse_same_items": parse_same_items,
                         "game[]": games,
                         "page": page
                     }
+                    if search_params is not None:
+                        for key, value in search_params.items():
+                            params[str(key)] = value
                     return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
                 def params(self, category_name: str):
                     """
                     GET https://api.lzt.market/category_name/params
 
                     Displays search parameters for a category.
@@ -2825,35 +2981,39 @@
                     :param category_name: Name of category.
 
                     :return: json server response
                     """
                     url = f"https://api.lzt.market/{category_name}/games"
                     return LolzteamApi.send_request(self=self.__api, method="GET", url=url)
 
-            def new(self, page: int = None):
+            def new(self, page: int = None, search_params: dict = None):
                 """
                 GET https://api.lzt.market/
 
                 Displays a list of the latest accounts.
 
                 Required scopes: market
 
                 :param page: The number of the page to display results from
+                :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
                 url = "https://api.lzt.market/"
                 params = {
                     "page": page
                 }
+                if search_params is not None:
+                    for key, value in search_params.items():
+                        params[str(key)] = value
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
-            def owned(self, user_id: int = None, category_id: int = None, pmin: int = None, pmax: int = None,
-                      title: str = None):
+            def owned(self, user_id: int = None, page: int = None, category_id: int = None, pmin: int = None,
+                      pmax: int = None, title: str = None, search_params: dict = None):
                 """
                 GET https://api.lzt.market/user/user_id/items
 
                 Displays a list of owned accounts.
 
                 Category id-names list:
 
@@ -2904,39 +3064,45 @@
                 26 - spotify - Spotify
 
                 27 - war-thunder - War Thunder
 
                 Required scopes: market
 
                 :param user_id: ID of user.
+                :param page: Page
                 :param category_id: Accounts category
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
+                :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
 
                 if user_id is None:  # Tweak
                     if type(self.__token_user_id) is not int:
                         self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 params = {
                     "user_id": user_id,
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
-                    "title": title
+                    "title": title,
+                    "page": page
                 }
+                if search_params is not None:
+                    for key, value in search_params.items():
+                        params[str(key)] = value
                 url = f"https://api.lzt.market/user/{user_id}/items"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
-            def purchased(self, user_id: int = None, category_id: int = None, pmin: int = None, pmax: int = None,
-                          title: str = None):
+            def purchased(self, user_id: int = None, page: int = None, category_id: int = None, pmin: int = None,
+                          pmax: int = None, title: str = None, search_params: dict = None):
                 """
                 GET https://api.lzt.market/user/user_id/orders
 
                 Displays a list of purchased accounts.
 
                 Category id-names list:
 
@@ -2987,72 +3153,86 @@
                 26 - spotify - Spotify
 
                 27 - war-thunder - War Thunder
 
                 Required scopes: market
 
                 :param user_id: ID of user.
+                :param page: Page
                 :param category_id: Accounts category
                 :param pmin: Minimal price of account (Inclusive)
                 :param pmax: Maximum price of account (Inclusive)
                 :param title: The word or words contained in the account title
+                :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
 
                 if user_id is None:  # Tweak
                     if type(self.__token_user_id) is not int:
                         self.__token_user_id = self.__token_user_id()
                     user_id = self.__token_user_id
                 params = {
                     "category_id": category_id,
                     "pmin": pmin,
                     "pmax": pmax,
-                    "title": title
+                    "title": title,
+                    "page": page
                 }
+                if search_params is not None:
+                    for key, value in search_params.items():
+                        params[str(key)] = value
                 url = f"https://api.lzt.market/user/{user_id}/orders"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
-            def favorite(self, page: int = None):
+            def favorite(self, page: int = None, search_params: dict = None):
                 """
                 GET https://api.lzt.market/fave
 
                 Displays a list of favourites accounts.
 
                 Required scopes: market
 
                 :param page: The number of the page to display results from
+                :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
                 url = "https://api.lzt.market/fave"
                 params = {
                     "page": page
                 }
+                if search_params is not None:
+                    for key, value in search_params.items():
+                        params[str(key)] = value
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
-            def viewed(self, page: int = None):
+            def viewed(self, page: int = None, search_params: dict = None):
                 """
                 GET https://api.lzt.market/viewed
 
                 Displays a list of viewed accounts.
 
                 Required scopes: market
 
                 :param page: The number of the page to display results from
+                :param search_params: Search params for your request. Example {"category_id":19} will return only VPN accounts
 
                 :return: json server response
 
                 """
                 url = "https://api.lzt.market/viewed"
                 params = {
                     "page": page
                 }
+                if search_params is not None:
+                    for key, value in search_params.items():
+                        params[str(key)] = value
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
             def get(self, item_id: int, steam_preview: bool = False, preview_type: str = None):
                 """
                 GET https://api.lzt.market/item_id
                 GET https://api.lzt.market/item_id/steam-preview
 
@@ -3137,15 +3317,16 @@
                     "comment": comment,
                     "is_hold": is_hold,
                     "show_payments_stats": show_payments_stats
                 }
                 url = f"https://api.lzt.market/user/{user_id}/payments"
                 return LolzteamApi.send_request(self=self.__api, method="GET", url=url, params=params)
 
-            def transfer(self, amount: int, secret_answer: str, currency: str = "rub", user_id: int = None,
+            def transfer(self, amount: int, secret_answer: str, currency: str = Types.Market.Currency.rub,
+                         user_id: int = None,
                          username: str = None, comment: str = None, transfer_hold: bool = None,
                          hold_length_option: str = None,
                          hold_length_value: int = None):
                 """
                 POST https://api.lzt.market/balance/transfer
 
                 Send money to any user.
@@ -3176,15 +3357,15 @@
                     "hold_length_value": hold_length_value,
                     "hold_length_option": hold_length_option
                 }
                 return LolzteamApi.send_request(self=self.__api, method="POST", url=url, params=params)
 
             @staticmethod
             def generate_link(amount: int, user_id: int = None, username: str = None, comment: str = None,
-                              redirect_url: str = None, currency: str = None,hold:bool=None):
+                              redirect_url: str = None, currency: str = None, hold: bool = None):
                 """
                 Generate payment link
 
                 Required scopes: None
 
                 :param amount: Amount to send in your currency.
                 :param user_id: ID of user to transfer money
@@ -3204,15 +3385,15 @@
                 params = {
                     "user_id": user_id,
                     "username": username,
                     "amount": amount,
                     "comment": comment,
                     "redirect": redirect_url,
                     "currency": currency,
-                    "hold":hold
+                    "hold": hold
                 }
                 url = "https://lzt.market/balance/transfer"
                 req = requests.models.PreparedRequest()
                 req.prepare_url(url=url, params=params)
                 return req.url
 
         class __Managing:
@@ -3789,16 +3970,15 @@
                 }
                 return LolzteamApi.send_request(self=self.__api, method="POST", url=url, params=params)
 
             def fast_sell(self, category_id: int, price: int, currency: str, item_origin: str, extended_guarantee: int,
                           title: str = None, title_en: str = None, description: str = None, information: str = None,
                           has_email_login_data: bool = None, email_login_data: str = None, email_type: str = None,
                           allow_ask_discount: bool = None, proxy_id: int = None, random_proxy: bool = None,
-                          login: str = None,
-                          password: str = None, login_password: str = None, extra: dict = None, ):
+                          login: str = None, password: str = None, login_password: str = None, extra: dict = None, ):
                 """
                 POST https://api.lzt.market/item/fast-sell
 
                 Adds and check account on validity. If account is valid, account will be published on the market.
 
                 Account origin:
```

### Comparing `LolzteamApi-1.0.18/LolzteamApi.egg-info/PKG-INFO` & `LolzteamApi-1.0.19/LolzteamApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.18
+Version: 1.0.19
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Lolzteam Python API
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.18 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.19 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
 darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/
 transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE) ## Installation
```

### Comparing `LolzteamApi-1.0.18/PKG-INFO` & `LolzteamApi-1.0.19/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: LolzteamApi
-Version: 1.0.18
+Version: 1.0.19
 Summary: A library that contains all the methods of the Lolzteam API (Market/Forum)
 Home-page: https://github.com/AS7RIDENIED/Lolzteam_Python_Api
 Author: AS7RID
 Author-email: as7ridwork@gmail.com
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 
 # Lolzteam Python API
 
 <p align="center">
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.18 Summary: A library that
+Metadata-Version: 2.1 Name: LolzteamApi Version: 1.0.19 Summary: A library that
 contains all the methods of the Lolzteam API (Market/Forum) Home-page: https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api Author: AS7RID Author-email:
 as7ridwork@gmail.com Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
 LICENSE # Lolzteam Python API
                              [Material_Bread_logo]
 [![Static Badge](https://img.shields.io/badge/DONATE-LOLZTEAM-
 darkgreen?style=flat-square&logo=qiwi)](https://lzt.market/balance/
 transfer?user_id=2410024&comment=Thanks%20for%20creating%20LolzteamApi&amount=250)
 [![License](https://img.shields.io/badge/license-MIT-blue.svg)](https://
 github.com/AS7RIDENIED/Lolzteam_Python_Api/blob/main/LICENSE) ## Installation
```

### Comparing `LolzteamApi-1.0.18/README.md` & `LolzteamApi-1.0.19/README.md`

 * *Files identical despite different names*

### Comparing `LolzteamApi-1.0.18/setup.py` & `LolzteamApi-1.0.19/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 requirements = ["requests", "beautifulsoup4"]
 
 setuptools.setup(
     name="LolzteamApi",
-    version="1.0.18",
+    version="1.0.19",
     author="AS7RID",
     author_email="as7ridwork@gmail.com",
     description="A library that contains all the methods of the Lolzteam API (Market/Forum)",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/AS7RIDENIED/Lolzteam_Python_Api",
     packages=setuptools.find_packages(),
     install_requires=requirements,
     classifiers=["Programming Language :: Python :: 3.11"],
-    python_requires='>=3.6'
+    python_requires='>=3.10'
 )
```

