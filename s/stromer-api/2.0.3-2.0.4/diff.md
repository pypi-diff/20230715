# Comparing `tmp/stromer_api-2.0.3.tar.gz` & `tmp/stromer_api-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stromer_api-2.0.3.tar", last modified: Wed Feb 15 21:42:31 2023, max compression
+gzip compressed data, was "stromer_api-2.0.4.tar", last modified: Sat Jul 15 18:44:33 2023, max compression
```

## Comparing `stromer_api-2.0.3.tar` & `stromer_api-2.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-02-15 21:42:31.648982 stromer_api-2.0.3/
--rw-rw-rw-   0        0        0    10931 2023-02-15 21:42:31.648982 stromer_api-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0    10610 2023-02-12 21:56:27.000000 stromer_api-2.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-02-15 21:42:31.648982 stromer_api-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0      491 2023-02-15 21:41:45.000000 stromer_api-2.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:42:31.602106 stromer_api-2.0.3/stromer_api/
--rw-rw-rw-   0        0        0     6489 2023-02-11 21:14:52.000000 stromer_api-2.0.3/stromer_api/__init__.py
--rw-rw-rw-   0        0        0      464 2023-02-01 20:50:35.000000 stromer_api-2.0.3/stromer_api/bikedata.py
--rw-rw-rw-   0        0        0     1078 2023-01-31 23:05:05.000000 stromer_api-2.0.3/stromer_api/bikemaintenance.py
--rw-rw-rw-   0        0        0     1756 2023-02-12 21:47:36.000000 stromer_api-2.0.3/stromer_api/bikemotortuning.py
--rw-rw-rw-   0        0        0      453 2023-02-08 21:00:06.000000 stromer_api-2.0.3/stromer_api/bikepart.py
--rw-rw-rw-   0        0        0     1311 2023-02-12 20:51:16.000000 stromer_api-2.0.3/stromer_api/bikeposition.py
--rw-rw-rw-   0        0        0     1508 2023-02-11 19:26:31.000000 stromer_api-2.0.3/stromer_api/bikesensors.py
--rw-rw-rw-   0        0        0     4047 2023-02-11 21:05:20.000000 stromer_api-2.0.3/stromer_api/bikesettings.py
--rw-rw-rw-   0        0        0     1768 2023-02-15 21:08:26.000000 stromer_api-2.0.3/stromer_api/bikeshop.py
--rw-rw-rw-   0        0        0     3073 2023-02-12 20:51:16.000000 stromer_api-2.0.3/stromer_api/bikestate.py
--rw-rw-rw-   0        0        0     1555 2023-02-01 21:12:36.000000 stromer_api-2.0.3/stromer_api/bikestatistics.py
--rw-rw-rw-   0        0        0     1894 2023-02-01 21:12:36.000000 stromer_api-2.0.3/stromer_api/bikeuser.py
--rw-rw-rw-   0        0        0     3781 2023-02-12 11:09:48.000000 stromer_api-2.0.3/stromer_api/daystats.py
--rw-rw-rw-   0        0        0      593 2023-02-15 20:52:00.000000 stromer_api-2.0.3/stromer_api/general.py
--rw-rw-rw-   0        0        0     5078 2023-02-12 11:09:48.000000 stromer_api-2.0.3/stromer_api/monthstats.py
--rw-rw-rw-   0        0        0      929 2023-01-31 23:03:46.000000 stromer_api-2.0.3/stromer_api/periodicinfo.py
--rw-rw-rw-   0        0        0     1400 2023-02-12 21:47:36.000000 stromer_api-2.0.3/stromer_api/periodstats.py
--rw-rw-rw-   0        0        0     3905 2023-02-15 20:55:13.000000 stromer_api-2.0.3/stromer_api/portal.py
--rw-rw-rw-   0        0        0     1359 2023-02-15 21:41:45.000000 stromer_api-2.0.3/stromer_api/service_info.py
--rw-rw-rw-   0        0        0      369 2023-02-08 21:13:05.000000 stromer_api-2.0.3/stromer_api/service_log.py
--rw-rw-rw-   0        0        0     4843 2023-02-12 11:09:48.000000 stromer_api-2.0.3/stromer_api/weekstats.py
--rw-rw-rw-   0        0        0     4587 2023-02-12 11:09:48.000000 stromer_api-2.0.3/stromer_api/yearstats.py
-drwxrwxrwx   0        0        0        0 2023-02-15 21:42:31.633355 stromer_api-2.0.3/stromer_api.egg-info/
--rw-rw-rw-   0        0        0    10931 2023-02-15 21:42:30.000000 stromer_api-2.0.3/stromer_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      733 2023-02-15 21:42:31.000000 stromer_api-2.0.3/stromer_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-15 21:42:30.000000 stromer_api-2.0.3/stromer_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-15 21:42:30.000000 stromer_api-2.0.3/stromer_api.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 18:44:33.419713 stromer_api-2.0.4/
+-rw-rw-rw-   0        0        0    10931 2023-07-15 18:44:33.418711 stromer_api-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0    10610 2023-02-12 21:56:27.000000 stromer_api-2.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 18:44:33.419713 stromer_api-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      491 2023-07-15 18:44:15.000000 stromer_api-2.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:44:33.407716 stromer_api-2.0.4/stromer_api/
+-rw-rw-rw-   0        0        0     6481 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/__init__.py
+-rw-rw-rw-   0        0        0      464 2023-02-01 20:50:35.000000 stromer_api-2.0.4/stromer_api/bikedata.py
+-rw-rw-rw-   0        0        0     1078 2023-01-31 23:05:05.000000 stromer_api-2.0.4/stromer_api/bikemaintenance.py
+-rw-rw-rw-   0        0        0     1610 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/bikemotortuning.py
+-rw-rw-rw-   0        0        0      453 2023-02-08 21:00:06.000000 stromer_api-2.0.4/stromer_api/bikepart.py
+-rw-rw-rw-   0        0        0     1256 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/bikeposition.py
+-rw-rw-rw-   0        0        0     1411 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/bikesensors.py
+-rw-rw-rw-   0        0        0     4045 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/bikesettings.py
+-rw-rw-rw-   0        0        0     1819 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/bikeshop.py
+-rw-rw-rw-   0        0        0     3018 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/bikestate.py
+-rw-rw-rw-   0        0        0     1555 2023-02-01 21:12:36.000000 stromer_api-2.0.4/stromer_api/bikestatistics.py
+-rw-rw-rw-   0        0        0     1894 2023-02-01 21:12:36.000000 stromer_api-2.0.4/stromer_api/bikeuser.py
+-rw-rw-rw-   0        0        0     3828 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/daystats.py
+-rw-rw-rw-   0        0        0      486 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/general.py
+-rw-rw-rw-   0        0        0     5125 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/monthstats.py
+-rw-rw-rw-   0        0        0      929 2023-01-31 23:03:46.000000 stromer_api-2.0.4/stromer_api/periodicinfo.py
+-rw-rw-rw-   0        0        0     1395 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/periodstats.py
+-rw-rw-rw-   0        0        0     3860 2023-07-15 18:41:05.000000 stromer_api-2.0.4/stromer_api/portal.py
+-rw-rw-rw-   0        0        0     1385 2023-03-05 12:07:09.000000 stromer_api-2.0.4/stromer_api/service_info.py
+-rw-rw-rw-   0        0        0      369 2023-02-08 21:13:05.000000 stromer_api-2.0.4/stromer_api/service_log.py
+-rw-rw-rw-   0        0        0     4888 2023-03-05 12:10:02.000000 stromer_api-2.0.4/stromer_api/weekstats.py
+-rw-rw-rw-   0        0        0     4634 2023-03-05 12:10:02.000000 stromer_api-2.0.4/stromer_api/yearstats.py
+drwxrwxrwx   0        0        0        0 2023-07-15 18:44:33.416705 stromer_api-2.0.4/stromer_api.egg-info/
+-rw-rw-rw-   0        0        0    10931 2023-07-15 18:44:33.000000 stromer_api-2.0.4/stromer_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      733 2023-07-15 18:44:33.000000 stromer_api-2.0.4/stromer_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 18:44:33.000000 stromer_api-2.0.4/stromer_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-15 18:44:33.000000 stromer_api-2.0.4/stromer_api.egg-info/top_level.txt
```

### Comparing `stromer_api-2.0.3/PKG-INFO` & `stromer_api-2.0.4/stromer_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: stromer_api
-Version: 2.0.3
+Name: stromer-api
+Version: 2.0.4
 Summary: Stromer API for accessing data from your Stromer Speed Bike.
 Home-page: https://github.com/elnkosc/stromer_api
 Author: Koen
 Author-email: koen@schilders.org
 License: GPL
 Keywords: Stromer,EBike,Python,API
 Description-Content-Type: text/markdown
```

### Comparing `stromer_api-2.0.3/README.md` & `stromer_api-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `stromer_api-2.0.3/stromer_api/__init__.py` & `stromer_api-2.0.4/stromer_api/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -163,34 +163,34 @@
 
     def year_stats(self, year: int, num_years: int = 1) -> YearStats:
         if self.__year_stats is None:
             self.__year_stats = YearStats(self.__portal, year, num_years)
         return self.__year_stats
 
     def reset_trip_data(self) -> bool:
-        return self.__portal.delete("bike/id/%s/trip_data" % self.bikeid)
+        return self.__portal.delete(f"bike/id/{self.bikeid}/trip_data")
 
     def lock(self) -> bool:
         data = {"lock": True}
-        new_data = self.__portal.post("bike/%s/settings" % self.bikeid, data)
+        new_data = self.__portal.post(f"bike/{self.bikeid}/settings", data)
         if new_data is not None:
             self.__state = None
             return True
         return False
 
     def unlock(self) -> bool:
         data = {"lock": False}
-        new_data = self.__portal.post("bike/%s/settings" % self.bikeid, data)
+        new_data = self.__portal.post(f"bike/{self.bikeid}/settings", data)
         if new_data is not None:
             self.__state = None
             return True
         return False
 
     def light(self, mode: str) -> bool:
         if mode.lower() not in ["on", "off", "flash"]:
             return False
         data = {"mode": mode.lower()}
-        new_data = self.__portal.post("bike/%s/light" % self.bikeid, data)
+        new_data = self.__portal.post(f"bike/{self.bikeid}/light", data)
         if new_data is not None:
             self.__state = None
             return True
         return False
```

### Comparing `stromer_api-2.0.3/stromer_api/bikemaintenance.py` & `stromer_api-2.0.4/stromer_api/bikemaintenance.py`

 * *Files identical despite different names*

### Comparing `stromer_api-2.0.3/stromer_api/bikemotortuning.py` & `stromer_api-2.0.4/stromer_api/bikemotortuning.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from .bikedata import BikeDataFromPortal
 
 
 class BikeMotorTuning(BikeDataFromPortal):
     def __init__(self, portal: Portal, bike_id: int) -> None:
         super().__init__(portal=portal)
         self.__params = {"fields": "tuning_speed,tuning_torque,tuning_agility"}
-        self.__endpoint = "bike/%s/settings" % bike_id
+        self.__endpoint = f"bike/{bike_id}/settings"
         self._data = self._portal.get(self.__endpoint, self.__params)
 
     @property
     def tuning_torque(self) -> int:
         return item(self._data, "tuning_torque")
 
     @property
@@ -19,29 +19,17 @@
         return item(self._data, "tuning_speed")
 
     @property
     def tuning_agility(self) -> int:
         return item(self._data, "tuning_agility")
 
     def set(self, speed: int = None, torque: int = None, agility: int = None) -> None:
-        if speed is None:
-            speed = self.tuning_speed
-        else:
-            speed = speed
-
-        if torque is None:
-            torque = self.tuning_speed
-        else:
-            torque = torque
-
-        if agility is None:
-            agility = self.tuning_agility
-        else:
-            agility = agility
-
+        speed = self.tuning_speed if speed is None else speed
+        torque = self.tuning_speed if torque is None else torque
+        agility = self.tuning_agility if agility is None else agility
         data = {"tuning_speed": speed,
                 "tuning_torque": torque,
                 "tuning_agility": agility}
         new_data = self._portal.post(self.__endpoint, data)
         if new_data is not None:
             self._data = new_data
```

### Comparing `stromer_api-2.0.3/stromer_api/bikeposition.py` & `stromer_api-2.0.4/stromer_api/bikeposition.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 from .portal import Portal
 from .bikedata import BikeDataFromPortal
 
 
 class BikePosition(BikeDataFromPortal):
     def __init__(self, portal: Portal, bike_id: int, cached: bool = False) -> None:
         super().__init__(portal=portal)
-        self.__endpoint = "bike/%s/position" % bike_id
-        if cached:
-            self.__params = {"cached": "true"}
-        else:
-            self.__params = {"cached": "false"}
+        self.__endpoint = f"bike/{bike_id}/position"
+        self.__params = {"cached": "true"} if cached else {"cached": "false"}
         self._data = self._portal.get(self.__endpoint, self.__params)
 
     @property
     def latitude(self) -> float:
         return item(self._data, "latitude")
 
     @property
```

### Comparing `stromer_api-2.0.3/stromer_api/bikesensors.py` & `stromer_api-2.0.4/stromer_api/bikesensors.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,36 +3,28 @@
 from .bikedata import BikeDataFromPortal
 
 
 class BikeSensors(BikeDataFromPortal):
     def __init__(self, portal: Portal, bike_id: int) -> None:
         super().__init__(portal=portal)
         self.__params = {"fields": "recup_level_user_offset,user_torque_sensitivity"}
-        self.__endpoint = "bike/%s/settings" % bike_id
+        self.__endpoint = f"bike/{bike_id}/settings"
         self._data = self._portal.get(self.__endpoint, self.__params)
 
     @property
     def user_torque_sensitivity(self) -> int:
         return item(self._data, "user_torque_sensitivity")
 
     @property
     def recup_level_user_offset(self) -> int:
         return item(self._data, "recup_level_user_offset")
 
     def set(self, recup: int = None, torque: int = None) -> None:
-        if recup is None:
-            recup = self.recup_level_user_offset
-        else:
-            recup = recup
-
-        if torque is None:
-            torque = self.user_torque_sensitivity
-        else:
-            torque = torque
-
+        recup = self.recup_level_user_offset if recup is None else recup
+        torque = self.user_torque_sensitivity if torque is None else torque
         data = {"recup_level_user_offset": recup,
                 "user_torque_sensitivity": torque}
         new_data = self._portal.post(self.__endpoint, data)
         if new_data is not None:
             self._data = new_data
 
     @recup_level_user_offset.setter
```

### Comparing `stromer_api-2.0.3/stromer_api/bikesettings.py` & `stromer_api-2.0.4/stromer_api/bikesettings.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 
 class BikeSettings(BikeDataFromPortal):
     def __init__(self, portal: Portal, bike_id: int) -> None:
         super().__init__(portal=portal)
         self.__params = {"fields": "auto_lock_mode,auto_power_off_time,date_format,"
                                    "distance_unit,language,speed_unit,clock_format"}
-        self.__endpoint = "bike/%s/settings" % bike_id
+        self.__endpoint = f"bike/{bike_id}/settings"
         self._data = self._portal.get(self.__endpoint, self.__params)
 
     @property
     def auto_lock_mode(self) -> bool:
         return item(self._data, "auto_lock_mode")
 
     @property
```

### Comparing `stromer_api-2.0.3/stromer_api/bikeshop.py` & `stromer_api-2.0.4/stromer_api/bikeshop.py`

 * *Files 10% similar despite different names*

```diff
@@ -50,18 +50,21 @@
 
 class BikeShopList(BikeDataFromPortal):
     def __init__(self, portal: Portal) -> None:
         super().__init__(portal=portal)
         self.__endpoint = "shops"
         self._data = []
         shops = self._portal.get(self.__endpoint, full_list=True)
-        for shop in shops:
-            self._data.append(BikeShop(shop))
+        self._data.extend(BikeShop(shop) for shop in shops)
 
     def __getitem__(self, i: int) -> BikeShop:
         return self._data[i]
 
     def lookup(self, shop_name: str):
-        for shop in self._data:
-            if shop_name.lower() in shop.name.lower():
-                return shop
-        return None
+        return next(
+            (
+                shop
+                for shop in self._data
+                if shop_name.lower() in shop.name.lower()
+            ),
+            None,
+        )
```

### Comparing `stromer_api-2.0.3/stromer_api/bikestate.py` & `stromer_api-2.0.4/stromer_api/bikestate.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,16 @@
 from .portal import Portal
 from .bikedata import BikeDataFromPortal
 
 
 class BikeState(BikeDataFromPortal):
     def __init__(self, portal: Portal, bike_id: int, cached: bool = False) -> None:
         super().__init__(portal=portal)
-        self.__endpoint = "bike/%s/state" % bike_id
-        if cached:
-            self.__params = {"cached": "true"}
-        else:
-            self.__params = {"cached": "false"}
+        self.__endpoint = f"bike/{bike_id}/state"
+        self.__params = {"cached": "true"} if cached else {"cached": "false"}
         self._data = self._portal.get(self.__endpoint, self.__params)
 
     @property
     def trip_distance(self) -> float:
         return item(self._data, "trip_distance")
 
     @property
```

### Comparing `stromer_api-2.0.3/stromer_api/bikestatistics.py` & `stromer_api-2.0.4/stromer_api/bikestatistics.py`

 * *Files identical despite different names*

### Comparing `stromer_api-2.0.3/stromer_api/bikeuser.py` & `stromer_api-2.0.4/stromer_api/bikeuser.py`

 * *Files identical despite different names*

### Comparing `stromer_api-2.0.3/stromer_api/daystats.py` & `stromer_api-2.0.4/stromer_api/daystats.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .portal import Portal
 from .bikedata import BikeDataFromPortal
 from .periodstats import PeriodStats
 
 
 class DayStats(BikeDataFromPortal, PeriodStats):
     def __init__(self, portal: Portal, year: int, month: int, day: int, num_days: int = 1) -> None:
+        # sourcery skip: raise-specific-error
         BikeDataFromPortal.__init__(self, portal)
         self.__statistics_endpoint = "bike/statistics"
         self.__extra_data_endpoint = "bike/statistics/extra_data"
 
         # start day cannot be in the future
         start_date = datetime.date(year, month, day)
         if start_date > datetime.date.today():
```

### Comparing `stromer_api-2.0.3/stromer_api/monthstats.py` & `stromer_api-2.0.4/stromer_api/monthstats.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from .periodstats import PeriodStats
 import datetime
 import calendar
 
 
 class MonthStats(BikeDataFromPortal, PeriodStats):
     def __init__(self, portal: Portal, year: int, month: int, num_months: int = 1) -> None:
+        # sourcery skip: raise-specific-error
         BikeDataFromPortal.__init__(self, portal)
         self.__statistics_endpoint = "bike/statistics"
         self.__extra_data_endpoint = "bike/statistics/extra_data"
 
         # start day cannot be in the future
         start_date = datetime.date(year, month, 1)
         if start_date > datetime.date.today():
```

### Comparing `stromer_api-2.0.3/stromer_api/periodicinfo.py` & `stromer_api-2.0.4/stromer_api/periodicinfo.py`

 * *Files identical despite different names*

### Comparing `stromer_api-2.0.3/stromer_api/periodstats.py` & `stromer_api-2.0.4/stromer_api/periodstats.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,12 +33,12 @@
         header_format = self.__workbook.add_format({"bold": True})
         self.__worksheet.write_row("A1", headers, header_format)
         self.__line_number = 1
 
     def add_line(self, *args):
         data = tuple(args)
         self.__line_number += 1
-        self.__worksheet.write_row("A" + str(self.__line_number), data)
+        self.__worksheet.write_row(f"A{self.__line_number}", data)
 
     def close_worksheet(self):
         self.__worksheet.autofit()
         self.__workbook.close()
```

### Comparing `stromer_api-2.0.3/stromer_api/portal.py` & `stromer_api-2.0.4/stromer_api/portal.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 class Portal:
     __url = "https://stromer-portal.ch/mobile/v4/login/"
     __token_url = "https://stromer-portal.ch/mobile/v4/o/token/"
     __api_url = "https://api3.stromer-portal.ch/rapi/mobile/v4.1/"
 
     def __init__(self, username: str, password: str, client_id: str) -> None:
+        # sourcery skip: raise-specific-error
         self.__username = username
         self.__password = password
         self.__client_id = client_id
         self.__session = requests.session()
         self.__session.get(self.__url)
         self.__access_token = None
 
@@ -26,76 +27,76 @@
                 }
             )
 
             data = {
                 "password": self.__password,
                 "username": self.__username,
                 "csrfmiddlewaretoken": self.__session.cookies.get("csrftoken"),
-                "next": "/mobile/v4/o/authorize/?" + qs
+                "next": f"/mobile/v4/o/authorize/?{qs}",
             }
 
             res = self.__session.post(self.__url, data=data, headers={"Referer": self.__url}, allow_redirects=False)
             res = self.__session.send(res.next, allow_redirects=False)
 
             _, qs = splitquery(res.headers["Location"])
             query = parse_qs(qs)
             code = query["code"][0]
-            params = {
+            data = {
                 "grant_type": "authorization_code",
                 "client_id": self.__client_id,
                 "code": code,
                 "redirect_uri": "stromer://auth"
             }
 
-            res = requests.post(self.__token_url, params=params)
+            res = requests.post(self.__token_url, data=data)
             self.__access_token = res.json()["access_token"]
             self.__bike = self.get("bike")
 
         except:
             raise Exception("Authentication failed")
 
     def delete(self, endpoint: str) -> bool:
+        # sourcery skip: raise-specific-error
         try:
-            res = self.__session.delete(self.__api_url + endpoint + "/",
-                                        headers={"Authorization": "Bearer %s" % self.__access_token})
-            if res.status_code == 204:
-                return True
-            else:
-                return False
+            res = self.__session.delete(
+                self.__api_url + endpoint + "/",
+                headers={"Authorization": f"Bearer {self.__access_token}"},
+            )
+            return res.status_code == 204
         except:
             raise Exception("Error setting parameters")
 
     def post(self, endpoint: str, data: dict):
+        # sourcery skip: raise-specific-error
         try:
-            res = self.__session.post(self.__api_url + endpoint + "/",
-                                      headers={"Authorization": "Bearer %s" % self.__access_token},
-                                      json=data)
-            if "data" in res.json():
-                return res.json()["data"]
-            else:
-                return None
+            res = self.__session.post(
+                self.__api_url + endpoint + "/",
+                headers={"Authorization": f"Bearer {self.__access_token}"},
+                json=data,
+            )
+            return res.json()["data"] if "data" in res.json() else None
         except:
             raise Exception("Error setting parameters")
 
     def get(self, endpoint: str, params=None, full_list: bool = False):
+        # sourcery skip: raise-specific-error
         try:
             if params is None:
                 params = {}
 
-            res = self.__session.get(self.__api_url + endpoint,
-                                     headers={"Authorization": "Bearer %s" % self.__access_token},
-                                     params=params)
+            res = self.__session.get(
+                self.__api_url + endpoint,
+                headers={"Authorization": f"Bearer {self.__access_token}"},
+                params=params,
+            )
             if "data" not in res.json():
                 return None
             elif isinstance(res.json()["data"], list):
                 if full_list:
                     return res.json()["data"]
                 else:
-                    if len(res.json()["data"]) > 0:
-                        return res.json()["data"][0]
-                    else:
-                        return None
+                    return res.json()["data"][0] if len(res.json()["data"]) > 0 else None
             else:
                 return res.json()["data"]
 
         except:
             raise Exception("Error getting parameters")
```

### Comparing `stromer_api-2.0.3/stromer_api/service_info.py` & `stromer_api-2.0.4/stromer_api/service_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from .bikepart import BikePart
 from .service_log import ServiceLog
 
 
 class ServiceInfo(BikeDataFromPortal):
     def __init__(self, portal: Portal, bike_id: int) -> None:
         super().__init__(portal=portal)
-        self.__endpoint = "bike/%s/service_info" % bike_id
+        self.__endpoint = f"bike/{bike_id}/service_info"
         self._data = self._portal.get(self.__endpoint)
         self._bike_parts = None
         self._service_logs = None
 
     @property
     def shop(self) -> BikeShop:
         return BikeShop(item(self._data, "shop"))
@@ -26,18 +26,20 @@
     def serial(self) -> str:
         return item(self._data, "serial")
 
     @property
     def service_logs(self) -> list:
         if self._service_logs is None:
             self._service_logs = []
-            for log in item(self._data, "servicelogs"):
-                self._service_logs.append(ServiceLog(log))
+            self._service_logs.extend(
+                ServiceLog(log) for log in item(self._data, "servicelogs")
+            )
         return self._service_logs
 
     @property
     def bike_parts(self) -> list:
         if self._bike_parts is None:
             self._bike_parts = []
-            for part in item(self._data, "bikeparts"):
-                self._bike_parts.append(BikePart(part))
+            self._bike_parts.extend(
+                BikePart(part) for part in item(self._data, "bikeparts")
+            )
         return self._bike_parts
```

### Comparing `stromer_api-2.0.3/stromer_api/weekstats.py` & `stromer_api-2.0.4/stromer_api/weekstats.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .bikedata import BikeDataFromPortal
 from .periodstats import PeriodStats
 import datetime
 
 
 class WeekStats(BikeDataFromPortal, PeriodStats):
     def __init__(self, portal: Portal, year: int, week: int, num_weeks: int = 1) -> None:
+        # sourcery skip: raise-specific-error
         BikeDataFromPortal.__init__(self, portal)
         self.__statistics_endpoint = "bike/statistics"
         self.__extra_data_endpoint = "bike/statistics/extra_data"
 
         # start day cannot be in the future
         start_date = datetime.date.fromisocalendar(year, week, 1)
         if start_date > datetime.date.today():
@@ -40,15 +41,15 @@
         for week_info in weekly_info:
             year_nr = datetime.datetime.strptime(week_info["start"], "%Y%m%d").year
             week_nr = datetime.datetime.strptime(week_info["start"], "%Y%m%d").isocalendar().week
             week_nr_str = "%04d-W%02d" % (year_nr, week_nr)
 
             # week_end_day cannot be in the future
             week_last_day = datetime.datetime.strptime(week_info["start"], "%Y%m%d") + datetime.timedelta(days=6)
-            if week_last_day > datetime.datetime.today():
+            if week_last_day > datetime.datetime.now():
                 week_end_day = stop
             else:
                 week_end_day = week_last_day.strftime("%Y%m%d")
 
             self.__data["weekly_info"][week_nr_str] = {"start_date": week_info["start"],
                                                        "end_date": week_end_day,
                                                        "total_days": week_info["total_days"],
```

### Comparing `stromer_api-2.0.3/stromer_api/yearstats.py` & `stromer_api-2.0.4/stromer_api/yearstats.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .bikedata import BikeDataFromPortal
 from .periodstats import PeriodStats
 import datetime
 
 
 class YearStats(BikeDataFromPortal, PeriodStats):
     def __init__(self, portal: Portal, year: int, num_years: int = 1) -> None:
+        # sourcery skip: raise-specific-error
         BikeDataFromPortal.__init__(self, portal)
         self.__statistics_endpoint = "bike/statistics"
         self.__extra_data_endpoint = "bike/statistics/extra_data"
 
         # start day cannot be in the future
         start_date = datetime.date.fromisocalendar(year, 1, 1)
         if start_date > datetime.date.today():
```

### Comparing `stromer_api-2.0.3/stromer_api.egg-info/PKG-INFO` & `stromer_api-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: stromer-api
-Version: 2.0.3
+Name: stromer_api
+Version: 2.0.4
 Summary: Stromer API for accessing data from your Stromer Speed Bike.
 Home-page: https://github.com/elnkosc/stromer_api
 Author: Koen
 Author-email: koen@schilders.org
 License: GPL
 Keywords: Stromer,EBike,Python,API
 Description-Content-Type: text/markdown
```

### Comparing `stromer_api-2.0.3/stromer_api.egg-info/SOURCES.txt` & `stromer_api-2.0.4/stromer_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

