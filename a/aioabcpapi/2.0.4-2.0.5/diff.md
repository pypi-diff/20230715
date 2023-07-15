# Comparing `tmp/aioabcpapi-2.0.4.tar.gz` & `tmp/aioabcpapi-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioabcpapi-2.0.4.tar", last modified: Sat Jul 15 19:03:49 2023, max compression
+gzip compressed data, was "aioabcpapi-2.0.5.tar", last modified: Sat Jul 15 20:06:51 2023, max compression
```

## Comparing `aioabcpapi-2.0.4.tar` & `aioabcpapi-2.0.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.938714 aioabcpapi-2.0.4/
--rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.4/LICENSE
--rw-rw-rw-   0        0        0     5371 2023-07-15 19:03:49.939715 aioabcpapi-2.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.813686 aioabcpapi-2.0.4/aioabcpapi/
--rw-rw-rw-   0        0        0      530 2023-07-15 19:02:39.000000 aioabcpapi-2.0.4/aioabcpapi/__init__.py
--rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.4/aioabcpapi/abcp.py
--rw-rw-rw-   0        0        0    20592 2023-07-15 18:42:11.000000 aioabcpapi-2.0.4/aioabcpapi/api.py
--rw-rw-rw-   0        0        0     4794 2023-06-24 13:28:13.000000 aioabcpapi-2.0.4/aioabcpapi/base.py
-drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.890703 aioabcpapi-2.0.4/aioabcpapi/cp/
--rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.4/aioabcpapi/cp/__init__.py
--rw-rw-rw-   0        0        0   113820 2023-06-24 12:52:15.000000 aioabcpapi-2.0.4/aioabcpapi/cp/admin.py
--rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.4/aioabcpapi/cp/base.py
--rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.4/aioabcpapi/cp/client.py
--rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.4/aioabcpapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.904706 aioabcpapi-2.0.4/aioabcpapi/ts/
--rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.4/aioabcpapi/ts/__init__.py
--rw-rw-rw-   0        0        0   126277 2023-07-15 18:59:44.000000 aioabcpapi-2.0.4/aioabcpapi/ts/admin.py
--rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.4/aioabcpapi/ts/base.py
--rw-rw-rw-   0        0        0    47055 2023-07-15 18:54:00.000000 aioabcpapi-2.0.4/aioabcpapi/ts/client.py
-drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.923710 aioabcpapi-2.0.4/aioabcpapi/utils/
--rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.4/aioabcpapi/utils/__init__.py
--rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.4/aioabcpapi/utils/fields_checker.py
--rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.4/aioabcpapi/utils/payload.py
-drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.842692 aioabcpapi-2.0.4/aioabcpapi.egg-info/
--rw-rw-rw-   0        0        0     5371 2023-07-15 19:03:49.000000 aioabcpapi-2.0.4/aioabcpapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      894 2023-07-15 19:03:49.000000 aioabcpapi-2.0.4/aioabcpapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 19:03:49.000000 aioabcpapi-2.0.4/aioabcpapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-07-15 19:03:49.000000 aioabcpapi-2.0.4/aioabcpapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-07-15 19:03:49.000000 aioabcpapi-2.0.4/aioabcpapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      206 2023-07-15 19:03:49.945715 aioabcpapi-2.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1329 2023-07-15 19:02:39.000000 aioabcpapi-2.0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 19:03:49.937713 aioabcpapi-2.0.4/test/
--rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.4/test/test_payload.py
+drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.484546 aioabcpapi-2.0.5/
+-rw-rw-rw-   0        0        0     1085 2022-05-10 19:34:18.000000 aioabcpapi-2.0.5/LICENSE
+-rw-rw-rw-   0        0        0     5371 2023-07-15 20:06:51.485547 aioabcpapi-2.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4549 2023-05-08 23:26:33.000000 aioabcpapi-2.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.400529 aioabcpapi-2.0.5/aioabcpapi/
+-rw-rw-rw-   0        0        0      530 2023-07-15 20:06:01.000000 aioabcpapi-2.0.5/aioabcpapi/__init__.py
+-rw-rw-rw-   0        0        0      653 2023-06-23 21:18:29.000000 aioabcpapi-2.0.5/aioabcpapi/abcp.py
+-rw-rw-rw-   0        0        0    20655 2023-07-15 19:33:16.000000 aioabcpapi-2.0.5/aioabcpapi/api.py
+-rw-rw-rw-   0        0        0     4794 2023-06-24 13:28:13.000000 aioabcpapi-2.0.5/aioabcpapi/base.py
+drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.444536 aioabcpapi-2.0.5/aioabcpapi/cp/
+-rw-rw-rw-   0        0        0        2 2022-07-27 23:21:17.000000 aioabcpapi-2.0.5/aioabcpapi/cp/__init__.py
+-rw-rw-rw-   0        0        0   114141 2023-07-15 20:04:31.000000 aioabcpapi-2.0.5/aioabcpapi/cp/admin.py
+-rw-rw-rw-   0        0        0      321 2023-06-23 21:51:21.000000 aioabcpapi-2.0.5/aioabcpapi/cp/base.py
+-rw-rw-rw-   0        0        0    60771 2023-06-24 10:40:46.000000 aioabcpapi-2.0.5/aioabcpapi/cp/client.py
+-rw-rw-rw-   0        0        0      535 2023-03-24 12:28:09.000000 aioabcpapi-2.0.5/aioabcpapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.453539 aioabcpapi-2.0.5/aioabcpapi/ts/
+-rw-rw-rw-   0        0        0        0 2022-05-22 19:06:06.000000 aioabcpapi-2.0.5/aioabcpapi/ts/__init__.py
+-rw-rw-rw-   0        0        0   126277 2023-07-15 18:59:44.000000 aioabcpapi-2.0.5/aioabcpapi/ts/admin.py
+-rw-rw-rw-   0        0        0      668 2023-06-24 10:35:56.000000 aioabcpapi-2.0.5/aioabcpapi/ts/base.py
+-rw-rw-rw-   0        0        0    47055 2023-07-15 18:54:00.000000 aioabcpapi-2.0.5/aioabcpapi/ts/client.py
+drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.468541 aioabcpapi-2.0.5/aioabcpapi/utils/
+-rw-rw-rw-   0        0        0        2 2022-12-13 06:33:44.000000 aioabcpapi-2.0.5/aioabcpapi/utils/__init__.py
+-rw-rw-rw-   0        0        0      805 2022-12-13 07:00:57.000000 aioabcpapi-2.0.5/aioabcpapi/utils/fields_checker.py
+-rw-rw-rw-   0        0        0     9063 2023-06-24 10:35:56.000000 aioabcpapi-2.0.5/aioabcpapi/utils/payload.py
+drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.419534 aioabcpapi-2.0.5/aioabcpapi.egg-info/
+-rw-rw-rw-   0        0        0     5371 2023-07-15 20:06:51.000000 aioabcpapi-2.0.5/aioabcpapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      894 2023-07-15 20:06:51.000000 aioabcpapi-2.0.5/aioabcpapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 20:06:51.000000 aioabcpapi-2.0.5/aioabcpapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-07-15 20:06:51.000000 aioabcpapi-2.0.5/aioabcpapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-07-15 20:06:51.000000 aioabcpapi-2.0.5/aioabcpapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      206 2023-07-15 20:06:51.487549 aioabcpapi-2.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1329 2023-07-15 20:06:01.000000 aioabcpapi-2.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 20:06:51.482545 aioabcpapi-2.0.5/test/
+-rw-rw-rw-   0        0        0    15807 2022-08-10 22:50:42.000000 aioabcpapi-2.0.5/test/test_payload.py
```

### Comparing `aioabcpapi-2.0.4/LICENSE` & `aioabcpapi-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/PKG-INFO` & `aioabcpapi-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 2.0.4
+Version: 2.0.5
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-2.0.4/README.md` & `aioabcpapi-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/aioabcpapi/__init__.py` & `aioabcpapi-2.0.5/aioabcpapi/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,9 +5,9 @@
                          AbcpParameterRequired, TeaPot)
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 
 __author__ = 'bl4ckm45k'
-__version__ = '2.0.4'
+__version__ = '2.0.5'
 __email__ = 'nonpowa@gmail.com'
```

### Comparing `aioabcpapi-2.0.4/aioabcpapi/abcp.py` & `aioabcpapi-2.0.5/aioabcpapi/abcp.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/aioabcpapi/api.py` & `aioabcpapi-2.0.5/aioabcpapi/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,15 @@
             GET_PAYMENTS_ONLINE: str = 'cp/onlinePayments'
             ADD_PAYMENTS: str = 'cp/finance/payments'
             DELETE_PAYMENT_LINK: str = 'cp/finance/deleteLinkPayments'
             LINK_EXISTING_PLAYMENT: str = 'cp/finance/paymentOrderLink'
             REFUND_PAYMENT: str = 'cp/finance/paymentRefund'
             GET_RECEIPTS: str = 'komtet/getChecks'
             GET_PAYMENTS_SETTINGS: str = 'cp/payments/getPaymentMethodSettings'
+            DELETE_PAYMENT: str = 'cp/finance/deletePayments'
 
         @dataclass(frozen=True)
         class Users:
             GET_USERS_LIST: str = 'cp/users'
             CREATE_USER: str = 'cp/user/new'
             GET_PROFILES: str = 'cp/users/profiles'
             EDIT_PROFILE: str = 'cp/users/profile'
```

### Comparing `aioabcpapi-2.0.4/aioabcpapi/base.py` & `aioabcpapi-2.0.5/aioabcpapi/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/aioabcpapi/cp/admin.py` & `aioabcpapi-2.0.5/aioabcpapi/cp/admin.py`

 * *Files 0% similar despite different names*

```diff
@@ -707,14 +707,20 @@
         :type refund_amount: int or str or float
         """
         if not all(x.isdigit() for x in [refund_payment_id, refund_amount] if isinstance(x, str)):
             raise AbcpAPIError('Все параметры должны являться цифрами')
         payload = generate_payload(**locals())
         return await self._base.request(_Methods.Admin.Finance.REFUND_PAYMENT, payload, True)
 
+    async def delete_payment(self, payment_id: int, delete_link: Union[int, bool] = 0):
+        if isinstance(delete_link, bool):
+            delete_link = int(delete_link)
+        payload = generate_payload(**locals())
+        return await self._base.request(_Methods.Admin.Finance.DELETE_PAYMENT, payload, True)
+
     async def get_receipts(
             self,
             shop_id: Union[int, str] = None,
             queue_id: Union[int, str] = None,
             date_created_start: Union[str, datetime] = None,
             date_created_end: Union[str, datetime] = None,
             calculation_method: Union[str, int] = None,
```

### Comparing `aioabcpapi-2.0.4/aioabcpapi/cp/client.py` & `aioabcpapi-2.0.5/aioabcpapi/cp/client.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/aioabcpapi/exceptions.py` & `aioabcpapi-2.0.5/aioabcpapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/aioabcpapi/ts/admin.py` & `aioabcpapi-2.0.5/aioabcpapi/ts/admin.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/aioabcpapi/ts/base.py` & `aioabcpapi-2.0.5/aioabcpapi/ts/base.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/aioabcpapi/ts/client.py` & `aioabcpapi-2.0.5/aioabcpapi/ts/client.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/aioabcpapi/utils/fields_checker.py` & `aioabcpapi-2.0.5/aioabcpapi/utils/fields_checker.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/aioabcpapi/utils/payload.py` & `aioabcpapi-2.0.5/aioabcpapi/utils/payload.py`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/aioabcpapi.egg-info/PKG-INFO` & `aioabcpapi-2.0.5/aioabcpapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioabcpapi
-Version: 2.0.4
+Version: 2.0.5
 Summary: Async library for ABCP API
 Home-page: https://github.com/bl4ckm45k/aioabcpapi
 Author: bl4ckm45k
 Author-email: nonpowa@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `aioabcpapi-2.0.4/aioabcpapi.egg-info/SOURCES.txt` & `aioabcpapi-2.0.5/aioabcpapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioabcpapi-2.0.4/setup.py` & `aioabcpapi-2.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 if sys.version_info < (3, 7):
     raise RuntimeError('Your Python version {0} is not supported, please install '
                        'Python 3.7+'.format('.'.join(map(str, sys.version_info[:3]))))
 requirements = ["aiohttp>=3.8.3", "certifi>=2022.12.7", "ujson>=5.7.0", "pytz>=2022.7.1", "pyrfc3339"]
 setup(
     name='aioabcpapi',
-    version='2.0.4',
+    version='2.0.5',
     author='bl4ckm45k',
     author_email='nonpowa@gmail.com',
     description='Async library for ABCP API',
     long_description_content_type="text/markdown",
     url="https://github.com/bl4ckm45k/aioabcpapi",
     license="MIT",
     packages=['aioabcpapi', 'aioabcpapi/cp', 'aioabcpapi/ts', 'aioabcpapi/utils'],
```

### Comparing `aioabcpapi-2.0.4/test/test_payload.py` & `aioabcpapi-2.0.5/test/test_payload.py`

 * *Files identical despite different names*

