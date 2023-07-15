# Comparing `tmp/azuredevopsX-0.0.19-py3-none-any.whl.zip` & `tmp/azuredevopsX-0.0.20-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 10214 bytes, number of entries: 17
+Zip file size: 10115 bytes, number of entries: 17
 -rwxrwxrwx  2.0 unx        0 b- defN 22-Nov-01 15:16 azuredevopsX/__init__.py
 -rwxrwxrwx  2.0 unx     1263 b- defN 23-Jul-15 20:32 azuredevopsX/abstractdevops.py
 -rwxrwxrwx  2.0 unx     1603 b- defN 23-Feb-15 14:36 azuredevopsX/backlog.py
 -rwxrwxrwx  2.0 unx     1857 b- defN 23-Jul-13 21:18 azuredevopsX/factories.py
 -rwxrwxrwx  2.0 unx      324 b- defN 23-Feb-15 13:05 azuredevopsX/identity.py
 -rwxrwxrwx  2.0 unx     1863 b- defN 23-Feb-15 13:05 azuredevopsX/interaction.py
--rwxrwxrwx  2.0 unx     1695 b- defN 23-Feb-15 13:13 azuredevopsX/project.py
+-rwxrwxrwx  2.0 unx     1291 b- defN 23-Jul-15 21:24 azuredevopsX/project.py
 -rwxrwxrwx  2.0 unx      351 b- defN 23-Feb-15 13:05 azuredevopsX/status.py
 -rwxrwxrwx  2.0 unx      992 b- defN 23-Feb-15 13:05 azuredevopsX/team.py
 -rwxrwxrwx  2.0 unx     1325 b- defN 23-Feb-15 13:05 azuredevopsX/teammember.py
 -rwxrwxrwx  2.0 unx     6557 b- defN 23-Jul-15 20:34 azuredevopsX/workitem.py
 -rwxrwxrwx  2.0 unx     1142 b- defN 23-Jul-15 20:42 azuredevopsX/workitem_history.py
 -rwxrwxrwx  2.0 unx     1438 b- defN 23-Feb-15 13:05 azuredevopsX/workitemtype.py
--rwxrwxrwx  2.0 unx     2236 b- defN 23-Jul-15 20:45 azuredevopsX-0.0.19.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-15 20:45 azuredevopsX-0.0.19.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       13 b- defN 23-Jul-15 20:45 azuredevopsX-0.0.19.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-15 20:45 azuredevopsX-0.0.19.dist-info/RECORD
-17 files, 24136 bytes uncompressed, 7940 bytes compressed:  67.1%
+-rwxrwxrwx  2.0 unx     2236 b- defN 23-Jul-15 21:28 azuredevopsX-0.0.20.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-15 21:28 azuredevopsX-0.0.20.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       13 b- defN 23-Jul-15 21:28 azuredevopsX-0.0.20.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-15 21:28 azuredevopsX-0.0.20.dist-info/RECORD
+17 files, 23732 bytes uncompressed, 7841 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: azuredevopsX/workitem_history.py
 Comment: 
 
 Filename: azuredevopsX/workitemtype.py
 Comment: 
 
-Filename: azuredevopsX-0.0.19.dist-info/METADATA
+Filename: azuredevopsX-0.0.20.dist-info/METADATA
 Comment: 
 
-Filename: azuredevopsX-0.0.19.dist-info/WHEEL
+Filename: azuredevopsX-0.0.20.dist-info/WHEEL
 Comment: 
 
-Filename: azuredevopsX-0.0.19.dist-info/top_level.txt
+Filename: azuredevopsX-0.0.20.dist-info/top_level.txt
 Comment: 
 
-Filename: azuredevopsX-0.0.19.dist-info/RECORD
+Filename: azuredevopsX-0.0.20.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## azuredevopsX/project.py

```diff
@@ -11,25 +11,18 @@
 	# Returns a list of project
 	def get_all(self, today=False): 
 		projects = []
 		try:
 			logging.info("Start function: get_projects")
 			
 			get_projects_response = self.core_client.get_projects()
-			
-			while get_projects_response is not None:
 				
-				for project in get_projects_response.value:
-					projects.append(project)
-				if get_projects_response.continuation_token is not None and get_projects_response.continuation_token != "":
-					# Get the next page of projects
-					get_projects_response = self.core_client.get_projects(continuation_token=get_projects_response.continuation_token)
-				else:
-					# All projects have been retrieved
-					get_projects_response = None
+			for project in get_projects_response:
+				projects.append(project)
+				
 
 		except Exception as e: 
 			logging.error("OS error: {0}".format(e))
 			logging.error(e.__dict__) 
 
 		logging.info("Retrieve All Projects")
```

## Comparing `azuredevopsX-0.0.19.dist-info/METADATA` & `azuredevopsX-0.0.20.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azuredevopsX
-Version: 0.0.19
+Version: 0.0.20
 Summary: DevOps é um produto da Microsoft que fornece controle de versão, relatórios, gerenciamento de requisitos, gerenciamento de projetos, compilações automatizadas, gerenciamento de laboratório, recursos de gerenciamento de testes e versões.
 Home-page: https://gitlab.com/integration_seon/libs/application/tfs
 Author: Paulo Sérgio dos Santos Júnior
 Author-email: paulossjunior@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `azuredevopsX-0.0.19.dist-info/RECORD` & `azuredevopsX-0.0.20.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 azuredevopsX/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 azuredevopsX/abstractdevops.py,sha256=mrGP6iT1ap4AT7trwVBdWodDZLvvzYfp7VhQV-UEzYM,1263
 azuredevopsX/backlog.py,sha256=CwhmPuXFjMsIt25Q9DsNSR7z8VOuhSZfGr3ZfDREcAM,1603
 azuredevopsX/factories.py,sha256=iLudT2f3tHsbSJC7GomIFAcnrBpt13SUz_SSKKy7ONI,1857
 azuredevopsX/identity.py,sha256=hYyz3jaChkXEzq58TQoz26k8yTNGLqv0Y2HDjpcqz2Q,324
 azuredevopsX/interaction.py,sha256=L0CI2gM_LaQgqzrqbUAbSy-SR31nMkbK9ayy3JLh7JM,1863
-azuredevopsX/project.py,sha256=ZRqG2cGP7MOZOWDf3NQOQp2mwib4Xb3BXtaJ8FQhdb0,1695
+azuredevopsX/project.py,sha256=BingdrDeHr5q7DzUs_U_-5srZtV8usW6A0iwsU0EDAw,1291
 azuredevopsX/status.py,sha256=EIYW3QFzPvma7rqcvipSNPdSvaQktqMU520nFJYHRWI,351
 azuredevopsX/team.py,sha256=-F5s9Xz1KTN6l2xEGUIUHj6CzBbqe6NaLbeELsLBudk,992
 azuredevopsX/teammember.py,sha256=YtmmibleH__yTgg-dpd_ZQr6FhfrNkveh4HJjb6mRCg,1325
 azuredevopsX/workitem.py,sha256=RANpRdkYx9ilwVsInFpXjTr7o04WBtbjhzFCrn0F40Y,6557
 azuredevopsX/workitem_history.py,sha256=j8OCHpMtLegPsFxz0oxBuVnm6VPpD5fT44XkTSDgj6Q,1142
 azuredevopsX/workitemtype.py,sha256=gxB3Nlc6s4VYRu0GtSvbt8BoZSKXS-hZRxJnEknkka4,1438
-azuredevopsX-0.0.19.dist-info/METADATA,sha256=IW-IyqTyaymWZE18fYZN4HnbtgoWyxe8CtBvL_sLSkc,2236
-azuredevopsX-0.0.19.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-azuredevopsX-0.0.19.dist-info/top_level.txt,sha256=5eqZIScBYOUIwspo--jA_bw95-aK1_S_7Nd0A-djvLo,13
-azuredevopsX-0.0.19.dist-info/RECORD,,
+azuredevopsX-0.0.20.dist-info/METADATA,sha256=NMx7XbDmQBmKo09SqKr_0swZB2yIzoaSuXE-kYNOrQ4,2236
+azuredevopsX-0.0.20.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+azuredevopsX-0.0.20.dist-info/top_level.txt,sha256=5eqZIScBYOUIwspo--jA_bw95-aK1_S_7Nd0A-djvLo,13
+azuredevopsX-0.0.20.dist-info/RECORD,,
```

