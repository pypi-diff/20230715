# Comparing `tmp/midas-data-util-0.2.9.tar.gz` & `tmp/midas-data-util-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "midas-data-util-0.2.9.tar", last modified: Wed Jun 28 00:53:00 2023, max compression
+gzip compressed data, was "midas-data-util-0.3.0.tar", last modified: Sat Jul 15 03:10:52 2023, max compression
```

## Comparing `midas-data-util-0.2.9.tar` & `midas-data-util-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-06-28 00:53:00.352896 midas-data-util-0.2.9/
--rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.2.9/LICENSE
--rw-rw-rw-   0        0        0      520 2023-06-28 00:53:00.351899 midas-data-util-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.2.9/README.md
--rw-rw-rw-   0        0        0      623 2023-06-28 00:52:31.000000 midas-data-util-0.2.9/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-28 00:53:00.353893 midas-data-util-0.2.9/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-28 00:53:00.293902 midas-data-util-0.2.9/src/
-drwxrwxrwx   0        0        0        0 2023-06-28 00:53:00.315318 midas-data-util-0.2.9/src/midas/
--rw-rw-rw-   0        0        0     2631 2023-04-12 07:17:33.000000 midas-data-util-0.2.9/src/midas/__init__.py
--rw-rw-rw-   0        0        0     6161 2023-06-28 00:52:17.000000 midas-data-util-0.2.9/src/midas/data_encoder.py
--rw-rw-rw-   0        0        0    11528 2023-06-28 00:39:41.000000 midas-data-util-0.2.9/src/midas/event.py
--rw-rw-rw-   0        0        0     9382 2023-06-26 00:40:40.000000 midas-data-util-0.2.9/src/midas/playfab.py
--rw-rw-rw-   0        0        0     4327 2023-04-12 12:04:40.000000 midas-data-util-0.2.9/src/midas/session.py
--rw-rw-rw-   0        0        0     3448 2023-04-12 12:05:02.000000 midas-data-util-0.2.9/src/midas/user.py
-drwxrwxrwx   0        0        0        0 2023-06-28 00:53:00.349905 midas-data-util-0.2.9/src/midas_data_util.egg-info/
--rw-rw-rw-   0        0        0      520 2023-06-28 00:53:00.000000 midas-data-util-0.2.9/src/midas_data_util.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2023-06-28 00:53:00.000000 midas-data-util-0.2.9/src/midas_data_util.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-28 00:53:00.000000 midas-data-util-0.2.9/src/midas_data_util.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-06-28 00:53:00.000000 midas-data-util-0.2.9/src/midas_data_util.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-28 00:53:00.000000 midas-data-util-0.2.9/src/midas_data_util.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 03:10:52.897663 midas-data-util-0.3.0/
+-rw-rw-rw-   0        0        0    11558 2023-04-07 08:14:57.000000 midas-data-util-0.3.0/LICENSE
+-rw-rw-rw-   0        0        0      520 2023-07-15 03:10:52.896682 midas-data-util-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      116 2023-04-07 08:58:48.000000 midas-data-util-0.3.0/README.md
+-rw-rw-rw-   0        0        0      623 2023-07-15 03:10:33.000000 midas-data-util-0.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 03:10:52.897663 midas-data-util-0.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-15 03:10:52.866375 midas-data-util-0.3.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 03:10:52.876435 midas-data-util-0.3.0/src/midas/
+-rw-rw-rw-   0        0        0     2762 2023-07-15 01:30:04.000000 midas-data-util-0.3.0/src/midas/__init__.py
+-rw-rw-rw-   0        0        0     6354 2023-07-15 01:06:50.000000 midas-data-util-0.3.0/src/midas/data_encoder.py
+-rw-rw-rw-   0        0        0    11578 2023-07-15 01:36:37.000000 midas-data-util-0.3.0/src/midas/event.py
+-rw-rw-rw-   0        0        0    10877 2023-07-15 01:03:25.000000 midas-data-util-0.3.0/src/midas/playfab.py
+-rw-rw-rw-   0        0        0     8593 2023-07-15 02:25:06.000000 midas-data-util-0.3.0/src/midas/session.py
+-rw-rw-rw-   0        0        0     3686 2023-07-15 03:01:06.000000 midas-data-util-0.3.0/src/midas/user.py
+drwxrwxrwx   0        0        0        0 2023-07-15 03:10:52.895180 midas-data-util-0.3.0/src/midas_data_util.egg-info/
+-rw-rw-rw-   0        0        0      520 2023-07-15 03:10:52.000000 midas-data-util-0.3.0/src/midas_data_util.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-07-15 03:10:52.000000 midas-data-util-0.3.0/src/midas_data_util.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 03:10:52.000000 midas-data-util-0.3.0/src/midas_data_util.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-07-15 03:10:52.000000 midas-data-util-0.3.0/src/midas_data_util.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-15 03:10:52.000000 midas-data-util-0.3.0/src/midas_data_util.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2578 2023-07-15 01:34:34.000000 midas-data-util-0.3.0/src/test.py
```

### Comparing `midas-data-util-0.2.9/LICENSE` & `midas-data-util-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `midas-data-util-0.2.9/PKG-INFO` & `midas-data-util-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.2.9
+Version: 0.3.0
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `midas-data-util-0.2.9/pyproject.toml` & `midas-data-util-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "midas-data-util"
-version = "0.2.9"
+version = "0.3.0"
 authors = [
   { name="nightcycle", email="coyer@nightcycle.us" },
 ]
 dependencies = [
 	"lxml~=4.9.2", 
 	"pandas~=2.0.0",
 	"adal~=1.2.7",
```

### Comparing `midas-data-util-0.2.9/src/midas/__init__.py` & `midas-data-util-0.3.0/src/midas/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 from pandas import DataFrame
 from typing import Any
 from .event import Event, get_events_from_df
-from .session import Session, SessionDumpData,  get_sessions_from_events, get_survival_rate
+from .session import Session, SessionDumpData,  get_sessions_from_events
 from .user import User, UserDumpData, get_users_from_session_list
 
 def dump(objects: list[Event] | list[Session] | list[User]):
 	untyped_objects: Any = objects
 	object_count = len(objects)
 	if type(objects[0]) == Event:
 		event_list: list[Event] = untyped_objects
@@ -30,36 +30,38 @@
 		user_df: Any = DataFrame(user_data_list)
 		return user_df	
 	
 
 	
 def load(
 	decoded_df: DataFrame,
-	stitch_session_separation_limit_seconds=180, 
+	# stitch_session_separation_limit_seconds=180, 
 	exit_event_name="UserExitQuit", 
 	enter_event_name="UserJoinEnter",
-	rejoin_event_name="UserRejoin",
-	teleport_event_name="UserTeleport",
-	sessions_must_include_exit_and_enter_events=True,
-	fill_down_enabled=False, 
-	recursive_fill_down_enabled=False
+	# rejoin_event_name="UserRejoin",
+	# teleport_event_name="UserTeleport",
+	sessions_must_include_exit_and_enter_events=False,
+	# fill_down_enabled=False, 
+	# recursive_fill_down_enabled=False
 ) -> tuple[list[Event], list[Session], list[User]]:
 
-	print(f"assembling events from {decoded_df.shape[0]} rows of data")
-	events = get_events_from_df(decoded_df, stitch_session_separation_limit_seconds, exit_event_name, enter_event_name, rejoin_event_name, teleport_event_name, fill_down_enabled, recursive_fill_down_enabled)
+	max_event_count = decoded_df.shape[0]
+	print(f"assembling events from {max_event_count} event entries")
+	events = get_events_from_df(decoded_df) #, stitch_session_separation_limit_seconds, exit_event_name, enter_event_name, rejoin_event_name, teleport_event_name, fill_down_enabled, recursive_fill_down_enabled)
+	# print("failed to load ",round(1000*(1-(len(events)/max_event_count)))/10, "%","of events")
 
 	print(f"assembling sessions from {len(events)} events")
 	sessions = get_sessions_from_events(events, sessions_must_include_exit_and_enter_events, exit_event_name, enter_event_name)
 	
 	print(f"assembling users from {len(sessions)} sessions")
 	users = get_users_from_session_list(sessions)
 	
-	survival_rate = get_survival_rate(sessions)
+	# survival_rate = get_survival_rate(sessions)
 
-	print("event survival rate: "+str(round(survival_rate*100000)/1000)+"%")
+	# print("event survival rate: "+str(round(survival_rate*100000)/1000)+"%")
 
 	final_sessions: list[Session] = []
 	for user in users:
 		for session in user.sessions:
 			final_sessions.append(session)
 
 	final_events: list[Event] = []
```

### Comparing `midas-data-util-0.2.9/src/midas/data_encoder.py` & `midas-data-util-0.3.0/src/midas/data_encoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 	State: BaseStateTree
 
 
 class DecodedRowData(TypedDict):
 	EventData: EventData
 	Timestamp: str
 	PlayFabUserId: str
+	SessionId: str
+	Time: float
 	EventName: str
 	EventId: str
 
 def encode(full_data: dict[str, Any], encoding_config: dict[str, Any]):
 
 	encoding_dict = encoding_config["dictionary"]
 	encoding_property_dict = encoding_dict["properties"]
@@ -132,26 +134,26 @@
 
 	encoding_dict = encoding_config["dictionary"]
 	encoding_property_dict = encoding_dict["properties"]
 	encoding_value_dict = encoding_dict["values"]
 	encoding_arrays = encoding_config["arrays"]
 	encoding_marker = encoding_config["marker"]
 
-
 	def restore_keys(data: dict[str, Any]):
 		out = {}
 		for k in data:
 			v = data[k]
+
 			if type(v) == dict:
 				v = restore_keys(v)
 
 			decoded_key = k
 			if k.startswith(encoding_marker):
 				for original_key, encoded_key in encoding_property_dict.items():
-					if k == encoding_marker + encoded_key:
+					if k.replace(encoding_marker, "") == encoded_key.replace(encoding_marker, ""):
 						decoded_key = original_key
 						break
 
 			out[decoded_key] = v
 
 		return out
 
@@ -184,15 +186,15 @@
 				if type(v) == str:
 					if encoding_marker in v:
 						if type(nxt_bin_array_reg) == list:
 							v = restore_binary_list(v, nxt_bin_array_reg)
 						elif k in val_dict:
 							for orig_v in val_dict[k]:
 								alt_v = val_dict[k][orig_v]
-								if v == encoding_marker+alt_v:
+								if v.replace(encoding_marker, "") == alt_v.replace(encoding_marker, ""):
 									v = orig_v
 
 			out[k] = v
 
 		return out
 
 	return restore_values(restore_keys(encoded_data), encoding_value_dict, encoding_arrays)
@@ -225,14 +227,16 @@
 			event_data = raw_row_data["EventData"]
 		encoded_state_data = event_data["State"]
 		decoded_state_data = decode(encoded_state_data, encoding_config)
 
 		event_data["State"] = decoded_state_data
 		decoded_row_data: DecodedRowData = {
 				"EventData": event_data,
+				"SessionId": raw_row_data["SessionId"],
+				"Time": raw_row_data["Time"],
 				"Timestamp": raw_row_data["Timestamp"],
 				"PlayFabUserId": raw_row_data["PlayFabUserId"],
 				"EventName": raw_row_data["EventName"],
 				"EventId": raw_row_data["EventId"],
 		}
 		decoded_record_list.append(decoded_row_data)
```

### Comparing `midas-data-util-0.2.9/src/midas/event.py` & `midas-data-util-0.3.0/src/midas/event.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 from typing import Any
 from .playfab import get_datetime_from_playfab_str, get_playfab_str_from_datetime
 from .data_encoder import DecodedRowData as RowData
 from .data_encoder import VersionData, EventData, BaseStateTree
 
 SID_GEN_REFIX = "!generated"
 
-def get_if_session_id_generated(session_id: str) -> bool:
-	pattern = session_id[0:len(SID_GEN_REFIX)]
-	result = pattern == SID_GEN_REFIX
-	# print(f"is_gen: {result} since {pattern} is start of {session_id}")
-	return result
+# def get_if_session_id_generated(session_id: str) -> bool:
+# 	pattern = session_id[0:len(SID_GEN_REFIX)]
+# 	result = pattern == SID_GEN_REFIX
+# 	# print(f"is_gen: {result} since {pattern} is start of {session_id}")
+# 	return result
 
 def version_to_version_text(version: VersionData, is_hotfix_included=True, is_tag_included=False, is_test_group_included=False, is_build_included=True):
 	major = version["Major"]
 	minor = version["Minor"]
 	patch = version["Patch"]
 	
 	version_text = f"v{major}.{minor}.{patch}"
@@ -41,330 +41,325 @@
 
 	return version_text
 
 class EventDumpData:
 	name: str
 	event_id: str
 	timestamp: str
-	seconds_since_previous_event: None | float
 	seconds_since_session_start: float
 	version_text: str
 	revenue: int
 	session_id: str
 	user_id: str
 	place_id: str
 	version: VersionData
 	index: int
 	is_studio: bool
 	is_sequential: bool
-	state_date: BaseStateTree
+	state_data: BaseStateTree
 
 class Event: 
 	name: str
 	event_id: str
 	timestamp: datetime
-	seconds_since_previous_event: None | float
 	seconds_since_session_start: float
 	version_text: str
 	revenue: int
 	session_id: str
 	user_id: str
 	place_id: str
 	version: VersionData
 	index: int
 	is_studio: bool
 	is_sequential: bool
-	state_date: BaseStateTree
+	state_data: BaseStateTree
 
 	def __init__(
 		self, 
 		row_data: RowData
 	):
 		
 		self.name = row_data["EventName"]
 		self.event_id = row_data["EventId"]
 		self.timestamp: datetime = get_datetime_from_playfab_str(row_data["Timestamp"])
 
 		event_data: EventData = row_data["EventData"]
 		state_data = event_data["State"]
 	
+		if not "Version" in state_data:
+			print(self.event_id)
+
 		self.version_text = version_to_version_text(state_data["Version"])
 		self.session_id = SID_GEN_REFIX + str(uuid4())
-		self.seconds_since_previous_event = None
 
 		id_data = state_data["Id"]
 		assert id_data != None
 		self.place_id = id_data["Place"]
 		self.user_id = id_data["User"]
-
-		if id_data["Session"] != "nil":
-			session_id = id_data["Session"]
-			assert session_id
-			self.session_id = session_id
-	
+		self.session_id = row_data["SessionId"]
+		
 		self.version = state_data["Version"]
 		self.index = state_data["Index"]["Event"]
 		self.is_studio = state_data["IsStudio"]
 		self.state_data = state_data
 		self.revenue = 0
-		self.seconds_since_session_start = 0
+		self.seconds_since_session_start = row_data["Time"]
 		self.is_sequential = False
 
 	def __lt__(self, other):
 		t1 = self.index
 		t2 = other.index
 		return t1 < t2
 
 	def dump(self) -> EventDumpData:
 		event_dump_date: Any = {
 			"name": self.name,
 			"event_id": self.event_id,
 			"timestamp": get_playfab_str_from_datetime(self.timestamp),
-			"seconds_since_previous_event": self.seconds_since_previous_event,
 			"seconds_since_session_start": self.seconds_since_session_start,
 			"version_text": self.version_text,
 			"revenue": self.revenue,
 			"session_id": self.session_id,
 			"user_id": self.user_id,
 			"place_id": self.place_id,
 			"version": deepcopy(self.version),
 			"index": self.index,
 			"is_studio": self.is_studio,
 			"is_sequential": self.is_sequential,
-			"state_date": deepcopy(self.state_data),
+			"state_data": deepcopy(self.state_data),
 		}
 		return event_dump_date
 
-def fill_down(current_data: dict | None, prev_data: dict | None):
-		if current_data == None:
-			current_data = {}
+# def fill_down(current_data: dict | None, prev_data: dict | None):
+# 		if current_data == None:
+# 			current_data = {}
 
-		assert current_data
+# 		assert current_data
 
-		if prev_data == None:
-			return current_data
+# 		if prev_data == None:
+# 			return current_data
 
-		assert prev_data
+# 		assert prev_data
 
-		for key in prev_data:
-			val = prev_data[key]
-			if not key in current_data:
-				current_data[key] = deepcopy(prev_data[key])
+# 		for key in prev_data:
+# 			val = prev_data[key]
+# 			if not key in current_data:
+# 				current_data[key] = deepcopy(prev_data[key])
 
-				return current_data
+# 				return current_data
 
-			if type(val) == dict:
-				fill_down(current_data[key], prev_data[key])
-			else:
-				current_data[key] = val
+# 			if type(val) == dict:
+# 				fill_down(current_data[key], prev_data[key])
+# 			else:
+# 				current_data[key] = val
 
-		return current_data
+# 		return current_data
 
-def transfer_property(previous_data: dict, current_data: dict):
-	for key in previous_data:
-		val = previous_data[key]
-		if not key in current_data:
-			current_data[key] = {}
+# def transfer_property(previous_data: dict, current_data: dict):
+# 	for key in previous_data:
+# 		val = previous_data[key]
+# 		if not key in current_data:
+# 			current_data[key] = {}
 
-		if type(val) == dict:
-			current_data[key] = fill_down(current_data[key], previous_data[key])
+# 		if type(val) == dict:
+# 			current_data[key] = fill_down(current_data[key], previous_data[key])
 		
 
-# fill down event data when previous index is available
-def fill_down_event_from_previous(previous: Event, current: Event):
-	if current.is_sequential:
-		previous_data: Any = previous.state_data
-		current_data: Any = current.state_data
-		transfer_property(previous_data, current_data)
-
-def fill_down_events(session_events: list[Event], current: Event, targetIndex: int, depth: int):
-	if current.is_sequential:
-		depth += 1
-		if depth > 100:
-			return
-
-		for previous in session_events:
-			if previous.index == targetIndex:
-				fill_down_event_from_previous(previous, current)
-				break
-		if targetIndex > 1:
-			fill_down_events(session_events, current, targetIndex-1, depth)
+# # fill down event data when previous index is available
+# def fill_down_event_from_previous(previous: Event, current: Event):
+# 	if current.is_sequential:
+# 		previous_data: Any = previous.state_data
+# 		current_data: Any = current.state_data
+# 		transfer_property(previous_data, current_data)
+
+# def fill_down_events(session_events: list[Event], current: Event, targetIndex: int, depth: int):
+# 	if current.is_sequential:
+# 		depth += 1
+# 		if depth > 100:
+# 			return
+
+# 		for previous in session_events:
+# 			if previous.index == targetIndex:
+# 				fill_down_event_from_previous(previous, current)
+# 				break
+# 		if targetIndex > 1:
+# 			fill_down_events(session_events, current, targetIndex-1, depth)
 
 def get_events_from_df(
-	decoded_df: DataFrame, 
-	stitch_session_separation_limit_seconds=180, 
-	exit_event_name="UserExitQuit", 
-	enter_event_name="UserJoinEnter",
-	rejoin_event_name="UserRejoin",
-	teleport_event_name="UserTeleport",
-	fill_down_enabled=False, 
-	recursive_fill_down_enabled=False
+	decoded_df: DataFrame
+	# stitch_session_separation_limit_seconds=180, 
+	# exit_event_name="UserExitQuit", 
+	# enter_event_name="UserJoinEnter",
+	# rejoin_event_name="UserRejoin",
+	# teleport_event_name="UserTeleport",
+	# fill_down_enabled=False, 
+	# recursive_fill_down_enabled=False
 ) -> list[Event]:
 	initial_events: list[Event] = []
 
 	user_events: dict[str, list[Event]] = {}
 
 	print("organizing events by user_id")
 	for row_index, row_data in decoded_df.iterrows():
 
 		if type(row_data["EventData"]) == str:
 			row_data["EventData"] = json.loads(row_data["EventData"].replace("'", "\"").replace("False", "false").replace("True", "true"))
 
 		event = Event(row_data)
-		if not event.user_id in user_events:
-			user_events[event.user_id] = []
+		# if not event.user_id in user_events:
+		# 	user_events[event.user_id] = []
 		
-		user_events[event.user_id].append(event)
+		# user_events[event.user_id].append(event)
 		initial_events.append(event)
 
-	final_events: list[Event] = []
-	print("organizing events into chronological series for session id")
-	for event_list in user_events.values():
-		sorted_event_list = sorted(event_list, key=lambda event: event.timestamp)
-		event_count = len(sorted_event_list)
-		final_index = event_count-1
-		session_id_order: list[str] = []
-		initial_session_registry: dict[str, list[Event]] = {}
+	# final_events: list[Event] = []
+	
+	# print("organizing events into chronological series for session id")
+	# for event_list in user_events.values():
+	# 	sorted_event_list = sorted(event_list, key=lambda event: event.timestamp)
+	# 	event_count = len(sorted_event_list)
+	# 	final_index = event_count-1
+	# 	session_id_order: list[str] = []
+	# 	initial_session_registry: dict[str, list[Event]] = {}
 
-		def assemble_session(start_index=0) -> None:
-			session_id = str(uuid4())
+	# 	def assemble_session(start_index=0) -> None:
+	# 		session_id = str(uuid4())
 			
-			session_events: list[Event] = []
-			next_index=start_index+1
-			if start_index == final_index:
-				session_events.append(sorted_event_list[start_index])
-			else:
-				# print("\nMULTI EVENT!")
-				for i in range(start_index, final_index):
+	# 		session_events: list[Event] = []
+	# 		next_index=start_index+1
+	# 		if start_index == final_index:
+	# 			session_events.append(sorted_event_list[start_index])
+	# 		else:
+	# 			# print("\nMULTI EVENT!")
+	# 			for i in range(start_index, final_index):
 					
-					event = sorted_event_list[i]
-					# print(f"index {i}: [{start_index}/{final_index}] at {event.timestamp}")
-					relative_index = i-start_index
-					next_index = i+1
-
-					if relative_index != 0 and event.name == enter_event_name:
-						# print("A")
-						break
-
-					is_session_id_generated = get_if_session_id_generated(event.session_id)
-					if relative_index > 0:
-						prev_event = session_events[relative_index-1]
-						is_prev_session_id_generated = get_if_session_id_generated(prev_event.session_id)
-						if is_session_id_generated and not is_prev_session_id_generated:
-							# print("B1")
-							break
-						elif not is_session_id_generated and not is_prev_session_id_generated and event.session_id != prev_event.session_id:
-							# print(f"B2: {event.session_id}, {prev_event.session_id}")
-							break
-						elif prev_event.name == exit_event_name:
-							# print("B3")
-							break
-						elif prev_event.is_studio != event.is_studio:
-							# print("B4")
-							break
-
-					session_events.append(event)
-
-			if len(session_events) > 0:
-				initial_session_registry[session_id] = session_events
-				session_id_order.append(session_id)
+	# 				event = sorted_event_list[i]
+	# 				# print(f"index {i}: [{start_index}/{final_index}] at {event.timestamp}")
+	# 				relative_index = i-start_index
+	# 				next_index = i+1
+
+	# 				if relative_index != 0 and event.name == enter_event_name:
+	# 					# print("A")
+	# 					break
+
+	# 				is_session_id_generated = get_if_session_id_generated(event.session_id)
+	# 				if relative_index > 0:
+	# 					prev_event = session_events[relative_index-1]
+	# 					is_prev_session_id_generated = get_if_session_id_generated(prev_event.session_id)
+	# 					if is_session_id_generated and not is_prev_session_id_generated:
+	# 						# print("B1")
+	# 						break
+	# 					elif not is_session_id_generated and not is_prev_session_id_generated and event.session_id != prev_event.session_id:
+	# 						# print(f"B2: {event.session_id}, {prev_event.session_id}")
+	# 						break
+	# 					elif prev_event.name == exit_event_name:
+	# 						# print("B3")
+	# 						break
+	# 					elif prev_event.is_studio != event.is_studio:
+	# 						# print("B4")
+	# 						break
+
+	# 				session_events.append(event)
+
+	# 		if len(session_events) > 0:
+	# 			initial_session_registry[session_id] = session_events
+	# 			session_id_order.append(session_id)
 
-			if next_index <= final_index:
-				assemble_session(next_index)
+	# 		if next_index <= final_index:
+	# 			assemble_session(next_index)
 
-			return None
+	# 		return None
 
-		assemble_session()
+	# 	assemble_session()
 		
-		initial_final_index = len(session_id_order)-1
-		final_session_list: list[list[Event]] = []
-		def merge_sessions(start_index=0) -> None:
-			final_index = start_index+1
-			session_run: list[list[Event]] = []
-			if start_index == initial_final_index:
-				session_run.append(initial_session_registry[session_id_order[start_index]])
-			else:
-				for i in range(start_index, initial_final_index):
-					relative_index = i-start_index
-					session_event_list = initial_session_registry[session_id_order[i]]
-
-					final_index = i + 1
-					# print("ri", relative_index, "sr", len(session_run))
-					if relative_index > 0:
-						prev_session_event_list = session_run[relative_index-1]
-						prev_final_event = prev_session_event_list[len(prev_session_event_list)-1]
-						first_event = session_event_list[0]
-						sec_dif = (first_event.timestamp - prev_final_event.timestamp).total_seconds()
-						if sec_dif < stitch_session_separation_limit_seconds:
-							session_run.append(session_event_list)
-						else:
-							break
-					else:
-						session_run.append(session_event_list)
+	# 	initial_final_index = len(session_id_order)-1
+	# 	final_session_list: list[list[Event]] = []
+	# 	def merge_sessions(start_index=0) -> None:
+	# 		final_index = start_index+1
+	# 		session_run: list[list[Event]] = []
+	# 		if start_index == initial_final_index:
+	# 			session_run.append(initial_session_registry[session_id_order[start_index]])
+	# 		else:
+	# 			for i in range(start_index, initial_final_index):
+	# 				relative_index = i-start_index
+	# 				session_event_list = initial_session_registry[session_id_order[i]]
+
+	# 				final_index = i + 1
+	# 				# print("ri", relative_index, "sr", len(session_run))
+	# 				if relative_index > 0:
+	# 					prev_session_event_list = session_run[relative_index-1]
+	# 					prev_final_event = prev_session_event_list[len(prev_session_event_list)-1]
+	# 					first_event = session_event_list[0]
+	# 					sec_dif = (first_event.timestamp - prev_final_event.timestamp).total_seconds()
+	# 					if sec_dif < stitch_session_separation_limit_seconds:
+	# 						session_run.append(session_event_list)
+	# 					else:
+	# 						break
+	# 				else:
+	# 					session_run.append(session_event_list)
 		
-			if len(session_run) > 1:
-				composite_event_list: list[Event] = []
-				for i, session_event_list in enumerate(session_run):
-					rename_first_event = i > 0
-					keep_final_event = i == len(session_run)-1
-
-					is_new_place = False
-					if i > 0:
-						prev_session_event_list = session_run[i-1]
-						is_new_place = prev_session_event_list[0].place_id == session_event_list[0].place_id
-
-					for j, event in enumerate(session_event_list):
-						if j == 0 and rename_first_event:
-							if is_new_place:
-								event.name == teleport_event_name
-							else:
-								event.name == rejoin_event_name
+	# 		if len(session_run) > 1:
+	# 			composite_event_list: list[Event] = []
+	# 			for i, session_event_list in enumerate(session_run):
+	# 				rename_first_event = i > 0
+	# 				keep_final_event = i == len(session_run)-1
+
+	# 				is_new_place = False
+	# 				if i > 0:
+	# 					prev_session_event_list = session_run[i-1]
+	# 					is_new_place = prev_session_event_list[0].place_id == session_event_list[0].place_id
+
+	# 				for j, event in enumerate(session_event_list):
+	# 					if j == 0 and rename_first_event:
+	# 						if is_new_place:
+	# 							event.name == teleport_event_name
+	# 						else:
+	# 							event.name == rejoin_event_name
 						
-						if j < len(session_event_list)-1 or keep_final_event:
-							composite_event_list.append(event)
+	# 					if j < len(session_event_list)-1 or keep_final_event:
+	# 						composite_event_list.append(event)
 
-				final_session_list.append(composite_event_list)
-			else:
-				final_session_list.append(session_run[0])		
-
-			if final_index <= len(session_id_order)-1:
-				merge_sessions(final_index)
-
-			return None
-
-		merge_sessions()
-
-		for session_event_list in final_session_list:
-			session_id = str(uuid4())
-			if len(session_event_list) > 1:
-				first_event = session_event_list[0]
-				for i, event in enumerate(session_event_list):
-					event.session_id = session_id
-					final_events.append(event)
-					if i > 0:
-						prev_event = session_event_list[i-1]
-						event.seconds_since_previous_event = (event.timestamp - prev_event.timestamp).total_seconds()
-						event.seconds_since_session_start = (event.timestamp - first_event.timestamp).total_seconds()
+	# 			final_session_list.append(composite_event_list)
+	# 		else:
+	# 			final_session_list.append(session_run[0])		
+
+	# 		if final_index <= len(session_id_order)-1:
+	# 			merge_sessions(final_index)
+
+	# 		return None
+
+	# 	merge_sessions()
+
+	# 	for session_event_list in final_session_list:
+	# 		session_id = str(uuid4())
+	# 		if len(session_event_list) > 1:
+	# 			first_event = session_event_list[0]
+	# 			for i, event in enumerate(session_event_list):
+	# 				event.session_id = session_id
+	# 				final_events.append(event)
+	# 				if i > 0:
+	# 					prev_event = session_event_list[i-1]
+	# 					event.seconds_since_session_start = (event.timestamp - first_event.timestamp).total_seconds()
 							
-						# handle sequential stuff
-						if event.index == 2:
-							prev_event.is_sequential = True
-							event.is_sequential = True
-						elif prev_event.index == event.index - 1:
-							event.is_sequential = True
-
-						# handle fill down stuff
-						if fill_down_enabled:
-							if recursive_fill_down_enabled:
-								fill_down_event_from_previous(prev_event, event)
-							else:
-								fill_down_events(session_event_list, prev_event, event.index - 1, 0)
-			else:
-				event = session_event_list[0]
-				event.session_id = session_id
-				final_events.append(event)
+	# 					# handle sequential stuff
+	# 					if event.index == 2:
+	# 						prev_event.is_sequential = True
+	# 						event.is_sequential = True
+	# 					elif prev_event.index == event.index - 1:
+	# 						event.is_sequential = True
+
+	# 					# handle fill down stuff
+	# 					if fill_down_enabled:
+	# 						if recursive_fill_down_enabled:
+	# 							fill_down_event_from_previous(prev_event, event)
+	# 						else:
+	# 							fill_down_events(session_event_list, prev_event, event.index - 1, 0)
+	# 		else:
+	# 			event = session_event_list[0]
+	# 			event.session_id = session_id
+	# 			final_events.append(event)
 		
-		# if len(event_list) > 1:
-		# 	break
+	# 	# if len(event_list) > 1:
+	# 	# 	break
 
-	return final_events
+	return initial_events
```

### Comparing `midas-data-util-0.2.9/src/midas/playfab.py` & `midas-data-util-0.3.0/src/midas/playfab.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from azure.kusto.data.exceptions import KustoServiceError
 from azure.kusto.data import KustoClient, KustoConnectionStringBuilder, ClientRequestProperties
 from adal import AuthenticationContext
 import time
 import json
 import math
 import pandas as pd
+from pandas import Timestamp
 from datetime import datetime
 from copy import deepcopy
 from typing import Any, TypedDict, Literal, Tuple
+import sys, os
 
 CLUSTER = "https://insights.playfab.com"
 DEFAULT_QUERY ="['events.all'] | limit 100"
 PLAYFAB_DATE_FORMAT = "%Y-%m-%d %H:%M:%S.%f%z"
 PLAYFAB_DATE_FORMAT_WITHOUT_FRACTION = '%Y-%m-%d %H:%M:%S%z'
 PLAYFAB_DATE_FORMAT_WITH_FRACTION_NO_TZ = '%Y-%m-%d %H:%M:%S.%f'
 class UserData(TypedDict):
@@ -21,23 +23,30 @@
 
 class RawRowData(TypedDict):
 	EventData: str
 	Timestamp: str
 	PlayFabUserId: str
 	EventName: str
 	EventId: str
+	SessionId: str
+	Time: float
 
-def get_datetime_from_playfab_str(playfab_str: str) -> datetime:
-	try:
-		return datetime.strptime(playfab_str, PLAYFAB_DATE_FORMAT)
-	except:
-		try: 
-			return datetime.strptime(playfab_str, PLAYFAB_DATE_FORMAT_WITHOUT_FRACTION)
+def get_datetime_from_playfab_str(playfab_str: str | Timestamp) -> datetime:
+	if type(playfab_str) == str:
+		try:
+			return datetime.strptime(playfab_str, PLAYFAB_DATE_FORMAT)
 		except:
-			return datetime.strptime(playfab_str, PLAYFAB_DATE_FORMAT_WITH_FRACTION_NO_TZ)
+			try: 
+				return datetime.strptime(playfab_str, PLAYFAB_DATE_FORMAT_WITHOUT_FRACTION)
+			except:
+				return datetime.strptime(playfab_str, PLAYFAB_DATE_FORMAT_WITH_FRACTION_NO_TZ)
+	elif type(playfab_str) == Timestamp:
+		return playfab_str.to_pydatetime()
+	else:
+		raise ValueError(str(type(playfab_str))+" is not a Timestamp or str")
 
 def get_playfab_str_from_datetime(datetime: datetime) -> str:
 	return datetime.strftime(PLAYFAB_DATE_FORMAT)
 
 def update_based_on_success(
 	is_success: bool, 
 	event_limit: int, 
@@ -86,19 +95,25 @@
 		self.client = KustoClient(kcsb)
 		self.client._query_endpoint = CLUSTER + "/v1/rest/query"
 
 		crp = ClientRequestProperties()
 		crp.application = "KustoPythonSDK"
 
 	def query(self, query=DEFAULT_QUERY):
+		print("executing query")
+		
+		sys.stdout = open(os.devnull, 'w')
 		response = self.client.execute(self.title_id, query)
+		sys.stdout = sys.__stdout__
 
 		# Response processing
 		result = str(response[0])
+		print("loading response")
 		df = pd.DataFrame(json.loads(result)["data"])
+		print("finished creating df")
 
 		return df.to_dict(orient='records')
 
 
 	def query_user_data_list(self, user_join_floor: datetime, join_window_in_days: int, user_limit=100000) -> list[UserData]:
 		query = f"""let filter_users_who_joined_before= datetime("{get_playfab_str_from_datetime(user_join_floor)}");
 let join_window_in_days = {join_window_in_days};
@@ -127,21 +142,49 @@
 | sort by EventCount
 """
 		return self.query(query)
 
 	def query_events_from_user_data(self, playfab_user_ids: list[str], user_join_floor: datetime) -> list[RawRowData]:
 		query = f"""let playfab_user_ids = dynamic({json.dumps(playfab_user_ids)});
 let only_events_after = datetime("{get_playfab_str_from_datetime(user_join_floor)}");
-['events.all']
+let session_list = ['events.all']
+| where FullName_Name == "player_logged_in"
+| project-keep Timestamp, EventId, EntityLineage_master_player_account
+| project-rename SessionId=EventId,PlayFabUserId=EntityLineage_master_player_account
+| where PlayFabUserId in (playfab_user_ids)
+| sort by Timestamp
+// | join kind=inner users_by_event_count on PlayFabUserId
+;
+let all_events = ['events.all']
 | where Timestamp > only_events_after
 | where FullName_Namespace  == "title.{self.title_id}"
 | project-rename PlayFabUserId=EntityLineage_master_player_account
 | where PlayFabUserId in (playfab_user_ids)
 | project-rename EventName=FullName_Name
 | project-keep EventData, Timestamp, PlayFabUserId, EventName, EventId
+;
+let session_events = all_events
+| join kind=fullouter  (
+    session_list
+    | project-rename SessionTimestamp=Timestamp
+) on PlayFabUserId
+| project-away PlayFabUserId1
+| extend Time = todouble(todouble(datetime_diff("millisecond", Timestamp, SessionTimestamp))/todouble(1000))
+| extend EventSessionId = strcat(EventId, Time)
+| where Time >= 0.0
+;
+let final_events = session_events
+| join kind=inner  (
+    session_events 
+    | summarize min(Time) by EventId
+    | extend EventSessionId = strcat(EventId, min_Time)
+) on EventSessionId
+| project-keep Timestamp, Time, SessionId, EventData, EventName, PlayFabUserId, EventId
+;
+final_events
 """
 		return self.query(query)
 
 	def recursively_query_events(
 		self,
 		user_data_list: list[UserData], 
 		event_limit: int,
```

### Comparing `midas-data-util-0.2.9/src/midas/user.py` & `midas-data-util-0.3.0/src/midas/user.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,52 @@
 import datetime as dt
 import copy
 from datetime import datetime
-from typing import Any, TypedDict
+from typing import Any, TypedDict, Optional
 from .session import Session
 from .playfab import get_playfab_str_from_datetime
 
 class UserDumpData(TypedDict):
 	user_id: str
 	timestamp: str
 	index: int
 	session_count: int
 	net_revenue: int
 	net_duration: float
-	is_retained_on_d0: bool
-	is_retained_on_d1: bool
-	is_retained_on_d7: bool
-	is_retained_on_d14: bool
-	is_retained_on_d28: bool
+	is_retained_on_d0: Optional[bool]
+	is_retained_on_d1: Optional[bool]
+	is_retained_on_d7: Optional[bool]
+	is_retained_on_d14: Optional[bool]
+	is_retained_on_d28: Optional[bool]
 
 class User:
 	user_id: str
 	timestamp: datetime
 	index: int
 	session_count: int
 	net_revenue: int
 	net_duration: float
-	is_retained_on_d0: bool
-	is_retained_on_d1: bool
-	is_retained_on_d7: bool
-	is_retained_on_d14: bool
-	is_retained_on_d28: bool
+	is_retained_on_d0: Optional[bool]
+	is_retained_on_d1: Optional[bool]
+	is_retained_on_d7: Optional[bool]
+	is_retained_on_d14: Optional[bool]
+	is_retained_on_d28: Optional[bool]
 
 	def __init__(self, sessions: list[Session]):
 		sessions.sort()
 
 		first_session = sessions[0]
 
 		self.user_id = first_session.user_id
 		self.sessions = sessions
 		self.timestamp = first_session.timestamp
 
 		last_session = sessions[len(sessions)-1]
+
+		final_timestamp = last_session.timestamp
 		
 		self.net_revenue = 0
 		self.net_duration = 0.0
 	
 		index = 0
 		for session in sessions:
 			index += 1
@@ -57,19 +59,22 @@
 
 			for session in sessions:
 				if session.timestamp >= start and session.timestamp <= finish:
 					sessionsBetween.append(session)
 
 			return sessionsBetween
 
-		def get_retention_status(day: int, threshold: int):
+		def get_retention_status(day: int, threshold: int) -> Optional[bool]:
 			start: datetime = self.timestamp + dt.timedelta(days=day)
 			finish: datetime = start + dt.timedelta(days=1)
-			return len(get_sessions_count_between(start, finish)) > threshold
-
+			if finish <= datetime.now():
+				return len(get_sessions_count_between(start, finish)) > threshold
+			else:
+				return None
+			
 		self.is_retained_on_d0 = get_retention_status(0, 1)
 		self.is_retained_on_d1 = get_retention_status(1, 2)
 		self.is_retained_on_d7 = get_retention_status(7, 8)
 		self.is_retained_on_d14 = get_retention_status(14, 15)
 		self.is_retained_on_d28 = get_retention_status(28, 29)
 
 		self.index = -1
```

### Comparing `midas-data-util-0.2.9/src/midas_data_util.egg-info/PKG-INFO` & `midas-data-util-0.3.0/src/midas_data_util.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: midas-data-util
-Version: 0.2.9
+Version: 0.3.0
 Summary: a package with useful functions for downloading and working with midas generated analytics data
 Author-email: nightcycle <coyer@nightcycle.us>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

