# Comparing `tmp/karrio.dpd-2023.4.4-py3-none-any.whl.zip` & `tmp/karrio.dpd-2023.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 13309 bytes, number of entries: 15
+Zip file size: 13333 bytes, number of entries: 15
 -rw-rw-r--  2.0 unx      462 b- defN 23-Apr-23 04:04 karrio/mappers/dpd/__init__.py
 -rw-rw-r--  2.0 unx     1576 b- defN 23-Apr-23 04:04 karrio/mappers/dpd/mapper.py
 -rw-rw-r--  2.0 unx     1855 b- defN 23-Apr-23 04:04 karrio/mappers/dpd/proxy.py
--rw-rw-r--  2.0 unx     1270 b- defN 23-Apr-23 04:04 karrio/mappers/dpd/settings.py
+-rw-rw-r--  2.0 unx     1304 b- defN 23-Jul-15 16:10 karrio/mappers/dpd/settings.py
 -rw-rw-r--  2.0 unx      242 b- defN 23-Mar-27 07:55 karrio/providers/dpd/__init__.py
 -rw-rw-r--  2.0 unx     1037 b- defN 23-Mar-27 07:55 karrio/providers/dpd/error.py
 -rw-rw-r--  2.0 unx     4241 b- defN 23-Apr-23 04:04 karrio/providers/dpd/tracking.py
 -rw-rw-r--  2.0 unx     7720 b- defN 23-Mar-27 07:55 karrio/providers/dpd/units.py
--rw-rw-r--  2.0 unx     3990 b- defN 23-Mar-27 07:55 karrio/providers/dpd/utils.py
+-rw-rw-r--  2.0 unx     4059 b- defN 23-Jul-15 17:00 karrio/providers/dpd/utils.py
 -rw-rw-r--  2.0 unx      104 b- defN 23-Mar-27 07:55 karrio/providers/dpd/shipment/__init__.py
--rw-rw-r--  2.0 unx    21830 b- defN 23-May-17 00:17 karrio/providers/dpd/shipment/create.py
--rw-rw-r--  2.0 unx      952 b- defN 23-May-20 11:14 karrio.dpd-2023.4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.dpd-2023.4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.dpd-2023.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1291 b- defN 23-May-20 11:14 karrio.dpd-2023.4.4.dist-info/RECORD
-15 files, 46669 bytes uncompressed, 11151 bytes compressed:  76.1%
+-rw-rw-r--  2.0 unx    21830 b- defN 23-May-21 02:20 karrio/providers/dpd/shipment/create.py
+-rw-rw-r--  2.0 unx      952 b- defN 23-Jul-15 19:12 karrio.dpd-2023.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-15 19:12 karrio.dpd-2023.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-15 19:12 karrio.dpd-2023.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1291 b- defN 23-Jul-15 19:12 karrio.dpd-2023.5.1.dist-info/RECORD
+15 files, 46772 bytes uncompressed, 11175 bytes compressed:  76.1%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: karrio/providers/dpd/shipment/__init__.py
 Comment: 
 
 Filename: karrio/providers/dpd/shipment/create.py
 Comment: 
 
-Filename: karrio.dpd-2023.4.4.dist-info/METADATA
+Filename: karrio.dpd-2023.5.1.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dpd-2023.4.4.dist-info/WHEEL
+Filename: karrio.dpd-2023.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dpd-2023.4.4.dist-info/top_level.txt
+Filename: karrio.dpd-2023.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dpd-2023.4.4.dist-info/RECORD
+Filename: karrio.dpd-2023.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/mappers/dpd/settings.py

```diff
@@ -22,15 +22,15 @@
 
     # generic properties
     id: str = None
     test_mode: bool = False
     carrier_id: str = "dpd"
     account_country_code: str = "BE"
     services: typing.List[models.ServiceLevel] = jstruct.JList[models.ServiceLevel, False, dict(default=provider_units.DEFAULT_SERVICES)]  # type: ignore
-    cache: lib.Cache = jstruct.JStruct[lib.Cache]
+    cache: lib.Cache = jstruct.JStruct[lib.Cache, False, dict(default=lib.Cache())]
     metadata: dict = {}
     config: dict = {}
 
     @property
     def shipping_services(self) -> typing.List[models.ServiceLevel]:
         if any(self.services or []):
             return self.services
```

## karrio/providers/dpd/utils.py

```diff
@@ -1,13 +1,15 @@
 import dpd_lib.Authentication20 as auth
 import dpd_lib.LoginServiceV21 as dpd
+
 import jstruct
 import datetime
 import karrio.lib as lib
 import karrio.core as core
+import karrio.core.errors as errors
 
 
 class Settings(core.Settings):
     """DPD connection settings."""
 
     delis_id: str
     password: str
@@ -104,18 +106,18 @@
         method="POST",
         headers={
             "Content-Type": "text/xml;charset=UTF-8",
             "SOAPAction": "http://dpd.com/common/service/types/LoginService/2.1/getAuth",
         },
     )
     response = lib.to_element(result)
-    errors = error.parse_error_response(response, settings)
+    messages = error.parse_error_response(response, settings)
 
-    if any(errors):
-        raise Exception(errors)
+    if any(messages):
+        raise errors.ParsedMessagesError(messages=messages)
 
     return _extract_login_details(response)
 
 
 def _extract_login_details(node: lib.Element):
     data: dpd.GetAuthResponseDto = lib.find_element(
         "return",
```

## Comparing `karrio.dpd-2023.4.4.dist-info/METADATA` & `karrio.dpd-2023.5.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dpd
-Version: 2023.4.4
+Version: 2023.5.1
 Summary: Karrio - DPD Shipping Extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.dpd-2023.4.4.dist-info/RECORD` & `karrio.dpd-2023.5.1.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 karrio/mappers/dpd/__init__.py,sha256=VNwkdMYU7ospY0_Bqyh9tgRIAnNLOE3nbL6DrWZzK28,462
 karrio/mappers/dpd/mapper.py,sha256=WDl4ypWHQYUPdu_06VqTVmgAzT8ghf5kDV6CROsS_MY,1576
 karrio/mappers/dpd/proxy.py,sha256=X75kXx1sBUU0BUgQTP0kqmdQTh01eJbgtc6uydgpe1A,1855
-karrio/mappers/dpd/settings.py,sha256=yWSi4yXm-NJ86C7hmTTP0IXemSKNiqbeJLZcprT3LYM,1270
+karrio/mappers/dpd/settings.py,sha256=7TW09lRj8tj7gbN9XNxaN8U8d6_fWjOW0SMt9CWasgE,1304
 karrio/providers/dpd/__init__.py,sha256=q84FCmlbGI4Wo94ixjqQL4Mkeo08V1zj1PF0wizJYvs,242
 karrio/providers/dpd/error.py,sha256=XBuROolEZedFyV9rCukYSZvRQDi9RjChbrmOTS7Tlv0,1037
 karrio/providers/dpd/tracking.py,sha256=ds_bML0xPjrYsJiZH-01ehdJwE1VXqu1Dw4sCvzk90k,4241
 karrio/providers/dpd/units.py,sha256=a1mDI8DyRgOqb2syhh9iNmF7slcrVcq0uuwIhUw-Hkw,7720
-karrio/providers/dpd/utils.py,sha256=ec-58iGrCmirgAIKtyRKIfVEHReqzRmm78Ca1lV41v0,3990
+karrio/providers/dpd/utils.py,sha256=1Mnfe-YBMurlIIdKIxR6pPQ2vXwnpIevVn8jK1XoYuw,4059
 karrio/providers/dpd/shipment/__init__.py,sha256=60BkyUw1p_8mF9wiv-lO30Pt73BZ1GblL8wcZsUViCo,104
 karrio/providers/dpd/shipment/create.py,sha256=YctaCjvs502jR07TlMTk-uY5WCcCMDMtn-rmNaESw0Q,21830
-karrio.dpd-2023.4.4.dist-info/METADATA,sha256=ah14ZjXamSWTilE2flTLVUsJUXKZbRKNFEcYhQ3XVb0,952
-karrio.dpd-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.dpd-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dpd-2023.4.4.dist-info/RECORD,,
+karrio.dpd-2023.5.1.dist-info/METADATA,sha256=ms_jz9NryKu1xQz1tpKSV8096BqDxwYXiqhBarsQ5f4,952
+karrio.dpd-2023.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dpd-2023.5.1.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.dpd-2023.5.1.dist-info/RECORD,,
```

