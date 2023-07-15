# Comparing `tmp/nriapp-1.1.19.tar.gz` & `tmp/nriapp-1.1.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nriapp-1.1.19.tar", last modified: Tue May 23 23:27:00 2023, max compression
+gzip compressed data, was "nriapp-1.1.21.tar", last modified: Sat Jul 15 01:38:45 2023, max compression
```

## Comparing `nriapp-1.1.19.tar` & `nriapp-1.1.21.tar`

### file list

```diff
@@ -1,37 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.766621 nriapp-1.1.19/
--rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.19/LICENSE
--rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.19/MANIFEST.in
--rw-rw-rw-   0        0        0      273 2023-05-23 23:27:00.766621 nriapp-1.1.19/PKG-INFO
--rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.19/README
--rw-rw-rw-   0        0        0      344 2023-05-06 05:28:38.000000 nriapp-1.1.19/requirements.txt
--rw-rw-rw-   0        0        0       86 2023-05-23 23:27:00.766621 nriapp-1.1.19/setup.cfg
--rw-rw-rw-   0        0        0     1108 2023-05-23 23:26:42.000000 nriapp-1.1.19/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.657421 nriapp-1.1.19/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.735421 nriapp-1.1.19/src/nriapp/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/__init__.py
--rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.19/src/nriapp/changelog.txt
-drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.735421 nriapp-1.1.19/src/nriapp/config/
--rw-rw-rw-   0        0        0        2 2023-03-02 07:59:35.000000 nriapp-1.1.19/src/nriapp/config/__init__.py
--rw-rw-rw-   0        0        0       55 2023-03-02 07:59:35.000000 nriapp-1.1.19/src/nriapp/config/config.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.751021 nriapp-1.1.19/src/nriapp/core/
--rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/core/__init__.py
--rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/core/abuseipdbapi.py
--rw-rw-rw-   0        0        0    20524 2023-05-16 04:22:17.000000 nriapp-1.1.19/src/nriapp/core/dataexplorer.py
--rw-rw-rw-   0        0        0    30935 2023-05-02 03:08:50.000000 nriapp-1.1.19/src/nriapp/core/msgraphapi.py
--rw-rw-rw-   0        0        0   105457 2023-05-23 23:18:48.000000 nriapp-1.1.19/src/nriapp/core/mssentinelapi.py
--rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/core/multifactor.py
--rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/core/vtquery.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.766621 nriapp-1.1.19/src/nriapp/helper/
--rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/helper/__init__.py
--rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/helper/doc.py
--rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/helper/excel.py
--rw-rw-rw-   0        0        0     8397 2023-04-29 03:04:07.000000 nriapp-1.1.19/src/nriapp/helper/login.py
--rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/helper/pylog.py
--rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.19/src/nriapp/helper/requestheader.py
-drwxrwxrwx   0        0        0        0 2023-05-23 23:27:00.719821 nriapp-1.1.19/src/nriapp/nriapp.egg-info/
--rw-rw-rw-   0        0        0      273 2023-05-23 23:26:59.000000 nriapp-1.1.19/src/nriapp/nriapp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      989 2023-05-23 23:26:59.000000 nriapp-1.1.19/src/nriapp/nriapp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 23:26:59.000000 nriapp-1.1.19/src/nriapp/nriapp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-05-23 23:26:59.000000 nriapp-1.1.19/src/nriapp/nriapp.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-05-23 23:26:59.000000 nriapp-1.1.19/src/nriapp/nriapp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    38168 2023-05-16 13:46:09.000000 nriapp-1.1.19/src/nriapp/nriapp.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.206638 nriapp-1.1.21/
+-rw-rw-rw-   0        0        0     1084 2023-02-12 09:09:41.000000 nriapp-1.1.21/LICENSE
+-rw-rw-rw-   0        0        0       57 2023-03-02 17:29:56.000000 nriapp-1.1.21/MANIFEST.in
+-rw-rw-rw-   0        0        0      273 2023-07-15 01:38:45.206638 nriapp-1.1.21/PKG-INFO
+-rw-rw-rw-   0        0        0        7 2023-02-12 09:19:02.000000 nriapp-1.1.21/README
+-rw-rw-rw-   0        0        0      344 2023-05-06 05:28:38.000000 nriapp-1.1.21/requirements.txt
+-rw-rw-rw-   0        0        0       86 2023-07-15 01:38:45.237838 nriapp-1.1.21/setup.cfg
+-rw-rw-rw-   0        0        0     1108 2023-07-15 01:38:31.000000 nriapp-1.1.21/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:38:44.941438 nriapp-1.1.21/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.003838 nriapp-1.1.21/src/nriapp/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/__init__.py
+-rw-rw-rw-   0        0        0     3672 2023-02-02 00:29:38.000000 nriapp-1.1.21/src/nriapp/changelog.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.050638 nriapp-1.1.21/src/nriapp/config/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/config/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/config/config.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.128638 nriapp-1.1.21/src/nriapp/core/
+-rw-rw-rw-   0        0        0        0 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/core/__init__.py
+-rw-rw-rw-   0        0        0     1520 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/core/abuseipdbapi.py
+-rw-rw-rw-   0        0        0    20773 2023-06-29 05:06:20.000000 nriapp-1.1.21/src/nriapp/core/dataexplorer.py
+-rw-rw-rw-   0        0        0    30995 2023-06-21 05:47:59.000000 nriapp-1.1.21/src/nriapp/core/msgraphapi.py
+-rw-rw-rw-   0        0        0   105842 2023-06-30 05:29:02.000000 nriapp-1.1.21/src/nriapp/core/mssentinelapi.py
+-rw-rw-rw-   0        0        0     6076 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/core/multifactor.py
+-rw-rw-rw-   0        0        0      640 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/core/vtquery.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.206638 nriapp-1.1.21/src/nriapp/helper/
+-rw-rw-rw-   0        0        0        2 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/__init__.py
+-rw-rw-rw-   0        0        0     5696 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/doc.py
+-rw-rw-rw-   0        0        0      246 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/excel.py
+-rw-rw-rw-   0        0        0     8397 2023-07-12 23:43:13.000000 nriapp-1.1.21/src/nriapp/helper/login.py
+-rw-rw-rw-   0        0        0     2443 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/pylog.py
+-rw-rw-rw-   0        0        0     1247 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/requestheader.py
+-rw-rw-rw-   0        0        0    15815 2023-04-19 13:47:32.000000 nriapp-1.1.21/src/nriapp/helper/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:38:45.003838 nriapp-1.1.21/src/nriapp/nriapp.egg-info/
+-rw-rw-rw-   0        0        0      273 2023-07-15 01:38:44.000000 nriapp-1.1.21/src/nriapp/nriapp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1016 2023-07-15 01:38:44.000000 nriapp-1.1.21/src/nriapp/nriapp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 01:38:44.000000 nriapp-1.1.21/src/nriapp/nriapp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-15 01:38:44.000000 nriapp-1.1.21/src/nriapp/nriapp.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-07-15 01:38:44.000000 nriapp-1.1.21/src/nriapp/nriapp.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    38177 2023-06-12 22:38:37.000000 nriapp-1.1.21/src/nriapp/nriapp.py
```

### Comparing `nriapp-1.1.19/LICENSE` & `nriapp-1.1.21/LICENSE`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.19/setup.py` & `nriapp-1.1.21/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 #with open('requirements.txt') as f:
 #    requirements = f.read().splitlines()
 
 
 setup(
    name='nriapp',
-   version='1.1.19',
+   version='1.1.21',
    description='This is an internal tool for crawling MS 365 Defender web with NRI',
     license='MIT',
    author='Llallum Victoria',
    author_email='llallumvictoria@gmail.com',
 #   packages=find_packages('src'),
    package_dir = {'':'src/nriapp'},
```

### Comparing `nriapp-1.1.19/src/nriapp/changelog.txt` & `nriapp-1.1.21/src/nriapp/changelog.txt`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.19/src/nriapp/core/abuseipdbapi.py` & `nriapp-1.1.21/src/nriapp/core/abuseipdbapi.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.19/src/nriapp/core/dataexplorer.py` & `nriapp-1.1.21/src/nriapp/core/dataexplorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,23 +55,23 @@
     def ingest_events(self, data, database="Incidents", table="Raw"):
   
         check_changes = '''
         Raw
         | extend a = parse_json(Events)
         | distinct items= tostring(a)
         | extend a = parse_json(items)
-        | project IncidentId=toint(a.IncidentId), Status=toint(a.Status)
+        | project IncidentId=toint(a.IncidentId), Status=toint(a.Status), LastEventTime=tostring(a.LastEventTime)
         | sort by IncidentId desc 
         '''
         response = self.client_query.execute(database, check_changes)
         
         results = response.primary_results[0]
 
-        set1 = set(json.dumps({"id":x["IncidentId"], "value": x["Status"]}, sort_keys=True) for x in results) #Serialize
-        set2 = set(json.dumps({"id":x["IncidentId"], "value": x["Status"]}, sort_keys=True) for x in data)    #Serialize
+        set1 = set(json.dumps({"id":x["IncidentId"], "value": x["Status"], "lastEventTime": parser.parse(x["LastEventTime"]).replace(microsecond=0).strftime("%Y-%m-%dT%H:%M:%S")}, sort_keys=True) for x in results) #Serialize
+        set2 = set(json.dumps({"id":x["IncidentId"], "value": x["Status"], "lastEventTime": parser.parse(x["LastEventTime"]).replace(microsecond=0).strftime("%Y-%m-%dT%H:%M:%S")}, sort_keys=True) for x in data)    #Serialize
 
         diff = [json.loads(x)["id"] for x in set2.difference(set1)]    #Deserialize
 
         diff = ', '.join(str(i) for i in diff)
 
         if diff:
             remove_list = '''
```

### Comparing `nriapp-1.1.19/src/nriapp/core/msgraphapi.py` & `nriapp-1.1.21/src/nriapp/core/msgraphapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,17 @@
             else:
                 device_list.extend(object["value"])
                 dbgPrint.info(len(device_list))
         return device_list
 
     def get_user_groups(self, userPrincipalName):
         user_object = self.search_user(userPrincipalName)
-
+        
+        if not user_object:
+            return []
         user_groups = 'https://graph.microsoft.com/beta/users/' + user_object[0]["id"] + '/memberOf/$/microsoft.graph.group'
 
 
         params = {
             '$select' : "id, displayName, securityEnabled",
             '$top'    : 5,
             '$filter' : "(mailEnabled eq false and securityEnabled eq true)",
```

### Comparing `nriapp-1.1.19/src/nriapp/core/mssentinelapi.py` & `nriapp-1.1.21/src/nriapp/core/mssentinelapi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1194,17 +1194,19 @@
                                         "pid"        : pid,
                                         "commandline": commandline,
                                         "sha1"       : sha1,
                                         "path"       : path
                                         }
                                     else:
                                         dbgPrint.error("No parent process")
-                                        raise("No parent process")
-#                                        dbgPrint.info("")
 
+#                                        raise("No parent process")
+                                        
+#                                        dbgPrint.info("")
+#                                    data["alertIds"] = alertIds
                                     data["sha1"] = sha1
                                     data["type"] = "others"
                                     data["parent"] = [{"pid"         : pid,
                                                       "commandline" : commandline,
                                                       "path"        : [path],
                                                       "alertIds"    : alertIds,
                                                       "title"       : [title],
@@ -1692,14 +1694,17 @@
             'entityType' : 'IncidentEntity',
             'id'         : incidentId,
             'pageIndex'  : 1,
             'pageSize'   : 100
             }
         response = self.tryrequest(audit_history, params=params)
 
+        while response.status_code != 200:
+            response = self.tryrequest(audit_history, params = params)
+
         sorted_list = sorted(json.loads(response.text), key=lambda x: x["auditId"])
         #1 - Undefine   Unassigned 
         #2 - Resolved  
         #4 - Progress
 
 
         assigned_timestamp = ""
@@ -1783,14 +1788,17 @@
             'pageSize'   : 100
             }
         response = self.tryrequest(audit_history, params=params)
         while(response.status_code !=200):
             if response.status_code == 440:
                 self.load_session()
                 response = self.tryrequest(audit_history, params=params)
+            elif response.status_code == 503:
+                self.load_session()
+                response = self.tryrequest(audit_history, params=params)
 
         sorted_list = sorted(json.loads(response.text), key=lambda x: x["auditId"])
         return sorted_list
 
     def get_all_audit_logs_raw(self, lookBackInDays=30, new_list=[]):
         
         incident_list = []
```

### Comparing `nriapp-1.1.19/src/nriapp/core/multifactor.py` & `nriapp-1.1.21/src/nriapp/core/multifactor.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.19/src/nriapp/core/vtquery.py` & `nriapp-1.1.21/src/nriapp/core/vtquery.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.19/src/nriapp/helper/doc.py` & `nriapp-1.1.21/src/nriapp/helper/doc.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.19/src/nriapp/helper/login.py` & `nriapp-1.1.21/src/nriapp/helper/login.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.19/src/nriapp/helper/pylog.py` & `nriapp-1.1.21/src/nriapp/helper/pylog.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.19/src/nriapp/helper/requestheader.py` & `nriapp-1.1.21/src/nriapp/helper/requestheader.py`

 * *Files identical despite different names*

### Comparing `nriapp-1.1.19/src/nriapp/nriapp.egg-info/SOURCES.txt` & `nriapp-1.1.21/src/nriapp/nriapp.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -23,12 +23,13 @@
 src/nriapp/core/vtquery.py
 src/nriapp/helper/__init__.py
 src/nriapp/helper/doc.py
 src/nriapp/helper/excel.py
 src/nriapp/helper/login.py
 src/nriapp/helper/pylog.py
 src/nriapp/helper/requestheader.py
+src/nriapp/helper/utils.py
 src/nriapp/nriapp.egg-info/PKG-INFO
 src/nriapp/nriapp.egg-info/SOURCES.txt
 src/nriapp/nriapp.egg-info/dependency_links.txt
 src/nriapp/nriapp.egg-info/entry_points.txt
 src/nriapp/nriapp.egg-info/top_level.txt
```

### Comparing `nriapp-1.1.19/src/nriapp/nriapp.py` & `nriapp-1.1.21/src/nriapp/nriapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -549,23 +549,23 @@
             recent_date = dataexplorer.check_latest_av_engines()
             if not recent_date:
                 dataexplorer.ingest_latest_av_engine(data=av_engines)
 
             elif utc_timezone.localize(parser.parse(av_engines["ReleaseDateUtc"])) > parser.parse(recent_date):
                 dataexplorer.ingest_latest_av_engine(data=av_engines)
 
-            signin_logs = []
-            last_created_time = dataexplorer.check_signin_last_timestamp()        
-            lower_limit = self.msgraph.get_all_signins(login_logs=signin_logs, min=last_created_time)
-            dataexplorer.ingest_signin_logs(data=signin_logs)
-            del signin_logs[:]
-            while(lower_limit):
-                lower_limit = self.msgraph.get_all_signins(login_logs=signin_logs, min=lower_limit)
-                dataexplorer.ingest_signin_logs(data=signin_logs)
-                del signin_logs[:]
+#            signin_logs = []
+#            last_created_time = dataexplorer.check_signin_last_timestamp()        
+#            lower_limit = self.msgraph.get_all_signins(login_logs=signin_logs, min=last_created_time)
+#            dataexplorer.ingest_signin_logs(data=signin_logs)
+#            del signin_logs[:]
+#            while(lower_limit):
+#                lower_limit = self.msgraph.get_all_signins(login_logs=signin_logs, min=lower_limit)
+#                dataexplorer.ingest_signin_logs(data=signin_logs)
+#                del signin_logs[:]
 
             if not dataexplorer.check_ingest_mfastats_tag():
                 mfa_list = self.msgraph.get_users_mfa()
                 dataexplorer.ingest_mfastats(data=mfa_list)
 
             if not dataexplorer.check_ingest_managed_devices_tag():
                 dbgPrint.debug("Fetching all Intune devices")
```

