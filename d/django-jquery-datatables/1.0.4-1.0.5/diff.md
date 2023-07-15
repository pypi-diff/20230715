# Comparing `tmp/django_jquery_datatables-1.0.4.tar.gz` & `tmp/django_jquery_datatables-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_jquery_datatables-1.0.4.tar", last modified: Mon Jul 10 11:30:30 2023, max compression
+gzip compressed data, was "django_jquery_datatables-1.0.5.tar", last modified: Sat Jul 15 15:51:53 2023, max compression
```

## Comparing `django_jquery_datatables-1.0.4.tar` & `django_jquery_datatables-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 11:30:30.276504 django_jquery_datatables-1.0.4/
--rw-rw-rw-   0        0        0     1067 2023-07-03 10:09:34.000000 django_jquery_datatables-1.0.4/License.txt
--rw-rw-rw-   0        0        0     9329 2023-07-10 11:30:30.275508 django_jquery_datatables-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8951 2023-07-03 10:09:34.000000 django_jquery_datatables-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 11:30:30.262512 django_jquery_datatables-1.0.4/django_jquery_datatables/
--rw-rw-rw-   0        0        0        0 2023-07-03 10:09:34.000000 django_jquery_datatables-1.0.4/django_jquery_datatables/__init__.py
--rw-rw-rw-   0        0        0     5014 2023-07-10 11:28:41.000000 django_jquery_datatables-1.0.4/django_jquery_datatables/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-10 11:30:30.272508 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/
--rw-rw-rw-   0        0        0     9329 2023-07-10 11:30:30.000000 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      340 2023-07-10 11:30:30.000000 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 11:30:30.000000 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-07-10 11:30:30.000000 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/requires.txt
--rw-rw-rw-   0        0        0       25 2023-07-10 11:30:30.000000 django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-10 11:30:30.276504 django_jquery_datatables-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      714 2023-07-10 11:30:01.000000 django_jquery_datatables-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:51:53.147114 django_jquery_datatables-1.0.5/
+-rw-rw-rw-   0        0        0     1067 2023-07-03 10:09:34.000000 django_jquery_datatables-1.0.5/License.txt
+-rw-rw-rw-   0        0        0     9329 2023-07-15 15:51:53.146114 django_jquery_datatables-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8951 2023-07-03 10:09:34.000000 django_jquery_datatables-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-07-15 15:51:53.132123 django_jquery_datatables-1.0.5/django_jquery_datatables/
+-rw-rw-rw-   0        0        0        0 2023-07-03 10:09:34.000000 django_jquery_datatables-1.0.5/django_jquery_datatables/__init__.py
+-rw-rw-rw-   0        0        0     5069 2023-07-15 15:51:26.000000 django_jquery_datatables-1.0.5/django_jquery_datatables/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:51:53.143116 django_jquery_datatables-1.0.5/django_jquery_datatables.egg-info/
+-rw-rw-rw-   0        0        0     9329 2023-07-15 15:51:52.000000 django_jquery_datatables-1.0.5/django_jquery_datatables.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      340 2023-07-15 15:51:53.000000 django_jquery_datatables-1.0.5/django_jquery_datatables.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 15:51:52.000000 django_jquery_datatables-1.0.5/django_jquery_datatables.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-07-15 15:51:52.000000 django_jquery_datatables-1.0.5/django_jquery_datatables.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-07-15 15:51:52.000000 django_jquery_datatables-1.0.5/django_jquery_datatables.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-15 15:51:53.147114 django_jquery_datatables-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      714 2023-07-15 15:51:44.000000 django_jquery_datatables-1.0.5/setup.py
```

### Comparing `django_jquery_datatables-1.0.4/License.txt` & `django_jquery_datatables-1.0.5/License.txt`

 * *Files identical despite different names*

### Comparing `django_jquery_datatables-1.0.4/PKG-INFO` & `django_jquery_datatables-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django_jquery_datatables
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python library that integrates the popular jQuery DataTables library with Django projects.
 Home-page: https://github.com/Saliksheraz/django_jquery_datatables.git
 Author: Salik Sheraz
 Author-email: salik.sheraz@it-masons.com
 Description-Content-Type: text/markdown
 License-File: License.txt
```

### Comparing `django_jquery_datatables-1.0.4/README.md` & `django_jquery_datatables-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `django_jquery_datatables-1.0.4/django_jquery_datatables/utils.py` & `django_jquery_datatables-1.0.5/django_jquery_datatables/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,18 +13,14 @@
             allColumns.append(columnValue.replace(".", "__"))
         ctr = ctr + 1
         columnValue = request.GET.get(f"columns[{ctr}][data]")
 
     if additionalColumns and isinstance(additionalColumns, list):
         allColumns = allColumns + additionalColumns
 
-    if requestType == 'export':
-        serializer = SerializerClass(queryset, many=True)
-        return JsonResponse({"data": serializer.data})
-
     # For main search
     search = request.GET.get("search[value]")
     if search:
         for eachWord in search.strip().split(" "):
             filteredDataEachWord = queryset.none()
             for eachColumn in allColumns:
                 try:
@@ -87,14 +83,20 @@
                         else:
                             selectedColumnName = eachRemapping[selectedColumnName]
             if columnOrder == "desc":
                 selectedColumnName = "-" + selectedColumnName
             queryset = queryset.order_by(selectedColumnName)
     except:
         pass
+
+    # Exporting full data if request type is export
+    if requestType == 'export':
+        serializer = SerializerClass(queryset, many=True)
+        return JsonResponse({"data": serializer.data})
+
     # Pagination
     draw = int(request.GET.get("draw", 0))
     start = int(request.GET.get("start", 0))
     length = int(request.GET.get("length", 10))
 
     data = queryset[start: start + length]
     total_records = queryset.count()
```

### Comparing `django_jquery_datatables-1.0.4/django_jquery_datatables.egg-info/PKG-INFO` & `django_jquery_datatables-1.0.5/django_jquery_datatables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-jquery-datatables
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python library that integrates the popular jQuery DataTables library with Django projects.
 Home-page: https://github.com/Saliksheraz/django_jquery_datatables.git
 Author: Salik Sheraz
 Author-email: salik.sheraz@it-masons.com
 Description-Content-Type: text/markdown
 License-File: License.txt
```

### Comparing `django_jquery_datatables-1.0.4/setup.py` & `django_jquery_datatables-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='django_jquery_datatables',
-    version='1.0.4',
+    version='1.0.5',
     description='Python library that integrates the popular jQuery DataTables library with Django projects.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Salik Sheraz',
     author_email='salik.sheraz@it-masons.com',
     url='https://github.com/Saliksheraz/django_jquery_datatables.git',
     packages=find_packages(),
```

