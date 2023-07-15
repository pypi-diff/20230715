# Comparing `tmp/python-wekan-0.1.5.tar.gz` & `tmp/python-wekan-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-wekan-0.1.5.tar", last modified: Sat May 28 09:12:52 2022, max compression
+gzip compressed data, was "python-wekan-0.1.6.tar", last modified: Sat Jul 15 20:57:43 2023, max compression
```

## Comparing `python-wekan-0.1.5.tar` & `python-wekan-0.1.6.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 09:12:51.997935 python-wekan-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-05-28 09:12:35.000000 python-wekan-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     4665 2022-05-28 09:12:51.997935 python-wekan-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4269 2022-05-28 09:12:35.000000 python-wekan-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 09:12:51.997935 python-wekan-0.1.5/python_wekan.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4665 2022-05-28 09:12:51.000000 python-wekan-0.1.5/python_wekan.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      510 2022-05-28 09:12:51.000000 python-wekan-0.1.5/python_wekan.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-05-28 09:12:51.000000 python-wekan-0.1.5/python_wekan.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-05-28 09:12:51.000000 python-wekan-0.1.5/python_wekan.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-05-28 09:12:51.000000 python-wekan-0.1.5/python_wekan.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-05-28 09:12:51.997935 python-wekan-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      590 2022-05-28 09:12:35.000000 python-wekan-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 09:12:51.997935 python-wekan-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-05-28 09:12:35.000000 python-wekan-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12410 2022-05-28 09:12:35.000000 python-wekan-0.1.5/tests/test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-05-28 09:12:51.997935 python-wekan-0.1.5/wekan/
--rw-r--r--   0 runner    (1001) docker     (121)      367 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    15820 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/board.py
--rw-r--r--   0 runner    (1001) docker     (121)     9516 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/card.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/card_checklist.py
--rw-r--r--   0 runner    (1001) docker     (121)     3646 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/card_checklist_item.py
--rw-r--r--   0 runner    (1001) docker     (121)     2459 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/card_comment.py
--rw-r--r--   0 runner    (1001) docker     (121)     2762 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/customfield.py
--rw-r--r--   0 runner    (1001) docker     (121)     4651 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/integration.py
--rw-r--r--   0 runner    (1001) docker     (121)     2033 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/label.py
--rw-r--r--   0 runner    (1001) docker     (121)     2103 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/swimlane.py
--rw-r--r--   0 runner    (1001) docker     (121)     2773 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/user.py
--rw-r--r--   0 runner    (1001) docker     (121)     7035 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/wekan_client.py
--rw-r--r--   0 runner    (1001) docker     (121)     4384 2022-05-28 09:12:35.000000 python-wekan-0.1.5/wekan/wekan_list.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:57:43.397710 python-wekan-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-15 20:57:28.000000 python-wekan-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-15 20:57:43.397710 python-wekan-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-15 20:57:28.000000 python-wekan-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:57:43.393710 python-wekan-0.1.6/python_wekan.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-07-15 20:57:43.000000 python-wekan-0.1.6/python_wekan.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-15 20:57:43.000000 python-wekan-0.1.6/python_wekan.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 20:57:43.000000 python-wekan-0.1.6/python_wekan.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-15 20:57:43.000000 python-wekan-0.1.6/python_wekan.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-15 20:57:43.000000 python-wekan-0.1.6/python_wekan.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 20:57:43.397710 python-wekan-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-15 20:57:28.000000 python-wekan-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:57:43.393710 python-wekan-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 20:57:28.000000 python-wekan-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12410 2023-07-15 20:57:28.000000 python-wekan-0.1.6/tests/test_cases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 20:57:43.397710 python-wekan-0.1.6/wekan/
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15911 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/board.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9516 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/card_checklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3646 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/card_checklist_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/card_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2762 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/customfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4651 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/label.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/swimlane.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7035 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/wekan_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4511 2023-07-15 20:57:28.000000 python-wekan-0.1.6/wekan/wekan_list.py
```

### Comparing `python-wekan-0.1.5/LICENSE` & `python-wekan-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/PKG-INFO` & `python-wekan-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-wekan
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is a python client for interacting with the WeKan® REST-API
 Home-page: https://github.com/bastianwenske/python-wekan
 Download-URL: https://github.com/bastianwenske/python-wekan
 Author: Bastian Wenske
 Author-email: 
 License: BSD 3-Clause License
 Keywords: python
```

### Comparing `python-wekan-0.1.5/README.md` & `python-wekan-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/python_wekan.egg-info/PKG-INFO` & `python-wekan-0.1.6/python_wekan.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-wekan
-Version: 0.1.5
+Version: 0.1.6
 Summary: This is a python client for interacting with the WeKan® REST-API
 Home-page: https://github.com/bastianwenske/python-wekan
 Download-URL: https://github.com/bastianwenske/python-wekan
 Author: Bastian Wenske
 Author-email: 
 License: BSD 3-Clause License
 Keywords: python
```

### Comparing `python-wekan-0.1.5/setup.py` & `python-wekan-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 
 setup(
     name='python-wekan',
-    version='0.1.5',
+    version='0.1.6',
     packages=['tests', 'wekan'],
     url='https://github.com/bastianwenske/python-wekan',
     download_url='https://github.com/bastianwenske/python-wekan',
     license='BSD 3-Clause License',
     author='Bastian Wenske',
     author_email='',
     description='This is a python client for interacting with the WeKan® REST-API',
```

### Comparing `python-wekan-0.1.5/tests/test_cases.py` & `python-wekan-0.1.6/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/wekan/board.py` & `python-wekan-0.1.6/wekan/board.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,44 +25,45 @@
         self.members = self.__raw_data['members']
         self.created_at = self.client.parse_iso_date(self.__raw_data['createdAt'])
         self.modified_at = self.client.parse_iso_date(self.__raw_data['modifiedAt'])
         self.permission = self.__raw_data['permission']
         self.color = self.__raw_data['color']
         self.subtasks_default_board_id = self.__raw_data['subtasksDefaultBoardId']
         self.subtasks_default_list_id = self.__raw_data['subtasksDefaultListId']
-        self.allows_card_counterList = self.__raw_data['allowsCardCounterList']
-        self.allows_board_member_list = self.__raw_data['allowsBoardMemberList']
-        self.date_settings_default_board_id = self.__raw_data['dateSettingsDefaultBoardId']
-        self.date_settings_default_list_id = self.__raw_data['dateSettingsDefaultListId']
+        self.allows_card_counterList = self.__raw_data.get('allowsCardCounterList', None)
+        self.allows_board_member_list = self.__raw_data.get('allowsBoardMemberList', None)
+        self.date_settings_default_board_id = self.__raw_data.get('dateSettingsDefaultBoardId', None)
+        self.date_settings_default_list_id = self.__raw_data.get('dateSettingsDefaultListId', None)
         self.allow_subtasks = self.__raw_data['allowsSubtasks']
         self.allows_attachments = self.__raw_data['allowsAttachments']
         self.allows_checklists = self.__raw_data['allowsChecklists']
         self.allows_comments = self.__raw_data['allowsComments']
         self.allows_description_title = self.__raw_data['allowsDescriptionTitle']
         self.allows_description_text = self.__raw_data['allowsDescriptionText']
-        self.allows_description_text_on_minicard = self.__raw_data['allowsDescriptionTextOnMinicard']
+        self.allows_description_text_on_minicard = self.__raw_data.get('allowsDescriptionTextOnMinicard', None)
         self.allows_card_number = self.__raw_data['allowsCardNumber']
         self.allows_activities = self.__raw_data['allowsActivities']
         self.allows_labels = self.__raw_data['allowsLabels']
-        self.allows_creator = self.__raw_data['allowsCreator']
+        self.allows_creator = self.__raw_data.get('allowsCreator', None)
         self.allows_assignee = self.__raw_data['allowsAssignee']
         self.allows_members = self.__raw_data['allowsMembers']
         self.allows_requested_by = self.__raw_data['allowsRequestedBy']
-        self.allows_card_sorting_by_number = self.__raw_data['allowsCardSortingByNumber']
-        self.allows_show_lists = self.__raw_data['allowsShowLists']
+        self.allows_card_sorting_by_number = self.__raw_data.get('allowsCardSortingByNumber', None)
+        self.allows_show_lists = self.__raw_data.get('allowsShowLists', None)
         self.allows_assigned_by = self.__raw_data['allowsAssignedBy']
         self.allows_received_date = self.__raw_data['allowsReceivedDate']
         self.allows_start_date = self.__raw_data['allowsStartDate']
         self.allows_end_date = self.__raw_data['allowsEndDate']
         self.allows_due_date = self.__raw_data['allowsDueDate']
-        self.present_parent_task = self.__raw_data['presentParentTask']
+        self.present_parent_task = self.__raw_data.get('presentParentTask', None)
         self.is_overtime = self.__raw_data['isOvertime']
         self.type = self.__raw_data['type']
         self.sort = self.__raw_data['sort']
 
+
     def __repr__(self) -> str:
         return f"<Board (id: {self.id}, title: {self.title})>"
 
     @classmethod
     def from_dict(cls, client, data: dict, ) -> Board:
         """
         Creates an instance of class Customfield by using the API-Response of Customfield creation.
```

### Comparing `python-wekan-0.1.5/wekan/card.py` & `python-wekan-0.1.6/wekan/card.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/wekan/card_checklist.py` & `python-wekan-0.1.6/wekan/card_checklist.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/wekan/card_checklist_item.py` & `python-wekan-0.1.6/wekan/card_checklist_item.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/wekan/card_comment.py` & `python-wekan-0.1.6/wekan/card_comment.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/wekan/customfield.py` & `python-wekan-0.1.6/wekan/customfield.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/wekan/integration.py` & `python-wekan-0.1.6/wekan/integration.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/wekan/label.py` & `python-wekan-0.1.6/wekan/label.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/wekan/swimlane.py` & `python-wekan-0.1.6/wekan/swimlane.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         self.board = parent_board
         self.id = swimlane_id
 
         data = self.board.client.fetch_json(f'/api/boards/{self.board.id}/swimlanes/{self.id}')
         self.title = data['title']
         self.archived = data['archived']
         self.created_at = self.board.client.parse_iso_date(data['createdAt'])
-        self.updated_at = self.board.client.parse_iso_date(data['updatedAt'])
+        self.updated_at = self.board.client.parse_iso_date(data.get('updatedAt', data['createdAt']))
         self.sort = data.get('sort')
         self.color = data.get('color', '')
         self.type = data['type']
 
     def __repr__(self) -> str:
         return f"<Swimlane (id: {self.id}, title: {self.title})>"
```

### Comparing `python-wekan-0.1.5/wekan/user.py` & `python-wekan-0.1.6/wekan/user.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/wekan/wekan_client.py` & `python-wekan-0.1.6/wekan/wekan_client.py`

 * *Files identical despite different names*

### Comparing `python-wekan-0.1.5/wekan/wekan_list.py` & `python-wekan-0.1.6/wekan/wekan_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,19 @@
         self.swimlane_id = data['swimlaneId']
         self.created_at = self.board.client.parse_iso_date(data['createdAt'])
         self.updated_at = self.board.client.parse_iso_date(data['updatedAt'])
         self.sort = data['sort']
         self.wip_limit = data['wipLimit']
         self.color = data.get('color', '')
 
-        data_cc = self.board.client.fetch_json(f'/api/boards/{self.board.id}/lists/{self.id}/cards_count')
-        self.cards_count = data_cc['list_cards_count']
+        try:
+            data_cc = self.board.client.fetch_json(f'/api/boards/{self.board.id}/lists/{self.id}/cards_count')
+            self.cards_count = data_cc['list_cards_count']
+        except:
+            print("Failed getting cards_count, instance possibly too old (stable snap?)")
 
     def __repr__(self) -> str:
         return f"<List (id: {self.id}, title: {self.title})>"
 
     def __get_all_cards_on_list(self) -> list:
         """
         Get all cards by calling the API according to https://wekan.github.io/api/v6.22/#get_list
```

