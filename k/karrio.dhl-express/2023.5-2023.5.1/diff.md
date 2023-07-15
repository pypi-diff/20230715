# Comparing `tmp/karrio.dhl_express-2023.5-py3-none-any.whl.zip` & `tmp/karrio.dhl_express-2023.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 26469 bytes, number of entries: 20
--rw-rw-r--  2.0 unx      623 b- defN 23-Jun-04 14:33 karrio/mappers/dhl_express/__init__.py
+Zip file size: 26568 bytes, number of entries: 20
+-rw-rw-r--  2.0 unx      623 b- defN 23-Jul-15 16:10 karrio/mappers/dhl_express/__init__.py
 -rw-rw-r--  2.0 unx     3374 b- defN 23-Apr-23 04:04 karrio/mappers/dhl_express/mapper.py
 -rw-rw-r--  2.0 unx     1938 b- defN 23-Apr-23 04:04 karrio/mappers/dhl_express/proxy.py
 -rw-rw-r--  2.0 unx      447 b- defN 23-Apr-23 04:04 karrio/mappers/dhl_express/settings.py
 -rw-rw-r--  2.0 unx      690 b- defN 22-Nov-15 19:21 karrio/providers/dhl_express/__init__.py
 -rw-rw-r--  2.0 unx     2855 b- defN 23-May-21 02:20 karrio/providers/dhl_express/address.py
 -rw-rw-r--  2.0 unx      642 b- defN 23-Apr-23 04:04 karrio/providers/dhl_express/error.py
--rw-rw-r--  2.0 unx     9022 b- defN 23-Jun-04 15:02 karrio/providers/dhl_express/rate.py
--rw-rw-r--  2.0 unx    18091 b- defN 23-May-21 02:20 karrio/providers/dhl_express/shipment.py
+-rw-rw-r--  2.0 unx     9229 b- defN 23-Jul-15 17:52 karrio/providers/dhl_express/rate.py
+-rw-rw-r--  2.0 unx    18297 b- defN 23-Jul-15 18:42 karrio/providers/dhl_express/shipment.py
 -rw-rw-r--  2.0 unx     3768 b- defN 23-Apr-23 04:04 karrio/providers/dhl_express/tracking.py
--rw-rw-r--  2.0 unx    26856 b- defN 23-Jun-04 14:19 karrio/providers/dhl_express/units.py
--rw-rw-r--  2.0 unx     1849 b- defN 23-Jun-04 14:11 karrio/providers/dhl_express/utils.py
+-rw-rw-r--  2.0 unx    26856 b- defN 23-Jul-15 16:10 karrio/providers/dhl_express/units.py
+-rw-rw-r--  2.0 unx     1849 b- defN 23-Jul-15 16:10 karrio/providers/dhl_express/utils.py
 -rw-rw-r--  2.0 unx      307 b- defN 22-Nov-15 19:21 karrio/providers/dhl_express/pickup/__init__.py
 -rw-rw-r--  2.0 unx     2369 b- defN 23-Apr-23 04:04 karrio/providers/dhl_express/pickup/cancel.py
 -rw-rw-r--  2.0 unx     4512 b- defN 23-May-21 02:20 karrio/providers/dhl_express/pickup/create.py
 -rw-rw-r--  2.0 unx     4754 b- defN 23-Apr-23 04:04 karrio/providers/dhl_express/pickup/update.py
--rw-rw-r--  2.0 unx     1020 b- defN 23-Jun-04 15:16 karrio.dhl_express-2023.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-04 15:16 karrio.dhl_express-2023.5.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-Jun-04 15:16 karrio.dhl_express-2023.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1889 b- defN 23-Jun-04 15:16 karrio.dhl_express-2023.5.dist-info/RECORD
-20 files, 85105 bytes uncompressed, 23305 bytes compressed:  72.6%
+-rw-rw-r--  2.0 unx     1022 b- defN 23-Jul-15 19:12 karrio.dhl_express-2023.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-15 19:12 karrio.dhl_express-2023.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-15 19:12 karrio.dhl_express-2023.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1897 b- defN 23-Jul-15 19:12 karrio.dhl_express-2023.5.1.dist-info/RECORD
+20 files, 85528 bytes uncompressed, 23388 bytes compressed:  72.7%
```

## zipnote {}

```diff
@@ -42,20 +42,20 @@
 
 Filename: karrio/providers/dhl_express/pickup/create.py
 Comment: 
 
 Filename: karrio/providers/dhl_express/pickup/update.py
 Comment: 
 
-Filename: karrio.dhl_express-2023.5.dist-info/METADATA
+Filename: karrio.dhl_express-2023.5.1.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dhl_express-2023.5.dist-info/WHEEL
+Filename: karrio.dhl_express-2023.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dhl_express-2023.5.dist-info/top_level.txt
+Filename: karrio.dhl_express-2023.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dhl_express-2023.5.dist-info/RECORD
+Filename: karrio.dhl_express-2023.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/dhl_express/rate.py

```diff
@@ -98,15 +98,23 @@
     ):
         raise errors.OriginNotServicedError(payload.shipper.country_code)
 
     if not is_international and payload.shipper.country_code in ["CA"]:
         raise errors.DestinationNotServicedError(payload.shipper.country_code)
 
     is_document = all([parcel.is_document for parcel in payload.parcels])
-    is_dutiable = is_international and not is_document
+    is_dutiable = (
+        is_international and
+        not is_document and
+        (
+            units.EUCountry.map(payload.shipper.country_code).value is None and
+            units.EUCountry.map(payload.recipient.country_code).value is None
+        )
+    )
+
     services = lib.to_services(
         payload.services,
         is_document=is_document,
         is_international=is_international,
         origin_country=payload.shipper.country_code,
         is_envelope=("envelope" in (packages.package_type or "")),
         initializer=provider_units.shipping_services_initializer,
```

## karrio/providers/dhl_express/shipment.py

```diff
@@ -96,15 +96,22 @@
         payload.customs,
         shipper=payload.shipper,
         recipient=payload.recipient,
         weight_unit=weight_unit.value,
     )
     is_document = all(p.parcel.is_document for p in packages)
     is_international = shipper.country_code != recipient.country_code
-    is_dutiable = is_international and not is_document
+    is_dutiable = (
+        is_international and
+        not is_document and
+        (
+            units.EUCountry.map(payload.shipper.country_code).value is None and
+            units.EUCountry.map(payload.recipient.country_code).value is None
+        )
+    )
     options = lib.to_shipping_options(
         payload.options,
         is_dutiable=is_dutiable,
         package_options=packages.options,
         shipper_country=payload.shipper.country_code,
         initializer=provider_units.shipping_options_initializer,
     )
```

## Comparing `karrio.dhl_express-2023.5.dist-info/METADATA` & `karrio.dhl_express-2023.5.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dhl-express
-Version: 2023.5
+Version: 2023.5.1
 Summary: Karrio - DHL Express Shipping Extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.dhl_express-2023.5.dist-info/RECORD` & `karrio.dhl_express-2023.5.1.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 karrio/mappers/dhl_express/__init__.py,sha256=ZOM6vz5SyIgdwRUl-uSEgQwpLeJAuG0rs8O8wd0huxU,623
 karrio/mappers/dhl_express/mapper.py,sha256=M2Px75ARflQDsG94aCl9mDUMsjXmglb0ltvAqD4EtpU,3374
 karrio/mappers/dhl_express/proxy.py,sha256=mD8E1X_UOkD9tWGnNGoR0BKIgArrgnMOZPqzUlCE4RY,1938
 karrio/mappers/dhl_express/settings.py,sha256=2HvIz_cxPTo1hscFGbw_AII834li5NnT8C0JLuf3wrM,447
 karrio/providers/dhl_express/__init__.py,sha256=LalDeH-5sDXL4IEc8QMvm6S3oEOprwQ9g6upfVQCJJw,690
 karrio/providers/dhl_express/address.py,sha256=kW7HpbTbvMgpRknr9cljbXUdC36pWdXeC7BhvybsGRE,2855
 karrio/providers/dhl_express/error.py,sha256=HvmPOfCW2SVard58n1FhLQXZZC24-T9c5JFJloZXmGc,642
-karrio/providers/dhl_express/rate.py,sha256=aSnbZmlAJBZ7vfHFdtleaXnrxHL9w8CQq3G5mxI4dgM,9022
-karrio/providers/dhl_express/shipment.py,sha256=4CKrLunmJJld7JRLBtDU8llK8B_ZeLUygnDUBAObiQQ,18091
+karrio/providers/dhl_express/rate.py,sha256=YgKV5RPb56pBUtoWed52ybkvQ98snQxP1y8BAYf5IiI,9229
+karrio/providers/dhl_express/shipment.py,sha256=MFzWaaK3UN7L8-AwmgsuQFlNEq8gOCfau2mhJ1IUuIk,18297
 karrio/providers/dhl_express/tracking.py,sha256=rLmnY1znPOxdQkIJ3nimZUSozjVidG-dRgNDK812M20,3768
 karrio/providers/dhl_express/units.py,sha256=JfBn1tumemrF6oPEuRAvGFlMf3s1tVxucpXKKtSuAiw,26856
 karrio/providers/dhl_express/utils.py,sha256=L1z1MjvW3SwGsg7hMUOzfGc6FRLCxcUM6MQBic4o-AU,1849
 karrio/providers/dhl_express/pickup/__init__.py,sha256=mKF_9pkJatfdM_CPMI9vwhFI6-R9OFFjXbnNtc_kiu0,307
 karrio/providers/dhl_express/pickup/cancel.py,sha256=5U5609IYDpZKH7DhgDmrSf8oQEBPVQQfFdCGmHIVDWE,2369
 karrio/providers/dhl_express/pickup/create.py,sha256=HtdopvNrnK0PQDA8OdA6FOsfg81nJ2j50AlE0aoOG8Y,4512
 karrio/providers/dhl_express/pickup/update.py,sha256=a7P-dJCwn01alnd_a0I2PUZzbcCCH0ZBHGZsxoRk2oA,4754
-karrio.dhl_express-2023.5.dist-info/METADATA,sha256=-qtj5tprqEso8Z_SJZO08gk4CmfPD_wgIJL2jRhwEhY,1020
-karrio.dhl_express-2023.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.dhl_express-2023.5.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dhl_express-2023.5.dist-info/RECORD,,
+karrio.dhl_express-2023.5.1.dist-info/METADATA,sha256=T06PR79uuh7jUxxNAIxhNgIO7H4Jr3mgpfVAlf0ocMo,1022
+karrio.dhl_express-2023.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dhl_express-2023.5.1.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.dhl_express-2023.5.1.dist-info/RECORD,,
```

