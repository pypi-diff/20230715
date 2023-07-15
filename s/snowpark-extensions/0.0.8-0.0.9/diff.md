# Comparing `tmp/snowpark_extensions-0.0.8.tar.gz` & `tmp/snowpark_extensions-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowpark_extensions-0.0.8.tar", last modified: Wed Dec 14 14:56:14 2022, max compression
+gzip compressed data, was "snowpark_extensions-0.0.9.tar", last modified: Wed Dec 14 21:32:28 2022, max compression
```

## Comparing `snowpark_extensions-0.0.8.tar` & `snowpark_extensions-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 14:56:14.197914 snowpark_extensions-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2022-12-14 14:56:14.197914 snowpark_extensions-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11549 2022-12-14 14:55:49.000000 snowpark_extensions-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 14:56:14.197914 snowpark_extensions-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-14 14:55:49.000000 snowpark_extensions-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 14:56:14.197914 snowpark_extensions-0.0.8/snowpark_extensions/
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2022-12-14 14:55:49.000000 snowpark_extensions-0.0.8/snowpark_extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-14 14:55:49.000000 snowpark_extensions-0.0.8/snowpark_extensions/column_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6269 2022-12-14 14:55:49.000000 snowpark_extensions-0.0.8/snowpark_extensions/dataframe_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2022-12-14 14:55:49.000000 snowpark_extensions-0.0.8/snowpark_extensions/functions_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2022-12-14 14:55:49.000000 snowpark_extensions-0.0.8/snowpark_extensions/session_builder_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-14 14:55:49.000000 snowpark_extensions-0.0.8/snowpark_extensions/types_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3391 2022-12-14 14:55:49.000000 snowpark_extensions-0.0.8/snowpark_extensions/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 14:56:14.197914 snowpark_extensions-0.0.8/snowpark_extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2022-12-14 14:56:14.000000 snowpark_extensions-0.0.8/snowpark_extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-14 14:56:14.000000 snowpark_extensions-0.0.8/snowpark_extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 14:56:14.000000 snowpark_extensions-0.0.8/snowpark_extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 14:56:13.000000 snowpark_extensions-0.0.8/snowpark_extensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-14 14:56:14.000000 snowpark_extensions-0.0.8/snowpark_extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-14 14:56:14.000000 snowpark_extensions-0.0.8/snowpark_extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 21:32:28.329406 snowpark_extensions-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2022-12-14 21:32:28.329406 snowpark_extensions-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11549 2022-12-14 21:31:59.000000 snowpark_extensions-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 21:32:28.329406 snowpark_extensions-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2022-12-14 21:31:59.000000 snowpark_extensions-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 21:32:28.329406 snowpark_extensions-0.0.9/snowpark_extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2022-12-14 21:31:59.000000 snowpark_extensions-0.0.9/snowpark_extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2022-12-14 21:31:59.000000 snowpark_extensions-0.0.9/snowpark_extensions/column_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6269 2022-12-14 21:31:59.000000 snowpark_extensions-0.0.9/snowpark_extensions/dataframe_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2022-12-14 21:31:59.000000 snowpark_extensions-0.0.9/snowpark_extensions/functions_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2022-12-14 21:31:59.000000 snowpark_extensions-0.0.9/snowpark_extensions/session_builder_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2022-12-14 21:31:59.000000 snowpark_extensions-0.0.9/snowpark_extensions/types_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3391 2022-12-14 21:31:59.000000 snowpark_extensions-0.0.9/snowpark_extensions/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 21:32:28.329406 snowpark_extensions-0.0.9/snowpark_extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2022-12-14 21:32:28.000000 snowpark_extensions-0.0.9/snowpark_extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2022-12-14 21:32:28.000000 snowpark_extensions-0.0.9/snowpark_extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 21:32:28.000000 snowpark_extensions-0.0.9/snowpark_extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 21:32:28.000000 snowpark_extensions-0.0.9/snowpark_extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2022-12-14 21:32:28.000000 snowpark_extensions-0.0.9/snowpark_extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2022-12-14 21:32:28.000000 snowpark_extensions-0.0.9/snowpark_extensions.egg-info/top_level.txt
```

### Comparing `snowpark_extensions-0.0.8/PKG-INFO` & `snowpark_extensions-0.0.9/snowpark_extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: snowpark_extensions
-Version: 0.0.8
+Name: snowpark-extensions
+Version: 0.0.9
 Summary: A set of helpers to extend snowpark functionality
 Home-page: http://github.com/MobilizeNet/snowpark-extensions-py
 Author: mauricio.rojas
 Author-email: mauricio.rojas@mobilize.net
 Description-Content-Type: text/markdown
 
 # snowpark-extensions-py
```

### Comparing `snowpark_extensions-0.0.8/README.md` & `snowpark_extensions-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `snowpark_extensions-0.0.8/setup.py` & `snowpark_extensions-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 # read the contents of your README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 
 setup(name='snowpark_extensions',
       version=VERSION,
       description='A set of helpers to extend snowpark functionality',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='http://github.com/MobilizeNet/snowpark-extensions-py',
```

### Comparing `snowpark_extensions-0.0.8/snowpark_extensions/__init__.py` & `snowpark_extensions-0.0.9/snowpark_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `snowpark_extensions-0.0.8/snowpark_extensions/dataframe_extensions.py` & `snowpark_extensions-0.0.9/snowpark_extensions/dataframe_extensions.py`

 * *Files identical despite different names*

### Comparing `snowpark_extensions-0.0.8/snowpark_extensions/functions_extensions.py` & `snowpark_extensions-0.0.9/snowpark_extensions/functions_extensions.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,14 +14,23 @@
 )
 from snowflake.snowpark.column import _to_col_if_str, _to_col_if_lit
 
 
 if not hasattr(F,"___extended"):
     F.___extended = True
 
+    def pairwise(iterable):
+        while len(iterable):
+            a = iterable.pop(0)
+            if len(iterable):
+                b = iterable.pop(0)
+            else:
+                b = None
+            yield (a,b)
+
     def regexp_extract(value:ColumnOrLiteralStr,regexp:ColumnOrLiteralStr,idx:int) -> Column:
         """
         Extract a specific group matched by a regex, from the specified string column. 
         If the regex did not match, or the specified group did not match, 
         an empty string is returned.        
         """
         value = _to_col_if_str(value,"regexp_extract")
@@ -51,22 +60,20 @@
     def create_map(*col_names):
         """
         Usage:
         res = df.select(create_map('name', 'age').alias("map")).collect()
         """
         from snowflake.snowpark.functions import col,lit, object_construct
         col_list = []
-        if isinstance(col_names, tuple):
-            col_names = list(col_names[0])
-        if isinstance(c, str):
-            col_list.append(lit(c))
-            col_list.append(col(c))
-        else:
-            col_list.append(lit(str(c._expression).replace("\"",'')))
-            col_list.append(c)
+        for name, value in pairwise(list(col_names)):
+            if isinstance(name, str):
+                col_list.append(lit(name))
+            else:
+                col_list.append(name)
+            col_list.append(value)
         return object_construct(*col_list)
 
 
 
     array_sort_udf=None
     def array_sort(array, asc: bool=True):
         global array_sort_udf
```

### Comparing `snowpark_extensions-0.0.8/snowpark_extensions/session_builder_extensions.py` & `snowpark_extensions-0.0.9/snowpark_extensions/session_builder_extensions.py`

 * *Files 4% similar despite different names*

```diff
@@ -91,9 +91,9 @@
                 }
                 self.configs(connection_parameters)
         else:
             _logger.error(f"Config section {config_section_name} not found in snowsql file: {configpath}")
         return self
 
     Session.SessionBuilder.from_snowsql = SessionBuilder_snowsql_config
-
+    Session.SessionBuilder.from_env = SessionBuilder_env
     Session.SessionBuilder.env = SessionBuilder_env
```

### Comparing `snowpark_extensions-0.0.8/snowpark_extensions/utils.py` & `snowpark_extensions-0.0.9/snowpark_extensions/utils.py`

 * *Files identical despite different names*

### Comparing `snowpark_extensions-0.0.8/snowpark_extensions.egg-info/PKG-INFO` & `snowpark_extensions-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: snowpark-extensions
-Version: 0.0.8
+Name: snowpark_extensions
+Version: 0.0.9
 Summary: A set of helpers to extend snowpark functionality
 Home-page: http://github.com/MobilizeNet/snowpark-extensions-py
 Author: mauricio.rojas
 Author-email: mauricio.rojas@mobilize.net
 Description-Content-Type: text/markdown
 
 # snowpark-extensions-py
```

### Comparing `snowpark_extensions-0.0.8/snowpark_extensions.egg-info/SOURCES.txt` & `snowpark_extensions-0.0.9/snowpark_extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

