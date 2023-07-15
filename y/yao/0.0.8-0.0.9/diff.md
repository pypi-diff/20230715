# Comparing `tmp/yao-0.0.8.tar.gz` & `tmp/yao-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yao-0.0.8.tar", last modified: Thu Jul  6 03:25:50 2023, max compression
+gzip compressed data, was "yao-0.0.9.tar", last modified: Sat Jul 15 07:34:57 2023, max compression
```

## Comparing `yao-0.0.8.tar` & `yao-0.0.9.tar`

### file list

```diff
@@ -1,57 +1,64 @@
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.044817 yao-0.0.8/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-07-06 03:25:50.044635 yao-0.0.8/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)       38 2023-07-06 03:25:50.044876 yao-0.0.8/setup.cfg
--rw-r--r--   0 ke         (501) wheel        (0)      971 2023-07-06 03:25:01.000000 yao-0.0.8/setup.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.038038 yao-0.0.8/yao/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.8/yao/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)    19955 2023-07-01 08:54:38.000000 yao-0.0.8/yao/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-05-04 09:42:20.000000 yao-0.0.8/yao/db.py
--rw-r--r--   0 ke         (501) wheel        (0)     8279 2023-05-04 09:42:20.000000 yao-0.0.8/yao/depends.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.039132 yao-0.0.8/yao/function/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/__init__.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.040001 yao-0.0.8/yao/function/annex/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/annex/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      187 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/annex/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/annex/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/annex/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.040660 yao-0.0.8/yao/function/appointment/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/appointment/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/appointment/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/appointment/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/appointment/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.041397 yao-0.0.8/yao/function/company/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/company/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      192 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/company/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/company/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/company/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.042351 yao-0.0.8/yao/function/department/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/department/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      189 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/department/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/department/main.py
--rw-r--r--   0 ke         (501) wheel        (0)      992 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/department/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.043003 yao-0.0.8/yao/function/log/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/log/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      169 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/log/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/log/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/log/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)      665 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     7973 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/model.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.043718 yao-0.0.8/yao/function/permission/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/permission/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)      199 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/permission/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/permission/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/permission/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.044412 yao-0.0.8/yao/function/user/
--rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/user/__init__.py
--rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/user/crud.py
--rw-r--r--   0 ke         (501) wheel        (0)    11211 2023-07-06 03:24:28.000000 yao-0.0.8/yao/function/user/main.py
--rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-05-04 09:42:20.000000 yao-0.0.8/yao/function/user/schema.py
--rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-05-04 09:42:20.000000 yao-0.0.8/yao/helpers.py
--rw-r--r--   0 ke         (501) wheel        (0)    12903 2023-06-28 03:18:34.000000 yao-0.0.8/yao/method.py
--rw-r--r--   0 ke         (501) wheel        (0)     2062 2023-05-12 09:17:23.000000 yao-0.0.8/yao/schema.py
-drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-06 03:25:50.038730 yao-0.0.8/yao.egg-info/
--rw-r--r--   0 ke         (501) wheel        (0)      433 2023-07-06 03:25:49.000000 yao-0.0.8/yao.egg-info/PKG-INFO
--rw-r--r--   0 ke         (501) wheel        (0)     1164 2023-07-06 03:25:50.000000 yao-0.0.8/yao.egg-info/SOURCES.txt
--rw-r--r--   0 ke         (501) wheel        (0)        1 2023-07-06 03:25:49.000000 yao-0.0.8/yao.egg-info/dependency_links.txt
--rw-r--r--   0 ke         (501) wheel        (0)      166 2023-07-06 03:25:49.000000 yao-0.0.8/yao.egg-info/requires.txt
--rw-r--r--   0 ke         (501) wheel        (0)        4 2023-07-06 03:25:49.000000 yao-0.0.8/yao.egg-info/top_level.txt
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.688459 yao-0.0.9/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-07-15 07:34:57.688268 yao-0.0.9/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)       38 2023-07-15 07:34:57.688505 yao-0.0.9/setup.cfg
+-rw-r--r--   0 ke         (501) wheel        (0)      971 2023-07-15 07:33:59.000000 yao-0.0.9/setup.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.680085 yao-0.0.9/yao/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.9/yao/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)    20042 2023-07-14 06:08:19.000000 yao-0.0.9/yao/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2211 2023-05-04 09:42:20.000000 yao-0.0.9/yao/db.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8279 2023-05-04 09:42:20.000000 yao-0.0.9/yao/depends.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.681330 yao-0.0.9/yao/function/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/__init__.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.682304 yao-0.0.9/yao/function/annex/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/annex/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      187 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/annex/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11202 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/annex/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1411 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/annex/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.683423 yao-0.0.9/yao/function/appointment/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/appointment/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1202 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/appointment/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4419 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/appointment/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1054 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/appointment/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.684036 yao-0.0.9/yao/function/company/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/company/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      192 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/company/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4071 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/company/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1249 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/company/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.684649 yao-0.0.9/yao/function/department/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/department/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      189 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/department/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4451 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/department/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)      992 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/department/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.685258 yao-0.0.9/yao/function/log/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/log/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      169 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/log/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3314 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/log/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1394 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/log/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)      746 2023-07-11 05:47:59.000000 yao-0.0.9/yao/function/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     9191 2023-07-14 09:34:53.000000 yao-0.0.9/yao/function/model.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.686061 yao-0.0.9/yao/function/permission/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/permission/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      199 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/permission/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     8271 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/permission/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2045 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/permission/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.687049 yao-0.0.9/yao/function/queue/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-02-18 01:09:21.000000 yao-0.0.9/yao/function/queue/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)      159 2023-07-11 03:59:04.000000 yao-0.0.9/yao/function/queue/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4092 2023-07-15 07:22:22.000000 yao-0.0.9/yao/function/queue/helper.py
+-rw-r--r--   0 ke         (501) wheel        (0)     4166 2023-07-11 04:00:10.000000 yao-0.0.9/yao/function/queue/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2210 2023-07-15 06:31:12.000000 yao-0.0.9/yao/function/queue/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)      547 2023-07-12 01:15:42.000000 yao-0.0.9/yao/function/queue/type.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.687980 yao-0.0.9/yao/function/user/
+-rw-r--r--   0 ke         (501) wheel        (0)        0 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/user/__init__.py
+-rw-r--r--   0 ke         (501) wheel        (0)     1364 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/user/crud.py
+-rw-r--r--   0 ke         (501) wheel        (0)    11188 2023-07-06 02:56:41.000000 yao-0.0.9/yao/function/user/main.py
+-rw-r--r--   0 ke         (501) wheel        (0)     3083 2023-05-04 09:42:20.000000 yao-0.0.9/yao/function/user/schema.py
+-rw-r--r--   0 ke         (501) wheel        (0)     6842 2023-05-04 09:42:20.000000 yao-0.0.9/yao/helpers.py
+-rw-r--r--   0 ke         (501) wheel        (0)    12903 2023-06-28 03:18:34.000000 yao-0.0.9/yao/method.py
+-rw-r--r--   0 ke         (501) wheel        (0)     2062 2023-05-12 09:17:23.000000 yao-0.0.9/yao/schema.py
+drwxr-xr-x   0 ke         (501) wheel        (0)        0 2023-07-15 07:34:57.680759 yao-0.0.9/yao.egg-info/
+-rw-r--r--   0 ke         (501) wheel        (0)      433 2023-07-15 07:34:57.000000 yao-0.0.9/yao.egg-info/PKG-INFO
+-rw-r--r--   0 ke         (501) wheel        (0)     1334 2023-07-15 07:34:57.000000 yao-0.0.9/yao.egg-info/SOURCES.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        1 2023-07-15 07:34:57.000000 yao-0.0.9/yao.egg-info/dependency_links.txt
+-rw-r--r--   0 ke         (501) wheel        (0)      166 2023-07-15 07:34:57.000000 yao-0.0.9/yao.egg-info/requires.txt
+-rw-r--r--   0 ke         (501) wheel        (0)        4 2023-07-15 07:34:57.000000 yao-0.0.9/yao.egg-info/top_level.txt
```

### Comparing `yao-0.0.8/setup.py` & `yao-0.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("readme.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="yao",
-    version="0.0.8",
+    version="0.0.9",
     description="Dev",
     python_requires=">=3.6",
     author="Lsshu",
     author_email="admin@lsshu.cn",
     url="https://github.com/lsshu/yao",
     packages=find_packages(),
     long_description=long_description,
```

### Comparing `yao-0.0.8/yao/crud.py` & `yao-0.0.9/yao/crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -427,21 +427,22 @@
 
         response = [session.delete(u) for u in self.query.all()] if event else self.query.delete()
 
         commit and session.commit()
         close and session.close()
         return response
 
-    def update_or_store_model(self, session, where=None, item: BaseModel = None, data: dict = None, commit: bool = True, refresh: bool = True, close: bool = False,
-                              exclude_unset: bool = True, event: bool = False, update_event: bool = False, **kwargs):
+    def update_or_store_model(self, session, where=None, item: BaseModel = None, store_item: BaseModel = None, data: dict = None, commit: bool = True, refresh: bool = True,
+                              close: bool = False, exclude_unset: bool = True, event: bool = False, update_event: bool = False, **kwargs):
         """
         更新或者创建
         :param session:
         :param where:
         :param item:
+        :param store_item:
         :param data:
         :param commit:
         :param refresh:
         :param close:
         :param exclude_unset:
         :param event:
         :param update_event:
@@ -449,15 +450,15 @@
         :return:
         """
         instance = self.first(session=session, where=where, **kwargs)
         if instance:
             return self.update(session=session, item=item, data=data, pk=getattr(instance, self.model_pk), exclude_unset=exclude_unset, commit=commit, refresh=refresh, close=close,
                                event=update_event, **kwargs)
         else:
-            return self.store(session=session, item=item, data=data, commit=commit, refresh=refresh, close=close, event=event, **kwargs)
+            return self.store(session=session, item=store_item if store_item else item, data=data, commit=commit, refresh=refresh, close=close, event=event, **kwargs)
 
     def find_or_store_model(self, session, where=None, item: BaseModel = None, data: dict = None, commit: bool = True, refresh: bool = True, close: bool = False, **kwargs):
         """
         查找或者创建
         :param session:
         :param where:
         :param item:
```

### Comparing `yao-0.0.8/yao/db.py` & `yao-0.0.9/yao/db.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/depends.py` & `yao-0.0.9/yao/depends.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/annex/main.py` & `yao-0.0.9/yao/function/annex/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/annex/schema.py` & `yao-0.0.9/yao/function/annex/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/appointment/crud.py` & `yao-0.0.9/yao/function/appointment/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/appointment/main.py` & `yao-0.0.9/yao/function/appointment/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/appointment/schema.py` & `yao-0.0.9/yao/function/appointment/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/company/main.py` & `yao-0.0.9/yao/function/company/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/company/schema.py` & `yao-0.0.9/yao/function/company/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/department/main.py` & `yao-0.0.9/yao/function/department/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/department/schema.py` & `yao-0.0.9/yao/function/department/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/log/main.py` & `yao-0.0.9/yao/function/log/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/log/schema.py` & `yao-0.0.9/yao/function/log/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/main.py` & `yao-0.0.9/yao/function/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,16 +3,18 @@
 from yao.function.company.main import router as company
 from yao.function.user.main import router as user
 from yao.function.permission.main import router as permission
 from yao.function.appointment.main import router as appointment
 from yao.function.department.main import router as department
 from yao.function.annex.main import router as annex
 from yao.function.log.main import router as log
+from yao.function.queue.main import router as queue
 
 router = APIRouter()
 router.include_router(company)
 router.include_router(user)
 router.include_router(permission)
 router.include_router(appointment)
 router.include_router(department)
 router.include_router(annex)
 router.include_router(log)
+router.include_router(queue)
```

### Comparing `yao-0.0.8/yao/function/model.py` & `yao-0.0.9/yao/function/model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from sqlalchemy import Column, String, Boolean, Text, Integer, ForeignKey, event, Table, JSON
+from sqlalchemy import Column, String, Boolean, Text, Integer, ForeignKey, event, Table, JSON, TIMESTAMP
 from sqlalchemy.orm import relationship, declared_attr
 from sqlalchemy_mptt.mixins import BaseNestedSets
 
 from yao.method import plural
 from yao.db import Model, Engine
 
 name = __name__[:__name__.rfind(".")].capitalize()
@@ -34,28 +34,33 @@
 function_annex_name = plural("%s.annex" % name)
 function_annex_table_name = function_annex_name.replace('.', '_')
 
 """日志"""
 function_log_name = plural("%s.log" % name)
 function_log_table_name = function_log_name.replace('.', '_')
 
+"""队列"""
+function_queue_name = plural("%s.queue" % name)
+function_queue_table_name = function_queue_name.replace('.', '_')
+
 SYSTEM_PERMISSIONS = [
     {
         "name": "职能信息",
         "scope": function_name,
         "icon": "ElementPlus",
         "children": [
             {"name": "公司信息", "scope": function_company_name, "icon": "Refrigerator"},
             {"name": "公司部门", "scope": function_department_name, "icon": "Help"},
             {"name": "员工职位", "scope": function_appointment_name, "icon": "User"},
             {"name": "权限管理", "scope": function_permission_name, "icon": "KnifeFork", "is_menu": False,
              "action": [{"name": "菜单", "scope": "menus"}, {"name": "树", "scope": "tree"}]},
             {"name": "后台账号", "scope": function_user_name, "icon": "User"},
             {"name": "附件文件", "scope": function_annex_name, "icon": "Folder", "is_menu": False},
             {"name": "操作日志", "scope": function_log_name, "icon": "Document"},
+            {"name": "后台队列", "scope": function_queue_name, "icon": "Finished"},
         ]
     }
 ]
 
 
 class BaseModel(Model):
     __abstract__ = True
@@ -168,7 +173,23 @@
 class ModelFunctionLogs(BaseCompanyModel):
     """ 日志 """
     __tablename__ = function_log_table_name
     scope = Column(String(100), nullable=True, comment="scope")
     methods = Column(String(32), nullable=True, comment="methods", index=True)
     data = Column(JSON, nullable=True, comment="Data")
     username = Column(String(32), ForeignKey("%s.username" % function_user_table_name, onupdate="CASCADE", ondelete="CASCADE"), index=True, nullable=True, comment="用户")
+
+
+class ModelFunctionQueues(BaseCompanyModel):
+    """队列"""
+    __tablename__ = function_queue_table_name
+    username = Column(String(32), ForeignKey("%s.username" % function_user_table_name, onupdate="CASCADE", ondelete="CASCADE"), index=True, nullable=True, comment="用户")
+    priority = Column(Integer, nullable=True, comment="优先级 小的最高")
+    scope = Column(String(100), nullable=True, comment="scope")
+    data = Column(JSON, nullable=True, comment="Data")
+    key = Column(Text, nullable=True, comment="去重Key")
+    start_at = Column(TIMESTAMP, nullable=True, comment="开始时间")
+    stop_at = Column(TIMESTAMP, nullable=True, comment="结束时间")
+    progress = Column(String(8), nullable=True, comment="进度条")
+    progress_text = Column(String(100), nullable=True, comment="进度条")
+    retry = Column(Integer, nullable=True, comment="重试次数")
+    queue_status = Column(Integer, nullable=True, comment="状态 0未运行 1成功 2失败")
```

### Comparing `yao-0.0.8/yao/function/permission/main.py` & `yao-0.0.9/yao/function/permission/main.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/permission/schema.py` & `yao-0.0.9/yao/function/permission/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/user/crud.py` & `yao-0.0.9/yao/function/user/crud.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/function/user/main.py` & `yao-0.0.9/yao/function/user/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     """
     验证用户信息
     :param session:
     :param username:
     :param password:
     :return:
     """
-    user = CrudFunctionUser.init().first(session=session, where=[("username", username), ("available", True)])
+    user = CrudFunctionUser.init().first(session=session, where=("username", username))
     if not user or not token_verify_password(plain_password=password, hashed_password=user.password):
         raise HTTPException(status_code=status.HTTP_400_BAD_REQUEST, detail="账号或者密码不正确！")
     return user
 
 
 def token_authenticate_access_token(session, username: str, password: str, scopes: list) -> str:
     """
```

### Comparing `yao-0.0.8/yao/function/user/schema.py` & `yao-0.0.9/yao/function/user/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/helpers.py` & `yao-0.0.9/yao/helpers.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/method.py` & `yao-0.0.9/yao/method.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao/schema.py` & `yao-0.0.9/yao/schema.py`

 * *Files identical despite different names*

### Comparing `yao-0.0.8/yao.egg-info/SOURCES.txt` & `yao-0.0.9/yao.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -34,11 +34,17 @@
 yao/function/log/crud.py
 yao/function/log/main.py
 yao/function/log/schema.py
 yao/function/permission/__init__.py
 yao/function/permission/crud.py
 yao/function/permission/main.py
 yao/function/permission/schema.py
+yao/function/queue/__init__.py
+yao/function/queue/crud.py
+yao/function/queue/helper.py
+yao/function/queue/main.py
+yao/function/queue/schema.py
+yao/function/queue/type.py
 yao/function/user/__init__.py
 yao/function/user/crud.py
 yao/function/user/main.py
 yao/function/user/schema.py
```

