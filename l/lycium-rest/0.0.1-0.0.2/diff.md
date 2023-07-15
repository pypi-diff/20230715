# Comparing `tmp/lycium-rest-0.0.1.tar.gz` & `tmp/lycium-rest-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycium-rest-0.0.1.tar", last modified: Sun Dec 18 13:08:28 2022, max compression
+gzip compressed data, was "lycium-rest-0.0.2.tar", last modified: Sat Jul 15 17:25:26 2023, max compression
```

## Comparing `lycium-rest-0.0.1.tar` & `lycium-rest-0.0.2.tar`

### file list

```diff
@@ -1,46 +1,49 @@
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.709263 lycium-rest-0.0.1/
--rw-r--r--   0 kevin      (501) staff       (20)    35149 2022-12-14 17:24:33.000000 lycium-rest-0.0.1/LICENSE
--rw-r--r--   0 kevin      (501) staff       (20)       33 2022-12-18 12:55:50.000000 lycium-rest-0.0.1/MANIFEST.in
--rw-r--r--   0 kevin      (501) staff       (20)      590 2022-12-18 13:08:28.708644 lycium-rest-0.0.1/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)      148 2022-12-14 17:24:33.000000 lycium-rest-0.0.1/README.md
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.573050 lycium-rest-0.0.1/lycium_rest/
--rw-r--r--   0 kevin      (501) staff       (20)      942 2022-12-14 17:28:25.000000 lycium-rest-0.0.1/lycium_rest/__init__.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.593059 lycium-rest-0.0.1/lycium_rest/formvalidation/
--rw-r--r--   0 kevin      (501) staff       (20)       46 2022-12-14 17:25:24.000000 lycium-rest-0.0.1/lycium_rest/formvalidation/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     2476 2022-12-17 16:25:28.000000 lycium-rest-0.0.1/lycium_rest/formvalidation/formutils.py
--rw-r--r--   0 kevin      (501) staff       (20)     9981 2022-12-17 15:10:46.000000 lycium-rest-0.0.1/lycium_rest/formvalidation/validators.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.686956 lycium-rest-0.0.1/lycium_rest/locales/
--rw-r--r--   0 kevin      (501) staff       (20)      675 2022-12-14 17:25:24.000000 lycium-rest-0.0.1/lycium_rest/locales/basic.en_US.yml
--rw-r--r--   0 kevin      (501) staff       (20)      620 2022-12-14 17:25:24.000000 lycium-rest-0.0.1/lycium_rest/locales/basic.zh_CN.yml
--rw-r--r--   0 kevin      (501) staff       (20)     3540 2022-12-15 01:13:58.000000 lycium-rest-0.0.1/lycium_rest/migrationutils.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.687791 lycium-rest-0.0.1/lycium_rest/model/
--rw-r--r--   0 kevin      (501) staff       (20)       46 2022-12-15 01:08:24.000000 lycium-rest-0.0.1/lycium_rest/model/__init__.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.691572 lycium-rest-0.0.1/lycium_rest/model/supports/
--rw-r--r--   0 kevin      (501) staff       (20)      176 2022-12-14 17:25:25.000000 lycium-rest-0.0.1/lycium_rest/model/supports/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)      711 2022-12-14 17:25:25.000000 lycium-rest-0.0.1/lycium_rest/model/supports/migration.py
--rw-r--r--   0 kevin      (501) staff       (20)      944 2022-12-15 01:13:15.000000 lycium-rest-0.0.1/lycium_rest/model/supports/migration_progress.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.698742 lycium-rest-0.0.1/lycium_rest/restfulwrapper/
--rw-r--r--   0 kevin      (501) staff       (20)     2329 2022-12-18 10:12:47.000000 lycium-rest-0.0.1/lycium_rest/restfulwrapper/__init__.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.700741 lycium-rest-0.0.1/lycium_rest/restfulwrapper/accesscontrol/
--rw-r--r--   0 kevin      (501) staff       (20)       46 2022-12-14 17:25:25.000000 lycium-rest-0.0.1/lycium_rest/restfulwrapper/accesscontrol/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)      468 2022-12-14 17:25:25.000000 lycium-rest-0.0.1/lycium_rest/restfulwrapper/accesscontrol/authorizedsession.py
--rw-r--r--   0 kevin      (501) staff       (20)    15166 2022-12-18 07:07:36.000000 lycium-rest-0.0.1/lycium_rest/restfulwrapper/modelapihandlers.py
--rw-r--r--   0 kevin      (501) staff       (20)    15447 2022-12-18 09:28:48.000000 lycium-rest-0.0.1/lycium_rest/restfulwrapper/modelrelationhandlers.py
--rw-r--r--   0 kevin      (501) staff       (20)     2562 2022-12-18 10:12:11.000000 lycium-rest-0.0.1/lycium_rest/restfulwrapper/pagedescriptorhandlers.py
--rw-r--r--   0 kevin      (501) staff       (20)     6726 2022-12-18 12:45:23.000000 lycium-rest-0.0.1/lycium_rest/restfulwrapper/register.py
--rw-r--r--   0 kevin      (501) staff       (20)     4992 2022-12-18 12:43:08.000000 lycium-rest-0.0.1/lycium_rest/restfulwrapper/restdescriptor.py
--rw-r--r--   0 kevin      (501) staff       (20)     9251 2022-12-17 16:29:27.000000 lycium-rest-0.0.1/lycium_rest/restfulwrapper/utils.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.701672 lycium-rest-0.0.1/lycium_rest/utilities/
--rw-r--r--   0 kevin      (501) staff       (20)      666 2022-12-15 01:11:45.000000 lycium-rest-0.0.1/lycium_rest/utilities/__init__.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.706961 lycium-rest-0.0.1/lycium_rest/valueobjects/
--rw-r--r--   0 kevin      (501) staff       (20)      250 2022-12-14 17:25:52.000000 lycium-rest-0.0.1/lycium_rest/valueobjects/__init__.py
--rw-r--r--   0 kevin      (501) staff       (20)     1612 2022-12-15 01:09:23.000000 lycium-rest-0.0.1/lycium_rest/valueobjects/responseobject.py
--rw-r--r--   0 kevin      (501) staff       (20)      582 2022-12-14 17:25:52.000000 lycium-rest-0.0.1/lycium_rest/valueobjects/resultcodes.py
-drwxr-xr-x   0 kevin      (501) staff       (20)        0 2022-12-18 13:08:28.584426 lycium-rest-0.0.1/lycium_rest.egg-info/
--rw-r--r--   0 kevin      (501) staff       (20)      590 2022-12-18 13:08:28.000000 lycium-rest-0.0.1/lycium_rest.egg-info/PKG-INFO
--rw-r--r--   0 kevin      (501) staff       (20)     1196 2022-12-18 13:08:28.000000 lycium-rest-0.0.1/lycium_rest.egg-info/SOURCES.txt
--rw-r--r--   0 kevin      (501) staff       (20)        1 2022-12-18 13:08:28.000000 lycium-rest-0.0.1/lycium_rest.egg-info/dependency_links.txt
--rw-r--r--   0 kevin      (501) staff       (20)       82 2022-12-18 13:08:28.000000 lycium-rest-0.0.1/lycium_rest.egg-info/requires.txt
--rw-r--r--   0 kevin      (501) staff       (20)       12 2022-12-18 13:08:28.000000 lycium-rest-0.0.1/lycium_rest.egg-info/top_level.txt
--rw-r--r--   0 kevin      (501) staff       (20)       38 2022-12-18 13:08:28.709442 lycium-rest-0.0.1/setup.cfg
--rw-r--r--   0 kevin      (501) staff       (20)     1013 2022-12-18 12:50:28.000000 lycium-rest-0.0.1/setup.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:26.271318 lycium-rest-0.0.2/
+-rw-r--r--   0 kevin      (501) staff       (20)    35149 2022-12-14 17:24:33.000000 lycium-rest-0.0.2/LICENSE
+-rw-r--r--   0 kevin      (501) staff       (20)       33 2022-12-18 12:55:50.000000 lycium-rest-0.0.2/MANIFEST.in
+-rw-r--r--   0 kevin      (501) staff       (20)      590 2023-07-15 17:25:26.270745 lycium-rest-0.0.2/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)      148 2022-12-14 17:24:33.000000 lycium-rest-0.0.2/README.md
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:25.261898 lycium-rest-0.0.2/lycium_rest/
+-rw-r--r--   0 kevin      (501) staff       (20)      942 2022-12-14 17:28:25.000000 lycium-rest-0.0.2/lycium_rest/__init__.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:25.474439 lycium-rest-0.0.2/lycium_rest/formvalidation/
+-rw-r--r--   0 kevin      (501) staff       (20)      170 2023-07-09 02:44:38.000000 lycium-rest-0.0.2/lycium_rest/formvalidation/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      855 2023-07-15 16:25:40.000000 lycium-rest-0.0.2/lycium_rest/formvalidation/formitemprops.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2476 2022-12-17 16:25:28.000000 lycium-rest-0.0.2/lycium_rest/formvalidation/formutils.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1793 2023-07-09 03:17:36.000000 lycium-rest-0.0.2/lycium_rest/formvalidation/modifyingbeheviorformfields.py
+-rw-r--r--   0 kevin      (501) staff       (20)    10686 2023-07-01 15:25:25.000000 lycium-rest-0.0.2/lycium_rest/formvalidation/validators.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:25.555899 lycium-rest-0.0.2/lycium_rest/locales/
+-rw-r--r--   0 kevin      (501) staff       (20)      803 2023-01-11 09:21:26.000000 lycium-rest-0.0.2/lycium_rest/locales/basic.en_US.yml
+-rw-r--r--   0 kevin      (501) staff       (20)      994 2023-06-29 13:55:43.000000 lycium-rest-0.0.2/lycium_rest/locales/basic.zh_CN.yml
+-rw-r--r--   0 kevin      (501) staff       (20)     3540 2022-12-15 01:13:58.000000 lycium-rest-0.0.2/lycium_rest/migrationutils.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:25.639017 lycium-rest-0.0.2/lycium_rest/model/
+-rw-r--r--   0 kevin      (501) staff       (20)       46 2022-12-15 01:08:24.000000 lycium-rest-0.0.2/lycium_rest/model/__init__.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:25.797719 lycium-rest-0.0.2/lycium_rest/model/supports/
+-rw-r--r--   0 kevin      (501) staff       (20)      176 2022-12-14 17:25:25.000000 lycium-rest-0.0.2/lycium_rest/model/supports/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      711 2022-12-14 17:25:25.000000 lycium-rest-0.0.2/lycium_rest/model/supports/migration.py
+-rw-r--r--   0 kevin      (501) staff       (20)      944 2022-12-15 01:13:15.000000 lycium-rest-0.0.2/lycium_rest/model/supports/migration_progress.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:25.967081 lycium-rest-0.0.2/lycium_rest/restfulwrapper/
+-rw-r--r--   0 kevin      (501) staff       (20)     3536 2023-07-11 17:57:44.000000 lycium-rest-0.0.2/lycium_rest/restfulwrapper/__init__.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:26.052409 lycium-rest-0.0.2/lycium_rest/restfulwrapper/accesscontrol/
+-rw-r--r--   0 kevin      (501) staff       (20)       46 2022-12-14 17:25:25.000000 lycium-rest-0.0.2/lycium_rest/restfulwrapper/accesscontrol/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)      474 2023-07-06 14:53:34.000000 lycium-rest-0.0.2/lycium_rest/restfulwrapper/accesscontrol/authorizedsession.py
+-rw-r--r--   0 kevin      (501) staff       (20)    20306 2023-07-09 04:01:59.000000 lycium-rest-0.0.2/lycium_rest/restfulwrapper/modelapihandlers.py
+-rw-r--r--   0 kevin      (501) staff       (20)    16178 2023-07-09 04:35:42.000000 lycium-rest-0.0.2/lycium_rest/restfulwrapper/modelrelationhandlers.py
+-rw-r--r--   0 kevin      (501) staff       (20)     2938 2023-06-29 12:58:21.000000 lycium-rest-0.0.2/lycium_rest/restfulwrapper/pagedescriptorhandlers.py
+-rw-r--r--   0 kevin      (501) staff       (20)     5900 2022-12-28 01:51:11.000000 lycium-rest-0.0.2/lycium_rest/restfulwrapper/register.py
+-rw-r--r--   0 kevin      (501) staff       (20)    12903 2023-07-15 16:26:16.000000 lycium-rest-0.0.2/lycium_rest/restfulwrapper/restdescriptor.py
+-rw-r--r--   0 kevin      (501) staff       (20)    10350 2023-07-09 04:04:15.000000 lycium-rest-0.0.2/lycium_rest/restfulwrapper/utils.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:26.113143 lycium-rest-0.0.2/lycium_rest/utilities/
+-rw-r--r--   0 kevin      (501) staff       (20)      676 2023-01-03 09:54:51.000000 lycium-rest-0.0.2/lycium_rest/utilities/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1244 2022-12-27 09:06:45.000000 lycium-rest-0.0.2/lycium_rest/utilities/treedata.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:26.269780 lycium-rest-0.0.2/lycium_rest/valueobjects/
+-rw-r--r--   0 kevin      (501) staff       (20)      326 2023-06-29 13:50:35.000000 lycium-rest-0.0.2/lycium_rest/valueobjects/__init__.py
+-rw-r--r--   0 kevin      (501) staff       (20)     1612 2022-12-15 01:09:23.000000 lycium-rest-0.0.2/lycium_rest/valueobjects/responseobject.py
+-rw-r--r--   0 kevin      (501) staff       (20)      582 2022-12-14 17:25:52.000000 lycium-rest-0.0.2/lycium_rest/valueobjects/resultcodes.py
+drwxr-xr-x   0 kevin      (501) staff       (20)        0 2023-07-15 17:25:25.363596 lycium-rest-0.0.2/lycium_rest.egg-info/
+-rw-r--r--   0 kevin      (501) staff       (20)      590 2023-07-15 17:25:24.000000 lycium-rest-0.0.2/lycium_rest.egg-info/PKG-INFO
+-rw-r--r--   0 kevin      (501) staff       (20)     1332 2023-07-15 17:25:24.000000 lycium-rest-0.0.2/lycium_rest.egg-info/SOURCES.txt
+-rw-r--r--   0 kevin      (501) staff       (20)        1 2023-07-15 17:25:24.000000 lycium-rest-0.0.2/lycium_rest.egg-info/dependency_links.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       82 2023-07-15 17:25:24.000000 lycium-rest-0.0.2/lycium_rest.egg-info/requires.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       12 2023-07-15 17:25:24.000000 lycium-rest-0.0.2/lycium_rest.egg-info/top_level.txt
+-rw-r--r--   0 kevin      (501) staff       (20)       38 2023-07-15 17:25:26.271501 lycium-rest-0.0.2/setup.cfg
+-rw-r--r--   0 kevin      (501) staff       (20)     1013 2023-06-29 12:58:46.000000 lycium-rest-0.0.2/setup.py
```

### Comparing `lycium-rest-0.0.1/LICENSE` & `lycium-rest-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lycium-rest-0.0.1/PKG-INFO` & `lycium-rest-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lycium-rest
-Version: 0.0.1
+Version: 0.0.2
 Summary: common python programing encapsulation library
 Home-page: https://github.com/libpub/lycium-rest
 Author: kevinyjn
 Author-email: kevinyjn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lycium-rest-0.0.1/lycium_rest/__init__.py` & `lycium-rest-0.0.2/lycium_rest/__init__.py`

 * *Files identical despite different names*

### Comparing `lycium-rest-0.0.1/lycium_rest/formvalidation/formutils.py` & `lycium-rest-0.0.2/lycium_rest/formvalidation/formutils.py`

 * *Files identical despite different names*

### Comparing `lycium-rest-0.0.1/lycium_rest/formvalidation/validators.py` & `lycium-rest-0.0.2/lycium_rest/formvalidation/validators.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 from wtforms.validators import StopValidation, ValidationError, Regexp
+import asyncio
 from hawthorn.dbproxy import DbProxy
 from hawthorn.modelutils import ModelBase, MongoBase
 from hawthorn.utilities import toint, tofloat
 
 class DataExistsValidator(object):
     """
     验证数据是否存在
@@ -37,15 +38,15 @@
         self.union_field = union_field
         self.fixed_field = fixed_field or {}
         self.message = message
         self.should_exists = should_exists
         self.allows_empty = allows_empty
         self.ignore_obsoleted = ignore_obsoleted
 
-    async def __call__(self, form, field):
+    def __call__(self, form, field):
         if not field.data or isinstance(field.data, str) and not field.data.strip():
             if self.allows_empty:
                 return
             if self.message is None:
                 message = field.gettext('This field is required.')
             else:
                 message = self.message
@@ -69,15 +70,15 @@
                 if primary:
                     mongo_condition[self.primary_field + '__ne'] = primary
                 if union:
                     for u in union:
                         if u.get('field') and u.get('data'):
                             mongo_condition[u.get('field')] = u.get('data')
                 try:
-                    val = await DbProxy().query_all_mongo(model, mongo_condition)
+                    val = self.fetch_async_result(DbProxy().query_all_mongo(model, mongo_condition))
                 except Exception as e:
                     field.errors[:] = []
                     raise StopValidation(str(e))
             elif issubclass(model, ModelBase):
                 pg_condition = [getattr(model, index_field) == field.data]
                 if self.fixed_field:
                     for key, value in self.fixed_field.items():
@@ -89,15 +90,15 @@
                 if primary:
                     pg_condition.append(getattr(model, self.primary_field) != primary)
                 if union:
                     for u in union:
                         if u.get('field') and u.get('data'):
                             pg_condition.append(getattr(model, u.get('field')) == u.get('data'))
                 try:
-                    val = await DbProxy().find_item(model, pg_condition)
+                    val = self.fetch_async_result(DbProxy().find_item(model, pg_condition))
                 except Exception as e:
                     field.errors[:] = []
                     raise StopValidation(str(e))
 
             message = None
             if self.should_exists:
                 if not val:
@@ -111,15 +112,15 @@
                         message = self.message
                     else:
                         message = field.gettext('The data should not exists.')
 
             if message:
                 field.errors[:] = []
                 raise StopValidation(message)
-    
+        
     def get_validate_model(self, form):
         model = self.model
         if isinstance(model, dict):
             if getattr(form, self.reference_field).data in model:
                 model = model[getattr(form, self.reference_field).data]
             else:
                 return None
@@ -139,14 +140,19 @@
         if isinstance(name_field, dict):
             if getattr(form, self.reference_field).data in name_field:
                 name_field = name_field[getattr(form, self.reference_field).data]
             else:
                 return None
         return name_field
     
+    def fetch_async_result(self, async_task):
+        # IOLoop.current()._ioloop_for_asyncio()
+        val = asyncio.get_event_loop().run_until_complete(async_task)
+        return val
+    
 class DataDictsValidator(object):
     """
     验证数据字典是否合法，并可根据字典值为名称为数据查询拼装名称
 
     :param dicts:
         The dict to be checked.
     :param message:
@@ -235,26 +241,43 @@
 
     :param regex:
         The regular expression string to use. Can also be a compiled regular
         expression pattern.
     :param flags:
         The regexp flags to use, for example re.IGNORECASE. Ignored if
         `regex` is not a string.
+    :param allow_empty:
+        If the field allows empty
     :param message:
         Error message to raise in case of a validation error.
     """
 
-    def __init__(self, regex=r'^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$', flags=0, message=None):
+    def __init__(self, regex=r'^\d{4}-\d{2}-\d{2} \d{2}:\d{2}:\d{2}$', flags=0, allow_empty=False, message=None):
         super().__init__(regex, flags, message)
+        self.allow_empty = allow_empty
 
     def __call__(self, form, field, message=None):
+        if self.allow_empty and not field.data:
+            return True
         match = self.regex.match(field.data or "")
         if match:
             return match
 
         if message is None:
             if self.message is None:
                 message = field.gettext("Invalid datetime format.")
             else:
                 message = self.message
 
         raise ValidationError(message)
+
+class DefaultValue():
+    """Specifies default value for input field
+    """
+    
+    def __init__(self, value: any):
+        self.value = value
+
+    def __call__(self, form, field, message=None):
+        if field.data is None:
+            field.data = self.value
+
```

### Comparing `lycium-rest-0.0.1/lycium_rest/migrationutils.py` & `lycium-rest-0.0.2/lycium_rest/migrationutils.py`

 * *Files identical despite different names*

### Comparing `lycium-rest-0.0.1/lycium_rest/model/supports/migration.py` & `lycium-rest-0.0.2/lycium_rest/model/supports/migration.py`

 * *Files identical despite different names*

### Comparing `lycium-rest-0.0.1/lycium_rest/model/supports/migration_progress.py` & `lycium-rest-0.0.2/lycium_rest/model/supports/migration_progress.py`

 * *Files identical despite different names*

### Comparing `lycium-rest-0.0.1/lycium_rest/restfulwrapper/modelapihandlers.py` & `lycium-rest-0.0.2/lycium_rest/restfulwrapper/modelapihandlers.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,33 +13,46 @@
 from typing import Iterable
 from wtforms import Form
 from hawthorn.asynchttphandler import GeneralTornadoHandler, request_body_as_json
 from hawthorn.session import TornadoSession
 from hawthorn.exceptionreporter import ExceptionReporter
 from hawthorn.modelutils import ModelBase, model_columns, get_model_class_name
 from hawthorn.dbproxy import DbProxy
+from hawthorn.utilities import pascal_case
+from ..utilities.treedata import format_items_as_tree
 from . import SESSION_UID_KEY
 from ..formvalidation.formutils import validate_form, save_form_fields
 from ..valueobjects.resultcodes import RESULT_CODE
 from ..valueobjects.responseobject import GeneralResponseObject, ListResponseObject
 
-from .utils import format_model_query_conditions, dump_model_data, read_request_parameters, get_locale_params, get_listquery_pager_info, get_listquery_sort_info
+from .utils import format_model_query_conditions, format_column_name_mappings, dump_model_data, read_request_parameters, get_locale_params, get_listquery_pager_info, get_listquery_sort_info
 
 LOG = logging.getLogger('services.generalmodelapi.apihandlers')
 
 class ModelRESTfulHandler(tornado.web.RequestHandler):
     """
     Model API handler wrapper
     """
-    def initialize(self, model: ModelBase, form: Form = None, ac=[]):
+    def initialize(self, model: ModelBase, form: Form = None, ac=[], auto_association: str|list[str]=None):
         self.model = model
         self.form = form
         self._ac = []
         self.session = TornadoSession(self)
         self.set_access_control(ac)
+        self.find_one_keys = {'fetchOne': True, 'findOne': True}
+        self.auto_association_keys = {}
+        if auto_association:
+            if isinstance(auto_association, str):
+                self.auto_association_keys['fetchTree'] = auto_association
+            elif isinstance(auto_association, list):
+                if len(auto_association) == 1:
+                    self.auto_association_keys['fetchTree'] = auto_association[0]
+                else:
+                    for k in auto_association:
+                        self.auto_association_keys['fetchTreeBy' + pascal_case(k)] = k
 
     def set_access_control(self, ac):
         self._ac = []
         if ac:
             if isinstance(ac, list):
                 for f in ac:
                     if callable(f):
@@ -91,81 +104,44 @@
     async def get(self, id: str|int = None):
         """
         API handler of get single model data
         """
         filters = read_request_parameters(self.request)
         locale_params = get_locale_params(self.request)
         if id:
-            columns, pk = model_columns(self.model)
-            if id not in ['fetchOne', 'findOne']:
-                filters[pk] = id
-            result = GeneralResponseObject(RESULT_CODE.DATA_DOES_NOT_EXISTS, message=i18n.t('basic.data_not_exists', **locale_params))
-            while result.code != RESULT_CODE.OK:
-                filter_conds, err_msg = format_model_query_conditions(self.model, filters=filters)
-                if err_msg:
-                    result.code = RESULT_CODE.INVALID_PARAM
-                    result.message = err_msg
+            if id in self.auto_association_keys:
+                result = await self.do_get_tree_list(id, filters, locale_params)
+            else:
+                columns, pk = model_columns(self.model)
+                if id not in self.find_one_keys:
+                    filters[pk] = id
+                result = GeneralResponseObject(RESULT_CODE.DATA_DOES_NOT_EXISTS, message=i18n.t('basic.data_not_exists', **locale_params))
+                while result.code != RESULT_CODE.OK:
+                    filter_conds, err_msg = format_model_query_conditions(self.model, filters=filters)
+                    if err_msg:
+                        result.code = RESULT_CODE.INVALID_PARAM
+                        result.message = err_msg
+                        break
+
+                    m = await DbProxy().find_item(self.model, filters=filter_conds)
+                    if m:
+                        result.code = RESULT_CODE.OK
+                        result.message = i18n.t('basic.success', **locale_params)
+                        if hasattr(m, 'as_dict'):
+                            result.data = getattr(m, 'as_dict')()
+                        else:
+                            result.data = dump_model_data(m, columns=columns, column_name_mapping=format_column_name_mappings(self.form))
                     break
-
-                m = await DbProxy().find_item(self.model, filters=filter_conds)
-                if m:
-                    result.code = RESULT_CODE.OK
-                    result.message = i18n.t('basic.success', **locale_params)
-                    if hasattr(m, 'as_dict'):
-                        result.data = getattr(m, 'as_dict')()
-                    else:
-                        result.data = dump_model_data(m, columns=columns)
-                break
         else:
             result = await self.do_get_list(filters, locale_params)
         
         self.set_header('Content-Type', 'application/json')
         self.write(result.encode_json())
         self.finish()
 
-    async def do_get_list(self, params: dict, locale_params: dict):
-        """
-        API handler of get model list data by filter condition and pagination
-        """
-        filters = params.get('filter', {})
-        fields = params.get('fields', [])
-        if not filters or not isinstance(filters, dict):
-            filters = {}
-        limit, offset = get_listquery_pager_info(params)
-        orderby, direction = get_listquery_sort_info(params)
-
-        result = ListResponseObject(RESULT_CODE.DATA_DOES_NOT_EXISTS, message=i18n.t('basic.data_not_exists', **locale_params))
-        while result.code != RESULT_CODE.OK:
-            filter_conds, err_msg = format_model_query_conditions(self.model, filters=filters)
-            if err_msg:
-                result.code = RESULT_CODE.INVALID_PARAM
-                result.message = err_msg
-                break
-
-            rows, total = await DbProxy().query_list(self.model, filters=filter_conds, limit=limit, offset=offset, sort=orderby, direction=direction, selections=fields)
-            
-            if not fields:
-                if hasattr(self.model, 'as_dict'):
-                    formatted_rows = []
-                    for row in rows:
-                        m = self.model()
-                        for k, v in row.items():
-                            setattr(m, k, v)
-                        formatted_rows.append(getattr(m, 'as_dict')())
-                    rows = formatted_rows
-
-            result.code = RESULT_CODE.OK
-            result.message = i18n.t('basic.success', **locale_params)
-            result.total = total
-            result.data = rows
-            if limit:
-                result.pageSize = limit
-                result.page = int(offset/limit) + 1
-        return result
-
     async def post(self, id: str|int = None):
         """
         API handler of add model instance data
         """
         if id:
             self.set_status(HTTPStatus.NOT_FOUND)
             self.finish()
@@ -184,26 +160,39 @@
         if isinstance(inputs, list):
             for ele in inputs:
                 form_items.append(self.form(formdata=None, data=ele, meta={'csrf': False}))
         else:
             form_items.append(self.form(formdata=None, data=inputs, meta={'csrf': False}))
             
         insert_models = []
+        after_saves = []
         for form_item in form_items:
             result = validate_form(form_item)
             if not result.is_success():
                 self.set_header('Content-Type', 'application/json')
                 self.write(result.encode_json())
                 self.finish()
                 return
 
             m = self.model()
             if hasattr(m, 'set_session_uid'):
                 session_uid = self.session[SESSION_UID_KEY]
                 setattr(m, 'set_session_uid', session_uid)
+                
+            b, msg = await self._check_before_save(form_item)
+            if not b:
+                result.code = RESULT_CODE.INVALID_PARAM
+                result.message = msg
+                self.set_header('Content-Type', 'application/json')
+                self.write(result.encode_json())
+                self.finish()
+                return
+            if hasattr(form_item, 'after_save'):
+                after_saves.append(getattr(form_item, 'after_save'))
+                
             save_form_fields(form_item, m, ignore_empty=True)
             insert_models.append(m)
 
         result = GeneralResponseObject(code=RESULT_CODE.FAIL, message=i18n.t('basic.create_data_failed', **locale_params))
         
         # m = self.model()
         # if hasattr(m, 'set_session_uid'):
@@ -223,14 +212,16 @@
                     else:
                         resp_data.append(dump_model_data(m))
                 if isinstance(inputs, list):
                     result.data = resp_data
                 else:
                     result.data = resp_data[0]
                 LOG.info('insert [%s] succeed', get_model_class_name(self.model))
+                if after_saves:
+                    [await self._call(cb, data=insert_models[i], session=self.session) for i, cb in after_saves]
             else:
                 LOG.warning('insert [%s] failed', get_model_class_name(self.model))
         except Exception as e:
             LOG.error('insert [%s] failed with error:%s', get_model_class_name(self.model), str(e))
             result.code = RESULT_CODE.FAIL
             result.message = str(e)
         
@@ -248,14 +239,150 @@
     async def patch(self, id: str|int = None):
         if not id:
             self.set_status(HTTPStatus.NOT_FOUND)
             self.finish()
             return
         await self.do_edit(id, False)
 
+    async def delete(self, id: str|int = None):
+        """
+        API handler of delete model instance data
+        """
+        if not id:
+            self.set_status(HTTPStatus.NOT_FOUND)
+            self.finish()
+            return
+        # inputs = request_body_as_json(self.request)
+        locale_params = get_locale_params(self.request)
+        columns, pk = model_columns(self.model)
+        form_pk_id = id
+        if not form_pk_id:
+            LOG.warning('delete %s while not giving any id to delete', get_model_class_name(self.model))
+            return GeneralResponseObject(code=RESULT_CODE.INVALID_PARAM, message=i18n.t('basic.invalid_param', **locale_params)).encode_json()
+        m = await DbProxy().find_item(self.model, {getattr(self.model, pk)==form_pk_id})
+        if not m:
+            LOG.warning('delete %s [%s] info failed while data does not extsts', get_model_class_name(self.model), str(form_pk_id))
+            return GeneralResponseObject(code=RESULT_CODE.DATA_DOES_NOT_EXISTS, message=i18n.t('basic.data_not_exists', **locale_params)).encode_json()
+        
+        result = GeneralResponseObject(code=RESULT_CODE.FAIL, message=i18n.t('basic.delete_data_failed', **locale_params))
+        try:
+            res = False
+            if False and hasattr(m, 'obsoleted'):
+                if hasattr(m, 'set_session_uid'):
+                    session_uid = self.session[SESSION_UID_KEY]
+                    setattr(m, 'set_session_uid', session_uid)
+                setattr(m, 'obsoleted', 1)
+                res = await DbProxy().update_item(m)
+            else:
+                res = await DbProxy().del_item(m)
+            if res:
+                result.code = RESULT_CODE.OK
+                result.message = i18n.t('basic.success', **locale_params)
+                LOG.info('delete %s [%s] succeed', get_model_class_name(self.model), str(form_pk_id))
+            else:
+                LOG.warning('delete %s [%s] failed', get_model_class_name(self.model), str(form_pk_id))
+        except Exception as e:
+            LOG.error('delete %s [%s] failed with error:%s', get_model_class_name(self.model), str(form_pk_id), str(e))
+            result.code = RESULT_CODE.FAIL
+            result.message = str(e)
+
+        self.set_header('Content-Type', 'application/json')
+        self.write(result.encode_json())
+        self.finish()
+
+    async def do_get_list(self, params: dict, locale_params: dict):
+        """
+        API handler of get model list data by filter condition and pagination
+        """
+        filters = params.get('filter', {})
+        fields = params.get('fields', [])
+        if not filters or not isinstance(filters, dict):
+            filters = {}
+        limit, offset = get_listquery_pager_info(params)
+        orderby, direction = get_listquery_sort_info(params)
+
+        result = ListResponseObject(RESULT_CODE.DATA_DOES_NOT_EXISTS, message=i18n.t('basic.data_not_exists', **locale_params))
+        while result.code != RESULT_CODE.OK:
+            filter_conds, err_msg = format_model_query_conditions(self.model, filters=filters)
+            if err_msg:
+                result.code = RESULT_CODE.INVALID_PARAM
+                result.message = err_msg
+                break
+
+            rows, total = await DbProxy().query_list(self.model, filters=filter_conds, limit=limit, offset=offset, sort=orderby, direction=direction, selections=fields)
+            
+            if not fields and hasattr(self.model, 'as_dict'):
+                formatted_rows = []
+                for row in rows:
+                    m = self.model()
+                    for k, v in row.items():
+                        setattr(m, k, v)
+                    formatted_rows.append(getattr(m, 'as_dict')())
+                rows = formatted_rows
+            else:
+                column_name_mapping = format_column_name_mappings(self.form)
+                if column_name_mapping:
+                    rows = [{column_name_mapping.get(k, k): v for k, v in row.items()} for row in rows]
+
+            result.code = RESULT_CODE.OK
+            result.message = i18n.t('basic.success', **locale_params)
+            result.total = total
+            result.data = rows
+            if limit:
+                result.pageSize = limit
+                result.page = int(offset/limit) + 1
+        return result
+
+    async def do_get_tree_list(self, id: str, params: dict, locale_params: dict):
+        """
+        API handler of get model tree list data by filter condition
+        """
+        filters = params.get('filter', {})
+        fields = params.get('fields', [])
+        if not filters or not isinstance(filters, dict):
+            filters = {}
+        limit, offset = get_listquery_pager_info(params, default_list_limit=3000, max_list_limit=5000)
+        orderby, direction = get_listquery_sort_info(params)
+
+        result = ListResponseObject(RESULT_CODE.DATA_DOES_NOT_EXISTS, message=i18n.t('basic.data_not_exists', **locale_params))
+        while result.code != RESULT_CODE.OK:
+            filter_conds, err_msg = format_model_query_conditions(self.model, filters=filters)
+            if err_msg:
+                result.code = RESULT_CODE.INVALID_PARAM
+                result.message = err_msg
+                break
+            
+            try:
+                rows, total = await DbProxy().query_list(self.model, filters=filter_conds, limit=limit, offset=offset, sort=orderby, direction=direction, selections=fields)
+            except Exception as e:
+                LOG.error('get %s tree list failed with error:%s', get_model_class_name(self.model), str(e))
+                result.code = RESULT_CODE.INTERNAL_ERROR
+                result.message = str(e)
+                break
+
+            if not fields:
+                if hasattr(self.model, 'as_dict'):
+                    formatted_rows = []
+                    for row in rows:
+                        m = self.model()
+                        for k, v in row.items():
+                            setattr(m, k, v)
+                        formatted_rows.append(getattr(m, 'as_dict')())
+                    rows = formatted_rows
+
+            _, pk = model_columns(self.model)
+            result.code = RESULT_CODE.OK
+            result.message = i18n.t('basic.success', **locale_params)
+            result.total = total
+            result.data = format_items_as_tree(rows, pk, self.auto_association_keys[id], locale_params)
+            if limit:
+                result.pageSize = limit
+                result.page = int(offset/limit) + 1
+        return result
+
     async def do_edit(self, id: str|int, ignore_empty: bool):
         """
         API handler of edit model instance data
         """
         locale_params = get_locale_params(self.request)
         if not self.form:
             self.set_status(HTTPStatus.INTERNAL_SERVER_ERROR, '%s form not configured for general form handler, please specify form when register model general api handlers' % (get_model_class_name(self.model)))
@@ -272,73 +399,52 @@
             if not m:
                 LOG.warning('get %s [%s] info failed while data does not extsts', get_model_class_name(self.model), str(form_pk_id))
                 result = GeneralResponseObject(code=RESULT_CODE.DATA_DOES_NOT_EXISTS, message=i18n.t('basic.data_not_exists', **locale_params)).encode_json()
                 break
             if hasattr(m, 'set_session_uid'):
                 session_uid = self.session[SESSION_UID_KEY]
                 setattr(m, 'set_session_uid', session_uid)
+            
+            b, msg = await self._check_before_save(form_item)
+            if not b:
+                result.code = RESULT_CODE.INVALID_PARAM
+                result.message = msg
+                break
             save_form_fields(form_item, m, ignore_empty=ignore_empty)
 
             result = GeneralResponseObject(code=RESULT_CODE.FAIL, message=i18n.t('basic.edit_data_failed', **locale_params))
             try:
                 res = await DbProxy().update_item(m)
                 if res:
                     result.code = RESULT_CODE.OK
                     result.message = i18n.t('basic.success', **locale_params)
                     if hasattr(m, 'as_dict'):
                         result.data = getattr(m, 'as_dict')()
                     else:
                         result.data = dump_model_data(m, columns=columns)
                     LOG.info('edit %s [%s] succeed', get_model_class_name(self.model), str(form_pk_id))
+                    if hasattr(form_item, 'after_save'):
+                        await self._call(getattr(form_item, data=m, session=self.session))
                 else:
                     LOG.warning('edit %s [%s] failed', get_model_class_name(self.model), str(form_pk_id))
             except Exception as e:
                 LOG.error('edit %s [%s] failed with error:%s', get_model_class_name(self.model), str(form_pk_id), str(e))
                 result.code = RESULT_CODE.FAIL
                 result.message = str(e)
             break
         self.set_header('Content-Type', 'application/json')
         self.write(result.encode_json())
         self.finish()
-
-    async def delete(self, id: str|int = None):
-        """
-        API handler of delete model instance data
-        """
-        if not id:
-            self.set_status(HTTPStatus.NOT_FOUND)
-            self.finish()
-            return
-        # inputs = request_body_as_json(self.request)
-        locale_params = get_locale_params(self.request)
-        columns, pk = model_columns(self.model)
-        form_pk_id = id
-        if not form_pk_id:
-            LOG.warning('delete %s while not giving any id to delete', get_model_class_name(self.model))
-            return GeneralResponseObject(code=RESULT_CODE.INVALID_PARAM, message=i18n.t('basic.invalid_param', **locale_params)).encode_json()
-        m = await DbProxy().find_item(self.model, {getattr(self.model, pk)==form_pk_id})
-        if not m:
-            LOG.warning('delete %s [%s] info failed while data does not extsts', get_model_class_name(self.model), str(form_pk_id))
-            return GeneralResponseObject(code=RESULT_CODE.DATA_DOES_NOT_EXISTS, message=i18n.t('basic.data_not_exists', **locale_params)).encode_json()
         
-        result = GeneralResponseObject(code=RESULT_CODE.FAIL, message=i18n.t('basic.delete_data_failed', **locale_params))
-        try:
-            res = False
-            if False and hasattr(m, 'obsoleted'):
-                if hasattr(m, 'set_session_uid'):
-                    session_uid = self.session[SESSION_UID_KEY]
-                    setattr(m, 'set_session_uid', session_uid)
-                setattr(m, 'obsoleted', 1)
-                res = await DbProxy().update_item(m)
-            else:
-                res = await DbProxy().del_item(m)
-            if res:
-                result.code = RESULT_CODE.OK
-                result.message = i18n.t('basic.success', **locale_params)
-                LOG.info('delete %s [%s] succeed', get_model_class_name(self.model), str(form_pk_id))
-            else:
-                LOG.warning('delete %s [%s] failed', get_model_class_name(self.model), str(form_pk_id))
-        except Exception as e:
-            LOG.error('delete %s [%s] failed with error:%s', get_model_class_name(self.model), str(form_pk_id), str(e))
-            result.code = RESULT_CODE.FAIL
-            result.message = str(e)
-        return result.encode_json()
+    async def _check_before_save(self, form_item: Form, **kwargs):
+        if hasattr(form_item, 'before_save'):
+            before_save = getattr(form_item, 'before_save')
+            b, msg = await self._call(before_save, session=self.session)
+            return b, msg
+        return True, ''
+
+    async def _call(self, callable: callable, **kwargs):
+        if tornado.gen.is_coroutine_function(callable) or asyncio.iscoroutinefunction(callable):
+            return await callable(**kwargs)
+        else:
+            return callable(**kwargs)
+
```

### Comparing `lycium-rest-0.0.1/lycium_rest/restfulwrapper/modelrelationhandlers.py` & `lycium-rest-0.0.2/lycium_rest/restfulwrapper/modelrelationhandlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from hawthorn.asynchttphandler import GeneralTornadoHandler, request_body_as_json
 from hawthorn.session import TornadoSession
 from hawthorn.modelutils import ModelBase, model_columns, get_model_class_name
 from hawthorn.dbproxy import DbProxy
 from ..valueobjects.resultcodes import RESULT_CODE
 from ..valueobjects.responseobject import GeneralResponseObject, ListResponseObject
 
-from .utils import format_model_query_conditions, read_request_parameters, get_locale_params
+from .utils import format_model_query_conditions, read_request_parameters, get_locale_params, get_listquery_sort_info
 
 LOG = logging.getLogger('services.generalmodelapi.apihandlers')
 
 class ModelRelationsRESTfulHandler(tornado.web.RequestHandler):
     """
     Model API many-to-many relationships handler wrapper
     """
@@ -69,14 +69,15 @@
         err_message = self.pre_check_middle_model_fields(**locale_params)
         if err_message:
             LOG.error('failed to execute handler of get %s relations id, %s', get_model_class_name(self.middle_model), err_message)
             self.set_status(HTTPStatus.INTERNAL_SERVER_ERROR, err_message)
             self.finish()
             return
         filters = read_request_parameters(self.request)
+        orderby, direction = get_listquery_sort_info(filters)
         filters[self.src_field] = instanceID
         dst_field: sqlalchemy.Column = None
         if self.src_field in filters:
             dst_field = getattr(self.middle_model, self.dst_field)
         elif self.dst_field in filters:
             dst_field = getattr(self.middle_model, self.src_field)
         
@@ -86,15 +87,15 @@
             if err_msg:
                 result.code = RESULT_CODE.INVALID_PARAM
                 result.message = err_msg
                 break
 
             limit = 1000
             offset = 0
-            rows, total = await DbProxy().query_list(self.middle_model, filters=filter_conds, limit=limit, offset=offset, selections=[dst_field.name])
+            rows, total = await DbProxy().query_list(self.middle_model, filters=filter_conds, limit=limit, offset=offset, sort=orderby, direction=direction, selections=[dst_field.name])
             result.code = RESULT_CODE.OK
             result.message = i18n.t('basic.success', **locale_params)
             result.total = total
             result.data = rows
             if limit:
                 result.pageSize = limit
                 result.page = int(offset/limit) + 1
@@ -134,28 +135,27 @@
         src_value = inputs.get(self.src_field, 0)
         dst_value = inputs.get(self.dst_field, 0)
         result = GeneralResponseObject(RESULT_CODE.INVALID_PARAM, i18n.t('basic.invalid_param', **locale_params))
         while result.code != RESULT_CODE.OK:
             check_fields = [(self.src_model, self.src_field, src_value), (self.dst_model, self.dst_field, dst_value)]
             check_failed = False
             for cks in check_fields:
-                if not cks[2]:
+                if not cks[2] and cks[1] != self.dst_field:
                     result.code = RESULT_CODE.INVALID_PARAM
                     result.message = '%s field should have a valid value' % (cks[1])
                     LOG.warning('delete relation ids for %s failed, %s', get_model_class_name(self.middle_model), result.message)
                     check_failed = True
                     break
             if check_failed:
                 break
 
             try:
-                del_conds = [
-                    self.format_relation_find_conditions(self.middle_model, self.src_field, src_value)[0],
-                    self.format_relation_find_conditions(self.middle_model, self.dst_field, dst_value)[0]
-                ]
+                del_conds = [self.format_relation_find_conditions(self.middle_model, self.src_field, src_value)[0]]
+                if dst_value:
+                    del_conds.append(self.format_relation_find_conditions(self.middle_model, self.dst_field, dst_value)[0])
                 res = await DbProxy().del_items(self.middle_model, del_conds)
                 if res:
                     result.code = RESULT_CODE.OK
                     result.message = i18n.t('basic.success', **locale_params)
                     LOG.info('delete relation ids for %s with %s:%s and %s:%s succeed, affected %d rows', get_model_class_name(self.middle_model), self.src_field, str(src_value), self.dst_field, str(dst_value), res)
                 else:
                     result.code = RESULT_CODE.DATA_DOES_NOT_EXISTS
@@ -180,17 +180,30 @@
             return
         locale_params = get_locale_params(self.request)
         err_message = self.pre_check_middle_model_fields(**locale_params)
         if err_message:
             LOG.error('failed to execute handler of %s %s relations id, %s', mode, get_model_class_name(self.middle_model), err_message)
             return err_message, HTTPStatus.INTERNAL_SERVER_ERROR
         inputs = request_body_as_json(self.request)
-        inputs[self.src_field] = instanceID
-        src_value = inputs.get(self.src_field, 0)
-        dst_value = inputs.get(self.dst_field, 0)
+        if isinstance(inputs, dict):
+            inputs[self.src_field] = instanceID
+            src_value = inputs.get(self.src_field, 0)
+            dst_value = inputs.get(self.dst_field, 0)
+        elif isinstance(inputs, list):
+            src_value = instanceID
+            dst_value = inputs
+            inputs = {
+                self.src_field: instanceID,
+                self.dst_field: dst_value
+            }
+        else:
+            err_message = i18n.t('basic.invalid_param', **locale_params)
+            LOG.warning('failed to execute handler of %s %s relations id, %s', mode, get_model_class_name(self.middle_model), err_message)
+            return err_message, HTTPStatus.BAD_REQUEST
+            
         extra_field_values = {}
         middle_model_columns, middle_model_pk = model_columns(self.middle_model)
         for k in middle_model_columns:
             if k == middle_model_pk:
                 continue
             if k in inputs and k != self.src_field and k != self.dst_field:
                 extra_field_values[k] = inputs[k]
```

### Comparing `lycium-rest-0.0.1/lycium_rest/restfulwrapper/pagedescriptorhandlers.py` & `lycium-rest-0.0.2/lycium_rest/restfulwrapper/pagedescriptorhandlers.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,14 +23,22 @@
 
 class ModelPageDescriptorsApiHandler():
     """
     Model page descriptor API handler wrapper
     """
     def __init__(self, get_page_descriptor_model: Callable[[str], RESTfulAPIWraper]):
         self.get_page_descriptor_model = get_page_descriptor_model
+        
+    def get_model_page_type(self, w: RESTfulAPIWraper):
+        page_type = 'autotable'
+        if w.cls:
+            m = w.cls()
+            if hasattr(m, '__page_type__'):
+                page_type = getattr(m, '__page_type__', 'autotable')
+        return page_type
 
     async def handler_get(self, handler: GeneralTornadoHandler, request: tornado.httputil.HTTPServerRequest):
         """
         API handler of get single model data
         """
         filters = read_request_parameters(request)
         locale_params = get_locale_params(request)
@@ -53,11 +61,14 @@
             if not w.cls:
                 result.code = RESULT_CODE.INTERNAL_ERROR
                 result.message = f'No model specified for page name: {page_name}' # i18n.t('basic.could_not_recognize_current_page', **locale_params)
                 break
 
             result.code = RESULT_CODE.OK
             result.message = i18n.t('basic.success', **locale_params)
-            result.data = w.destriptor()
+            result.data = {
+                'pageType': self.get_model_page_type(w),
+                'schema': w.destriptor()
+            }
             break
         
         return result.encode_json()
```

### Comparing `lycium-rest-0.0.1/lycium_rest/restfulwrapper/register.py` & `lycium-rest-0.0.2/lycium_rest/restfulwrapper/register.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,53 +4,83 @@
 import logging
 import tornado.web
 import tornado.httputil
 from wtforms import Form
 from hawthorn.asynchttphandler import GeneralTornadoHandler, routes
 from hawthorn.modelutils import ModelBase, meta_data, get_model_class_name, model_columns
 from .accesscontrol.authorizedsession import authorized_session_access_control
+from .restdescriptor import Relations
+from .utils import find_model_class_by_cls_name, find_model_class_by_table_name
 from .modelapihandlers import ModelRESTfulHandler
 from .modelrelationhandlers import ModelRelationsRESTfulHandler
 from .pagedescriptorhandlers import ModelPageDescriptorsApiHandler
 
 LOG = logging.getLogger('lycium.restfulwrapper.register')
 
-def find_model_class_by_table_name(table_name: str):
-    tbl_model: ModelBase = None
-    for model in ModelBase.registry.mappers:
-        if hasattr(model.class_, '__tablename__') and model.class_.__tablename__ == table_name:
-            # print(model.class_.__name__)
-            if model.class_.__name__[0] != '_':
-                tbl_model = model.class_
-                break
-    return tbl_model
-
-def find_model_class_by_cls_name(cls_name: str):
-    for model in ModelBase.registry.mappers:
-        if model.class_.__name__ == cls_name:
-            return model.class_
-    return None
-
 def register_model_general_api_handlers(model: ModelBase, endpoint: str = '', form: Form = None, web_app: tornado.web.Application=None, **options):
-    # handler = ModelApiHandler(model=model, add_form=add_form, edit_form=edit_form)
+    ac = options.pop('ac', [])
+    auto_association = options.pop('auto_association', None)
+    custom_relations: Relations | list[Relations] = options.pop('custom_relations', None)
+    if not ac:
+        ac = [authorized_session_access_control]
+    endpoint = prepare_model_endpoint(model, endpoint)
+    relationship_attrs, auto_association_attrs = lookup_model_relationship_attrs(model)
+    if not auto_association:
+        auto_association = auto_association_attrs
+
+    uri = endpoint+r'(?:/(?P<id>\w+))?'
+    local_routes = [
+        (uri, ModelRESTfulHandler, dict(model=model, form=form, ac=ac, auto_association=auto_association))
+    ]
+    LOG.info('registing RESTful endpoint %s', uri)
+    registered_middle_relations = {}
+    for attr_key, relation_params in relationship_attrs.items():
+        uri = endpoint + r'/(?P<instanceID>\w+)/' + attr_key
+        local_routes.append((uri, ModelRelationsRESTfulHandler, relation_params))
+        LOG.info('registing relations RESTful endpoint %s', uri)
+        registered_middle_relations[get_model_class_name(relation_params['middle_model'])] = True
+    if custom_relations:
+        crs: list[Relations] = custom_relations if isinstance(custom_relations, list) else [custom_relations]
+        for cr in crs:
+            cr.prepare()
+            if get_model_class_name(cr.middle_model) not in registered_middle_relations:
+                uri = endpoint + r'/(?P<instanceID>\w+)/' + get_model_class_name(cr.dst_model).lower() + 's'
+                local_routes.append((uri, ModelRelationsRESTfulHandler, dict(middle_model=cr.middle_model, src_field=cr.src_field, dst_field=cr.dst_field, src_model=model, dst_model=cr.dst_model)))
+                LOG.info('registing relations RESTful endpoint %s', uri)
+
+    if web_app:
+        [web_app.add_handlers(route[0], route) for route in local_routes]
+    else:
+        routes.routes.extend(local_routes)
+
+def register_model_page_descriptor_api_handler(get_page_descriptor_model, web_app: tornado.web.Application=None, **options):
+    handler = ModelPageDescriptorsApiHandler(get_page_descriptor_model)
     ac = options.pop('ac', [])
     if not ac:
         ac = [authorized_session_access_control]
+    local_routes = [
+        ('/api/pages/descriptors', GeneralTornadoHandler, dict(callback=handler.handler_get, methods=['GET'], ac=ac))
+    ]
+    if web_app:
+        [web_app.add_handlers(route[0], route) for route in local_routes]
+    else:
+        routes.routes.extend(local_routes)
+
+def prepare_model_endpoint(model: ModelBase, endpoint: str):
     if not endpoint:
         endpoint = '/' + str(get_model_class_name(model)).lower() + 's'
     if endpoint.endswith('/'):
         endpoint.rstrip('/')
     if not endpoint.startswith('/'):
         endpoint = '/' + endpoint
+    return endpoint
 
-    uri = endpoint+r'(?:/(?P<id>\w+))?'
-    local_routes = [
-        (uri, ModelRESTfulHandler, dict(model=model, form=form, ac=ac))
-    ]
-    LOG.info('registing RESTful endpoint %s', uri)
+def lookup_model_relationship_attrs(model: ModelBase):
+    relationship_attrs = {}
+    auto_association_attrs = []
     if hasattr(model, '_sa_class_manager'):
         for attr in model._sa_class_manager.local_attrs.values():
             if attr.prop.strategy_wildcard_key == 'relationship' and attr.prop.secondary:
                 tbl = meta_data.tables.get(attr.prop.secondary, None)
                 if tbl is not None:
                     middle_model = find_model_class_by_table_name(attr.prop.secondary)
                     src_field = ''
@@ -71,56 +101,13 @@
                                     continue
                                 if hasattr(model, '__tablename__') and tbl_cols[0] == model.__tablename__:
                                     src_field = col.key
                                 else:
                                     dst_field = col.key
                                 break
                     if middle_model is not None and src_field and dst_field and dst_model is not None:
-                        uri = endpoint + r'/(?P<instanceID>\w+)/' + attr.key
-                        local_routes.append((uri, ModelRelationsRESTfulHandler, dict(middle_model=middle_model, src_field=src_field, dst_field=dst_field, src_model=src_model, dst_model=dst_model)))
-                        LOG.info('registing relations RESTful endpoint %s', uri)
-    # local_routes.append((uri_prefix+'/get', GeneralTornadoHandler, dict(callback=handler.handler_get, methods=['GET'], ac=ac)))
-    # local_routes.append((uri_prefix+'/list', GeneralTornadoHandler, dict(callback=handler.handler_list, methods=['GET'], ac=ac)))
-    # local_routes.append((uri_prefix+'/add', GeneralTornadoHandler, dict(callback=handler.handler_add, methods=['POST'], ac=ac)))
-    # local_routes.append((uri_prefix+'/edit', GeneralTornadoHandler, dict(callback=handler.handler_edit, methods=['PATCH'], ac=ac)))
-    # local_routes.append((uri_prefix+'/delete', GeneralTornadoHandler, dict(callback=handler.handler_delete, methods=['DELETE'], ac=ac)))
-
-    if web_app:
-        [web_app.add_handlers(route[0], route) for route in local_routes]
-    else:
-        routes.routes.extend(local_routes)
-
-# def register_middle_relation_model_api_handlers(model: ModelBase, uri_prefix: str, src_field: str, dst_field: str, src_model: ModelBase, dst_model: ModelBase, web_app: tornado.web.Application=None, **options):
-#     handler = ModelRelationsApiHandler(model, src_field, dst_field, src_model, dst_model)
-#     ac = options.pop('ac', [])
-#     if not ac:
-#         ac = [authorized_session_access_control]
-#     if not uri_prefix:
-#         uri_prefix = '/' + str(get_model_class_name(model)).lower() + 's'
-#     if uri_prefix.endswith('/'):
-#         uri_prefix.rstrip('/')
-#     if not uri_prefix.startswith('/'):
-#         uri_prefix = '/' + uri_prefix
-
-#     local_routes = []
-#     local_routes.append((uri_prefix+'/list', GeneralTornadoHandler, dict(callback=handler.handler_relation_ids, methods=['GET'], ac=ac)))
-#     local_routes.append((uri_prefix+'/add', GeneralTornadoHandler, dict(callback=handler.handler_add, methods=['POST'], ac=ac)))
-#     local_routes.append((uri_prefix+'/update', GeneralTornadoHandler, dict(callback=handler.handler_update, methods=['PATCH'], ac=ac)))
-#     local_routes.append((uri_prefix+'/delete', GeneralTornadoHandler, dict(callback=handler.handler_delete, methods=['DELETE'], ac=ac)))
-
-#     if web_app:
-#         [web_app.add_handlers(route[0], route) for route in local_routes]
-#     else:
-#         routes.routes.extend(local_routes)
-
-def register_model_page_descriptor_api_handler(get_page_descriptor_model, web_app: tornado.web.Application=None, **options):
-    handler = ModelPageDescriptorsApiHandler(get_page_descriptor_model)
-    ac = options.pop('ac', [])
-    if not ac:
-        ac = [authorized_session_access_control]
-    local_routes = [
-        ('/api/pages/descriptors', GeneralTornadoHandler, dict(callback=handler.handler_get, methods=['GET'], ac=ac))
-    ]
-    if web_app:
-        [web_app.add_handlers(route[0], route) for route in local_routes]
-    else:
-        routes.routes.extend(local_routes)
+                        relationship_attrs[attr.key] = dict(middle_model=middle_model, src_field=src_field, dst_field=dst_field, src_model=src_model, dst_model=dst_model)
+            elif attr.expression.foreign_keys:
+                for fk in attr.expression.foreign_keys:
+                    if fk.constraint.parent.fullname == model.__tablename__:
+                        auto_association_attrs.append(attr.key)
+    return relationship_attrs, auto_association_attrs
```

### Comparing `lycium-rest-0.0.1/lycium_rest/restfulwrapper/utils.py` & `lycium-rest-0.0.2/lycium_rest/restfulwrapper/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,21 +2,38 @@
 # -*- coding: utf-8 -*-
 
 import json
 import logging
 import tornado.web
 import tornado.httputil
 import sqlalchemy
+from wtforms import Form, Field
 from typing import Iterable
 from hawthorn.asynchttphandler import args_as_dict, request_body_as_json
 from hawthorn.modelutils import ModelBase, model_columns
 from hawthorn.utilities import toint
 
 LOG = logging.getLogger('services.generalmodelapi.utils')
 
+def find_model_class_by_table_name(table_name: str) -> ModelBase | None:
+    tbl_model: ModelBase = None
+    for model in ModelBase.registry.mappers:
+        if hasattr(model.class_, '__tablename__') and model.class_.__tablename__ == table_name:
+            # print(model.class_.__name__)
+            if model.class_.__name__[0] != '_':
+                tbl_model = model.class_
+                break
+    return tbl_model
+
+def find_model_class_by_cls_name(cls_name: str) -> ModelBase | None:
+    for model in ModelBase.registry.mappers:
+        if model.class_.__name__ == cls_name:
+            return model.class_
+    return None
+
 def format_model_query_conditions(model: ModelBase, filters: dict = {}, skip_non_existed_column=True):
     filter_conds = []
     err_messages = []
     if filters:
         for k, v in filters.items():
             if not hasattr(model, k):
                 if not skip_non_existed_column:
@@ -85,29 +102,41 @@
             else:
                 if model_field.expression.type.__visit_name__ == 'string':
                     filter_conds.append(model_field.contains(str(v)))
                 else:
                     filter_conds.append(model_field==v)
     return filter_conds, ', '.join(err_messages)
 
-def dump_model_data(model: ModelBase, columns: list = None):
+def format_column_name_mappings(form: Form = None):
+    column_name_mapping = {}
+    if form:
+        form_inst = form()
+        for field in form_inst._fields.values():
+            if field.id:
+                column_name_mapping[field.id] = field.name
+    return column_name_mapping
+
+def dump_model_data(model: ModelBase, columns: list = None, column_name_mapping: dict = {}):
     values = {}
     if not columns:
         columns, _ = model_columns(model)
     hidden_fields = []
     if hasattr(model, '__hidden_response_fields__') and isinstance(getattr(model, '__hidden_response_fields__', None), list):
         hidden_fields = getattr(model, '__hidden_response_fields__')
     for c in columns:
         if c in hidden_fields:
             continue
         if hasattr(model, c):
             val = getattr(model, c)
             if isinstance(val, bytes):
                 val = val.decode('utf-8')
-            values[c] = val
+            if column_name_mapping:
+                values[column_name_mapping.get(c, c)] = val
+            else:
+                values[c] = val
     return values
 
 def read_request_parameters(request: tornado.httputil.HTTPServerRequest):
     params = args_as_dict(request)
     if request.method == 'POST':
         if request.headers['Content-Type'] == 'application/json':
             filters2 = request_body_as_json(request)
```

### Comparing `lycium-rest-0.0.1/lycium_rest/utilities/__init__.py` & `lycium-rest-0.0.2/lycium_rest/utilities/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 
 import time
 import bcrypt
+import re
 
 def get_current_timestamp():
     """
     Get current timestamp as milli seconds
     """
     return int(time.time() * 1000)
```

### Comparing `lycium-rest-0.0.1/lycium_rest/valueobjects/responseobject.py` & `lycium-rest-0.0.2/lycium_rest/valueobjects/responseobject.py`

 * *Files identical despite different names*

### Comparing `lycium-rest-0.0.1/lycium_rest/valueobjects/resultcodes.py` & `lycium-rest-0.0.2/lycium_rest/valueobjects/resultcodes.py`

 * *Files identical despite different names*

### Comparing `lycium-rest-0.0.1/lycium_rest.egg-info/PKG-INFO` & `lycium-rest-0.0.2/lycium_rest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lycium-rest
-Version: 0.0.1
+Version: 0.0.2
 Summary: common python programing encapsulation library
 Home-page: https://github.com/libpub/lycium-rest
 Author: kevinyjn
 Author-email: kevinyjn@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lycium-rest-0.0.1/lycium_rest.egg-info/SOURCES.txt` & `lycium-rest-0.0.2/lycium_rest.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,17 @@
 lycium_rest/migrationutils.py
 lycium_rest.egg-info/PKG-INFO
 lycium_rest.egg-info/SOURCES.txt
 lycium_rest.egg-info/dependency_links.txt
 lycium_rest.egg-info/requires.txt
 lycium_rest.egg-info/top_level.txt
 lycium_rest/formvalidation/__init__.py
+lycium_rest/formvalidation/formitemprops.py
 lycium_rest/formvalidation/formutils.py
+lycium_rest/formvalidation/modifyingbeheviorformfields.py
 lycium_rest/formvalidation/validators.py
 lycium_rest/locales/basic.en_US.yml
 lycium_rest/locales/basic.zh_CN.yml
 lycium_rest/model/__init__.py
 lycium_rest/model/supports/__init__.py
 lycium_rest/model/supports/migration.py
 lycium_rest/model/supports/migration_progress.py
@@ -24,10 +26,11 @@
 lycium_rest/restfulwrapper/pagedescriptorhandlers.py
 lycium_rest/restfulwrapper/register.py
 lycium_rest/restfulwrapper/restdescriptor.py
 lycium_rest/restfulwrapper/utils.py
 lycium_rest/restfulwrapper/accesscontrol/__init__.py
 lycium_rest/restfulwrapper/accesscontrol/authorizedsession.py
 lycium_rest/utilities/__init__.py
+lycium_rest/utilities/treedata.py
 lycium_rest/valueobjects/__init__.py
 lycium_rest/valueobjects/responseobject.py
 lycium_rest/valueobjects/resultcodes.py
```

### Comparing `lycium-rest-0.0.1/setup.py` & `lycium-rest-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="lycium-rest",
-    version="0.0.1",
+    version="0.0.2",
     author="kevinyjn",
     author_email="kevinyjn@gmail.com",
     description="common python programing encapsulation library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/libpub/lycium-rest",
     packages=setuptools.find_packages(exclude=[".tests", ".tests.", "tests.*", "tests"]),
```

