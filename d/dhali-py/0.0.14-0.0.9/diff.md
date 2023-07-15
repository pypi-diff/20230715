# Comparing `tmp/dhali-py-0.0.14.tar.gz` & `tmp/dhali-py-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dhali-py-0.0.14.tar", last modified: Sat Jul 15 15:34:10 2023, max compression
+gzip compressed data, was "dhali-py-0.0.9.tar", last modified: Thu May 11 19:21:46 2023, max compression
```

## Comparing `dhali-py-0.0.14.tar` & `dhali-py-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:34:10.253399 dhali-py-0.0.14/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:34:10.249398 dhali-py-0.0.14/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-07-15 15:33:58.000000 dhali-py-0.0.14/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:34:10.249398 dhali-py-0.0.14/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-07-15 15:33:58.000000 dhali-py-0.0.14/.github/workflows/package_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-07-15 15:33:58.000000 dhali-py-0.0.14/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-15 15:33:58.000000 dhali-py-0.0.14/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-15 15:33:58.000000 dhali-py-0.0.14/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-07-15 15:33:58.000000 dhali-py-0.0.14/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-15 15:33:58.000000 dhali-py-0.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-15 15:34:10.253399 dhali-py-0.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-15 15:33:58.000000 dhali-py-0.0.14/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:34:10.253399 dhali-py-0.0.14/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-15 15:33:58.000000 dhali-py-0.0.14/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:34:10.253399 dhali-py-0.0.14/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-15 15:33:58.000000 dhali-py-0.0.14/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-15 15:33:58.000000 dhali-py-0.0.14/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-15 15:33:58.000000 dhali-py-0.0.14/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-07-15 15:33:58.000000 dhali-py-0.0.14/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-15 15:33:58.000000 dhali-py-0.0.14/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-07-15 15:33:58.000000 dhali-py-0.0.14/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-15 15:33:58.000000 dhali-py-0.0.14/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-15 15:33:58.000000 dhali-py-0.0.14/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-15 15:33:58.000000 dhali-py-0.0.14/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-15 15:33:58.000000 dhali-py-0.0.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-07-15 15:34:10.253399 dhali-py-0.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-07-15 15:33:58.000000 dhali-py-0.0.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:34:10.249398 dhali-py-0.0.14/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:34:10.253399 dhali-py-0.0.14/src/dhali/
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-07-15 15:33:58.000000 dhali-py-0.0.14/src/dhali/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-07-15 15:33:58.000000 dhali-py-0.0.14/src/dhali/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6173 2023-07-15 15:33:58.000000 dhali-py-0.0.14/src/dhali/payment_claim_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-07-15 15:33:58.000000 dhali-py-0.0.14/src/dhali/transaction_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:34:10.253399 dhali-py-0.0.14/src/dhali_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-15 15:34:10.000000 dhali-py-0.0.14/src/dhali_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-07-15 15:34:10.000000 dhali-py-0.0.14/src/dhali_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:34:10.000000 dhali-py-0.0.14/src/dhali_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-15 15:34:10.000000 dhali-py-0.0.14/src/dhali_py.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 15:34:09.000000 dhali-py-0.0.14/src/dhali_py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-15 15:34:10.000000 dhali-py-0.0.14/src/dhali_py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-15 15:34:10.000000 dhali-py-0.0.14/src/dhali_py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 15:34:10.253399 dhali-py-0.0.14/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-15 15:33:58.000000 dhali-py-0.0.14/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-15 15:33:58.000000 dhali-py-0.0.14/tests/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-07-15 15:33:58.000000 dhali-py-0.0.14/tests/test_transaction_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-07-15 15:33:58.000000 dhali-py-0.0.14/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.852405 dhali-py-0.0.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-11 19:21:37.000000 dhali-py-0.0.9/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.852405 dhali-py-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-05-11 19:21:37.000000 dhali-py-0.0.9/.github/workflows/package_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 19:21:37.000000 dhali-py-0.0.9/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-11 19:21:37.000000 dhali-py-0.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-11 19:21:37.000000 dhali-py-0.0.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-05-11 19:21:37.000000 dhali-py-0.0.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-05-11 19:21:37.000000 dhali-py-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-11 19:21:46.856405 dhali-py-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-11 19:21:37.000000 dhali-py-0.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9716 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-11 19:21:37.000000 dhali-py-0.0.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-11 19:21:37.000000 dhali-py-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-11 19:21:46.856405 dhali-py-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-11 19:21:37.000000 dhali-py-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.852405 dhali-py-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/src/dhali/
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-11 19:21:37.000000 dhali-py-0.0.9/src/dhali/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5854 2023-05-11 19:21:37.000000 dhali-py-0.0.9/src/dhali/payment_claim_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10130 2023-05-11 19:21:37.000000 dhali-py-0.0.9/src/dhali/transaction_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/src/dhali_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1664 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-11 19:21:46.000000 dhali-py-0.0.9/src/dhali_py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 19:21:46.856405 dhali-py-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-11 19:21:37.000000 dhali-py-0.0.9/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-11 19:21:37.000000 dhali-py-0.0.9/tests/test_transaction_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2690 2023-05-11 19:21:37.000000 dhali-py-0.0.9/tox.ini
```

### Comparing `dhali-py-0.0.14/.github/workflows/package_test.yaml` & `dhali-py-0.0.9/.github/workflows/package_test.yaml`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.14/.github/workflows/release.yaml` & `dhali-py-0.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.14/CONTRIBUTING.rst` & `dhali-py-0.0.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.14/LICENSE` & `dhali-py-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.14/PKG-INFO` & `dhali-py-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhali-py
-Version: 0.0.14
+Version: 0.0.9
 Summary: A Python package for interfacing with Dhali
 Home-page: https://github.com/Dhali-org/Dhali-py
 Author: Dhali Holdings Ltd
 Author-email: engagement@dhali.io
 License: BSD 3-Clause License
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dhali-py-0.0.14/README.rst` & `dhali-py-0.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.14/docs/Makefile` & `dhali-py-0.0.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.14/docs/conf.py` & `dhali-py-0.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.14/docs/index.rst` & `dhali-py-0.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.14/setup.cfg` & `dhali-py-0.0.9/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -28,17 +28,14 @@
 	google==3.0.0
 	google-api-core==2.11.0
 	google-auth==2.16.2
 	google-cloud==0.34.0
 	google-cloud-vision==3.4.0
 	googleapis-common-protos==1.58.0
 	google-cloud-firestore==2.10.0
-	mockito==1.4.0
-	mock-firestore==0.11.0
-	pytest-asyncio==0.21.0
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
```

### Comparing `dhali-py-0.0.14/setup.py` & `dhali-py-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.14/src/dhali/__init__.py` & `dhali-py-0.0.9/src/dhali/__init__.py`

 * *Files identical despite different names*

### Comparing `dhali-py-0.0.14/src/dhali/payment_claim_generator.py` & `dhali-py-0.0.9/src/dhali/payment_claim_generator.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,17 +24,14 @@
     #           https://xrpl.org/use-payment-channels.html            #
     ###################################################################
     #           Submit a payment channel create transaction           #
     ###################################################################
     last_ledger_sequence = xrpl.ledger.get_latest_validated_ledger_sequence(client) + 10
     fee = xrpl.ledger.get_fee(client=client, fee_type="dynamic")
 
-    # TODO: We do not want to be creating a new payment channel each time this function is called.
-    # Let's instead give the payment channel as an argument to the function.  We can also validate that only
-    # one payment channel is open between the source classic address and Dhali somewhere else in this library.
     payment_channel = PaymentChannelCreate(
         account=source_wallet.classic_address,
         amount=total_xrp_in_channel,
         destination=destination_classic_address,
         public_key=source_wallet.public_key,
         settle_delay=settle_delay,
         last_ledger_sequence=last_ledger_sequence,
```

### Comparing `dhali-py-0.0.14/src/dhali/transaction_utils.py` & `dhali-py-0.0.9/src/dhali/transaction_utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,94 +1,71 @@
 import json
 import xrpl
-import uuid
 from fastapi import HTTPException
+import uuid
 from google.cloud import firestore
 
+
 @firestore.transactional
-def _transactional_validation(
+def transactional_validation(
     transaction,
-    public_doc_ref,
-    private_doc_ref,
+    doc_ref,
     ledger_client,
     parsed_claim,
     single_request_cost_estimate: int,
     settle_delay,
 ) -> float:
-    private_payment_channels_doc = next(transaction.get(private_doc_ref))
-    public_payment_channels_doc = next(transaction.get(public_doc_ref))
+    payment_channels_doc = next(transaction.get(doc_ref))
 
     updating_payment_claim = True
-    if private_payment_channels_doc.exists:
+    if payment_channels_doc.exists:
         # Check if payment claim was previously submitted. If so, we do not need
         # to cryptographically verify it again 
-        updating_payment_claim = json.loads(private_payment_channels_doc.to_dict()["payment_claim"]) != parsed_claim
-        if private_payment_channels_doc.to_dict()["currency"]["code"] != "XRP":
+        updating_payment_claim = json.loads(payment_channels_doc.to_dict()["payment_claim"]) != parsed_claim
+        if payment_channels_doc.to_dict()["currency"]["code"] != "XRP":
             raise HTTPException(
                 status_code=402,
                 detail="Your stored payment channel's currency code is invalid",
             )
-        if private_payment_channels_doc.to_dict()["currency"]["scale"] != 0.000001:
+        if payment_channels_doc.to_dict()["currency"]["scale"] != 0.000001:
             raise HTTPException(
                 status_code=402,
                 detail="Your stored payment channel's currency scale is invalid",
             )
 
         to_claim = (
-            private_payment_channels_doc.to_dict()["to_claim"] + single_request_cost_estimate
+            payment_channels_doc.to_dict()["to_claim"] + single_request_cost_estimate
         )
     else:
         to_claim = single_request_cost_estimate
 
     authorized_to_claim = parsed_claim["authorized_to_claim"]
     if int(authorized_to_claim) < int(to_claim):
         raise HTTPException(
             status_code=402,
             detail=f"Your payment claim is not sufficient to fund this request: authorized_to_claim = {authorized_to_claim}, to_claim = {to_claim}",
         )
 
     if updating_payment_claim:
         validate(parsed_claim=parsed_claim, ledger_client=ledger_client, settle_delay=settle_delay)
 
-    if private_payment_channels_doc.exists:
-        transaction.update(
-            private_doc_ref,
-            {
-                "authorized_to_claim": parsed_claim["authorized_to_claim"],
-                "to_claim": to_claim, # TODO: Remove this once other infra migrated to use public firestore
-                "currency": {"code": "XRP", "scale": 0.000001},
-                "payment_claim": json.dumps(parsed_claim),
-            },
-        )
+    if payment_channels_doc.exists:
+        transaction.update(doc_ref, {"to_claim": to_claim})
     else:
         # The expectations are:
         # authorized_to_claim >= to_claim
         transaction.set(
-            private_doc_ref,
+            doc_ref,
             {
                 "authorized_to_claim": parsed_claim["authorized_to_claim"],
-                "to_claim": to_claim, # TODO: Remove this once other infra migrated to use public firestore
-                "currency": {"code": "XRP", "scale": 0.000001},
-                "payment_claim": json.dumps(parsed_claim),
-            },
-        )
-
-    if public_payment_channels_doc.exists:
-        transaction.update(public_doc_ref, {"to_claim": to_claim})
-    else:
-        # The expectations are:
-        # authorized_to_claim >= to_claim
-        transaction.set(
-            public_doc_ref,
-            {
                 "to_claim": to_claim,
                 "currency": {"code": "XRP", "scale": 0.000001},
+                "payment_claim": json.dumps(parsed_claim),
             },
         )
-
     return to_claim
 
 def validate(parsed_claim, ledger_client, settle_delay):
 
     account_channels = xrpl.models.requests.AccountChannels(
         account=parsed_claim["account"],
         destination_account=parsed_claim["destination_account"],
@@ -187,41 +164,14 @@
     consumed_GiB_s = (
         GiB_memory * runtime_ms * request_size_bytes * response_size_bytes / 1000
     )
 
     return consumed_GiB_s * GiB_s_dollars_price
 
 
-@firestore.transactional
-def _transactional_update_estimated_cost_with_exact(transaction, 
-                                                    public_doc_ref,
-                                                    private_doc_ref,
-                                                    single_request_cost_estimate: int, 
-                                                    single_request_exact_cost: int):
-    private_payment_channels_doc = next(transaction.get(private_doc_ref))
-    public_payment_channels_doc = next(transaction.get(public_doc_ref))
-
-    if public_payment_channels_doc.exists and private_payment_channels_doc.exists: # TODO: Remove private_payment_claim_doc
-                                                                             # clause once migrated other code to use
-                                                                             # public firestore
-        to_claim = (
-            public_payment_channels_doc.to_dict()["to_claim"]
-            - single_request_cost_estimate
-            + single_request_exact_cost
-        )
-        
-        transaction.update(public_doc_ref, {"to_claim": to_claim})
-        transaction.update(private_doc_ref, {"to_claim": to_claim}) # TODO: Remove this line once migrated
-                                                                                  # other code to use public firestore
-        return to_claim
-
-    raise HTTPException(status_code=402)
-
-
-# TODO: Make this transactional!
 async def update_estimated_cost_with_exact(
     claim, single_request_cost_estimate: int, single_request_exact_cost: int, db
 ) -> float:
     """
     TODO
 
     Parameters
@@ -239,41 +189,42 @@
     void
     """
     try:
         parsed_claim = json.loads(claim)
     except ValueError as e:
         raise HTTPException(
             status_code=402,
-            detail=f"You must provide a payment channel claim that can be parsed via json.loads. Error: {e}.",
+            detail="You must provide a payment channel claim that can be parsed via json.loads",
         )
 
     if (
         "channel_id" not in parsed_claim.keys()
-        or single_request_exact_cost < 0
-        or single_request_cost_estimate < 0
+        or single_request_exact_cost <= 0
+        or single_request_cost_estimate <= 0
     ):
         raise HTTPException(
             status_code=402,
         )
 
     uuid_channel_id = str(uuid.uuid5(uuid.NAMESPACE_URL, parsed_claim["channel_id"]))
-    public_collection_name = "payment_channels"
-    private_collection_name = "public_claim_info"
+    collection_name = "payment_channels"
 
-    public_payment_claim_doc_ref = db.collection(public_collection_name).document(uuid_channel_id)
-    private_payment_claim_doc_ref = db.collection(private_collection_name).document(uuid_channel_id)
-    
-    transaction = db.transaction()
-    to_claim = _transactional_update_estimated_cost_with_exact(transaction, 
-                                                           public_payment_claim_doc_ref, 
-                                                           private_payment_claim_doc_ref, 
-                                                           single_request_cost_estimate, 
-                                                           single_request_exact_cost)
-    return to_claim
+    payment_claim_doc_ref = db.collection(collection_name).document(uuid_channel_id)
+    payment_claim_doc = payment_claim_doc_ref.get()
 
+    if payment_claim_doc.exists:
+        to_claim = (
+            payment_claim_doc.to_dict()["to_claim"]
+            - single_request_cost_estimate
+            + single_request_exact_cost
+        )
+        payment_claim_doc_ref.update({"to_claim": to_claim})
+        return to_claim
+    else:
+        raise HTTPException(status_code=402)
 
 
 # TODO - Test this!
 async def validate_claim(
     client, claim, single_request_cost_estimate: int, db, destination_account: str, settle_delay=15768000
 ):
     """
@@ -331,25 +282,20 @@
         raise HTTPException(
             status_code=402,
             detail=f"Your claim has an incorrect destination_account",
         )
 
 
     uuid_channel_id = str(uuid.uuid5(uuid.NAMESPACE_URL, parsed_claim["channel_id"]))
-    private_collection_name = "payment_channels"
-    public_collection_name = "public_claim_info"
+    collection_name = "payment_channels"
 
     transaction = db.transaction()
-    public_payment_claim_doc_ref = db.collection(public_collection_name).document(uuid_channel_id)
-    private_payment_claim_doc_ref = db.collection(private_collection_name).document(uuid_channel_id)
-
-    to_claim = _transactional_validation(
+    payment_claim_doc_ref = db.collection(collection_name).document(uuid_channel_id)
+    to_claim = transactional_validation(
         transaction,
-        public_payment_claim_doc_ref,
-        private_payment_claim_doc_ref,
+        payment_claim_doc_ref,
         ledger_client=client,
         parsed_claim=parsed_claim,
         single_request_cost_estimate=single_request_cost_estimate,
         settle_delay=settle_delay,
     )
-
     return to_claim
```

### Comparing `dhali-py-0.0.14/src/dhali_py.egg-info/PKG-INFO` & `dhali-py-0.0.9/src/dhali_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dhali-py
-Version: 0.0.14
+Version: 0.0.9
 Summary: A Python package for interfacing with Dhali
 Home-page: https://github.com/Dhali-org/Dhali-py
 Author: Dhali Holdings Ltd
 Author-email: engagement@dhali.io
 License: BSD 3-Clause License
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `dhali-py-0.0.14/src/dhali_py.egg-info/SOURCES.txt` & `dhali-py-0.0.9/src/dhali_py.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,20 +17,18 @@
 docs/contributing.rst
 docs/index.rst
 docs/license.rst
 docs/readme.rst
 docs/requirements.txt
 docs/_static/.gitignore
 src/dhali/__init__.py
-src/dhali/module.py
 src/dhali/payment_claim_generator.py
 src/dhali/transaction_utils.py
 src/dhali_py.egg-info/PKG-INFO
 src/dhali_py.egg-info/SOURCES.txt
 src/dhali_py.egg-info/dependency_links.txt
 src/dhali_py.egg-info/entry_points.txt
 src/dhali_py.egg-info/not-zip-safe
 src/dhali_py.egg-info/requires.txt
 src/dhali_py.egg-info/top_level.txt
 tests/conftest.py
-tests/test_module.py
 tests/test_transaction_utils.py
```

### Comparing `dhali-py-0.0.14/tox.ini` & `dhali-py-0.0.9/tox.ini`

 * *Files identical despite different names*

