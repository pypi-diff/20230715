# Comparing `tmp/karrio.usps-2023.4.4-py3-none-any.whl.zip` & `tmp/karrio.usps-2023.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,23 +1,23 @@
-Zip file size: 18073 bytes, number of entries: 21
+Zip file size: 18195 bytes, number of entries: 21
 -rw-rw-r--  2.0 unx      450 b- defN 22-Nov-15 19:21 karrio/mappers/usps/__init__.py
 -rw-rw-r--  2.0 unx     3442 b- defN 23-Apr-23 04:04 karrio/mappers/usps/mapper.py
 -rw-rw-r--  2.0 unx     1969 b- defN 23-Apr-23 04:04 karrio/mappers/usps/proxy.py
 -rw-rw-r--  2.0 unx      572 b- defN 23-Apr-23 04:04 karrio/mappers/usps/settings.py
 -rw-rw-r--  2.0 unx      613 b- defN 22-Nov-15 19:21 karrio/providers/usps/__init__.py
 -rw-rw-r--  2.0 unx      722 b- defN 22-Nov-15 19:21 karrio/providers/usps/error.py
 -rw-rw-r--  2.0 unx     6216 b- defN 23-Apr-23 04:04 karrio/providers/usps/rate.py
 -rw-rw-r--  2.0 unx     3419 b- defN 23-Apr-23 04:04 karrio/providers/usps/tracking.py
--rw-rw-r--  2.0 unx    16295 b- defN 23-Mar-27 07:55 karrio/providers/usps/units.py
+-rw-rw-r--  2.0 unx    17086 b- defN 23-Jul-15 16:10 karrio/providers/usps/units.py
 -rw-rw-r--  2.0 unx      734 b- defN 23-Apr-23 04:04 karrio/providers/usps/utils.py
 -rw-rw-r--  2.0 unx      286 b- defN 22-Nov-15 19:21 karrio/providers/usps/pickup/__init__.py
 -rw-rw-r--  2.0 unx     1568 b- defN 23-Apr-23 04:04 karrio/providers/usps/pickup/cancel.py
 -rw-rw-r--  2.0 unx     1926 b- defN 23-Apr-23 04:04 karrio/providers/usps/pickup/create.py
 -rw-rw-r--  2.0 unx     2008 b- defN 23-Apr-23 04:04 karrio/providers/usps/pickup/update.py
 -rw-rw-r--  2.0 unx      198 b- defN 22-Nov-15 19:21 karrio/providers/usps/shipment/__init__.py
 -rw-rw-r--  2.0 unx     1614 b- defN 23-Apr-23 04:04 karrio/providers/usps/shipment/cancel.py
--rw-rw-r--  2.0 unx     7619 b- defN 23-May-17 00:17 karrio/providers/usps/shipment/create.py
--rw-rw-r--  2.0 unx      966 b- defN 23-May-20 11:14 karrio.usps-2023.4.4.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-20 11:14 karrio.usps-2023.4.4.dist-info/WHEEL
--rw-rw-r--  2.0 unx        7 b- defN 23-May-20 11:14 karrio.usps-2023.4.4.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1867 b- defN 23-May-20 11:14 karrio.usps-2023.4.4.dist-info/RECORD
-21 files, 52583 bytes uncompressed, 14983 bytes compressed:  71.5%
+-rw-rw-r--  2.0 unx     7619 b- defN 23-May-21 02:20 karrio/providers/usps/shipment/create.py
+-rw-rw-r--  2.0 unx      966 b- defN 23-Jul-15 19:12 karrio.usps-2023.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jul-15 19:12 karrio.usps-2023.5.1.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        7 b- defN 23-Jul-15 19:12 karrio.usps-2023.5.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1867 b- defN 23-Jul-15 19:12 karrio.usps-2023.5.1.dist-info/RECORD
+21 files, 53374 bytes uncompressed, 15105 bytes compressed:  71.7%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: karrio/providers/usps/shipment/cancel.py
 Comment: 
 
 Filename: karrio/providers/usps/shipment/create.py
 Comment: 
 
-Filename: karrio.usps-2023.4.4.dist-info/METADATA
+Filename: karrio.usps-2023.5.1.dist-info/METADATA
 Comment: 
 
-Filename: karrio.usps-2023.4.4.dist-info/WHEEL
+Filename: karrio.usps-2023.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: karrio.usps-2023.4.4.dist-info/top_level.txt
+Filename: karrio.usps-2023.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: karrio.usps-2023.4.4.dist-info/RECORD
+Filename: karrio.usps-2023.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## karrio/providers/usps/units.py

```diff
@@ -212,14 +212,19 @@
     usps_retail_ground = "Retail Ground"
     usps_media = "Media"
     usps_library = "Library"
     usps_all = "All"
     usps_online = "Online"
     usps_plus = "Plus"
     usps_bpm = "BPM"
+    usps_ground_advantage = "Ground Advantage"
+    usps_ground_advantage_commercial = "Ground Advantage Commercial"
+    usps_ground_advantage_hfp = "Ground Advantage HFP"
+    usps_ground_advantage_hfp_commercial = "Ground Advantage HFP Commercial"
+    usps_ground_advantage_cubic = "Ground Advantage Cubic"
 
 
 class ServiceClassID(Enum):
     usps_first_class = "0"
     usps_first_class_mail_large_envelope = usps_first_class
     usps_first_class_mail_lt_letter = usps_first_class
     usps_first_class_mail_lt_parcel = usps_first_class
@@ -275,25 +280,35 @@
     usps_priority_mail_express_sunday_holiday_delivery_padded_flat_rate_envelope = "64"
     usps_parcel_select_ground = "77"
     usps_priority_mail_cubic = "84"
     usps_parcel_select_ground_cubic = "92"
     usps_bpm_flats_hold_for_pickup = "2020"
     usps_parcel_select_ground_hold_for_pickup = "2071"
     usps_bpm_parcels_hold_for_pickup = "2077"
+    usps_ground_advantage_cubic = "1096"
+    usps_ground_advantage_cubic_hold_for_pickup = "2096"
+    usps_ground_advantage_cubic_hazmat = "4096"
+    usps_ground_advantage_cubic_parcel_locker = "6096"
+    usps_ground_advantage = "1058"
+    usps_ground_advantage_hold_for_pickup = "2058"
+    usps_ground_advantage_hazmat = "4058"
+    usps_ground_advantage_parcel_locker = "6058"
 
 
 class ServiceType(Enum):
     usps_bpm = "BPM"
     usps_media = "MEDIA"
     usps_library = "LIBRARY"
     usps_priority = "PRIORITY"
     usps_first_class = "FIRST CLASS"
     usps_priority_mail_express = "PRIORITY EXPRESS"
     usps_priority_mail_cubic = "PRIORITY MAIL CUBIC"
     usps_parcel_select_ground = "PARCEL SELECT GROUND"
+    usps_ground_advantage = "GROUND ADVANTAGE"
+    usps_ground_advantage_cubic = "GROUND ADVANTAGE CUBIC"
 
     """ ShipmentService type correspondence """
     usps_first_class_mail_large_envelope = usps_first_class
     usps_first_class_mail_lt_letter = usps_first_class
     usps_first_class_mail_lt_parcel = usps_first_class
     usps_first_class_mail_postcards = usps_first_class
     usps_first_class_mail_large_postcards = usps_first_class
```

## Comparing `karrio.usps-2023.4.4.dist-info/METADATA` & `karrio.usps-2023.5.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: karrio.usps
-Version: 2023.4.4
+Version: 2023.5.1
 Summary: Karrio - USPS Shipping extension
 Home-page: https://github.com/karrioapi/karrio
 Author: karrio
 Author-email: hello@karrio.io
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
```

## Comparing `karrio.usps-2023.4.4.dist-info/RECORD` & `karrio.usps-2023.5.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 karrio/mappers/usps/mapper.py,sha256=IrpBySFltW77hA7A7G5k6FTaBjyfrHVH4tUiW2ksYg4,3442
 karrio/mappers/usps/proxy.py,sha256=OGlmf9TkRJ-7KZP3Liw7txDY2GHiam6_iFYJxA3hfp4,1969
 karrio/mappers/usps/settings.py,sha256=IXvSexRZBw6sxGWVplgOkbf5I0sQeQAgj8jRi918S4U,572
 karrio/providers/usps/__init__.py,sha256=llieveNGqPEAGRVVMUMKC40YCsgxwsb8_BGjgfEetFU,613
 karrio/providers/usps/error.py,sha256=awhVC-kiqCKWjHFEOeMq9JOuSzwuMqoAlZH3BcPqUYk,722
 karrio/providers/usps/rate.py,sha256=wgr-ADcMh3t7hPwlXRaWR-uicn7P1V6d6axHMb6erxY,6216
 karrio/providers/usps/tracking.py,sha256=78k_j-sC51GDhD3jH3YKftrbmG_9HwWGxSjTHhEZvl8,3419
-karrio/providers/usps/units.py,sha256=KfbiaTZ_F4CFGYYdJdENUw2X8ZWkPB8odKIecX8nBHI,16295
+karrio/providers/usps/units.py,sha256=GsCU_HJbXSfrl2U7RFU45k33a4jHU6lPsVcX4fGgH6E,17086
 karrio/providers/usps/utils.py,sha256=EB5z8FZrk24So3s267pv2TeCtOeKB8zAqzOG4Ba9Ypc,734
 karrio/providers/usps/pickup/__init__.py,sha256=YTFtc6O-bbi1NhsYbug5vag4GmbmvXms88lGbSWeZ0E,286
 karrio/providers/usps/pickup/cancel.py,sha256=BBewXX3WNjO_aQIoY6h2O4H14cHApe3fsGzeOhBFkZg,1568
 karrio/providers/usps/pickup/create.py,sha256=MtoEZXmbJpPe3q5nZB8XkeFHwWYJa5ykpvMD7EaP67s,1926
 karrio/providers/usps/pickup/update.py,sha256=4xDQRQ36aWlgpu_TEIJp1D_6Zmi6Hznk6__APuD5bAw,2008
 karrio/providers/usps/shipment/__init__.py,sha256=ZGECAADplncp0tiq9F_mawDECcgZS_kOCVMIzVfTnKE,198
 karrio/providers/usps/shipment/cancel.py,sha256=Noo8-0R1sJIzLaGN1Dx6eF0qT_PDIbkQvisbgV7zbh0,1614
 karrio/providers/usps/shipment/create.py,sha256=R6FPF3UJv5pR2hAbupegBGhDJxaiUN4kCD2Lz-FnpVM,7619
-karrio.usps-2023.4.4.dist-info/METADATA,sha256=3AmCoo5601EPWHRe8RLtrTc5cRmm1HaoMM45fK0RqOE,966
-karrio.usps-2023.4.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-karrio.usps-2023.4.4.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
-karrio.usps-2023.4.4.dist-info/RECORD,,
+karrio.usps-2023.5.1.dist-info/METADATA,sha256=PUpNzuFZZPb6AWTzTT9DzGlKeDP9syGYpNsV-8jPo8Y,966
+karrio.usps-2023.5.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+karrio.usps-2023.5.1.dist-info/top_level.txt,sha256=mfkVZXzNuVRmA7NRlck_Ub-C8Zgtqxbx3gX1Rq_W-i0,7
+karrio.usps-2023.5.1.dist-info/RECORD,,
```

