# Comparing `tmp/gitcoll-0.0.20-py3-none-any.whl.zip` & `tmp/gitcoll-0.0.21-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 59262 bytes, number of entries: 22
+Zip file size: 59267 bytes, number of entries: 22
 -rw-r--r--  2.0 unx       14 b- defN 23-Jun-11 11:48 gcln/__init__.py
 -rw-r--r--  2.0 unx     6751 b- defN 23-Jun-11 11:48 gcln/cfg_file.py
 -rw-r--r--  2.0 unx       51 b- defN 23-Jun-11 11:48 gcln/exceptions.py
 -rw-r--r--  2.0 unx     7232 b- defN 23-Jun-11 11:48 gcln/helpers.py
 -rw-r--r--  2.0 unx    43203 b- defN 23-Jun-11 11:48 gcln/main.py
 -rw-r--r--  2.0 unx    29661 b- defN 23-Jun-11 11:48 gcln/main_context.py
 -rw-r--r--  2.0 unx     4207 b- defN 23-Jun-11 11:48 gcln/records.py
 -rw-r--r--  2.0 unx    12693 b- defN 23-Jun-11 11:48 gcln/srv_connector.py
--rw-r--r--  2.0 unx       90 b- defN 23-Jul-15 12:45 gcln2/__init__.py
+-rw-r--r--  2.0 unx       90 b- defN 23-Jul-15 14:54 gcln2/__init__.py
 -rw-r--r--  2.0 unx     9775 b- defN 23-Jul-15 12:45 gcln2/db.py
 -rw-r--r--  2.0 unx       51 b- defN 23-Jun-11 11:48 gcln2/exceptions.py
 -rw-r--r--  2.0 unx     9464 b- defN 23-Jul-15 12:45 gcln2/helpers.py
--rw-r--r--  2.0 unx    43383 b- defN 23-Jul-15 12:45 gcln2/main.py
+-rw-r--r--  2.0 unx    43390 b- defN 23-Jul-15 14:54 gcln2/main.py
 -rw-r--r--  2.0 unx     2534 b- defN 23-Jul-15 12:45 gcln2/schema.py
 -rw-r--r--  2.0 unx    25325 b- defN 23-Jul-15 12:45 gcln2/sync.py
 -rw-r--r--  2.0 unx      434 b- defN 23-Jun-11 11:48 gcln2/yaml_loader.py
--rw-rw-rw-  2.0 unx        0 b- defN 23-Jul-15 12:45 gitcoll-0.0.20.dist-info/LICENSE
--rw-r--r--  2.0 unx    12374 b- defN 23-Jul-15 12:45 gitcoll-0.0.20.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 12:45 gitcoll-0.0.20.dist-info/WHEEL
--rw-r--r--  2.0 unx       72 b- defN 23-Jul-15 12:45 gitcoll-0.0.20.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 23-Jul-15 12:45 gitcoll-0.0.20.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1650 b- defN 23-Jul-15 12:45 gitcoll-0.0.20.dist-info/RECORD
-22 files, 209067 bytes uncompressed, 56644 bytes compressed:  72.9%
+-rw-rw-rw-  2.0 unx        0 b- defN 23-Jul-15 14:54 gitcoll-0.0.21.dist-info/LICENSE
+-rw-r--r--  2.0 unx    12374 b- defN 23-Jul-15 14:54 gitcoll-0.0.21.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jul-15 14:54 gitcoll-0.0.21.dist-info/WHEEL
+-rw-r--r--  2.0 unx       72 b- defN 23-Jul-15 14:54 gitcoll-0.0.21.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-Jul-15 14:54 gitcoll-0.0.21.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1650 b- defN 23-Jul-15 14:54 gitcoll-0.0.21.dist-info/RECORD
+22 files, 209074 bytes uncompressed, 56649 bytes compressed:  72.9%
```

## zipnote {}

```diff
@@ -42,26 +42,26 @@
 
 Filename: gcln2/sync.py
 Comment: 
 
 Filename: gcln2/yaml_loader.py
 Comment: 
 
-Filename: gitcoll-0.0.20.dist-info/LICENSE
+Filename: gitcoll-0.0.21.dist-info/LICENSE
 Comment: 
 
-Filename: gitcoll-0.0.20.dist-info/METADATA
+Filename: gitcoll-0.0.21.dist-info/METADATA
 Comment: 
 
-Filename: gitcoll-0.0.20.dist-info/WHEEL
+Filename: gitcoll-0.0.21.dist-info/WHEEL
 Comment: 
 
-Filename: gitcoll-0.0.20.dist-info/entry_points.txt
+Filename: gitcoll-0.0.21.dist-info/entry_points.txt
 Comment: 
 
-Filename: gitcoll-0.0.20.dist-info/top_level.txt
+Filename: gitcoll-0.0.21.dist-info/top_level.txt
 Comment: 
 
-Filename: gitcoll-0.0.20.dist-info/RECORD
+Filename: gitcoll-0.0.21.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## gcln2/__init__.py

```diff
@@ -1,2 +1,2 @@
 # note that the CI job to release the package overwrites this file
-__version__ = "0.0.20"
+__version__ = "0.0.21"
```

## gcln2/main.py

```diff
@@ -967,15 +967,15 @@
             return
 
         if sub_url:
             pass # already know the sub_url
         else:
             origin_url = repo.remotes["origin"].url
             if not origin_url.startswith(srv_url):
-                print (f"* {p} remote origin doesn't start with {srv_url} ({origin_url})")
+                print (f"* {wsp_path} remote origin doesn't start with {srv_url} ({origin_url})")
                 return
 
             sub_url = origin_url[len(srv_url):]
 
         if sub_url.lower().endswith(".git"):
             sub_url = sub_url[:-4]
         else:
```

## Comparing `gitcoll-0.0.20.dist-info/METADATA` & `gitcoll-0.0.21.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitcoll
-Version: 0.0.20
+Version: 0.0.21
 Summary: Git collection utilities
 Home-page: https://gitlab.com/jesrib/gitcoll
 Author: Jesper Ribbe
 Author-email: jesper@ribbe.se
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `gitcoll-0.0.20.dist-info/RECORD` & `gitcoll-0.0.21.dist-info/RECORD`

 * *Files 17% similar despite different names*

```diff
@@ -2,21 +2,21 @@
 gcln/cfg_file.py,sha256=iTOwGr8npJClP-ELTy6MIwkxFgigy3GdiKNp3LFPR2E,6751
 gcln/exceptions.py,sha256=GZbjPYBLS3FKSzXwOuiLv5b9ZNHFfldGUnZfOD8vOtE,51
 gcln/helpers.py,sha256=HbQmumEkjpq2FBMpw58eZZwf_TjSvt3Fj5p5wcPsE7U,7232
 gcln/main.py,sha256=wmuuiaRnv7MxdmrQ_o4CMX26lnBojxSAwniUwo0O3XU,43203
 gcln/main_context.py,sha256=kXjeePjGrHmX46anoE7dunggEyqYEGn1sQwbjVim-Vo,29661
 gcln/records.py,sha256=jVX3WJ9LMfghMxCMBku8YCVmTN1X-dhRxCCr6VogKuo,4207
 gcln/srv_connector.py,sha256=f6QeLWY7YjQzsVbCju7BO30MHaj1YPmfcEEkU6EKFWo,12693
-gcln2/__init__.py,sha256=CvmlBUZEbLZ_wgqB6nEfTYidXZWP-nE62luQ-bnyIS0,90
+gcln2/__init__.py,sha256=QmH3VzTJwX6QTvpcos81z4lFWuOpbnDzJsRmbsCMzX4,90
 gcln2/db.py,sha256=IzqT3jbdGFs-m1OBPHai3mQhYWqnQsX1pTM4DbcYWb0,9775
 gcln2/exceptions.py,sha256=GZbjPYBLS3FKSzXwOuiLv5b9ZNHFfldGUnZfOD8vOtE,51
 gcln2/helpers.py,sha256=D2HLZuRHy_3Z84NMzSVVbEBNc4PiaJ3oV8M_1yx6ikQ,9464
-gcln2/main.py,sha256=w3XJWUonCxGoHcX18H-x99i_fNNcCsgXevtFf-K5aD0,43383
+gcln2/main.py,sha256=gZ5qkiDa8zjjE9-kMPAEQkB7q-TvXR7b2yVcp_Ck9E0,43390
 gcln2/schema.py,sha256=ll1GukSVGqD-rhukuLw9zkvSgB6kSUaZVUQt9F4DAHY,2534
 gcln2/sync.py,sha256=I31SLm9Is8ESSfeQUIbf0zQtr8AB70wv7RcUr9E8L7U,25325
 gcln2/yaml_loader.py,sha256=D1pLV_hfr6roz1iit302pePns1z1UGjMN1mBL5FvK5Q,434
-gitcoll-0.0.20.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-gitcoll-0.0.20.dist-info/METADATA,sha256=lxDCcKuqR_5D3onA8_D46LOp_VqUxB9Wh9qTwUz5c10,12374
-gitcoll-0.0.20.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-gitcoll-0.0.20.dist-info/entry_points.txt,sha256=TAAvOpPYfpazo0L_xk795du7ctf-LHyNuzkaHobdrR4,72
-gitcoll-0.0.20.dist-info/top_level.txt,sha256=jwu689bt4chLp_WwR2BhqIzS1l5W88m0LZ-6fQurdY8,11
-gitcoll-0.0.20.dist-info/RECORD,,
+gitcoll-0.0.21.dist-info/LICENSE,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+gitcoll-0.0.21.dist-info/METADATA,sha256=SVKn0mq5XbhJN5qY-54cnaXM4fEDShPoHPZUMefXAhw,12374
+gitcoll-0.0.21.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+gitcoll-0.0.21.dist-info/entry_points.txt,sha256=TAAvOpPYfpazo0L_xk795du7ctf-LHyNuzkaHobdrR4,72
+gitcoll-0.0.21.dist-info/top_level.txt,sha256=jwu689bt4chLp_WwR2BhqIzS1l5W88m0LZ-6fQurdY8,11
+gitcoll-0.0.21.dist-info/RECORD,,
```

