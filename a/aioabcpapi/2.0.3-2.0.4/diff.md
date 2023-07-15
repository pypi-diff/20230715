# Comparing `tmp/aioabcpapi-2.0.3.tar.gz` & `tmp/aioabcpapi-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioabcpapi-2.0.3.tar", last modified: Sat Jun 24 18:10:02 2023, max compression
+gzip compressed data, was "aioabcpapi-2.0.4.tar", last modified: Sat Jul 15 19:03:49 2023, max compression
```

## Comparing `aioabcpapi-2.0.3.tar` & `aioabcpapi-2.0.4.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.149711 aioabcpapi-2.0.3/
--rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.3/LICENSE
--rw-rw-rw-   0        0        0     5371 2023-06-24 18:10:02.149711 aioabcpapi-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.013440 aioabcpapi-2.0.3/aioabcpapi/
--rw-rw-rw-   0        0        0      530 2023-06-24 18:09:53.000000 aioabcpapi-2.0.3/aioabcpapi/__init__.py
--rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.3/aioabcpapi/abcp.py
--rw-rw-rw-   0        0        0    20198 2023-06-24 10:52:34.000000 aioabcpapi-2.0.3/aioabcpapi/api.py
--rw-rw-rw-   0        0        0     4794 2023-06-24 13:28:13.000000 aioabcpapi-2.0.3/aioabcpapi/base.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.078085 aioabcpapi-2.0.3/aioabcpapi/cp/
--rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.3/aioabcpapi/cp/__init__.py
--rw-rw-rw-   0        0        0   113820 2023-06-24 12:52:15.000000 aioabcpapi-2.0.3/aioabcpapi/cp/admin.py
--rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.3/aioabcpapi/cp/base.py
--rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.3/aioabcpapi/cp/client.py
--rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.3/aioabcpapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.113142 aioabcpapi-2.0.3/aioabcpapi/ts/
--rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.3/aioabcpapi/ts/__init__.py
--rw-rw-rw-   0        0        0   123974 2023-06-24 13:18:40.000000 aioabcpapi-2.0.3/aioabcpapi/ts/admin.py
--rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.3/aioabcpapi/ts/base.py
--rw-rw-rw-   0        0        0    45528 2023-06-24 13:28:13.000000 aioabcpapi-2.0.3/aioabcpapi/ts/client.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.132145 aioabcpapi-2.0.3/aioabcpapi/utils/
--rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.3/aioabcpapi/utils/__init__.py
--rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.3/aioabcpapi/utils/fields_checker.py
--rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.3/aioabcpapi/utils/payload.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.039082 aioabcpapi-2.0.3/aioabcpapi.egg-info/
--rw-rw-rw-   0        0        0     5371 2023-06-24 18:10:01.000000 aioabcpapi-2.0.3/aioabcpapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-06-24 18:10:01.000000 aioabcpapi-2.0.3/aioabcpapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-24 18:10:01.000000 aioabcpapi-2.0.3/aioabcpapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-06-24 18:10:01.000000 aioabcpapi-2.0.3/aioabcpapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-06-24 18:10:01.000000 aioabcpapi-2.0.3/aioabcpapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      206 2023-06-24 18:10:02.151712 aioabcpapi-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1329 2023-06-24 18:09:53.000000 aioabcpapi-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-24 18:10:02.147711 aioabcpapi-2.0.3/test/
--rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.3/test/test_payload.py
+drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.938714 aioabcpapi-2.0.4/
+-rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5371 2023-07-15 19:03:49.939715 aioabcpapi-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.813686 aioabcpapi-2.0.4/aioabcpapi/
+-rw-rw-rw-   0        0        0      530 2023-07-15 19:02:39.000000 aioabcpapi-2.0.4/aioabcpapi/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.4/aioabcpapi/abcp.py
+-rw-rw-rw-   0        0        0    20592 2023-07-15 18:42:11.000000 aioabcpapi-2.0.4/aioabcpapi/api.py
+-rw-rw-rw-   0        0        0     4794 2023-06-24 13:28:13.000000 aioabcpapi-2.0.4/aioabcpapi/base.py
+drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.890703 aioabcpapi-2.0.4/aioabcpapi/cp/
+-rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.4/aioabcpapi/cp/__init__.py
+-rw-rw-rw-   0        0        0   113820 2023-06-24 12:52:15.000000 aioabcpapi-2.0.4/aioabcpapi/cp/admin.py
+-rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.4/aioabcpapi/cp/base.py
+-rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.4/aioabcpapi/cp/client.py
+-rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.4/aioabcpapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.904706 aioabcpapi-2.0.4/aioabcpapi/ts/
+-rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.4/aioabcpapi/ts/__init__.py
+-rw-rw-rw-   0        0        0   126277 2023-07-15 18:59:44.000000 aioabcpapi-2.0.4/aioabcpapi/ts/admin.py
+-rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.4/aioabcpapi/ts/base.py
+-rw-rw-rw-   0        0        0    47055 2023-07-15 18:54:00.000000 aioabcpapi-2.0.4/aioabcpapi/ts/client.py
+drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.923710 aioabcpapi-2.0.4/aioabcpapi/utils/
+-rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.4/aioabcpapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.4/aioabcpapi/utils/fields_checker.py
+-rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.4/aioabcpapi/utils/payload.py
+drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.842692 aioabcpapi-2.0.4/aioabcpapi.egg-info/
+-rw-rw-rw-   0        0        0     5371 2023-07-15 19:03:49.000000 aioabcpapi-2.0.4/aioabcpapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-07-15 19:03:49.000000 aioabcpapi-2.0.4/aioabcpapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 19:03:49.000000 aioabcpapi-2.0.4/aioabcpapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-15 19:03:49.000000 aioabcpapi-2.0.4/aioabcpapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-07-15 19:03:49.000000 aioabcpapi-2.0.4/aioabcpapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      206 2023-07-15 19:03:49.945715 aioabcpapi-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1329 2023-07-15 19:02:39.000000 aioabcpapi-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.937713 aioabcpapi-2.0.4/test/
+-rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.4/test/test_payload.py
```

### Comparing `aioabcpapi-2.0.3/LICENSE` & `aioabcpapi-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/PKG-INFO` & `aioabcpapi-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 2.0.3
+Version: 2.0.4
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-2.0.3/README.md` & `aioabcpapi-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/aioabcpapi/__init__.py` & `aioabcpapi-2.0.4/aioabcpapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,9 +5,9 @@
                          AbcpParameterRequired, TeaPot)
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 
 __author__ = 'bl4ckm45k'
-__version__ = '2.0.3'
+__version__ = '2.0.4'
 __email__ = 'nonpowa@gmail.com'
```

### Comparing `aioabcpapi-2.0.3/aioabcpapi/abcp.py` & `aioabcpapi-2.0.4/aioabcpapi/abcp.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/aioabcpapi/api.py` & `aioabcpapi-2.0.4/aioabcpapi/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -330,14 +330,18 @@
         @dataclass(frozen=True)
         class Positions:
             GET: str = 'ts/positions/get'
             GET_LIST: str = 'ts/positions/list'
             CANCEL: str = 'ts/positions/cancel'
             MASS_CANCEL: str = 'ts/positions/massCancel'
 
+        @dataclass(frozen=True)
+        class Agreements:
+            get_list: str = 'cp/ts/agreements/list'
+
     @dataclass(frozen=True)
     class TsAdmin:
         @dataclass(frozen=True)
         class OrderPickings:
             FAST_GET_OUT: str = 'cp/ts/orderPickings/fastGetOut'
             GET: str = 'cp/ts/orderPickings/get'
             GET_GOODS: str = 'cp/ts/orderPickings/getGoods'
@@ -390,28 +394,29 @@
 
         @dataclass(frozen=True)
         class DistributorOwners:
             DISTRIBUTOR_OWNERS: str = 'cp/ts/distributorOwners'
 
         @dataclass(frozen=True)
         class Orders:
-            CREATE: str = 'cp/ts/orders/create'
-            CREATE_BY_CART: str = 'cp/ts/orders/createByCart'
-            LIST: str = 'cp/ts/orders/list'
-            GET: str = 'cp/ts/orders/get'
-            REFUSE: str = 'cp/ts/orders/refuse'
-            UPDATE: str = 'cp/ts/orders/update'
-            MERGE: str = 'cp/ts/orders/merge'
-            SPLIT: str = 'cp/ts/orders/split'
-            REPRICE: str = 'cp/ts/orders/reprice'
-            MESSAGES_CREATE: str = 'cp/ts/orders/messages/create'
-            MESSAGES_GET_ONE: str = 'cp/ts/orders/messages/get'
-            MESSAGES_LIST: str = 'cp/ts/orders/messages/list'
-            MESSAGES_UPDATE: str = 'cp/ts/orders/messages/update'
-            MESSAGES_DELETE: str = 'cp/ts/orders/messages/delete'
+            __section: str = 'cp/ts/orders'
+            CREATE: str = f'{__section}/create'
+            CREATE_BY_CART: str = f'{__section}/createByCart'
+            LIST: str = f'{__section}/list'
+            GET: str = f'{__section}/get'
+            REFUSE: str = f'{__section}/refuse'
+            UPDATE: str = f'{__section}/update'
+            MERGE: str = f'{__section}/merge'
+            SPLIT: str = f'{__section}/split'
+            REPRICE: str = f'{__section}/reprice'
+            MESSAGES_CREATE: str = f'{__section}/messages/create'
+            MESSAGES_GET_ONE: str = f'{__section}/messages/get'
+            MESSAGES_LIST: str = f'{__section}/messages/list'
+            MESSAGES_UPDATE: str = f'{__section}/messages/update'
+            MESSAGES_DELETE: str = f'{__section}/messages/delete'
 
         @dataclass(frozen=True)
         class Cart:
             CREATE: str = 'cp/ts/cart/create'
             UPDATE: str = 'cp/ts/cart/update'
             GET_LIST: str = 'cp/ts/cart/list'
             EXIST: str = 'cp/ts/cart/exists'
@@ -468,14 +473,22 @@
             GET_LIST: str = 'cp/ts/payments/list'
             CREATE: str = 'cp/ts/payments/create'
 
         @dataclass(frozen=True)
         class PaymentMethods:
             METHODS_LIST: str = 'cp/ts/paymentMethods/list'
 
+        @dataclass(frozen=True)
+        class Agreements:
+            get_list: str = 'cp/ts/agreements/list'
+
+        @dataclass(frozen=True)
+        class LegalPersons:
+            get_list: str = 'cp/ts/legalPersons/list'
+
     class VinQu:
         pass
 
     class TecDoc:
         pass
```

### Comparing `aioabcpapi-2.0.3/aioabcpapi/base.py` & `aioabcpapi-2.0.4/aioabcpapi/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/aioabcpapi/cp/admin.py` & `aioabcpapi-2.0.4/aioabcpapi/cp/admin.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/aioabcpapi/cp/client.py` & `aioabcpapi-2.0.4/aioabcpapi/cp/client.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/aioabcpapi/exceptions.py` & `aioabcpapi-2.0.4/aioabcpapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/aioabcpapi/ts/admin.py` & `aioabcpapi-2.0.4/aioabcpapi/ts/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         self.cart = Cart(base)
         self.positions = Positions(base)
         self.good_receipts = GoodReceipts(base)
         self.tags = Tags(base)
         self.tags_relationships = TagsRelationships(base)
         self.payments = Payments(base)
         self.payment_methods = PaymentMethods(base)
+        self.agrements = Agreements(base)
+        self.legal_persons = LegalPersons(base)
 
 
 class SupplierReturns:
 
     def __init__(self, base: BaseAbcp):
         self._base = base
         self.operations = SupplierReturnsOperations(base)
@@ -1993,7 +1995,51 @@
         """
         if isinstance(allow_change_payment, str) and allow_change_payment not in self._Fields.allow_change_param:
             raise AbcpWrongParameterError(f'Неверное значение параметра "allow_change_payment" {allow_change_payment}.'
                                           f'Допустимые значения {self._Fields.allow_change_param}')
 
         payload = generate_payload(**locals())
         return await self._base.request(_Methods.TsAdmin.PaymentMethods.METHODS_LIST, payload)
+
+
+class Agreements:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
+    async def get_list(self, contractor_ids: Union[int, List[int]] = None,
+                       contractor_requisite_ids: Union[int, List[int]] = None,
+                       shop_requisite_ids: Union[int, List[int]] = None,
+                       is_active: bool = None, is_delete: bool = None, is_default: bool = None,
+                       agreement_type: int = None, relation_type: int = None,
+                       number: str = None, currency: str = None,
+                       date_start: Union[datetime, str] = None, date_end: Union[datetime, str] = None,
+                       credit_limit: Union[float, int] = None,
+                       limit: int = None, skip: int = None):
+        if isinstance(date_start, datetime):
+            date_start = generate(date_start.replace(tzinfo=pytz.utc))
+        if isinstance(date_end, datetime):
+            date_end = generate(date_end.replace(tzinfo=pytz.utc))
+
+        if isinstance(contractor_ids, int):
+            contractor_ids = [contractor_ids]
+        if isinstance(contractor_requisite_ids, int):
+            contractor_requisite_ids = [contractor_requisite_ids]
+        if isinstance(shop_requisite_ids, int):
+            shop_requisite_ids = [shop_requisite_ids]
+
+        payload = generate_payload(**locals())
+        return await self._base.request(_Methods.TsAdmin.Agreements.get_list, payload)
+
+
+class LegalPersons:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
+    async def get_list(self, ids: Union[str, List[str]] = None, contractor_id: Optional[int] = None,
+                       form: Optional[int] = None, org_type: Optional[int] = None,
+                       agreement_with_individuals_required: Optional[int] = None,
+                       with_tax_systems: Optional[int] = None,
+                       limit: Optional[int] = None, offset: Optional[int] = None):
+        if isinstance(ids, list):
+            ids = ','.join(map(str, ids))
+        payload = generate_payload(**locals())
+        return await self._base.request(_Methods.TsAdmin.LegalPersons.get_list, payload)
```

### Comparing `aioabcpapi-2.0.3/aioabcpapi/ts/base.py` & `aioabcpapi-2.0.4/aioabcpapi/ts/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/aioabcpapi/ts/client.py` & `aioabcpapi-2.0.4/aioabcpapi/ts/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         self._base = base
         self.good_receipts = GoodReceipts(base)
         self.order_pickings = OrderPickings(base)
         self.customer_complaints = CustomerComplaints(base)
         self.orders = Orders(base)
         self.cart = Cart(base)
         self.positions = Positions(base)
+        self.agrements = Agreements(base)
 
 
 class GoodReceipts:
     def __init__(self, base: BaseAbcp):
         self._base = base
 
     async def create(self, code: Union[str, int],
@@ -703,7 +704,36 @@
             additional_info = check_fields(additional_info, self.FieldsChecker.additional_info)
         payload = generate_payload(**locals())
         return await self._base.request(_Methods.TsClient.Positions.CANCEL, payload, True)
 
     async def mass_cancel(self, position_ids: Union[List, str, int], additional_info: Union[List, str] = None):
         payload = generate_payload(**locals())
         return await self._base.request(_Methods.TsClient.Positions.MASS_CANCEL, payload, True)
+
+
+class Agreements:
+    def __init__(self, base: BaseAbcp):
+        self._base = base
+
+    async def get_list(self, contractor_ids: Union[int, List[int]] = None,
+                       contractor_requisite_ids: Union[int, List[int]] = None,
+                       shop_requisite_ids: Union[int, List[int]] = None,
+                       is_active: bool = None, is_delete: bool = None, is_default: bool = None,
+                       agreement_type: int = None, relation_type: int = None,
+                       number: str = None, currency: str = None,
+                       date_start: Union[datetime, str] = None, date_end: Union[datetime, str] = None,
+                       credit_limit: Union[float, int] = None,
+                       limit: int = None, skip: int = None):
+        if isinstance(date_start, datetime):
+            date_start = generate(date_start.replace(tzinfo=pytz.utc))
+        if isinstance(date_end, datetime):
+            date_end = generate(date_end.replace(tzinfo=pytz.utc))
+
+        if isinstance(contractor_ids, int):
+            contractor_ids = [contractor_ids]
+        if isinstance(contractor_requisite_ids, int):
+            contractor_requisite_ids = [contractor_requisite_ids]
+        if isinstance(shop_requisite_ids, int):
+            shop_requisite_ids = [shop_requisite_ids]
+
+        payload = generate_payload(**locals())
+        return await self._base.request(_Methods.TsClient.Agreements.get_list, payload)
```

### Comparing `aioabcpapi-2.0.3/aioabcpapi/utils/fields_checker.py` & `aioabcpapi-2.0.4/aioabcpapi/utils/fields_checker.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/aioabcpapi/utils/payload.py` & `aioabcpapi-2.0.4/aioabcpapi/utils/payload.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/aioabcpapi.egg-info/PKG-INFO` & `aioabcpapi-2.0.4/aioabcpapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 2.0.3
+Version: 2.0.4
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-2.0.3/aioabcpapi.egg-info/SOURCES.txt` & `aioabcpapi-2.0.4/aioabcpapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.3/setup.py` & `aioabcpapi-2.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 requirements = ["aiohttp>=3.8.3", "certifi>=2022.12.7", "ujson>=5.7.0", "pytz>=2022.7.1", "pyrfc3339"]
 setup(
     name='aioabcpapi',
-    version='2.0.3',
+    version='2.0.4',
     author='bl4ckm45k',
     author_email='nonpowa@gmail.com',
     description='Async library for ABCP API',
     long_description_content_type="text/markdown",
     url="https://github.com/bl4ckm45k/aioabcpapi",
     license="MIT",
     packages=['aioabcpapi', 'aioabcpapi/cp', 'aioabcpapi/ts', 'aioabcpapi/utils'],
```

### Comparing `aioabcpapi-2.0.3/test/test_payload.py` & `aioabcpapi-2.0.4/test/test_payload.py`

 * *Files identical despite different names*

