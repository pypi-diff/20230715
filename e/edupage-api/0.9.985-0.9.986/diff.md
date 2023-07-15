# Comparing `tmp/edupage_api-0.9.985.tar.gz` & `tmp/edupage_api-0.9.986.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edupage_api-0.9.985.tar", last modified: Wed May  4 13:22:07 2022, max compression
+gzip compressed data, was "edupage_api-0.9.986.tar", last modified: Fri Jun 24 17:23:23 2022, max compression
```

## Comparing `edupage_api-0.9.985.tar` & `edupage_api-0.9.986.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 13:22:07.514601 edupage_api-0.9.985/
--rw-r--r--   0 runner    (1001) docker     (121)    35148 2022-05-04 13:21:45.000000 edupage_api-0.9.985/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2622 2022-05-04 13:22:07.514601 edupage_api-0.9.985/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-05-04 13:21:45.000000 edupage_api-0.9.985/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 13:22:07.514601 edupage_api-0.9.985/edupage_api/
--rw-r--r--   0 runner    (1001) docker     (121)     8061 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/cloud.py
--rw-r--r--   0 runner    (1001) docker     (121)      437 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/custom_request.py
--rw-r--r--   0 runner    (1001) docker     (121)     4118 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/dbi.py
--rw-r--r--   0 runner    (1001) docker     (121)      614 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5479 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/foreign_timetables.py
--rw-r--r--   0 runner    (1001) docker     (121)     4164 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/grades.py
--rw-r--r--   0 runner    (1001) docker     (121)     3184 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/login.py
--rw-r--r--   0 runner    (1001) docker     (121)     5564 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/lunches.py
--rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/messages.py
--rw-r--r--   0 runner    (1001) docker     (121)     2746 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     6782 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/people.py
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/ringing.py
--rw-r--r--   0 runner    (1001) docker     (121)     4804 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/substitution.py
--rw-r--r--   0 runner    (1001) docker     (121)     6031 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/timeline.py
--rw-r--r--   0 runner    (1001) docker     (121)     5355 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/timetables.py
--rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-05-04 13:21:45.000000 edupage_api-0.9.985/edupage_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-04 13:22:07.514601 edupage_api-0.9.985/edupage_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2622 2022-05-04 13:22:06.000000 edupage_api-0.9.985/edupage_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-05-04 13:22:07.000000 edupage_api-0.9.985/edupage_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-04 13:22:06.000000 edupage_api-0.9.985/edupage_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-05-04 13:22:07.000000 edupage_api-0.9.985/edupage_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-04 13:22:07.000000 edupage_api-0.9.985/edupage_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      142 2022-05-04 13:21:45.000000 edupage_api-0.9.985/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      738 2022-05-04 13:22:07.514601 edupage_api-0.9.985/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      140 2022-05-04 13:21:45.000000 edupage_api-0.9.985/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:23:23.812956 edupage_api-0.9.986/
+-rw-r--r--   0 runner    (1001) docker     (121)    35148 2022-06-24 17:23:00.000000 edupage_api-0.9.986/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-06-24 17:23:23.812956 edupage_api-0.9.986/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1906 2022-06-24 17:23:00.000000 edupage_api-0.9.986/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:23:23.812956 edupage_api-0.9.986/edupage_api/
+-rw-r--r--   0 runner    (1001) docker     (121)     8038 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2769 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (121)      437 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/custom_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4118 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/dbi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5478 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/foreign_timetables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4394 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/grades.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3142 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/login.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5563 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/lunches.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1049 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/messages.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2746 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6812 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/people.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2266 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/ringing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4766 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6084 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5826 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/timetables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2684 2022-06-24 17:23:00.000000 edupage_api-0.9.986/edupage_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-24 17:23:23.812956 edupage_api-0.9.986/edupage_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-06-24 17:23:23.000000 edupage_api-0.9.986/edupage_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-06-24 17:23:23.000000 edupage_api-0.9.986/edupage_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-24 17:23:23.000000 edupage_api-0.9.986/edupage_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-06-24 17:23:23.000000 edupage_api-0.9.986/edupage_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-06-24 17:23:23.000000 edupage_api-0.9.986/edupage_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2022-06-24 17:23:00.000000 edupage_api-0.9.986/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2022-06-24 17:23:23.812956 edupage_api-0.9.986/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      140 2022-06-24 17:23:00.000000 edupage_api-0.9.986/setup.py
```

### Comparing `edupage_api-0.9.985/LICENSE` & `edupage_api-0.9.986/LICENSE`

 * *Files identical despite different names*

### Comparing `edupage_api-0.9.985/PKG-INFO` & `edupage_api-0.9.986/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: edupage_api
-Version: 0.9.985
+Version: 0.9.986
 Summary: A python library for accessing your Edupage account
 Home-page: https://github.com/ivanhrabcak/edupage-api
 Author: ivanhrabcak
 Author-email: ivan@hrabcak.eu
-License: UNKNOWN
 Keywords: edupage,edupage api,library
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
@@ -54,9 +52,7 @@
 The docs are available [here](https://yesdaddyfuck.me/edupage-api/)
 
 # I have a problem or an idea!
 
 - If you find any issue with this code, or it doesn't work please, let us know by opening an [issue](https://github.com/ivanhrabcak/edupage-api/issues/new/choose)!
 - Feel free to suggest any other features! Just open an [issue with the _Feature Request_ tag](https://github.com/ivanhrabcak/edupage-api/issues/new?labels=feature+request&template=feature_request.md&title=%5BFeature+request%5D+).
 - If you, even better, have fixed the issue, added a new feature, or made something work better, please, open a [pull request](https://github.com/ivanhrabcak/edupage-api/compare)!
-
-
```

### Comparing `edupage_api-0.9.985/README.md` & `edupage_api-0.9.986/README.md`

 * *Files identical despite different names*

### Comparing `edupage_api-0.9.985/edupage_api/__init__.py` & `edupage_api-0.9.986/edupage_api/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,25 +227,24 @@
         Args:
             date_time (datetime.datetime): The (date)time you want to get this information for.
 
         Returns:
             RingingTime: The type (break or lesson) and time of the next ringing.
         """
         return RingingTimes(self).get_next_ringing_time(date_time)
-    
+
     @classmethod
-    def from_session_id(cls, sessiond_id: str, subdomain: str):
+    def from_session_id(cls, session_id: str, subdomain: str):
         """Create an edupage instance with a session id and subdomain.
 
         Args:
             session_id (str): The "PHPSESSID" cookie
             subdomain (str): Subdomain of the school which `cookie` is from
-        
+
         Returns:
             Edupage: A new edupage instance
         """
         instance = cls()
 
-        Login(instance).reload_data(subdomain, sessiond_id)
+        Login(instance).reload_data(subdomain, session_id)
 
         return instance
-
```

### Comparing `edupage_api-0.9.985/edupage_api/cloud.py` & `edupage_api-0.9.986/edupage_api/cloud.py`

 * *Files identical despite different names*

### Comparing `edupage_api-0.9.985/edupage_api/dbi.py` & `edupage_api-0.9.986/edupage_api/dbi.py`

 * *Files identical despite different names*

### Comparing `edupage_api-0.9.985/edupage_api/exceptions.py` & `edupage_api-0.9.986/edupage_api/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,9 +37,10 @@
 class InvalidTeacherException(Exception):
     pass
 
 
 class RequestError(Exception):
     pass
 
+
 class InvalidLunchData(Exception):
-    pass
+    pass
```

### Comparing `edupage_api-0.9.985/edupage_api/foreign_timetables.py` & `edupage_api-0.9.986/edupage_api/foreign_timetables.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
             raise MissingDataException("The server returned an incorrect response.")
 
         if timetable_data_error is not None:
             raise RequestError(f"Edupage returned an error response: {timetable_data_error}")
 
         return timetable_data_response.get("ttitems")
 
-    @ ModuleHelper.logged_in
+    @ModuleHelper.logged_in
     def get_timetable_for_person(self, id: int, date: datetime) -> List[LessonSkeleton]:
         all_teachers = People(self.edupage).get_teachers()
         students = People(self.edupage).get_students()
 
         def teacher_by_id(id: int):
             filtered = list(filter(lambda x: x.person_id == id, all_teachers))
             if not filtered:
```

### Comparing `edupage_api-0.9.985/edupage_api/grades.py` & `edupage_api-0.9.986/edupage_api/grades.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import json
 from dataclasses import dataclass
 from datetime import datetime
-from typing import Optional
+from typing import Optional, Union
 
 from edupage_api.dbi import DbiHelper
 from edupage_api.exceptions import FailedToParseGradeDataError
 from edupage_api.module import Module, ModuleHelper
 from edupage_api.people import EduTeacher
 
 
 @dataclass
 class EduGrade:
     event_id: int
     title: str
-    grade_n: Optional[int]
+    grade_n: Optional[Union[int, float, str]]
     comment: Optional[str]
     date: datetime
     subject_id: int
     subject_name: Optional[str]
     teacher: Optional[EduTeacher]
     max_points: Optional[float]
     importance: float
@@ -58,22 +58,14 @@
 
             event_id = int(event_id_str)
 
             # Title
             details = grade_details.get(event_id_str)
             title = details.get("p_meno")
 
-            # Grade
-            grade_raw = grade.get("data").split(" (", 1)
-            grade_n = float(grade_raw[0])
-            try:
-                comment = grade_raw[1].rsplit(")", 1)[0]
-            except IndexError:
-                comment = None
-
             # Date
             date_str = grade.get("datum")
             date = datetime.strptime(date_str, "%Y-%m-%d %H:%M:%S")
 
             # Subject ID and name
             subject_id_str = details.get("PredmetID")
             if subject_id_str is None or subject_id_str == "vsetky":
@@ -86,15 +78,18 @@
             teacher_id_str = details.get("UcitelID")
             if teacher_id_str is None:
                 teacher = None
             else:
                 teacher_id = int(teacher_id_str)
                 teacher_data = DbiHelper(self.edupage).fetch_teacher_data(teacher_id)
 
-                teacher = EduTeacher.parse(teacher_data, teacher_id, self.edupage)
+                if teacher_data is None:
+                    teacher = None
+                else:
+                    teacher = EduTeacher.parse(teacher_data, teacher_id, self.edupage)
 
             # Maximal points and importance
             grade_type = details.get("p_typ_udalosti")
             if grade_type == "1":
                 # Normal grade (1 – 5)
                 max_points = None
                 importance = float(details.get("p_vaha")) / 20
@@ -103,14 +98,26 @@
                 max_points = int(details.get("p_vaha"))
                 importance = None
             elif grade_type == "3":
                 # Percental grade (0 – 100 %)
                 max_points = int(details.get("p_vaha_body"))
                 importance = float(details.get("p_vaha")) / 20
 
+             # Grade
+            grade_raw = grade.get("data").split(" (", 1)
+            if grade_raw[0].isdigit():
+                grade_n = float(grade_raw[0])
+            else:
+                grade_n = grade_raw[0]
+
+            try:
+                comment = grade_raw[1].rsplit(")", 1)[0]
+            except IndexError:
+                comment = None
+
             # Verbal and percents
             try:
                 verbal = False
 
                 if max_points:
                     percent = round(float(grade_n) / float(max_points) * 100, 2)
                 elif max_points == 0:
```

### Comparing `edupage_api-0.9.985/edupage_api/login.py` & `edupage_api-0.9.986/edupage_api/login.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,9 @@
 import json
-from typing import Union
-
-from requests import JSONDecodeError
+from json import JSONDecodeError
 
 from edupage_api.exceptions import BadCredentialsException
 from edupage_api.module import Module
 
 
 class Login(Module):
     def __parse_login_data(self, data):
@@ -76,18 +74,18 @@
         response = self.edupage.session.post(request_url, parameters)
 
         if "bad=1" in response.url:
             raise BadCredentialsException()
 
         self.__parse_login_data(response.content.decode())
         self.edupage.subdomain = subdomain
-    
+
     def reload_data(self, subdomain: str, session_id: str):
         request_url = f"https://{subdomain}.edupage.org/user"
-        
+
         self.edupage.session.cookies.set("PHPSESSID", session_id)
 
         response = self.edupage.session.get(request_url)
 
         try:
             self.__parse_login_data(response.content.decode())
             self.edupage.subdomain = subdomain
```

### Comparing `edupage_api-0.9.985/edupage_api/lunches.py` & `edupage_api-0.9.986/edupage_api/lunches.py`

 * *Files 0% similar despite different names*

```diff
@@ -111,15 +111,14 @@
         lunches_data = lunch_data.get(self.edupage.subdomain)
 
         try:
             boarder_id = lunches_data.get("novyListok").get("addInfo").get("stravnikid")
         except AttributeError as e:
             raise InvalidLunchData(f"Missing boarder id: {e}")
 
-
         lunch = lunches_data.get("novyListok").get(date.strftime("%Y-%m-%d"))
 
         if lunch is None:
             return None
 
         lunch = lunch.get("2")
```

### Comparing `edupage_api-0.9.985/edupage_api/messages.py` & `edupage_api-0.9.986/edupage_api/messages.py`

 * *Files identical despite different names*

### Comparing `edupage_api-0.9.985/edupage_api/module.py` & `edupage_api-0.9.986/edupage_api/module.py`

 * *Files identical despite different names*

### Comparing `edupage_api-0.9.985/edupage_api/people.py` & `edupage_api-0.9.986/edupage_api/people.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         super().__init__(person_id, name, gender, in_school_since, EduAccountType.STUDENT)
 
         self.class_id = class_id
         self.number_in_class = number_in_class
 
 
 @dataclass
-class EduStudentSkeleton():
+class EduStudentSkeleton:
     person_id: int
     name_short: str
     class_id: int
 
 
 @dataclass
 class EduParent(EduAccount):
@@ -156,15 +156,15 @@
 
         response = self.edupage.session.post(request_url, json=data).content.decode()
         students = json.loads(response).get("r").get("tables")[0].get("data_rows")
 
         result = []
         for student in students:
             student_id = int(student["id"])
-            student_class_id = int(student["classid"])
+            student_class_id = int(student["classid"]) if student["classid"] else None
             student_name_short = student["short"]
 
             student = EduStudentSkeleton(student_id, student_name_short, student_class_id)
             result.append(student)
 
         return result
```

### Comparing `edupage_api-0.9.985/edupage_api/ringing.py` & `edupage_api-0.9.986/edupage_api/ringing.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,25 @@
     def get_next_ringing_time(self, date_time: datetime) -> RingingTime:
         date_time = RingingTimes.__get_next_workday(date_time)
 
         ringing_times = self.edupage.data.get("zvonenia")
         for ringing_time in ringing_times:
             start_time = RingingTimes.__parse_time(ringing_time.get("starttime"))
             if date_time.time() < start_time:
-                date_time = RingingTimes.__set_hours_and_minutes(date_time, start_time.hour, start_time.minute)
+                date_time = RingingTimes.__set_hours_and_minutes(
+                    date_time, start_time.hour, start_time.minute
+                )
 
                 return RingingTime(RingingType.LESSON, date_time)
 
             end_time = RingingTimes.__parse_time(ringing_time.get("endtime"))
             if date_time.time() < end_time:
-                date_time = RingingTimes.__set_hours_and_minutes(date_time, end_time.hour, end_time.minute)
+                date_time = RingingTimes.__set_hours_and_minutes(
+                    date_time, end_time.hour, end_time.minute
+                )
 
                 return RingingTime(RingingType.BREAK, date_time)
 
         date_time += timedelta(1)
         date_time = RingingTimes.__set_hours_and_minutes(date_time, 0, 0)
 
         return self.get_next_ringing_time(date_time)
```

### Comparing `edupage_api-0.9.985/edupage_api/substitution.py` & `edupage_api-0.9.986/edupage_api/substitution.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,16 +3,15 @@
 
 import json
 from dataclasses import dataclass
 from datetime import date
 from enum import Enum
 from typing import Optional, Union
 
-from edupage_api.exceptions import (ExpiredSessionException,
-                                    InvalidTeacherException)
+from edupage_api.exceptions import ExpiredSessionException, InvalidTeacherException
 from edupage_api.module import Module, ModuleHelper
 from edupage_api.people import EduTeacher, People
 
 
 class Action(str, Enum):
     ADDITION = "add"
     CHANGE = "change"
```

### Comparing `edupage_api-0.9.985/edupage_api/timeline.py` & `edupage_api-0.9.986/edupage_api/timeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
     CONFIRMATION = "confirmation"
     CONTEST = "contest"
 
     # Photo album
     ALBUM = "album"
 
     # Other
+    BEE = "vcelicka"
     OTHER = "other"
 
     # Helper
     H_ATTENDANCE = "h_attendance"
     H_BEE = "h_vcelicka"
     H_CLEARCACHE = "h_clearcache"
     H_CLEARDBI = "h_cleardbi"
@@ -126,14 +127,15 @@
     H_GRADES = "h_znamky"
     H_HOMEWORK = "h_homework"
     H_PROCESS = "h_process"
     H_PROCESSTYPES = "h_processtypes"
     H_SETTINGS = "h_settings"
     H_SUBSTITUTION = "h_substitution"
     H_TIMETABLE = "h_timetable"
+    H_USERPHOTO = "h_userphoto"
 
     @staticmethod
     def parse(event_type_str: str) -> Optional[EventType]:
         return ModuleHelper.parse_enum(event_type_str, EventType)
 
 
 @dataclass
```

### Comparing `edupage_api-0.9.985/edupage_api/timetables.py` & `edupage_api-0.9.986/edupage_api/timetables.py`

 * *Files 10% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 
         lessons = []
         for subject in plan:
             header = subject.get("header")
             if len(header) == 0:
                 continue
 
-            subject_id = int(subject.get("subjectid"))
+            subject_id = int(subject.get("subjectid")) if subject.get("subjectid") else None
             if subject_id:
                 subject_name = DbiHelper(self.edupage).fetch_subject_name(subject_id)
             else:
                 subject_name = header[0].get("text")
 
             teachers = []
             teacher_ids = subject.get("teacherids")
@@ -145,16 +145,27 @@
                     classrooms.append(classroom_number)
 
             start_of_lesson_str = subject.get("starttime")
             end_of_lesson_str = subject.get("endtime")
 
             ModuleHelper.assert_none(start_of_lesson_str, end_of_lesson_str)
 
-            start_of_lesson = datetime.strptime(start_of_lesson_str, "%H:%M")
-            end_of_lesson = datetime.strptime(end_of_lesson_str, "%H:%M")
+            now = datetime.now()
+
+            try:
+                start_of_lesson = datetime.strptime(start_of_lesson_str, "%H:%M")
+            except ValueError:
+                start_of_lesson = datetime(hour=0, minute=0, day=now.day,
+                                           month=now.month, year=now.year)
+
+            try:
+                end_of_lesson = datetime.strptime(end_of_lesson_str, "%H:%M")
+            except ValueError:
+                end_of_lesson = datetime(hour=0, minute=0, day=now.day,
+                                         month=now.month, year=now.year)
 
             online_lesson_link = subject.get("ol_url")
 
             lesson = Lesson(teachers, classrooms, start_of_lesson, end_of_lesson,
                             online_lesson_link, subject_id, subject_name)
             lessons.append(lesson)
```

### Comparing `edupage_api-0.9.985/edupage_api/utils.py` & `edupage_api-0.9.986/edupage_api/utils.py`

 * *Files identical despite different names*

### Comparing `edupage_api-0.9.985/edupage_api.egg-info/PKG-INFO` & `edupage_api-0.9.986/edupage_api.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: edupage-api
-Version: 0.9.985
+Version: 0.9.986
 Summary: A python library for accessing your Edupage account
 Home-page: https://github.com/ivanhrabcak/edupage-api
 Author: ivanhrabcak
 Author-email: ivan@hrabcak.eu
-License: UNKNOWN
 Keywords: edupage,edupage api,library
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.9
@@ -54,9 +52,7 @@
 The docs are available [here](https://yesdaddyfuck.me/edupage-api/)
 
 # I have a problem or an idea!
 
 - If you find any issue with this code, or it doesn't work please, let us know by opening an [issue](https://github.com/ivanhrabcak/edupage-api/issues/new/choose)!
 - Feel free to suggest any other features! Just open an [issue with the _Feature Request_ tag](https://github.com/ivanhrabcak/edupage-api/issues/new?labels=feature+request&template=feature_request.md&title=%5BFeature+request%5D+).
 - If you, even better, have fixed the issue, added a new feature, or made something work better, please, open a [pull request](https://github.com/ivanhrabcak/edupage-api/compare)!
-
-
```

### Comparing `edupage_api-0.9.985/edupage_api.egg-info/SOURCES.txt` & `edupage_api-0.9.986/edupage_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edupage_api-0.9.985/setup.cfg` & `edupage_api-0.9.986/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = edupage_api
-version = 0.9.985
+version = 0.9.986
 description = A python library for accessing your Edupage account
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = ivanhrabcak
 author_email = ivan@hrabcak.eu
 keywords = edupage, edupage api, library
 url = https://github.com/ivanhrabcak/edupage-api
```

