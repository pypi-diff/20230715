# Comparing `tmp/studydrive-0.3.1.tar.gz` & `tmp/studydrive-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "studydrive-0.3.1.tar", last modified: Wed Aug 24 06:24:18 2022, max compression
+gzip compressed data, was "studydrive-0.3.2.tar", last modified: Sat Jul 15 12:56:13 2023, max compression
```

## Comparing `studydrive-0.3.1.tar` & `studydrive-0.3.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2022-08-24 06:24:18.211501 studydrive-0.3.1/
--rw-rw-r--   0 henry     (1000) henry     (1000)    35149 2022-06-01 13:33:11.000000 studydrive-0.3.1/LICENSE
--rw-rw-r--   0 henry     (1000) henry     (1000)    13776 2022-08-24 06:24:18.211501 studydrive-0.3.1/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)    13494 2022-08-24 06:22:09.000000 studydrive-0.3.1/README.md
--rw-rw-r--   0 henry     (1000) henry     (1000)       38 2022-08-24 06:24:18.211501 studydrive-0.3.1/setup.cfg
--rw-rw-r--   0 henry     (1000) henry     (1000)      874 2022-08-24 06:23:59.000000 studydrive-0.3.1/setup.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2022-08-24 06:24:18.207500 studydrive-0.3.1/studydrive/
--rw-rw-r--   0 henry     (1000) henry     (1000)       63 2022-06-01 13:33:11.000000 studydrive-0.3.1/studydrive/__init__.py
--rw-rw-r--   0 henry     (1000) henry     (1000)    18586 2022-08-24 06:20:13.000000 studydrive-0.3.1/studydrive/studydriveapi.py
-drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2022-08-24 06:24:18.211501 studydrive-0.3.1/studydrive.egg-info/
--rw-rw-r--   0 henry     (1000) henry     (1000)    13776 2022-08-24 06:24:18.000000 studydrive-0.3.1/studydrive.egg-info/PKG-INFO
--rw-rw-r--   0 henry     (1000) henry     (1000)      246 2022-08-24 06:24:18.000000 studydrive-0.3.1/studydrive.egg-info/SOURCES.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)        1 2022-08-24 06:24:18.000000 studydrive-0.3.1/studydrive.egg-info/dependency_links.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       18 2022-08-24 06:24:18.000000 studydrive-0.3.1/studydrive.egg-info/requires.txt
--rw-rw-r--   0 henry     (1000) henry     (1000)       11 2022-08-24 06:24:18.000000 studydrive-0.3.1/studydrive.egg-info/top_level.txt
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-07-15 12:56:13.401124 studydrive-0.3.2/
+-rw-r--r--   0 henry     (1000) henry     (1000)    35149 2023-01-29 16:40:04.000000 studydrive-0.3.2/LICENSE
+-rw-rw-r--   0 henry     (1000) henry     (1000)    13812 2023-07-15 12:56:13.401124 studydrive-0.3.2/PKG-INFO
+-rw-r--r--   0 henry     (1000) henry     (1000)    13494 2023-01-29 16:40:04.000000 studydrive-0.3.2/README.md
+-rw-rw-r--   0 henry     (1000) henry     (1000)       38 2023-07-15 12:56:13.401124 studydrive-0.3.2/setup.cfg
+-rw-r--r--   0 henry     (1000) henry     (1000)      874 2023-07-15 12:55:42.000000 studydrive-0.3.2/setup.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-07-15 12:56:13.401124 studydrive-0.3.2/studydrive/
+-rw-r--r--   0 henry     (1000) henry     (1000)       63 2023-01-29 16:40:04.000000 studydrive-0.3.2/studydrive/__init__.py
+-rw-r--r--   0 henry     (1000) henry     (1000)    19110 2023-04-18 15:37:57.000000 studydrive-0.3.2/studydrive/studydriveapi.py
+drwxrwxr-x   0 henry     (1000) henry     (1000)        0 2023-07-15 12:56:13.401124 studydrive-0.3.2/studydrive.egg-info/
+-rw-rw-r--   0 henry     (1000) henry     (1000)    13812 2023-07-15 12:56:13.000000 studydrive-0.3.2/studydrive.egg-info/PKG-INFO
+-rw-rw-r--   0 henry     (1000) henry     (1000)      246 2023-07-15 12:56:13.000000 studydrive-0.3.2/studydrive.egg-info/SOURCES.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)        1 2023-07-15 12:56:13.000000 studydrive-0.3.2/studydrive.egg-info/dependency_links.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       18 2023-07-15 12:56:13.000000 studydrive-0.3.2/studydrive.egg-info/requires.txt
+-rw-rw-r--   0 henry     (1000) henry     (1000)       11 2023-07-15 12:56:13.000000 studydrive-0.3.2/studydrive.egg-info/top_level.txt
```

### Comparing `studydrive-0.3.1/LICENSE` & `studydrive-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `studydrive-0.3.1/PKG-INFO` & `studydrive-0.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: studydrive
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Wrapper for the (unofficial) Studydrive API
 Home-page: https://github.com/henrydatei/studydrive-api
 Author: Henry Haustein
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # studydrive-api
 A Python Wrapper for the (unofficial) Studydrive API
 
@@ -527,7 +529,8 @@
    },
    "verification_popup":"None",
    "positions":[
       
    ]
 }
 ```
+
```

### Comparing `studydrive-0.3.1/README.md` & `studydrive-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `studydrive-0.3.1/setup.py` & `studydrive-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 HERE = pathlib.Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name = "studydrive",                     # This is the name of the package
-    version = "0.3.1",                        # The initial release version
+    version = "0.3.2",                        # The initial release version
     author = "Henry Haustein",                     # Full name of the author
     description = "A Python Wrapper for the (unofficial) Studydrive API",
     packages = setuptools.find_packages(),    # List of all python modules to be installed
     python_requires = '>=3.6',                # Minimum version requirement of the package
     install_requires=["requests", "datetime"],
     url = "https://github.com/henrydatei/studydrive-api",
     long_description=README,
```

### Comparing `studydrive-0.3.1/studydrive/studydriveapi.py` & `studydrive-0.3.2/studydrive/studydriveapi.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 from datetime import datetime
 import re
 import json
 import hashlib
 
 class StudydriveAPI:
-    baseurl = "https://api.studydrive.net/"
+    baseurl = "https://gateway.production-01.studydrive.net"
     token = ""
 
     def __init__(self, token = ""):
         self.token = token
 
     def login(self, user, passwd):
         params = {"client_id": 8,
@@ -21,81 +21,81 @@
         req = requests.post('{}oauth/token'.format(self.baseurl), data = params)
         req.raise_for_status()
         self.token = req.json()['access_token']
         return req.json()
 
     def getUniversityCourses(self, universityID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/universities/{}/courses'.format(self.baseurl, universityID), headers = headers)
+        req = requests.get('{}/legacy-api/v1/universities/{}/courses'.format(self.baseurl, universityID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def register(self, email, password):
         params = {"client_id": 8, 
             "client_secret": "7ixMuuCHm8vmMQcHCT3AMc3uMPUhMIBeOmw67QXB", 
             "first_name": "", 
             "last_name": "", 
             "locale": "DE", 
             "password": password, 
             "username": email}
-        req = requests.post('{}api/app/v1/users/register/email'.format(self.baseurl), params = params)
+        req = requests.post('{}/legacy-api/v1/users/register/email'.format(self.baseurl), params = params)
         req.raise_for_status()
         self.token = req.json()["access_token"]
         return req.json()
 
     def setNickname(self, nickname):
         headers = {"authorization": "Bearer " + self.token}
         params = {"is_edit": 0, "nickname": nickname}
-        req = requests.post('{}api/app/v1/users/nickname'.format(self.baseurl), headers = headers, params = params)
+        req = requests.post('{}/legacy-api/v1/users/nickname'.format(self.baseurl), headers = headers, params = params)
         req.raise_for_status()
         return req.json()
 
     def setProgram(self, universityID, programID, semesterID):
         headers = {"authorization": "Bearer " + self.token}
         params = {"university_ids[]": universityID}
-        requests.post('{}api/app/v1/universities/subscribe'.format(self.baseurl), params = params, headers = headers)
+        requests.post('{}/legacy-api/v1/universities/subscribe'.format(self.baseurl), params = params, headers = headers)
         params = {"degree_program_ids[]": programID}
-        requests.post('{}api/app/v1/universities/{}/degree_program/subscribe'.format(self.baseurl, universityID), params = params, headers = headers)
+        requests.post('{}/legacy-api/v1/universities/{}/degree_program/subscribe'.format(self.baseurl, universityID), params = params, headers = headers)
         params = {"semester_id": semesterID, "university_id": universityID}
-        requests.post('{}api/app/v1/semester'.format(self.baseurl), params = params, headers = headers)
+        requests.post('{}/legacy-api/v1/semester'.format(self.baseurl), params = params, headers = headers)
 
     def getUniversities(self):
         headers = {"authorization": "Bearer " + self.token}
         params = {"popularity_order_id": 1}
-        req = requests.get('{}api/app/v1/universities'.format(self.baseurl), headers = headers, params = params)
+        req = requests.get('{}/legacy-api/v1/universities'.format(self.baseurl), headers = headers, params = params)
         req.raise_for_status()
         return req.json()
 
     def getSemester(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/semester'.format(self.baseurl), headers = headers)
+        req = requests.get('{}/legacy-api/v1/semester'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getMyself(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/myself'.format(self.baseurl), headers = headers)
+        req = requests.get('{}/legacy-api/v1/myself'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def followUser(self, userID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/profiles/{}/follow'.format(self.baseurl, userID), headers = headers)
+        req = requests.post('{}/legacy-api/v1/profiles/{}/follow'.format(self.baseurl, userID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def saveDocument(self, docID, filename): # from https://stackoverflow.com/questions/56950987/download-file-from-url-and-save-it-in-a-folder-python
         # calculate download-token -> extracted method from decompiled studydrive app
         # https://www.geeksforgeeks.org/md5-hash-python/
         str2hash = "studydrive-app-download-7>%jsc" + str(docID)
         result = hashlib.md5(str2hash.encode())
 
         headers = {"authorization": "Bearer " + self.token}
         params = {"converted_file": "false", "download-token": result.hexdigest(), "preview": "false"}
-        req = requests.get('{}api/app/v1/documents/{}/download'.format(self.baseurl, docID), headers = headers, stream = True, params = params)
+        req = requests.get('{}/legacy-api/v1/documents/{}/download'.format(self.baseurl, docID), headers = headers, stream = True, params = params)
 
         if req.ok:
             if not os.path.exists(filename):
                 with open(filename, "wb") as f:
                     for chunk in req.iter_content(chunk_size = 1024 * 8):
                         if chunk:
                             f.write(chunk)
@@ -106,18 +106,19 @@
         else:  # HTTP status code 4XX/5XX
             print("Download failed: status code {}\n{}".format(req.status_code, req.text))
 
     # type 60 = Klausuren
     # type 30 = Übungen & Tutorien
     # type 80 = Zusammenfassungen
     # type 10 = Andere
+    # type 20 = Vorlesungen
     def uploadDocument(self, filename, name, description, professor, courseID, semesterID, type, anonymous = 1, selfMade = 0):
         # get upload hash
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/documents/upload/init'.format(self.baseurl), headers = headers)
+        req = requests.post('{}/legacy-api/v1/documents/upload/init'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         hash = req.json()["upload_hash"]
 
         # upload
         file = open(filename, "rb")
         parameters = {'name': name, 
             'description': description, 
@@ -125,122 +126,122 @@
             'course_id': courseID, 
             'semester_id': semesterID, 
             'type': type, 
             'anonymous': anonymous, 
             'self_made': selfMade, 
             'upload_hash': hash}
         files = {'file': file}
-        req = requests.post('{}api/app/v1/documents/upload'.format(self.baseurl), headers = headers, data = parameters, files = files)
+        req = requests.post('{}/legacy-api/v1/documents/upload'.format(self.baseurl), headers = headers, data = parameters, files = files)
         # print(req.json())
 
         # finalize
         parameters = {'upload_hash': hash}
-        req = requests.post('{}api/app/v1/documents/upload/{}/finalize'.format(self.baseurl, hash), headers = headers, params = parameters)
+        req = requests.post('{}/legacy-api/v1/documents/upload/{}/finalize'.format(self.baseurl, hash), headers = headers, params = parameters)
         return req.json()
 
     def getProfileDocuments(self, profileID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/profiles/{}/documents'.format(self.baseurl, profileID), headers = headers)
+        req = requests.get('{}/legacy-api/v1/profiles/{}/documents'.format(self.baseurl, profileID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getProfileFlashcards(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/feed/my_flashcard_sets'.format(self.baseurl), headers = headers)
+        req = requests.get('{}/legacy-api/v1/feed/my_flashcard_sets'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getDocumentDetails(self, docID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/documents/{}/details'.format(self.baseurl, docID), headers = headers)
+        req = requests.get('{}/legacy-api/v1/documents/{}/details'.format(self.baseurl, docID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getMyDocuments(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/feed/my_documents'.format(self.baseurl), headers = headers)
+        req = requests.get('{}/legacy-api/v1/feed/my_documents'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getMyAnswers(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/feed/my_answers_feed'.format(self.baseurl), headers = headers)
+        req = requests.get('{}/legacy-api/v1/feed/my_answers_feed'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getMyStats(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/users/right_sidebar_stats'.format(self.baseurl), headers = headers)
+        req = requests.get('{}/legacy-api/v1/users/right_sidebar_stats'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getInformationAboutQuestion(self, questionType, questionID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/{}/questions/{}'.format(self.baseurl, questionType, questionID), headers = headers)
+        req = requests.get('{}/legacy-api/v1/{}/questions/{}'.format(self.baseurl, questionType, questionID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getCourseDetails(self, courseID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/courses/{}/details'.format(self.baseurl, courseID), headers = headers)
+        req = requests.get('{}/legacy-api/v1/courses/{}/details'.format(self.baseurl, courseID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getMyQuestions(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/feed/my_questions_feed'.format(self.baseurl), headers = headers)
+        req = requests.get('{}/legacy-api/v1/feed/my_questions_feed'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def upvoteAnswer(self, answerType, answerID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/{}/answers/{}/upvote'.format(self.baseurl, answerType, answerID), headers = headers)
+        req = requests.post('{}/legacy-api/v1/{}/answers/{}/upvote'.format(self.baseurl, answerType, answerID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def upvoteQuestion(self, questionType, questionID):
         headers = {"authorization": "Bearer " + self.token}
         params = {'question_id': questionID, 'question_type': questionType}
-        req = requests.post('{}api/app/v1/questions/upvote'.format(self.baseurl), headers=headers, data = params)
+        req = requests.post('{}/legacy-api/v1/questions/upvote'.format(self.baseurl), headers=headers, data = params)
         req.raise_for_status()
         return req.json()
 
     def upvoteDocument(self, fileID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/documents/{}/upvote'.format(self.baseurl, fileID), headers = headers)
+        req = requests.post('{}/legacy-api/v1/documents/{}/upvote'.format(self.baseurl, fileID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def upvoteFlashcard(self, flashcardID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/flashcards/sets/{}/vote/up'.format(self.baseurl, flashcardID), headers = headers)
+        req = requests.post('{}/legacy-api/v1/flashcards/sets/{}/vote/up'.format(self.baseurl, flashcardID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def startFlashcard(self, flashcardID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/flashcards/sets/{}/study/start'.format(self.baseurl, flashcardID), headers = headers)
+        req = requests.post('{}/legacy-api/v1/flashcards/sets/{}/study/start'.format(self.baseurl, flashcardID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def finishFlashcard(self, flashcardID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/flashcards/sets/{}/study/finish'.format(self.baseurl, flashcardID), headers = headers)
+        req = requests.post('{}/legacy-api/v1/flashcards/sets/{}/study/finish'.format(self.baseurl, flashcardID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getLeftSidebar(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/users/left_sidebar'.format(self.baseurl), headers = headers)
+        req = requests.get('{}/legacy-api/v1/users/left_sidebar'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def setCourseOrder(self, courses):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/community/order'.format(self.baseurl), headers = headers, data = {'context':'course', 'ids[]': courses})
+        req = requests.post('{}/legacy-api/v1/community/order'.format(self.baseurl), headers = headers, data = {'context':'course', 'ids[]': courses})
         req.raise_for_status()
         return req.json()
 
     def sortCourses(self):
         list = []
         ids = []
         courses = self.getMyCourses()
@@ -252,122 +253,122 @@
         for courseData in sortedList:
             id = courseData[0]
             ids.append(id)
         return self.setCourseOrder(ids[::-1])
 
     def joinCourse(self, courseID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/courses/{}/join'.format(self.baseurl, courseID), headers = headers)
+        req = requests.post('{}/legacy-api/v1/courses/{}/join'.format(self.baseurl, courseID), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getMyCourses(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/myself/courses'.format(self.baseurl), headers = headers)
+        req = requests.get('{}/legacy-api/v1/myself/courses'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getMajors(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}/api/app/v1/users/majors'.format(self.baseurl), headers = headers)
+        req = requests.get('{}//legacy-api/v1/users/majors'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getAllMajors(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}/api/app/v1/majors'.format(self.baseurl), headers = headers)
+        req = requests.get('{}//legacy-api/v1/majors'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def giveKarma(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}/api/app/v1/users/give-karma'.format(self.baseurl), headers = headers)
+        req = requests.post('{}//legacy-api/v1/users/give-karma'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def courseExpertDashboard(self):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}/api/app/v1/ke/dashboard'.format(self.baseurl), headers = headers)
+        req = requests.get('{}//legacy-api/v1/ke/dashboard'.format(self.baseurl), headers = headers)
         req.raise_for_status()
         return req.json()
 
     def getFileListofCourse(self, courseID):
         liste = []
         page = 0
         hasMore = True
         headers = {"authorization": "Bearer " + self.token}
         while hasMore:
             parameters = {"sort": "time", "page": page, "semester_from": 0, "semester_until": 0, "type_ids": 0}
             if page > 0:
                 parameters["reference_time"] = datetime.now().strftime('%Y-%m-%d %H:%M:%S')
-            req = requests.get('{}api/app/v1/feed/courses/{}/documents'.format(self.baseurl, courseID), headers = headers, params = parameters)
+            req = requests.get('{}/legacy-api/v1/feed/courses/{}/documents'.format(self.baseurl, courseID), headers = headers, params = parameters)
             req.raise_for_status()
             daten = req.json()
             liste.extend(daten["files"])
             hasMore = daten["has_more"]
             page = page + 1
         return liste
 
     def createCourseQuestion(self, text, courseID):
         headers = {"authorization": "Bearer " + self.token}
         params = {"course_id": courseID, "file_id": courseID, "group_id": courseID, "question_type": "course"}
-        req = requests.post('{}api/app/v1/course/questions/init'.format(self.baseurl), headers = headers, params = params)
+        req = requests.post('{}/legacy-api/v1/course/questions/init'.format(self.baseurl), headers = headers, params = params)
         req.raise_for_status()
         questionID = req.json()["question_id"]
 
         params2 = {"is_anonymous": "true", "multi_vote": "false", "question_id": questionID, "question_type": "course", "text": text}
-        req = requests.post('{}api/app/v1/course/questions/{}/create'.format(self.baseurl, questionID), headers = headers, params = params2)
+        req = requests.post('{}/legacy-api/v1/course/questions/{}/create'.format(self.baseurl, questionID), headers = headers, params = params2)
         req.raise_for_status()
         return req.json()
 
     def createGroupQuestion(self, text, groupID):
         headers = {"authorization": "Bearer " + self.token}
         params = {"course_id": groupID, "file_id": groupID, "group_id": groupID, "question_type": "group"}
-        req = requests.post('{}api/app/v1/group/questions/init'.format(self.baseurl), headers = headers, params = params)
+        req = requests.post('{}/legacy-api/v1/group/questions/init'.format(self.baseurl), headers = headers, params = params)
         req.raise_for_status()
         questionID = req.json()["question_id"]
 
         params2 = {"is_anonymous": "true", "multi_vote": "false", "question_id": questionID, "question_type": "group", "text": text}
-        req = requests.post('{}api/app/v1/group/questions/{}/create'.format(self.baseurl, questionID), headers = headers, params = params2)
+        req = requests.post('{}/legacy-api/v1/group/questions/{}/create'.format(self.baseurl, questionID), headers = headers, params = params2)
         req.raise_for_status()
         return req.json()
 
     def createAnswerForCourseQuestion(self, text, questionID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/course/questions/{}/answers/init'.format(self.baseurl, questionID), headers = headers)
+        req = requests.post('{}/legacy-api/v1/course/questions/{}/answers/init'.format(self.baseurl, questionID), headers = headers)
         req.raise_for_status()
         answerID = req.json()["answer_id"]
 
         params2 = {"is_anonymous": "true", "text": text}
-        req = requests.post('{}api/app/v1/course/answers/{}/create'.format(self.baseurl, answerID), headers = headers, params = params2)
+        req = requests.post('{}/legacy-api/v1/course/answers/{}/create'.format(self.baseurl, answerID), headers = headers, params = params2)
         req.raise_for_status()
         return req.json()
 
     def createAnswerForGroupQuestion(self, text, questionID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.post('{}api/app/v1/group/questions/{}/answers/init'.format(self.baseurl, questionID), headers = headers)
+        req = requests.post('{}/legacy-api/v1/group/questions/{}/answers/init'.format(self.baseurl, questionID), headers = headers)
         req.raise_for_status()
         answerID = req.json()["answer_id"]
 
         params2 = {"is_anonymous": "true", "text": text}
-        req = requests.post('{}api/app/v1/group/answers/{}/create'.format(self.baseurl, answerID), headers = headers, params = params2)
+        req = requests.post('{}/legacy-api/v1/group/answers/{}/create'.format(self.baseurl, answerID), headers = headers, params = params2)
         req.raise_for_status()
         return req.text
 
     def setBestAnswer(self, questionID, answerID):
         headers = {"authorization": "Bearer " + self.token}
         params = {'answer_id': answerID}
-        req = requests.post('{}api/app/v1/course/questions/{}/best_answer'.format(self.baseurl, questionID), headers = headers, data = params)
+        req = requests.post('{}/legacy-api/v1/course/questions/{}/best_answer'.format(self.baseurl, questionID), headers = headers, data = params)
         req.raise_for_status()
         return req.json()
 
     def switchNotification(self, id, notificationType):
         headers = {"authorization": "Bearer " + self.token}
         params = {"id": id, "notification_type": notificationType}
-        req = requests.post('{}api/app/v1/users/settings'.format(self.baseurl), headers = headers, data = params)
+        req = requests.post('{}/legacy-api/v1/users/settings'.format(self.baseurl), headers = headers, data = params)
         req.raise_for_status()
         return req.json()
 
     def switchPushNotification(self):
         ids = [8, 10, 11, 14, 15, 28, 29, 45, 46, 44]
         for id in ids:
             self.switchNotification(id, "app")
@@ -392,16 +393,22 @@
         req = requests.get("https://www.studydrive.net/de/profile/sauron/{}#documents".format(userID))
         result = re.search('sdWindow.profile = (.*);sdWindow.isTablet', req.text)
         return json.loads(result.group(1))["credits"]
 
     def getGroupQuestions(self, groupID, pageNumber):
         headers = {"authorization": "Bearer " + self.token}
         params = {"group_id": groupID, "page": pageNumber}
-        req = requests.get('{}api/app/v1/feed/groups/{}/discussion'.format(self.baseurl, groupID), headers = headers, params = params)
+        req = requests.get('{}/legacy-api/v1/feed/groups/{}/discussion'.format(self.baseurl, groupID), headers = headers, params = params)
         req.raise_for_status()
         return req.json()
 
     def getAnswersForQuestion(self, questionID):
         headers = {"authorization": "Bearer " + self.token}
-        req = requests.get('{}api/app/v1/group/questions/{}'.format(self.baseurl, questionID), headers = headers)
+        req = requests.get('{}/legacy-api/v1/group/questions/{}'.format(self.baseurl, questionID), headers = headers)
         req.raise_for_status()
         return req.json()
+
+    def deleteDocument(self, documentID):
+        headers = {"authorization": "Bearer " + self.token}
+        req = requests.post('{}/legacy-api/v1/documents/{}/delete'.format(self.baseurl, documentID), headers = headers)
+        req.raise_for_status()
+        return req.json()
```

### Comparing `studydrive-0.3.1/studydrive.egg-info/PKG-INFO` & `studydrive-0.3.2/studydrive.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 Metadata-Version: 2.1
 Name: studydrive
-Version: 0.3.1
+Version: 0.3.2
 Summary: A Python Wrapper for the (unofficial) Studydrive API
 Home-page: https://github.com/henrydatei/studydrive-api
 Author: Henry Haustein
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # studydrive-api
 A Python Wrapper for the (unofficial) Studydrive API
 
@@ -527,7 +529,8 @@
    },
    "verification_popup":"None",
    "positions":[
       
    ]
 }
 ```
+
```

