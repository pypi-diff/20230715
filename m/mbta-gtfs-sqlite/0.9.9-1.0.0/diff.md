# Comparing `tmp/mbta-gtfs-sqlite-0.9.9.tar.gz` & `tmp/mbta_gtfs_sqlite-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbta-gtfs-sqlite-0.9.9.tar", max compression
+gzip compressed data, was "mbta_gtfs_sqlite-1.0.0.tar", max compression
```

## Comparing `mbta-gtfs-sqlite-0.9.9.tar` & `mbta_gtfs_sqlite-1.0.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
--rw-r--r--   0        0        0       86 2023-05-02 12:38:56.937705 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/__init__.py
--rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/archive.py
--rw-r--r--   0        0        0     3014 2023-05-04 05:00:58.846666 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/build.py
--rw-r--r--   0        0        0      389 2023-05-04 05:03:03.344844 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/compact.py
--rw-r--r--   0        0        0     4369 2023-05-04 15:02:00.233311 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/feed.py
--rw-r--r--   0        0        0     6333 2023-05-04 22:19:23.539885 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/ingest.py
--rw-r--r--   0        0        0      322 2023-05-02 12:51:09.476358 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/__init__.py
--rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/base.py
--rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar.py
--rw-r--r--   0        0        0     1504 2023-05-02 13:18:44.004053 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar_attributes.py
--rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar_dates.py
--rw-r--r--   0        0        0      865 2023-05-28 23:25:35.414018 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/feed_info.py
--rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/lines.py
--rw-r--r--   0        0        0     1229 2023-05-02 13:18:34.963353 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/route_patterns.py
--rw-r--r--   0        0        0     1527 2023-05-02 13:17:54.982833 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/routes.py
--rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/shapes.py
--rw-r--r--   0        0        0      851 2023-04-30 02:22:40.117387 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/stop_times.py
--rw-r--r--   0        0        0     2326 2023-05-02 13:18:29.723968 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/stops.py
--rw-r--r--   0        0        0     1745 2023-05-02 13:18:22.018700 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/transfers.py
--rw-r--r--   0        0        0     2005 2023-05-04 22:18:43.022321 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/trips.py
--rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/reader.py
--rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/session.py
--rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/decorators.py
--rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/enum.py
--rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/indexes.py
--rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/time.py
--rw-r--r--   0        0        0      454 2023-05-28 23:26:42.128230 mbta-gtfs-sqlite-0.9.9/pyproject.toml
--rw-r--r--   0        0        0      742 2023-05-28 23:27:00.437581 mbta-gtfs-sqlite-0.9.9/setup.py
--rw-r--r--   0        0        0      494 2023-05-28 23:27:00.437810 mbta-gtfs-sqlite-0.9.9/PKG-INFO
+-rw-r--r--   0        0        0       86 2023-05-02 12:38:56.937705 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/__init__.py
+-rw-r--r--   0        0        0     2522 2023-05-01 20:26:55.513197 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/archive.py
+-rw-r--r--   0        0        0     3014 2023-05-04 05:00:58.846666 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/build.py
+-rw-r--r--   0        0        0      389 2023-05-04 05:03:03.344844 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/compact.py
+-rw-r--r--   0        0        0     4369 2023-05-04 15:02:00.233311 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/feed.py
+-rw-r--r--   0        0        0     6423 2023-06-13 19:45:15.263136 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/ingest.py
+-rw-r--r--   0        0        0      322 2023-05-02 12:51:09.476358 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/__init__.py
+-rw-r--r--   0        0        0      587 2023-03-30 20:22:33.250775 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/base.py
+-rw-r--r--   0        0        0     1421 2023-04-30 02:22:06.798132 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/calendar.py
+-rw-r--r--   0        0        0     1591 2023-06-14 14:12:15.148429 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/calendar_attributes.py
+-rw-r--r--   0        0        0      787 2023-04-30 02:21:58.055747 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/calendar_dates.py
+-rw-r--r--   0        0        0      801 2023-06-13 19:31:13.787983 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/feed_info.py
+-rw-r--r--   0        0        0      558 2023-04-30 02:22:13.201469 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/lines.py
+-rw-r--r--   0        0        0     1229 2023-05-02 13:18:34.963353 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/route_patterns.py
+-rw-r--r--   0        0        0     1527 2023-05-02 13:17:54.982833 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/routes.py
+-rw-r--r--   0        0        0      460 2023-04-30 02:22:37.057231 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/shapes.py
+-rw-r--r--   0        0        0      881 2023-06-15 19:53:21.029371 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/stop_times.py
+-rw-r--r--   0        0        0     2326 2023-05-02 13:18:29.723968 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/stops.py
+-rw-r--r--   0        0        0     1769 2023-06-15 19:43:09.061919 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/transfers.py
+-rw-r--r--   0        0        0     2067 2023-06-16 00:23:07.386114 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/trips.py
+-rw-r--r--   0        0        0     1370 2023-05-01 19:11:09.771246 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/reader.py
+-rw-r--r--   0        0        0      311 2023-05-01 18:39:38.649035 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/session.py
+-rw-r--r--   0        0        0      319 2023-03-30 17:44:07.909839 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/utils/decorators.py
+-rw-r--r--   0        0        0      228 2023-03-30 02:19:27.943839 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/utils/enum.py
+-rw-r--r--   0        0        0      764 2023-05-01 17:17:20.290734 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/utils/indexes.py
+-rw-r--r--   0        0        0      646 2023-03-30 19:49:23.509879 mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/utils/time.py
+-rw-r--r--   0        0        0      454 2023-07-15 21:20:12.768809 mbta_gtfs_sqlite-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      545 1970-01-01 00:00:00.000000 mbta_gtfs_sqlite-1.0.0/PKG-INFO
```

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/archive.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/archive.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/build.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/build.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/feed.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/feed.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/ingest.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/ingest.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,20 @@
 
     return inner_transform
 
 
 def transform_row_dict(
     row_dict: Dict[str, str],
     transforms: RowTransforms,
+    model: Type[Base],
 ) -> Dict[str, Any]:
     return {
         key: (transforms[key](value) if transforms.get(key) else value)
         for key, value in row_dict.items()
+        if key in model.__table__.columns
     }
 
 
 @listify
 def get_trip_rows_with_extra_time_fields(
     trip_rows: List[Dict[str, str]],
     stop_time_rows: List[Dict[str, str]],
@@ -78,14 +80,15 @@
             "retrieved_from_url": download.url,
             "zip_md5_checksum": download.zip_md5_checksum,
         },
         {
             "feed_start_date": date_from_string,
             "feed_end_date": date_from_string,
         },
+        FeedInfo,
     )
     feed_info = FeedInfo(**feed_info_dict)
     session.add(feed_info)
     session.commit()
     return feed_info
 
 
@@ -95,15 +98,15 @@
     feed_info: FeedInfo,
     rows: Iterable[Dict[str, str]],
     transforms: RowTransforms = {},
     individually: bool = False,
 ):
     mappings = [
         {
-            **transform_row_dict(row, transforms),
+            **transform_row_dict(row, transforms, model),
             "feed_info_id": feed_info.id,
         }
         for row in rows
     ]
     if individually:
         for mapping in mappings:
             session.add(model(**mapping))
```

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/base.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/base.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/calendar.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar_attributes.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/calendar_attributes.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,23 +13,25 @@
     NO_VALUE = ""  # Not in GTFS but sometimes seen
     NOT_DEFINED = "0"
     MINOR_MODIFICATIONS = "1"
     EXTRA_SERVICE = "2"
     REDUCED_TO_WEEKEND_SERVICE = "3"
     MAJOR_PLANNED_DISRUPTION = "4"
     MAJOR_ATYPICAL_REDUCTIONS = "5"
+    NOT_ACTIVELY_SCHEDULED = "6"
 
 
 TServiceScheduleTypicality = Literal[
     ServiceScheduleTypicality.NOT_DEFINED,
     ServiceScheduleTypicality.MINOR_MODIFICATIONS,
     ServiceScheduleTypicality.EXTRA_SERVICE,
     ServiceScheduleTypicality.REDUCED_TO_WEEKEND_SERVICE,
     ServiceScheduleTypicality.MAJOR_PLANNED_DISRUPTION,
     ServiceScheduleTypicality.MAJOR_ATYPICAL_REDUCTIONS,
+    ServiceScheduleTypicality.NOT_ACTIVELY_SCHEDULED,
 ]
 
 
 class CalendarAttribute(Base):
     service_id: Mapped[str] = mapped_column(String, index=True)
     service_description: Mapped[str] = mapped_column(String)
     service_schedule_name: Mapped[str] = mapped_column(String)
```

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/calendar_dates.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/calendar_dates.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/feed_info.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/feed_info.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,11 +11,10 @@
     feed_publisher_url: Mapped[str] = mapped_column(String)
     feed_lang: Mapped[str] = mapped_column(String)
     feed_start_date: Mapped[date] = mapped_column(Date)
     feed_end_date: Mapped[date] = mapped_column(Date)
     feed_version: Mapped[str] = mapped_column(String)
     feed_contact_email: Mapped[str] = mapped_column(String, nullable=True)
     feed_contact_url: Mapped[str] = mapped_column(String, nullable=True)
-    feed_id: Mapped[str] = mapped_column(String, nullable=True)
     # These are not part of GTFS
     retrieved_from_url: Mapped[str] = mapped_column(String)
     zip_md5_checksum: Mapped[str] = mapped_column(String)
```

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/lines.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/lines.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/route_patterns.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/route_patterns.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/routes.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/routes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/stop_times.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/stop_times.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,11 +9,11 @@
     stop_id: Mapped[str] = mapped_column(String, index=True)
     arrival_time: Mapped[int] = mapped_column(Integer)
     departure_time: Mapped[int] = mapped_column(Integer)
     stop_sequence: Mapped[int] = mapped_column(Integer)
     stop_headsign: Mapped[str] = mapped_column(String)
     pickup_type: Mapped[str] = mapped_column(String)
     drop_off_type: Mapped[str] = mapped_column(String)
-    timepoint: Mapped[str] = mapped_column(String)
-    checkpoint_id: Mapped[str] = mapped_column(String)
+    timepoint: Mapped[str] = mapped_column(String, nullable=True)
+    checkpoint_id: Mapped[str] = mapped_column(String, nullable=True)
     continuous_pickup: Mapped[str] = mapped_column(String, nullable=True)
     continuous_drop_off: Mapped[str] = mapped_column(String, nullable=True)
```

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/stops.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/stops.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/transfers.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/transfers.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,11 +47,12 @@
     to_stop_id: Mapped[str] = mapped_column(String)
     transfer_type: Mapped[TTranferType] = mapped_column(gtfs_enum_type(TransferType))
     min_transfer_time: Mapped[int] = mapped_column(Integer, nullable=True)
     min_walk_time: Mapped[int] = mapped_column(Integer, nullable=True)
     min_wheelchair_time: Mapped[int] = mapped_column(Integer, nullable=True)
     suggested_buffer_time: Mapped[int] = mapped_column(Integer, nullable=True)
     wheelchair_transfer: Mapped[TWheelchairAccessibility] = mapped_column(
-        gtfs_enum_type(WheelchairAccessibility)
+        gtfs_enum_type(WheelchairAccessibility),
+        nullable=True,
     )
     from_trip_id: Mapped[str] = mapped_column(String, nullable=True)
     to_trip_id: Mapped[str] = mapped_column(String, nullable=True)
```

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/models/trips.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/models/trips.py`

 * *Files 16% similar despite different names*

```diff
@@ -43,17 +43,21 @@
     trip_id: Mapped[str] = mapped_column(String)
     trip_headsign: Mapped[str] = mapped_column(String)
     trip_short_name: Mapped[str] = mapped_column(String)
     direction_id: Mapped[str] = mapped_column(String)
     block_id: Mapped[str] = mapped_column(String)
     shape_id: Mapped[str] = mapped_column(String)
     wheelchair_accessible: Mapped[TWheelchairAccessibility] = mapped_column(
-        gtfs_enum_type(WheelchairAccessibility)
+        gtfs_enum_type(WheelchairAccessibility),
+        nullable=True,
+    )
+    trip_route_type: Mapped[TRouteType] = mapped_column(
+        gtfs_enum_type(RouteType),
+        nullable=True,
     )
-    trip_route_type: Mapped[TRouteType] = mapped_column(gtfs_enum_type(RouteType))
     route_pattern_id: Mapped[str] = mapped_column(String, nullable=True)
     bikes_allowed: Mapped[TBikesAllowed] = mapped_column(
         gtfs_enum_type(BikesAllowed),
         nullable=True,
     )
     # These are not part of GTFS but they're useful information to have
     # in smaller versions of the database without StopTimes
```

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/reader.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/reader.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/indexes.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/utils/indexes.py`

 * *Files identical despite different names*

### Comparing `mbta-gtfs-sqlite-0.9.9/mbta_gtfs_sqlite/utils/time.py` & `mbta_gtfs_sqlite-1.0.0/mbta_gtfs_sqlite/utils/time.py`

 * *Files identical despite different names*

