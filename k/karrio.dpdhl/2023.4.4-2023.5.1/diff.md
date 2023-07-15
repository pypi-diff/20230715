# Comparing `tmp/karrio.dpdhl-2023.4.4-py3-none-any.whl.zip` & `tmp/karrio.dpdhl-2023.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 14772 bytes, number of entries: 16
+Zip file size: 14804 bytes, number of entries: 16
 -rw-rw-r--  2.0 unx      558 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/__init__.py
 -rw-rw-r--  2.0 unx     2030 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/mapper.py
 -rw-rw-r--  2.0 unx     2431 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/proxy.py
 -rw-rw-r--  2.0 unx     1021 b- defN 23-Apr-23 04:04 karrio/mappers/dpdhl/settings.py
 -rw-rw-r--  2.0 unx      313 b- defN 22-Nov-15 19:21 karrio/providers/dpdhl/__init__.py
--rw-rw-r--  2.0 unx     4884 b- defN 23-Apr-24 04:01 karrio/providers/dpdhl/error.py
+-rw-rw-r--  2.0 unx     5038 b- defN 23-Jul-15 18:33 karrio/providers/dpdhl/error.py
 -rw-rw-r--  2.0 unx     3657 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/tracking.py
--rw-rw-r--  2.0 unx     8251 b- defN 23-May-20 10:45 karrio/providers/dpdhl/units.py
--rw-rw-r--  2.0 unx     1903 b- defN 23-May-17 00:17 karrio/providers/dpdhl/utils.py
+-rw-rw-r--  2.0 unx     8251 b- defN 23-May-21 02:20 karrio/providers/dpdhl/units.py
+-rw-rw-r--  2.0 unx     1903 b- defN 23-May-21 02:20 karrio/providers/dpdhl/utils.py
 -rw-rw-r--  2.0 unx      226 b- defN 22-Nov-15 19:21 karrio/providers/dpdhl/shipment/__init__.py
 -rw-rw-r--  2.0 unx     2425 b- defN 23-Apr-23 04:04 karrio/providers/dpdhl/shipment/cancel.py
--rw-rw-r--  2.0 unx    19628 b- defN 23-May-17 00:17 karrio/providers/dpdhl/shipment/create.py
--rw-rw-r--  2.0 unx      994 b- defN 23-May-20 11:14 karrio.dpdhl-2023.4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.dpdhl-2023.4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.dpdhl-2023.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1419 b- defN 23-May-20 11:14 karrio.dpdhl-2023.4.4.dist-info/RECORD
-16 files, 49839 bytes uncompressed, 12396 bytes compressed:  75.1%
+-rw-rw-r--  2.0 unx    19628 b- defN 23-May-21 02:20 karrio/providers/dpdhl/shipment/create.py
+-rw-rw-r--  2.0 unx      994 b- defN 23-Jul-15 19:12 karrio.dpdhl-2023.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-15 19:12 karrio.dpdhl-2023.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-15 19:12 karrio.dpdhl-2023.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1419 b- defN 23-Jul-15 19:12 karrio.dpdhl-2023.5.1.dist-info/RECORD
+16 files, 49993 bytes uncompressed, 12428 bytes compressed:  75.1%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: karrio/providers/dpdhl/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/dpdhl/shipment/create.py
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.4.dist-info/METADATA
+Filename: karrio.dpdhl-2023.5.1.dist-info/METADATA
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.4.dist-info/WHEEL
+Filename: karrio.dpdhl-2023.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.4.dist-info/top_level.txt
+Filename: karrio.dpdhl-2023.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.dpdhl-2023.4.4.dist-info/RECORD
+Filename: karrio.dpdhl-2023.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/dpdhl/error.py

```diff
@@ -1,8 +1,7 @@
-from urllib.error import HTTPError
 import dpdhl_lib.business_interface as dpdhl
 import typing
 import karrio.lib as lib
 import karrio.core.models as models
 import karrio.providers.dpdhl.utils as provider_utils
 
 
@@ -51,44 +50,47 @@
     ]
 
     return [
         models.Message(
             carrier_id=settings.carrier_id,
             carrier_name=settings.carrier_name,
             code=error.statusCode,
-            message=error.statusText,
-            details={
-                **(
-                    lib.failsafe(
-                        lambda: lib.to_dict(
-                            {
-                                "message": lib.join(
-                                    *[
-                                        _
-                                        for _ in error.statusMessage
-                                        if isinstance(_, str)
-                                    ],
-                                    join=" ",
-                                )
-                            }
-                        )
+            message=(
+                lib.failsafe(
+                    lambda: lib.join(
+                        *set([_ for _ in error.statusMessage if isinstance(_, str)]),
+                        join=" ",
                     )
-                    or {}
-                    if any(error.statusMessage or [])
-                    else {}
-                ),
+                )
+                or lib.failsafe(
+                    lambda: lib.join(
+                        *set(
+                            [
+                                f"{_.statusElement}: {_.statusMessage}"
+                                for _ in error.errorMessage
+                            ]
+                        ),
+                        join=" ",
+                    )
+                )
+                or error.statusText
+            ),
+            details={
+                "statusText": error.statusText,
                 **(
                     lib.failsafe(
                         lambda: lib.to_dict(
                             {
                                 "error": lib.join(
-                                    *[
-                                        f"{_.statusElement}: {_.statusMessage}"
-                                        for _ in error.errorMessage
-                                    ],
+                                    *set(
+                                        [
+                                            f"{_.statusElement}: {_.statusMessage}"
+                                            for _ in error.errorMessage
+                                        ]
+                                    ),
                                     join=" ",
                                 )
                             }
                         )
                     )
                     or {}
                     if any(error.errorMessage or [])
@@ -96,19 +98,21 @@
                 ),
                 **(
                     lib.failsafe(
                         lambda: lib.to_dict(
                             {
                                 "warning": lib.join(
                                     *(
-                                        [
-                                            _
-                                            for _ in error.warningMessage
-                                            if isinstance(_, str)
-                                        ]
+                                        set(
+                                            [
+                                                _
+                                                for _ in error.warningMessage
+                                                if isinstance(_, str)
+                                            ]
+                                        )
                                         if isinstance(error.warningMessage, list)
                                         else (
                                             [error.warningMessage]
                                             if isinstance(error.warningMessage, str)
                                             else []
                                         )
                                     ),
```

## Comparing `karrio.dpdhl-2023.4.4.dist-info/METADATA` & `karrio.dpdhl-2023.5.1.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.dpdhl
-Version: 2023.4.4
+Version: 2023.5.1
 Summary: Karrio - Deutsche Post DHL Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.dpdhl-2023.4.4.dist-info/RECORD` & `karrio.dpdhl-2023.5.1.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 karrio/mappers/dpdhl/__init__.py,sha256=hI9K0SVajo90niTvmU5BP9iV2QoOFh8tEbtZfVRax_c,558
 karrio/mappers/dpdhl/mapper.py,sha256=PX1mAMSFl8JmtAQ-SaKr8xDrV0eybOXzNLJbrUGKLfM,2030
 karrio/mappers/dpdhl/proxy.py,sha256=29jmjAngUb4FkLHu3bTB4leP7VxDROBb78-s8aAj4nk,2431
 karrio/mappers/dpdhl/settings.py,sha256=nRq7QoFa8Amrg1glJy_UmZ9fQUxuseC8KNKPltbifm0,1021
 karrio/providers/dpdhl/__init__.py,sha256=XtaZQrNssm_oho6v6SAYEH3cViuOZ3VFAPhHgW6f-yw,313
-karrio/providers/dpdhl/error.py,sha256=IKFlWE1FbfeNf6TjeB3L_lraLX716XpoDKCe87kgcDc,4884
+karrio/providers/dpdhl/error.py,sha256=5nRY2iG92AFviRvwMFq4k_vda1d97ehda65_CWl2D4M,5038
 karrio/providers/dpdhl/tracking.py,sha256=Qn2luGRnyIlJkaa2JSRjlawLVq-jMnAkfFGRcJFugqc,3657
 karrio/providers/dpdhl/units.py,sha256=6o2FddsCw2K49EwskglkMVWAjGODsgaaXFrlnnqdmc4,8251
 karrio/providers/dpdhl/utils.py,sha256=dDS7xkLYtrAeh89S5BnP3He3NmQXi8iSpCJ-BzuUjPI,1903
 karrio/providers/dpdhl/shipment/__init__.py,sha256=5tF7dih8kTSVa5pw4UXU8_byCMnuvtsJIz_h7VAOOyY,226
 karrio/providers/dpdhl/shipment/cancel.py,sha256=1Z_h5EUUNLS7LAiLLU04dkEPufmXSJGavvn543FGxQE,2425
 karrio/providers/dpdhl/shipment/create.py,sha256=KinIFL3yosgs4v7nXHMy5XNDzjAI1XYrtvCu3GqnfYQ,19628
-karrio.dpdhl-2023.4.4.dist-info/METADATA,sha256=2F5rrzY3oaqKNnKn2vwFRh4BK3JNeAhV4-m2jkdsdUA,994
-karrio.dpdhl-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.dpdhl-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.dpdhl-2023.4.4.dist-info/RECORD,,
+karrio.dpdhl-2023.5.1.dist-info/METADATA,sha256=Xs4a9DiYBcTI7WxCOGQveENPHF4nzCgeVKfBTdPUFOU,994
+karrio.dpdhl-2023.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.dpdhl-2023.5.1.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.dpdhl-2023.5.1.dist-info/RECORD,,
```

