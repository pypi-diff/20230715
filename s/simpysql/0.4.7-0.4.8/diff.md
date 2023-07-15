# Comparing `tmp/simpysql-0.4.7.tar.gz` & `tmp/simpysql-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simpysql-0.4.7.tar", last modified: Sat Jul 15 03:44:29 2023, max compression
+gzip compressed data, was "dist/simpysql-0.4.8.tar", last modified: Sat Jul 15 04:27:09 2023, max compression
```

## Comparing `simpysql-0.4.7.tar` & `simpysql-0.4.8.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 03:44:29.000000 simpysql-0.4.7/
--rw-r--r--   0 jemes      (501) staff       (20)     3511 2023-07-15 03:44:29.000000 simpysql-0.4.7/PKG-INFO
--rw-r--r--   0 jemes      (501) staff       (20)     2482 2022-08-15 06:24:43.000000 simpysql-0.4.7/README.md
--rw-r--r--   0 jemes      (501) staff       (20)       38 2023-07-15 03:44:29.000000 simpysql-0.4.7/setup.cfg
--rw-r--r--   0 jemes      (501) staff       (20)      878 2023-07-15 03:44:18.000000 simpysql-0.4.7/setup.py
-drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql/
-drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql/Connections/
--rw-r--r--   0 jemes      (501) staff       (20)      311 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Connections/Connection.py
--rw-r--r--   0 jemes      (501) staff       (20)     1563 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Connections/ConnectionFactory.py
--rw-r--r--   0 jemes      (501) staff       (20)     3235 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Connections/MongoConnection.py
--rw-r--r--   0 jemes      (501) staff       (20)     2634 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Connections/MysqlConnection.py
--rw-r--r--   0 jemes      (501) staff       (20)     1630 2022-08-15 07:00:44.000000 simpysql-0.4.7/simpysql/Connections/MysqlConnectionpool.py
--rw-r--r--   0 jemes      (501) staff       (20)     3036 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Connections/PostgresConnection.py
--rw-r--r--   0 jemes      (501) staff       (20)      632 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Connections/PostgresConnectionpool.py
--rw-r--r--   0 jemes      (501) staff       (20)     2572 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Connections/SqlServerConnection.py
--rw-r--r--   0 jemes      (501) staff       (20)        0 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Connections/__init__.py
--rw-r--r--   0 jemes      (501) staff       (20)      956 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/DBModel.py
-drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql/Eloquent/
--rw-r--r--   0 jemes      (501) staff       (20)      509 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Eloquent/BaseBuilder.py
--rw-r--r--   0 jemes      (501) staff       (20)     1482 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Eloquent/BuilderFactory.py
--rw-r--r--   0 jemes      (501) staff       (20)     9747 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Eloquent/MongoBuilder.py
--rw-r--r--   0 jemes      (501) staff       (20)    21964 2023-07-15 03:41:59.000000 simpysql-0.4.7/simpysql/Eloquent/MysqlBuilder.py
--rw-r--r--   0 jemes      (501) staff       (20)    21926 2022-08-15 06:24:43.000000 simpysql-0.4.7/simpysql/Eloquent/MysqlBuilder_back.py
--rw-r--r--   0 jemes      (501) staff       (20)    21077 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Eloquent/PostgresBuilder.py
--rw-r--r--   0 jemes      (501) staff       (20)    20590 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Eloquent/SqlServerBuilder.py
--rw-r--r--   0 jemes      (501) staff       (20)        0 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Eloquent/__init__.py
-drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql/Util/
--rw-r--r--   0 jemes      (501) staff       (20)     1616 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Util/Config.py
--rw-r--r--   0 jemes      (501) staff       (20)      812 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Util/Dynamic.py
--rw-r--r--   0 jemes      (501) staff       (20)     1221 2023-07-15 03:41:16.000000 simpysql-0.4.7/simpysql/Util/Expression.py
--rw-r--r--   0 jemes      (501) staff       (20)     1092 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Util/Logger.py
--rw-r--r--   0 jemes      (501) staff       (20)      441 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Util/MagicMetaClass.py
--rw-r--r--   0 jemes      (501) staff       (20)     1148 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Util/Response.py
--rw-r--r--   0 jemes      (501) staff       (20)       88 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/Util/__init__.py
--rw-r--r--   0 jemes      (501) staff       (20)       77 2022-08-15 06:51:36.000000 simpysql-0.4.7/simpysql/__init__.py
-drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql.egg-info/
--rw-r--r--   0 jemes      (501) staff       (20)     3511 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql.egg-info/PKG-INFO
--rw-r--r--   0 jemes      (501) staff       (20)     1087 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql.egg-info/SOURCES.txt
--rw-r--r--   0 jemes      (501) staff       (20)        1 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql.egg-info/dependency_links.txt
--rw-r--r--   0 jemes      (501) staff       (20)       46 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql.egg-info/entry_points.txt
--rw-r--r--   0 jemes      (501) staff       (20)       44 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql.egg-info/requires.txt
--rw-r--r--   0 jemes      (501) staff       (20)       62 2023-07-15 03:44:29.000000 simpysql-0.4.7/simpysql.egg-info/top_level.txt
+drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 04:27:09.000000 simpysql-0.4.8/
+-rw-r--r--   0 jemes      (501) staff       (20)     3511 2023-07-15 04:27:09.000000 simpysql-0.4.8/PKG-INFO
+-rw-r--r--   0 jemes      (501) staff       (20)     2482 2022-08-15 06:24:43.000000 simpysql-0.4.8/README.md
+-rw-r--r--   0 jemes      (501) staff       (20)       38 2023-07-15 04:27:09.000000 simpysql-0.4.8/setup.cfg
+-rw-r--r--   0 jemes      (501) staff       (20)      878 2023-07-15 04:26:59.000000 simpysql-0.4.8/setup.py
+drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql/
+drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql/Connections/
+-rw-r--r--   0 jemes      (501) staff       (20)      311 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Connections/Connection.py
+-rw-r--r--   0 jemes      (501) staff       (20)     1563 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Connections/ConnectionFactory.py
+-rw-r--r--   0 jemes      (501) staff       (20)     3235 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Connections/MongoConnection.py
+-rw-r--r--   0 jemes      (501) staff       (20)     2634 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Connections/MysqlConnection.py
+-rw-r--r--   0 jemes      (501) staff       (20)     1630 2022-08-15 07:00:44.000000 simpysql-0.4.8/simpysql/Connections/MysqlConnectionpool.py
+-rw-r--r--   0 jemes      (501) staff       (20)     3036 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Connections/PostgresConnection.py
+-rw-r--r--   0 jemes      (501) staff       (20)      632 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Connections/PostgresConnectionpool.py
+-rw-r--r--   0 jemes      (501) staff       (20)     2572 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Connections/SqlServerConnection.py
+-rw-r--r--   0 jemes      (501) staff       (20)        0 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Connections/__init__.py
+-rw-r--r--   0 jemes      (501) staff       (20)      956 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/DBModel.py
+drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql/Eloquent/
+-rw-r--r--   0 jemes      (501) staff       (20)      509 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Eloquent/BaseBuilder.py
+-rw-r--r--   0 jemes      (501) staff       (20)     1482 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Eloquent/BuilderFactory.py
+-rw-r--r--   0 jemes      (501) staff       (20)     9747 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Eloquent/MongoBuilder.py
+-rw-r--r--   0 jemes      (501) staff       (20)    21856 2023-07-15 03:59:26.000000 simpysql-0.4.8/simpysql/Eloquent/MysqlBuilder.py
+-rw-r--r--   0 jemes      (501) staff       (20)    21926 2022-08-15 06:24:43.000000 simpysql-0.4.8/simpysql/Eloquent/MysqlBuilder_back.py
+-rw-r--r--   0 jemes      (501) staff       (20)    21077 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Eloquent/PostgresBuilder.py
+-rw-r--r--   0 jemes      (501) staff       (20)    20590 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Eloquent/SqlServerBuilder.py
+-rw-r--r--   0 jemes      (501) staff       (20)        0 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Eloquent/__init__.py
+drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql/Util/
+-rw-r--r--   0 jemes      (501) staff       (20)     1616 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Util/Config.py
+-rw-r--r--   0 jemes      (501) staff       (20)      812 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Util/Dynamic.py
+-rw-r--r--   0 jemes      (501) staff       (20)     1221 2023-07-15 04:00:03.000000 simpysql-0.4.8/simpysql/Util/Expression.py
+-rw-r--r--   0 jemes      (501) staff       (20)     1092 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Util/Logger.py
+-rw-r--r--   0 jemes      (501) staff       (20)      441 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Util/MagicMetaClass.py
+-rw-r--r--   0 jemes      (501) staff       (20)     1148 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Util/Response.py
+-rw-r--r--   0 jemes      (501) staff       (20)       88 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/Util/__init__.py
+-rw-r--r--   0 jemes      (501) staff       (20)       77 2022-08-15 06:51:36.000000 simpysql-0.4.8/simpysql/__init__.py
+drwxr-xr-x   0 jemes      (501) staff       (20)        0 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql.egg-info/
+-rw-r--r--   0 jemes      (501) staff       (20)     3511 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql.egg-info/PKG-INFO
+-rw-r--r--   0 jemes      (501) staff       (20)     1087 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql.egg-info/SOURCES.txt
+-rw-r--r--   0 jemes      (501) staff       (20)        1 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql.egg-info/dependency_links.txt
+-rw-r--r--   0 jemes      (501) staff       (20)       46 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql.egg-info/entry_points.txt
+-rw-r--r--   0 jemes      (501) staff       (20)       44 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql.egg-info/requires.txt
+-rw-r--r--   0 jemes      (501) staff       (20)       62 2023-07-15 04:27:09.000000 simpysql-0.4.8/simpysql.egg-info/top_level.txt
```

### Comparing `simpysql-0.4.7/PKG-INFO` & `simpysql-0.4.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpysql
-Version: 0.4.7
+Version: 0.4.8
 Summary: A simple mysql orm base on pymysql
 Home-page: UNKNOWN
 Author: jeanku, liubin
 Author-email: 
 License: UNKNOWN
 Description: # SimpySql
```

### Comparing `simpysql-0.4.7/README.md` & `simpysql-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Connections/ConnectionFactory.py` & `simpysql-0.4.8/simpysql/Connections/ConnectionFactory.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Connections/MongoConnection.py` & `simpysql-0.4.8/simpysql/Connections/MongoConnection.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Connections/MysqlConnection.py` & `simpysql-0.4.8/simpysql/Connections/MysqlConnection.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Connections/MysqlConnectionpool.py` & `simpysql-0.4.8/simpysql/Connections/MysqlConnectionpool.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Connections/PostgresConnection.py` & `simpysql-0.4.8/simpysql/Connections/PostgresConnection.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Connections/PostgresConnectionpool.py` & `simpysql-0.4.8/simpysql/Connections/PostgresConnectionpool.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Connections/SqlServerConnection.py` & `simpysql-0.4.8/simpysql/Connections/SqlServerConnection.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/DBModel.py` & `simpysql-0.4.8/simpysql/DBModel.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Eloquent/BuilderFactory.py` & `simpysql-0.4.8/simpysql/Eloquent/BuilderFactory.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Eloquent/MongoBuilder.py` & `simpysql-0.4.8/simpysql/Eloquent/MongoBuilder.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Eloquent/MysqlBuilder.py` & `simpysql-0.4.8/simpysql/Eloquent/MysqlBuilder_back.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from .BaseBuilder import BaseBuilder
 from simpysql.Util.Dynamic import Dynamic
 
 
 class MysqlBuilder(BaseBuilder):
     operators = [
         '=', '<', '>', '<=', '>=', '<>', '!=',
-        'is', 'like', 'like binary', 'not like', 'between', 'ilike',
+        'like', 'like binary', 'not like', 'between', 'ilike',
         '&', '|', '^', '<<', '>>',
         'rlike', 'regexp', 'not regexp',
         '~', '~*', '!~', '!~*', 'similar to',
-        'not similar to', 'not ilike', '~~*', '!~~*', 'in', 'not in', 'not between', 'is not'
+        'not similar to', 'not ilike', '~~*', '!~~*', 'in', 'not in', 'not between'
     ]
 
     def __init__(self, model, alias=None):
         self.__model__ = model
         self.__alias__ = alias
         self.__where__ = []
         self.__orwhere__ = []  # orwhere处理逻辑
@@ -311,15 +311,15 @@
         subsql = ''.join(
             [self._compile_where(), self._compile_whereor(), self._compile_orwhere(), self._compile_groupby(),
              self._compile_orderby(),
              self._compile_having(), self._compile_limit(), self._compile_offset(), self._compile_lock()])
         joinsql = ''.join(self._compile_leftjoin())
         returnsql = "select {} from {}{}{}".format(','.join(self.__select__), self._tablename(), joinsql, subsql)
         if self.__union__:
-            return '({})'.format(returnsql) + self._compile_union()
+            return '{}'.format(returnsql) + self._compile_union()
         return returnsql
 
     def _compile_create(self, data):
         return "insert into {} {} values {}".format(self._tablename(), self._columnize(data[0]), self._valueize(data))
 
     def _compile_replace(self, data):
         return "replace into {} {} values {}".format(self._tablename(), self._columnize(data[0]), self._valueize(data))
@@ -538,15 +538,15 @@
                 index[update_column] = currtime
         return data
 
     def _set_update_time(self, data):
         currtime = self.__model__.fresh_timestamp()
         update_column = self.__model__.update_time_column()
         if update_column and update_column not in data:
-            data[update_column] = expr.format_string(currtime)
+            data[update_column] = currtime
         return data
 
     def transaction(self, callback):
         return self._get_connection().transaction(callback)
 
     def transaction_wrapper(self, callback):
         return self._get_connection().transaction_wrapper(callback)
```

### Comparing `simpysql-0.4.7/simpysql/Eloquent/MysqlBuilder_back.py` & `simpysql-0.4.8/simpysql/Eloquent/MysqlBuilder.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 from .BaseBuilder import BaseBuilder
 from simpysql.Util.Dynamic import Dynamic
 
 
 class MysqlBuilder(BaseBuilder):
     operators = [
         '=', '<', '>', '<=', '>=', '<>', '!=',
-        'like', 'like binary', 'not like', 'between', 'ilike',
+        'is', 'like', 'like binary', 'not like', 'between', 'ilike',
         '&', '|', '^', '<<', '>>',
         'rlike', 'regexp', 'not regexp',
         '~', '~*', '!~', '!~*', 'similar to',
-        'not similar to', 'not ilike', '~~*', '!~~*', 'in', 'not in', 'not between'
+        'not similar to', 'not ilike', '~~*', '!~~*', 'in', 'not in', 'not between', 'is not'
     ]
 
     def __init__(self, model, alias=None):
         self.__model__ = model
         self.__alias__ = alias
         self.__where__ = []
         self.__orwhere__ = []  # orwhere处理逻辑
@@ -311,15 +311,15 @@
         subsql = ''.join(
             [self._compile_where(), self._compile_whereor(), self._compile_orwhere(), self._compile_groupby(),
              self._compile_orderby(),
              self._compile_having(), self._compile_limit(), self._compile_offset(), self._compile_lock()])
         joinsql = ''.join(self._compile_leftjoin())
         returnsql = "select {} from {}{}{}".format(','.join(self.__select__), self._tablename(), joinsql, subsql)
         if self.__union__:
-            return '{}'.format(returnsql) + self._compile_union()
+            return '({})'.format(returnsql) + self._compile_union()
         return returnsql
 
     def _compile_create(self, data):
         return "insert into {} {} values {}".format(self._tablename(), self._columnize(data[0]), self._valueize(data))
 
     def _compile_replace(self, data):
         return "replace into {} {} values {}".format(self._tablename(), self._columnize(data[0]), self._valueize(data))
@@ -328,16 +328,15 @@
         return "insert into {} {} values {}".format(self._tablename(), self._columnize(columns),
                                                     ','.join([tuple(index).__str__() for index in data]))
 
     def _compile_update(self, data):
         return "update {} set {}{}".format(self._tablename(), ','.join(self._compile_dict(data)), self._compile_where())
 
     def _compile_increment(self, data):
-        subsql = ','.join(
-            ['{}={}'.format(expr.format_column(index, self.__model__), value) for index, value in data.items()])
+        subsql = ','.join(self._compile_dict(data))
         return "update {} set {}{}".format(self._tablename(), subsql, self._compile_where())
 
     def _compile_delete(self):
         return 'delete from {}{}'.format(self._tablename(), self._compile_where())
 
     def _compile_lastid(self):
         return 'select last_insert_id() as lastid'
```

### Comparing `simpysql-0.4.7/simpysql/Eloquent/PostgresBuilder.py` & `simpysql-0.4.8/simpysql/Eloquent/PostgresBuilder.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Eloquent/SqlServerBuilder.py` & `simpysql-0.4.8/simpysql/Eloquent/SqlServerBuilder.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Util/Config.py` & `simpysql-0.4.8/simpysql/Util/Config.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Util/Dynamic.py` & `simpysql-0.4.8/simpysql/Util/Dynamic.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Util/Expression.py` & `simpysql-0.4.8/simpysql/Util/Expression.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Util/Logger.py` & `simpysql-0.4.8/simpysql/Util/Logger.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql/Util/Response.py` & `simpysql-0.4.8/simpysql/Util/Response.py`

 * *Files identical despite different names*

### Comparing `simpysql-0.4.7/simpysql.egg-info/PKG-INFO` & `simpysql-0.4.8/simpysql.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simpysql
-Version: 0.4.7
+Version: 0.4.8
 Summary: A simple mysql orm base on pymysql
 Home-page: UNKNOWN
 Author: jeanku, liubin
 Author-email: 
 License: UNKNOWN
 Description: # SimpySql
```

### Comparing `simpysql-0.4.7/simpysql.egg-info/SOURCES.txt` & `simpysql-0.4.8/simpysql.egg-info/SOURCES.txt`

 * *Files identical despite different names*

