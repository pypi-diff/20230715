# Comparing `tmp/mysqlx-1.5.2.tar.gz` & `tmp/mysqlx-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\mysqlx-1.5.2.tar", last modified: Sat Jul 15 04:32:36 2023, max compression
+gzip compressed data, was "dist\mysqlx-1.5.3.tar", last modified: Sat Jul 15 04:33:41 2023, max compression
```

## Comparing `mysqlx-1.5.2.tar` & `mysqlx-1.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 04:32:36.000000 mysqlx-1.5.2/
--rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.5.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-07-15 04:32:36.000000 mysqlx-1.5.2/mysqlx/
--rw-rw-rw-   0        0        0      623 2023-07-10 16:08:00.000000 mysqlx-1.5.2/mysqlx/constant.py
--rw-rw-rw-   0        0        0    19185 2023-07-14 16:59:37.000000 mysqlx-1.5.2/mysqlx/db.py
--rw-rw-rw-   0        0        0    13298 2023-07-14 21:56:44.000000 mysqlx-1.5.2/mysqlx/dbx.py
--rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 mysqlx-1.5.2/mysqlx/log_support.py
--rw-rw-rw-   0        0        0    37131 2023-07-14 23:52:54.000000 mysqlx-1.5.2/mysqlx/orm.py
--rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.2/mysqlx/snowflake.py
--rw-rw-rw-   0        0        0     4077 2023-07-13 04:01:58.000000 mysqlx-1.5.2/mysqlx/sql_mapper.py
--rw-rw-rw-   0        0        0     6349 2023-07-13 04:01:58.000000 mysqlx-1.5.2/mysqlx/support.py
--rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.2/mysqlx/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 04:32:36.000000 mysqlx-1.5.2/mysqlx.egg-info/
--rw-rw-rw-   0        0        0        1 2023-07-15 04:32:36.000000 mysqlx-1.5.2/mysqlx.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-07-13 04:06:39.000000 mysqlx-1.5.2/mysqlx.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     4327 2023-07-15 04:32:36.000000 mysqlx-1.5.2/mysqlx.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       14 2023-07-15 04:32:36.000000 mysqlx-1.5.2/mysqlx.egg-info/requires.txt
--rw-rw-rw-   0        0        0      365 2023-07-15 04:32:36.000000 mysqlx-1.5.2/mysqlx.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        7 2023-07-15 04:32:36.000000 mysqlx-1.5.2/mysqlx.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4327 2023-07-15 04:32:36.000000 mysqlx-1.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     3802 2023-07-15 04:32:14.000000 mysqlx-1.5.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-15 04:32:36.000000 mysqlx-1.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1211 2023-07-14 23:25:59.000000 mysqlx-1.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 04:33:41.000000 mysqlx-1.5.3/
+-rw-rw-rw-   0        0        0    11558 2021-11-30 10:47:21.000000 mysqlx-1.5.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx/
+-rw-rw-rw-   0        0        0      623 2023-07-10 16:08:00.000000 mysqlx-1.5.3/mysqlx/constant.py
+-rw-rw-rw-   0        0        0    19185 2023-07-14 16:59:37.000000 mysqlx-1.5.3/mysqlx/db.py
+-rw-rw-rw-   0        0        0    13298 2023-07-14 21:56:44.000000 mysqlx-1.5.3/mysqlx/dbx.py
+-rw-rw-rw-   0        0        0     3984 2023-07-13 13:31:18.000000 mysqlx-1.5.3/mysqlx/log_support.py
+-rw-rw-rw-   0        0        0    37131 2023-07-14 23:52:54.000000 mysqlx-1.5.3/mysqlx/orm.py
+-rw-rw-rw-   0        0        0     2392 2023-06-26 14:23:12.000000 mysqlx-1.5.3/mysqlx/snowflake.py
+-rw-rw-rw-   0        0        0     4077 2023-07-13 04:01:58.000000 mysqlx-1.5.3/mysqlx/sql_mapper.py
+-rw-rw-rw-   0        0        0     6349 2023-07-13 04:01:58.000000 mysqlx-1.5.3/mysqlx/support.py
+-rw-rw-rw-   0        0        0        0 2021-11-30 12:54:44.000000 mysqlx-1.5.3/mysqlx/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-07-13 04:06:39.000000 mysqlx-1.5.3/mysqlx.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     4327 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      365 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        7 2023-07-15 04:33:41.000000 mysqlx-1.5.3/mysqlx.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4327 2023-07-15 04:33:41.000000 mysqlx-1.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3802 2023-07-15 04:33:38.000000 mysqlx-1.5.3/README.rst
+-rw-rw-rw-   0        0        0       42 2023-07-15 04:33:41.000000 mysqlx-1.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1211 2023-07-15 04:33:38.000000 mysqlx-1.5.3/setup.py
```

### Comparing `mysqlx-1.5.2/LICENSE` & `mysqlx-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.2/mysqlx/constant.py` & `mysqlx-1.5.3/mysqlx/constant.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.2/mysqlx/db.py` & `mysqlx-1.5.3/mysqlx/db.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.2/mysqlx/dbx.py` & `mysqlx-1.5.3/mysqlx/dbx.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.2/mysqlx/log_support.py` & `mysqlx-1.5.3/mysqlx/log_support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.2/mysqlx/orm.py` & `mysqlx-1.5.3/mysqlx/orm.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.2/mysqlx/snowflake.py` & `mysqlx-1.5.3/mysqlx/snowflake.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.2/mysqlx/sql_mapper.py` & `mysqlx-1.5.3/mysqlx/sql_mapper.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.2/mysqlx/support.py` & `mysqlx-1.5.3/mysqlx/support.py`

 * *Files identical despite different names*

### Comparing `mysqlx-1.5.2/mysqlx.egg-info/PKG-INFO` & `mysqlx-1.5.3/mysqlx.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.2
+Version: 1.5.3
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
@@ -143,10 +143,10 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
 
-If you want to operate PostgreSQL database, please use PgSqlx: https://gitee.com/summry/pgsqlx/
+If you want to operate PostgreSQL database, please use PgSqlx: https://pypi.org/project/pgsqlx/
```

### Comparing `mysqlx-1.5.2/PKG-INFO` & `mysqlx-1.5.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysqlx
-Version: 1.5.2
+Version: 1.5.3
 Summary: MySqlx is a simple python sql executor for MySQL like MyBatis.
 Home-page: https://gitee.com/summry/mysqlx
 Author: summry
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sql,MySQL,MyBatis,python
 Platform: UNKNOWN
@@ -143,10 +143,10 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
 
-If you want to operate PostgreSQL database, please use PgSqlx: https://gitee.com/summry/pgsqlx/
+If you want to operate PostgreSQL database, please use PgSqlx: https://pypi.org/project/pgsqlx/
```

### Comparing `mysqlx-1.5.2/README.rst` & `mysqlx-1.5.3/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -129,8 +129,8 @@
    def test_transaction2():
        with transaction():
            insert_func(....)
            update_func(....)
 
 You can generate model class with mysqlx-generator: https://pypi.org/project/mysqlx-generator
 
-If you want to operate PostgreSQL database, please use PgSqlx: https://gitee.com/summry/pgsqlx/
+If you want to operate PostgreSQL database, please use PgSqlx: https://pypi.org/project/pgsqlx/
```

### Comparing `mysqlx-1.5.2/setup.py` & `mysqlx-1.5.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     description="MySqlx is a simple python sql executor for MySQL like MyBatis.",
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=[
         'Jinja2>=2.7.0',
         # 'mysql-connector-python>=8.0.13',
     ],
-    version='1.5.2',
+    version='1.5.3',
     url='https://gitee.com/summry/mysqlx',
     author='summry',
     author_email='xiazhongbiao@126.com',
     keywords=['sql', 'MySQL', 'MyBatis', 'python'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

