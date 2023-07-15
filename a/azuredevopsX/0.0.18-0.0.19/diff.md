# Comparing `tmp/azuredevopsX-0.0.18-py3-none-any.whl.zip` & `tmp/azuredevopsX-0.0.19-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 11095 bytes, number of entries: 17
+Zip file size: 10214 bytes, number of entries: 17
 -rwxrwxrwx  2.0 unx        0 b- defN 22-Nov-01 15:16 azuredevopsX/__init__.py
--rwxrwxrwx  2.0 unx     1263 b- defN 22-Nov-02 12:45 azuredevopsX/abstractdevops.py
+-rwxrwxrwx  2.0 unx     1263 b- defN 23-Jul-15 20:32 azuredevopsX/abstractdevops.py
 -rwxrwxrwx  2.0 unx     1603 b- defN 23-Feb-15 14:36 azuredevopsX/backlog.py
 -rwxrwxrwx  2.0 unx     1857 b- defN 23-Jul-13 21:18 azuredevopsX/factories.py
 -rwxrwxrwx  2.0 unx      324 b- defN 23-Feb-15 13:05 azuredevopsX/identity.py
 -rwxrwxrwx  2.0 unx     1863 b- defN 23-Feb-15 13:05 azuredevopsX/interaction.py
 -rwxrwxrwx  2.0 unx     1695 b- defN 23-Feb-15 13:13 azuredevopsX/project.py
 -rwxrwxrwx  2.0 unx      351 b- defN 23-Feb-15 13:05 azuredevopsX/status.py
 -rwxrwxrwx  2.0 unx      992 b- defN 23-Feb-15 13:05 azuredevopsX/team.py
 -rwxrwxrwx  2.0 unx     1325 b- defN 23-Feb-15 13:05 azuredevopsX/teammember.py
--rwxrwxrwx  2.0 unx     6557 b- defN 23-Feb-15 13:05 azuredevopsX/workitem.py
--rwxrwxrwx  2.0 unx     6802 b- defN 23-Jul-13 23:31 azuredevopsX/workitem_history.py
+-rwxrwxrwx  2.0 unx     6557 b- defN 23-Jul-15 20:34 azuredevopsX/workitem.py
+-rwxrwxrwx  2.0 unx     1142 b- defN 23-Jul-15 20:42 azuredevopsX/workitem_history.py
 -rwxrwxrwx  2.0 unx     1438 b- defN 23-Feb-15 13:05 azuredevopsX/workitemtype.py
--rwxrwxrwx  2.0 unx     2224 b- defN 23-Jul-13 23:35 azuredevopsX-0.0.18.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-13 23:35 azuredevopsX-0.0.18.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       13 b- defN 23-Jul-13 23:35 azuredevopsX-0.0.18.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-13 23:35 azuredevopsX-0.0.18.dist-info/RECORD
-17 files, 29784 bytes uncompressed, 8821 bytes compressed:  70.4%
+-rwxrwxrwx  2.0 unx     2236 b- defN 23-Jul-15 20:45 azuredevopsX-0.0.19.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-15 20:45 azuredevopsX-0.0.19.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       13 b- defN 23-Jul-15 20:45 azuredevopsX-0.0.19.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-15 20:45 azuredevopsX-0.0.19.dist-info/RECORD
+17 files, 24136 bytes uncompressed, 7940 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: azuredevopsX/workitem_history.py
 Comment: 
 
 Filename: azuredevopsX/workitemtype.py
 Comment: 
 
-Filename: azuredevopsX-0.0.18.dist-info/METADATA
+Filename: azuredevopsX-0.0.19.dist-info/METADATA
 Comment: 
 
-Filename: azuredevopsX-0.0.18.dist-info/WHEEL
+Filename: azuredevopsX-0.0.19.dist-info/WHEEL
 Comment: 
 
-Filename: azuredevopsX-0.0.18.dist-info/top_level.txt
+Filename: azuredevopsX-0.0.19.dist-info/top_level.txt
 Comment: 
 
-Filename: azuredevopsX-0.0.18.dist-info/RECORD
+Filename: azuredevopsX-0.0.19.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azuredevopsX/abstractdevops.py

```diff
@@ -1,28 +1,28 @@
 from azure.devops.credentials import BasicAuthentication
 from azure.devops.connection import Connection
-from azure.devops.v5_1.work.models import TeamContext
-from azure.devops.v5_1.client_factory import ClientFactoryV5_1
-from azure.devops.v5_1.work_item_tracking import WorkItemTrackingClient 
-from azure.devops.v5_1.work_item_tracking.models import Wiql
+from azure.devops.v7_1.work.models import TeamContext
+from azure.devops.v7_1.client_factory import ClientFactoryV7_1
+from azure.devops.v7_1.work_item_tracking import WorkItemTrackingClient 
+from azure.devops.v7_1.work_item_tracking.models import Wiql
 from pprint import pprint
 from abc import ABC
 
 class AbstractDevOps(ABC):
 
     def __init__(self, personal_access_token, organization_url):
 
         self.personal_access_token = personal_access_token
         self.organization_url = organization_url
 
         self.credentials = BasicAuthentication('', personal_access_token)
         self.connection = Connection(base_url=organization_url, creds=self.credentials)
 
         self.core_client = self.connection.clients.get_core_client()
-        self.work_client = self.connection.clients_v5_1.get_work_client()
-        self.work_item_tracking_client = self.connection.clients_v5_1.get_work_item_tracking_client()
-        self.work_item_process_tracking_client = self.connection.clients_v5_1.get_work_item_tracking_process_client()
+        self.work_client = self.connection.clients_v7_1.get_work_client()
+        self.work_item_tracking_client = self.connection.clients_v7_1.get_work_item_tracking_client()
+        self.work_item_process_tracking_client = self.connection.clients_v7_1.get_work_item_tracking_process_client()
     
     def create_team_context(self, project, team):
         return  TeamContext(project, project.id, team, team.id)
```

## azuredevopsX/workitem.py

```diff
@@ -1,12 +1,12 @@
 import logging
 logging.basicConfig(level=logging.INFO)
 from azuredevopsX.abstractdevops import AbstractDevOps
-from azure.devops.v5_1.work_item_tracking import WorkItemTrackingClient 
-from azure.devops.v5_1.work_item_tracking.models import Wiql
+from azure.devops.v7_1.work_item_tracking import WorkItemTrackingClient 
+from azure.devops.v7_1.work_item_tracking.models import Wiql
 from azuredevopsX import factories
 
 # Represent a item of work in a project xxx
 
 class WorkItem(AbstractDevOps):
 
 	def __init__(self,personal_access_token, organization_url):
```

## azuredevopsX/workitem_history.py

```diff
@@ -1,234 +1,34 @@
 import logging
 logging.basicConfig(level=logging.INFO)
 from azuredevopsX.abstractdevops import AbstractDevOps
-from azure.devops.v5_1.work_item_tracking import WorkItemTrackingClient 
-from azure.devops.v5_1.work_item_tracking.models import Wiql
 from azuredevopsX import factories
-from pprint import pprint
 
 class WorkItemHistory(AbstractDevOps):
 
 	def __init__(self,personal_access_token, organization_url):
 		super(WorkItemHistory,self).__init__(personal_access_token=personal_access_token,organization_url=organization_url)
-	
+		self.serviceWorkitem = factories.WorkItemFactory(personal_access_token=personal_access_token,organization_url=organization_url)
+		
 
 	def get_all (self, today=False):
 		try:
-			logging.info("Start function: get_work_items")
+			logging.info("Start function: WorkItemHistory")
 			
-			work_items_list = []
+			work_items_list = self.serviceWorkitem.get_all(today=today)
 			revisions_list = []
-			work_items = None
-			if today:
-				work_items = self.get_query_today()
-			else:
-				work_items = self.get_work_item_query_by_wiql()
-			
-			# Dividindo em vetores de no máximo 200 itens. O serviço permite no máximo 200 ids por requisição;
-			work_items_list_split = [work_items[x:x+200] for x in range(0,len(work_items), 200)]
-
-			for work_items_list_item in work_items_list_split:
-				
-				work_item_list_retrieve = []
-				#criando o vertor a ser enviado
-				for work_item in work_items_list_item:
-					work_item_list_retrieve.append(int(work_item.id))
-				
-				work_item_retrieved = self.get_work_items(ids=[*work_item_list_retrieve])				
-				
-				work_items_list.extend(work_item_retrieved)
 			
-			logging.info("End function: get_work_items")
-
 			for work_item in work_items_list:
-			
+				logging.info("Getting Revisisons: "+work_item.fields['System.TeamProject']+"--"+str(work_item.id))
 				revisions = self.work_item_tracking_client.get_revisions(project=work_item.fields['System.TeamProject'], id = work_item.id, expand="All")
 				revisions_list.extend (revisions)
 				
 
 			return revisions_list
 
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
 			logging.error(e.__dict__) 
 
 	
 
-	# Return a specifc workitem from a project with detais
-	def get_work_items(self,ids):
-		try:
-			logging.info("Start function: get_work_items")
-			result = self.work_item_tracking_client.get_work_items(ids=ids, 
-                                                        project=None,                                                       
-                                                       expand="All")
-			logging.info("End function: get_work_items")
-
-			list_result = []
-			
-			for item in result:
-				item._links = item._links.__dict__
-
-				if item.comment_version_ref is not None:
-					item.comment_version_ref = item.comment_version_ref.__dict__
-
-				if item.relations is not None:
-					item_relations = []
-					
-					for relation in item.relations:
-						item_relations.append(relation.__dict__)
-					
-					item.relations = item_relations
-			
-				list_result.append(item)
-			return list_result
-		except Exception as e: 
-			logging.error("OS error: {0}".format(e))
-			logging.error(e.__dict__) 
-		
-	
-	# Return a specifc workitem from a project with detais
-	def get_work_item(self,work_item_id):
-		try:
-			logging.info("Start function: get_work_item")
-			logging.info("End function: get_work_item")
-
-			return self.work_item_tracking_client.get_work_item(id=work_item_id, 
-                                                        project=None,                                                       
-                                                       expand="All")
-		except Exception as e: 
-			logging.error("OS error: {0}".format(e))
-			logging.error(e.__dict__) 
-
-
-	def get_relation(self, relation):
-		try:
-			logging.info("Start function: get_work_item")
-			logging.info("End function: get_work_item")
-
-			return self.work_item_tracking_client.get_relation_type(relation)
-		except Exception as e: 
-			logging.error("OS error: {0}".format(e))
-			logging.error(e.__dict__) 
-    
-	def get_backlog_work_items(self, project,team, backlog):
-		try:
-			logging.info("Start function: get_work_item")
-			logging.info("End function: get_work_item")
-			team_context = self.create_team_context(project, team)
-			return self.work_client.get_backlog_level_work_items(team_context, backlog.id)
-		except Exception as e: 
-			logging.error("OS error: {0}".format(e))
-			logging.error(e.__dict__) 
-
-	def get_work_item_query_by_wiql(self):
-		try:
-			wiql = Wiql(
-			query="""select 
-					*
-					from WorkItems"""
-					
-				)
-			wiql_results = self.work_item_tracking_client.query_by_wiql(wiql).work_items
-			if wiql_results:
-				return wiql_results
-			else:
-				return []
-		except Exception as e: 
-			logging.error("OS error: {0}".format(e))
-			logging.error(e.__dict__) 	
-
-	def get_query_today(self):
-		try:
-			wiql = Wiql(
-			query="""select 
-					*
-					from WorkItems
-					where 
-					[System.CreatedDate] = @Today 
-					OR [System.ChangedDate] = @Today 
-					OR [Microsoft.VSTS.Common.ClosedDate] = @Today 
-					OR [Microsoft.VSTS.Common.ResolvedDate] = @Today
-					OR [System.RevisedDate] = @Today
-					OR [Microsoft.VSTS.Common.StateChangeDate]= @Today
-					order by [System.ChangedDate] desc"""
-				)
-			wiql_results = self.work_item_tracking_client.query_by_wiql(wiql).work_items
-			if wiql_results:
-				return wiql_results
-			else:
-				return []
-		
-		except Exception as e: 
-			logging.error("OS error: {0}".format(e))
-			logging.error(e.__dict__) 
-	
-	
-	
-	def get_work_item_query_by_wiql_epic_user_story_product_backlog_item(self):
-		try:
-			wiql = Wiql(
-			query="""select 
-					*
-					from WorkItems
-					order by [System.ChangedDate] desc"""
-					
-				)
-			wiql_results = self.work_item_tracking_client.query_by_wiql(wiql).work_items
-			if wiql_results:
-				return wiql_results
-			else:
-				return []
-		
-		except Exception as e: 
-			logging.error("OS error: {0}".format(e))
-			logging.error(e.__dict__) 
-
-	def get_work_item_query_by_wiql_task(self):
-		try:
-			wiql = Wiql(
-			query="""
-					select [System.Id],
-						[System.WorkItemType],
-						[System.Title],
-						[System.State],
-						[System.AreaPath],
-						[System.IterationPath],
-						[System.Tags],
-						[System.TeamProject]
-					from WorkItems
-					where 
-					[System.WorkItemType] = 'Task' 
-					order by [System.ChangedDate] desc"""
-				)
-			wiql_results = self.work_item_tracking_client.query_by_wiql(wiql).work_items
-			if wiql_results:
-				return wiql_results
-			else:
-				return []
-
-		except Exception as e: 
-			logging.error("OS error: {0}".format(e))
-			logging.error(e.__dict__) 
-
-	def get_work_item_query_by_wiql(self):
-		try:
-			wiql = Wiql(
-			query="""
-					select [System.Id],
-						[System.WorkItemType],
-						[System.Title],
-						[System.State],
-						[System.AreaPath],
-						[System.IterationPath],
-						[System.Tags]
-					from WorkItems
-					order by [System.ChangedDate] desc"""
-				)
-			wiql_results = self.work_item_tracking_client.query_by_wiql(wiql).work_items
-			if wiql_results:
-				return wiql_results
-			else:
-				return []
-		except Exception as e: 
-			logging.error("OS error: {0}".format(e))
-			logging.error(e.__dict__) 
+
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `azuredevopsX-0.0.18.dist-info/METADATA` & `azuredevopsX-0.0.19.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: azuredevopsX
-Version: 0.0.18
+Version: 0.0.19
 Summary: DevOps é um produto da Microsoft que fornece controle de versão, relatórios, gerenciamento de requisitos, gerenciamento de projetos, compilações automatizadas, gerenciamento de laboratório, recursos de gerenciamento de testes e versões.
 Home-page: https://gitlab.com/integration_seon/libs/application/tfs
 Author: Paulo Sérgio dos Santos Júnior
 Author-email: paulossjunior@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Requires-Dist: azure-devops
+Requires-Dist: azure-devops (==7.1.0b3)
 Requires-Dist: factory-boy
 Requires-Dist: requestx
 
 # DevopsX
 
 ## General Information
 * **Software**:DevopsX
```

## Comparing `azuredevopsX-0.0.18.dist-info/RECORD` & `azuredevopsX-0.0.19.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 azuredevopsX/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-azuredevopsX/abstractdevops.py,sha256=NvCx1N7ra-tRdpjxpYBezv9mGNkVL_BinFe-Nhdt9fs,1263
+azuredevopsX/abstractdevops.py,sha256=mrGP6iT1ap4AT7trwVBdWodDZLvvzYfp7VhQV-UEzYM,1263
 azuredevopsX/backlog.py,sha256=CwhmPuXFjMsIt25Q9DsNSR7z8VOuhSZfGr3ZfDREcAM,1603
 azuredevopsX/factories.py,sha256=iLudT2f3tHsbSJC7GomIFAcnrBpt13SUz_SSKKy7ONI,1857
 azuredevopsX/identity.py,sha256=hYyz3jaChkXEzq58TQoz26k8yTNGLqv0Y2HDjpcqz2Q,324
 azuredevopsX/interaction.py,sha256=L0CI2gM_LaQgqzrqbUAbSy-SR31nMkbK9ayy3JLh7JM,1863
 azuredevopsX/project.py,sha256=ZRqG2cGP7MOZOWDf3NQOQp2mwib4Xb3BXtaJ8FQhdb0,1695
 azuredevopsX/status.py,sha256=EIYW3QFzPvma7rqcvipSNPdSvaQktqMU520nFJYHRWI,351
 azuredevopsX/team.py,sha256=-F5s9Xz1KTN6l2xEGUIUHj6CzBbqe6NaLbeELsLBudk,992
 azuredevopsX/teammember.py,sha256=YtmmibleH__yTgg-dpd_ZQr6FhfrNkveh4HJjb6mRCg,1325
-azuredevopsX/workitem.py,sha256=JX8k3bmhUeGKfrB92-jWuKzfhP9ny_L1wOV8rR8oCUg,6557
-azuredevopsX/workitem_history.py,sha256=XSXqc1ONG1Y9SI8gy2gC6ENA28ZizaVnvT4i97VXB9A,6802
+azuredevopsX/workitem.py,sha256=RANpRdkYx9ilwVsInFpXjTr7o04WBtbjhzFCrn0F40Y,6557
+azuredevopsX/workitem_history.py,sha256=j8OCHpMtLegPsFxz0oxBuVnm6VPpD5fT44XkTSDgj6Q,1142
 azuredevopsX/workitemtype.py,sha256=gxB3Nlc6s4VYRu0GtSvbt8BoZSKXS-hZRxJnEknkka4,1438
-azuredevopsX-0.0.18.dist-info/METADATA,sha256=yfhWUHW-92XNgwqZ2XsZCgEAe2D07vfHBENYYsWEmqo,2224
-azuredevopsX-0.0.18.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-azuredevopsX-0.0.18.dist-info/top_level.txt,sha256=5eqZIScBYOUIwspo--jA_bw95-aK1_S_7Nd0A-djvLo,13
-azuredevopsX-0.0.18.dist-info/RECORD,,
+azuredevopsX-0.0.19.dist-info/METADATA,sha256=IW-IyqTyaymWZE18fYZN4HnbtgoWyxe8CtBvL_sLSkc,2236
+azuredevopsX-0.0.19.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+azuredevopsX-0.0.19.dist-info/top_level.txt,sha256=5eqZIScBYOUIwspo--jA_bw95-aK1_S_7Nd0A-djvLo,13
+azuredevopsX-0.0.19.dist-info/RECORD,,
```

