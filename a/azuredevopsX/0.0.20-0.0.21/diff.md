# Comparing `tmp/azuredevopsX-0.0.20-py3-none-any.whl.zip` & `tmp/azuredevopsX-0.0.21-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -8,12 +8,12 @@
 -rwxrwxrwx  2.0 unx     1291 b- defN 23-Jul-15 21:24 azuredevopsX/project.py
 -rwxrwxrwx  2.0 unx      351 b- defN 23-Feb-15 13:05 azuredevopsX/status.py
 -rwxrwxrwx  2.0 unx      992 b- defN 23-Feb-15 13:05 azuredevopsX/team.py
 -rwxrwxrwx  2.0 unx     1325 b- defN 23-Feb-15 13:05 azuredevopsX/teammember.py
 -rwxrwxrwx  2.0 unx     6557 b- defN 23-Jul-15 20:34 azuredevopsX/workitem.py
 -rwxrwxrwx  2.0 unx     1142 b- defN 23-Jul-15 20:42 azuredevopsX/workitem_history.py
 -rwxrwxrwx  2.0 unx     1438 b- defN 23-Feb-15 13:05 azuredevopsX/workitemtype.py
--rwxrwxrwx  2.0 unx     2236 b- defN 23-Jul-15 21:28 azuredevopsX-0.0.20.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-15 21:28 azuredevopsX-0.0.20.dist-info/WHEEL
--rwxrwxrwx  2.0 unx       13 b- defN 23-Jul-15 21:28 azuredevopsX-0.0.20.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-15 21:28 azuredevopsX-0.0.20.dist-info/RECORD
+-rwxrwxrwx  2.0 unx     2236 b- defN 23-Jul-15 21:50 azuredevopsX-0.0.21.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-Jul-15 21:50 azuredevopsX-0.0.21.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx       13 b- defN 23-Jul-15 21:50 azuredevopsX-0.0.21.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1385 b- defN 23-Jul-15 21:50 azuredevopsX-0.0.21.dist-info/RECORD
 17 files, 23732 bytes uncompressed, 7841 bytes compressed:  67.0%
```

## zipnote {}

```diff
@@ -33,20 +33,20 @@
 
 Filename: azuredevopsX/workitem_history.py
 Comment: 
 
 Filename: azuredevopsX/workitemtype.py
 Comment: 
 
-Filename: azuredevopsX-0.0.20.dist-info/METADATA
+Filename: azuredevopsX-0.0.21.dist-info/METADATA
 Comment: 
 
-Filename: azuredevopsX-0.0.20.dist-info/WHEEL
+Filename: azuredevopsX-0.0.21.dist-info/WHEEL
 Comment: 
 
-Filename: azuredevopsX-0.0.20.dist-info/top_level.txt
+Filename: azuredevopsX-0.0.21.dist-info/top_level.txt
 Comment: 
 
-Filename: azuredevopsX-0.0.20.dist-info/RECORD
+Filename: azuredevopsX-0.0.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `azuredevopsX-0.0.20.dist-info/METADATA` & `azuredevopsX-0.0.21.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azuredevopsX
-Version: 0.0.20
+Version: 0.0.21
 Summary: DevOps é um produto da Microsoft que fornece controle de versão, relatórios, gerenciamento de requisitos, gerenciamento de projetos, compilações automatizadas, gerenciamento de laboratório, recursos de gerenciamento de testes e versões.
 Home-page: https://gitlab.com/integration_seon/libs/application/tfs
 Author: Paulo Sérgio dos Santos Júnior
 Author-email: paulossjunior@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `azuredevopsX-0.0.20.dist-info/RECORD` & `azuredevopsX-0.0.21.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -7,11 +7,11 @@
 azuredevopsX/project.py,sha256=BingdrDeHr5q7DzUs_U_-5srZtV8usW6A0iwsU0EDAw,1291
 azuredevopsX/status.py,sha256=EIYW3QFzPvma7rqcvipSNPdSvaQktqMU520nFJYHRWI,351
 azuredevopsX/team.py,sha256=-F5s9Xz1KTN6l2xEGUIUHj6CzBbqe6NaLbeELsLBudk,992
 azuredevopsX/teammember.py,sha256=YtmmibleH__yTgg-dpd_ZQr6FhfrNkveh4HJjb6mRCg,1325
 azuredevopsX/workitem.py,sha256=RANpRdkYx9ilwVsInFpXjTr7o04WBtbjhzFCrn0F40Y,6557
 azuredevopsX/workitem_history.py,sha256=j8OCHpMtLegPsFxz0oxBuVnm6VPpD5fT44XkTSDgj6Q,1142
 azuredevopsX/workitemtype.py,sha256=gxB3Nlc6s4VYRu0GtSvbt8BoZSKXS-hZRxJnEknkka4,1438
-azuredevopsX-0.0.20.dist-info/METADATA,sha256=NMx7XbDmQBmKo09SqKr_0swZB2yIzoaSuXE-kYNOrQ4,2236
-azuredevopsX-0.0.20.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-azuredevopsX-0.0.20.dist-info/top_level.txt,sha256=5eqZIScBYOUIwspo--jA_bw95-aK1_S_7Nd0A-djvLo,13
-azuredevopsX-0.0.20.dist-info/RECORD,,
+azuredevopsX-0.0.21.dist-info/METADATA,sha256=iyNZeOktJgWxz1V38HDH3biYZvkFShGvQQUtOuSwNSc,2236
+azuredevopsX-0.0.21.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+azuredevopsX-0.0.21.dist-info/top_level.txt,sha256=5eqZIScBYOUIwspo--jA_bw95-aK1_S_7Nd0A-djvLo,13
+azuredevopsX-0.0.21.dist-info/RECORD,,
```

