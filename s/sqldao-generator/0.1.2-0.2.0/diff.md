# Comparing `tmp/sqldao-generator-0.1.2.tar.gz` & `tmp/sqldao-generator-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldao-generator-0.1.2.tar", last modified: Sun Jul  9 11:06:17 2023, max compression
+gzip compressed data, was "sqldao-generator-0.2.0.tar", last modified: Sat Jul 15 06:40:52 2023, max compression
```

## Comparing `sqldao-generator-0.1.2.tar` & `sqldao-generator-0.2.0.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-09 11:06:17.523282 sqldao-generator-0.1.2/
--rw-rw-rw-   0        0        0      440 2023-07-09 11:06:17.523282 sqldao-generator-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1892 2023-07-09 06:19:24.000000 sqldao-generator-0.1.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-09 11:06:17.523282 sqldao-generator-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-07-09 11:05:53.000000 sqldao-generator-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:06:17.523282 sqldao-generator-0.1.2/sqldao_generator.egg-info/
--rw-rw-rw-   0        0        0      440 2023-07-09 11:06:17.000000 sqldao-generator-0.1.2/sqldao_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2023-07-09 11:06:17.000000 sqldao-generator-0.1.2/sqldao_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-09 11:06:17.000000 sqldao-generator-0.1.2/sqldao_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-09 11:06:17.000000 sqldao-generator-0.1.2/sqldao_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-09 11:06:17.000000 sqldao-generator-0.1.2/sqldao_generator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-09 11:06:17.492073 sqldao-generator-0.1.2/sqldaogenerator/
-drwxrwxrwx   0        0        0        0 2023-07-09 11:06:17.507654 sqldao-generator-0.1.2/sqldaogenerator/common/
--rw-rw-rw-   0        0        0      514 2023-07-04 13:19:49.000000 sqldao-generator-0.1.2/sqldaogenerator/common/Criterion.py
--rw-rw-rw-   0        0        0      263 2023-07-09 05:32:41.000000 sqldao-generator-0.1.2/sqldaogenerator/common/Database.py
--rw-rw-rw-   0        0        0     2045 2023-07-09 05:42:10.000000 sqldao-generator-0.1.2/sqldaogenerator/common/TransactionManager.py
--rw-rw-rw-   0        0        0        0 2023-07-01 05:44:52.000000 sqldao-generator-0.1.2/sqldaogenerator/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:06:17.507654 sqldao-generator-0.1.2/sqldaogenerator/entity/
--rw-rw-rw-   0        0        0      245 2023-07-04 11:14:21.000000 sqldao-generator-0.1.2/sqldaogenerator/entity/General.py
--rw-rw-rw-   0        0        0      142 2023-07-04 12:50:50.000000 sqldao-generator-0.1.2/sqldaogenerator/entity/Page.py
--rw-rw-rw-   0        0        0        0 2023-07-01 13:43:56.000000 sqldao-generator-0.1.2/sqldaogenerator/entity/__init__.py
--rw-rw-rw-   0        0        0       86 2023-06-30 13:49:06.000000 sqldao-generator-0.1.2/sqldaogenerator/entity/base.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:06:17.507654 sqldao-generator-0.1.2/sqldaogenerator/generator/
--rw-rw-rw-   0        0        0        0 2023-06-28 05:41:54.000000 sqldao-generator-0.1.2/sqldaogenerator/generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:06:17.507654 sqldao-generator-0.1.2/sqldaogenerator/generator/enums/
--rw-rw-rw-   0        0        0      324 2023-07-02 06:41:27.000000 sqldao-generator-0.1.2/sqldaogenerator/generator/enums/MySqlTypeEnum.py
--rw-rw-rw-   0        0        0        0 2023-06-28 06:35:09.000000 sqldao-generator-0.1.2/sqldaogenerator/generator/enums/__init__.py
--rw-rw-rw-   0        0        0     8638 2023-07-08 09:37:34.000000 sqldao-generator-0.1.2/sqldaogenerator/generator/mysql_generator.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:06:17.507654 sqldao-generator-0.1.2/sqldaogenerator/logger/
--rw-rw-rw-   0        0        0        0 2023-06-28 05:41:42.000000 sqldao-generator-0.1.2/sqldaogenerator/logger/__init__.py
--rw-rw-rw-   0        0        0      139 2023-07-02 12:44:00.000000 sqldao-generator-0.1.2/sqldaogenerator/logger/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-09 11:06:17.507654 sqldao-generator-0.1.2/sqldaogenerator/resources/
--rw-rw-rw-   0        0        0        0 2023-07-02 05:38:36.000000 sqldao-generator-0.1.2/sqldaogenerator/resources/__init__.py
--rw-rw-rw-   0        0        0      489 2023-07-09 05:46:36.000000 sqldao-generator-0.1.2/sqldaogenerator/resources/base_dao_template.txt
--rw-rw-rw-   0        0        0     1029 2023-07-08 06:30:32.000000 sqldao-generator-0.1.2/sqldaogenerator/resources/criterion_template.txt
--rw-rw-rw-   0        0        0     2543 2023-07-09 05:46:36.000000 sqldao-generator-0.1.2/sqldaogenerator/resources/dao_template.txt
--rw-rw-rw-   0        0        0      644 2023-07-09 05:46:36.000000 sqldao-generator-0.1.2/sqldaogenerator/resources/datasource_template.txt
--rw-rw-rw-   0        0        0      356 2023-07-08 06:30:32.000000 sqldao-generator-0.1.2/sqldaogenerator/resources/entity_template.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.830769 sqldao-generator-0.2.0/
+-rw-rw-rw-   0        0        0      440 2023-07-15 06:40:52.830769 sqldao-generator-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2059 2023-07-15 06:37:28.000000 sqldao-generator-0.2.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 06:40:52.830769 sqldao-generator-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      921 2023-07-15 06:35:31.000000 sqldao-generator-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.815144 sqldao-generator-0.2.0/sqldao_generator.egg-info/
+-rw-rw-rw-   0        0        0      440 2023-07-15 06:40:52.000000 sqldao-generator-0.2.0/sqldao_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1857 2023-07-15 06:40:52.000000 sqldao-generator-0.2.0/sqldao_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 06:40:52.000000 sqldao-generator-0.2.0/sqldao_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-15 06:40:52.000000 sqldao-generator-0.2.0/sqldao_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-15 06:40:52.000000 sqldao-generator-0.2.0/sqldao_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.783894 sqldao-generator-0.2.0/sqldaogenerator/
+drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.799519 sqldao-generator-0.2.0/sqldaogenerator/common/
+-rw-rw-rw-   0        0        0      575 2023-07-15 05:33:46.000000 sqldao-generator-0.2.0/sqldaogenerator/common/Criterion.py
+-rw-rw-rw-   0        0        0      263 2023-07-09 05:32:41.000000 sqldao-generator-0.2.0/sqldaogenerator/common/Database.py
+-rw-rw-rw-   0        0        0     2045 2023-07-09 05:42:10.000000 sqldao-generator-0.2.0/sqldaogenerator/common/TransactionManager.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 05:44:52.000000 sqldao-generator-0.2.0/sqldaogenerator/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.799519 sqldao-generator-0.2.0/sqldaogenerator/entity/
+-rw-rw-rw-   0        0        0      245 2023-07-04 11:14:21.000000 sqldao-generator-0.2.0/sqldaogenerator/entity/General.py
+-rw-rw-rw-   0        0        0      142 2023-07-04 12:50:50.000000 sqldao-generator-0.2.0/sqldaogenerator/entity/Page.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 13:43:56.000000 sqldao-generator-0.2.0/sqldaogenerator/entity/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-06-30 13:49:06.000000 sqldao-generator-0.2.0/sqldaogenerator/entity/base.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.799519 sqldao-generator-0.2.0/sqldaogenerator/generator/
+-rw-rw-rw-   0        0        0        0 2023-06-28 05:41:54.000000 sqldao-generator-0.2.0/sqldaogenerator/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.799519 sqldao-generator-0.2.0/sqldaogenerator/generator/enums/
+-rw-rw-rw-   0        0        0      324 2023-07-02 06:41:27.000000 sqldao-generator-0.2.0/sqldaogenerator/generator/enums/MySqlTypeEnum.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 06:35:09.000000 sqldao-generator-0.2.0/sqldaogenerator/generator/enums/__init__.py
+-rw-rw-rw-   0        0        0     8638 2023-07-08 09:37:34.000000 sqldao-generator-0.2.0/sqldaogenerator/generator/mysql_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.799519 sqldao-generator-0.2.0/sqldaogenerator/logger/
+-rw-rw-rw-   0        0        0        0 2023-06-28 05:41:42.000000 sqldao-generator-0.2.0/sqldaogenerator/logger/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-07-02 12:44:00.000000 sqldao-generator-0.2.0/sqldaogenerator/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.815144 sqldao-generator-0.2.0/sqldaogenerator/resources/
+-rw-rw-rw-   0        0        0        0 2023-07-02 05:38:36.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/__init__.py
+-rw-rw-rw-   0        0        0      812 2023-07-15 06:32:45.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/base_dao_template.txt
+-rw-rw-rw-   0        0        0     1095 2023-07-15 05:33:47.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/criterion_template.txt
+-rw-rw-rw-   0        0        0     3020 2023-07-15 06:32:45.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/dao_template.txt
+-rw-rw-rw-   0        0        0      723 2023-07-15 05:28:29.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/datasource_template.txt
+-rw-rw-rw-   0        0        0      361 2023-07-15 05:28:29.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/entity_template.txt
```

### Comparing `sqldao-generator-0.1.2/README.md` & `sqldao-generator-0.2.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -12,49 +12,75 @@
 - Generate a dao and entity from a table
 
 ```python
 from example import dao, entity
 from sqldaogenerator.generator.mysql_generator import generate
 
 generate('user', 'password', 'host', port, 'database',
-         datasource_package=dao, datasource_name='Datasource', base_dao_package=dao, base_dao_name='BaseDao',
-         dao_package=dao, entity_package=entity, entity_name='Sample', table='t_sample', override_datasource=True)
+         datasource_package=dao, datasource_name='Datasource', 
+         base_dao_package=dao, base_dao_name='BaseDao', dao_package=dao, 
+         entity_package=entity, entity_name='Sample', table='t_sample', 
+         override_datasource=True)
 ```
 
 - Select
 
 ```python
-criterion = SampleCriterion.builder().col_var_like('df').col_text_in(['6']).col_tinyint_gte(1).col_int_lte(5).col_double(3.5)
-.col_datetime_start('2023-07-04 08:26:40').col_datetime_end('2023-07-04 08:26:40').page_no(1).page_size(10).build()
-entities, total = sample_dao.select_sample(criterion)
+criterion = SampleCriterion.builder()
+    .col_var_like('df')
+    .col_text_in(['6'])
+    .col_tinyint_gte(1)
+    .col_int_lte(5)
+    .col_double(3.5)
+    .col_datetime_start('2023-07-04 08:26:40')
+    .col_datetime_end('2023-07-04 08:26:40')
+    .page_no(1)
+    .page_size(10)
+    .build()
+entities, total = sample_dao.select(criterion)
 ```
 
 - Insert
 
 ```python
 now = datetime.now().strftime(date_format)
-sample = SampleCriterion.builder().set_col_var('i').set_col_text('6').set_col_tinyint(1).set_col_int(5).set_col_double(3.5)
-.set_col_datetime(now).build()
-entity = sample_dao.insert_sample(sample)
+sample = SampleCriterion.builder()
+    .set_col_var('i')
+    .set_col_text('6')
+    .set_col_tinyint(1)
+    .set_col_int(5)
+    .set_col_double(3.5)
+    .set_col_datetime(now)
+    .build()
+entity = sample_dao.insert(sample)
 print(entity.id)
 ```
 
 - Update
 
 ```python
-criterion = SampleCriterion.builder().id_in([13, 15]).set_col_var('g').set_col_text('m').set_col_tinyint(3).set_col_int(9)
-.set_col_double(6.5).set_col_datetime(datetime.fromisoformat('2023-07-04T21:30:56')).build()
-sample_dao.update_sample(criterion)
+criterion = SampleCriterion.builder()
+    .id_in([13, 15])
+    .set_col_var('g')
+    .set_col_text('m')
+    .set_col_tinyint(3)
+    .set_col_int(9)
+    .set_col_double(6.5)
+    .set_col_datetime(datetime.fromisoformat('2023-07-04T21:30:56'))
+    .build()
+total = sample_dao.update(criterion)
 ```
 
 - Delete
 
 ```python
-criterion = SampleCriterion.builder().id(8).build()
-sample_dao.delete_sample(criterion)
+criterion = SampleCriterion.builder()
+    .id(8)
+    .build()
+total = sample_dao.delete(criterion)
 ```
 
 - Execute in the same transaction
 
 ```python
 from sqldaogenerator.common.TransactionManager import transactional
```

### Comparing `sqldao-generator-0.1.2/setup.py` & `sqldao-generator-0.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sqldao-generator',
-    version='0.1.2',
+    version='0.2.0',
     author='Daniel Hsu',
     description='SqlAlchemy DAO generator',
     long_description_content_type='text/markdown',
     url='https://github.com/davidhsusl/sqldao-generator',
     keywords='SQLAlchemy, mysql',
     python_requires='>=3.10, <4',
     py_modules=['sqldaogenerator'],  # Name of the python package
```

### Comparing `sqldao-generator-0.1.2/sqldao_generator.egg-info/SOURCES.txt` & `sqldao-generator-0.2.0/sqldao_generator.egg-info/SOURCES.txt`

 * *Files 19% similar despite different names*

```diff
@@ -20,8 +20,28 @@
 ./sqldaogenerator/resources/dao_template.txt
 ./sqldaogenerator/resources/datasource_template.txt
 ./sqldaogenerator/resources/entity_template.txt
 sqldao_generator.egg-info/PKG-INFO
 sqldao_generator.egg-info/SOURCES.txt
 sqldao_generator.egg-info/dependency_links.txt
 sqldao_generator.egg-info/requires.txt
-sqldao_generator.egg-info/top_level.txt
+sqldao_generator.egg-info/top_level.txt
+sqldaogenerator/common/Criterion.py
+sqldaogenerator/common/Database.py
+sqldaogenerator/common/TransactionManager.py
+sqldaogenerator/common/__init__.py
+sqldaogenerator/entity/General.py
+sqldaogenerator/entity/Page.py
+sqldaogenerator/entity/__init__.py
+sqldaogenerator/entity/base.py
+sqldaogenerator/generator/__init__.py
+sqldaogenerator/generator/mysql_generator.py
+sqldaogenerator/generator/enums/MySqlTypeEnum.py
+sqldaogenerator/generator/enums/__init__.py
+sqldaogenerator/logger/__init__.py
+sqldaogenerator/logger/logger.py
+sqldaogenerator/resources/__init__.py
+sqldaogenerator/resources/base_dao_template.txt
+sqldaogenerator/resources/criterion_template.txt
+sqldaogenerator/resources/dao_template.txt
+sqldaogenerator/resources/datasource_template.txt
+sqldaogenerator/resources/entity_template.txt
```

### Comparing `sqldao-generator-0.1.2/sqldaogenerator/common/Criterion.py` & `sqldao-generator-0.2.0/sqldaogenerator/common/Criterion.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from dataclasses import dataclass, field
 
+from sqlalchemy import BinaryExpression
+
 from sqldaogenerator.entity.Page import Page
 
 
 @dataclass
 class Criterion:
     page: Page
-    filters: list[any] = field(default_factory=list)
-    values: dict[any] = field(default_factory=dict)
+    filters: list[BinaryExpression] = field(default_factory=list)
+    values: dict[str, any] = field(default_factory=dict)
 
     def __getitem__(self, item):
         return self.values[item]
 
     def get(self, key, default):
         return self.values.get(key, default)
```

### Comparing `sqldao-generator-0.1.2/sqldaogenerator/common/TransactionManager.py` & `sqldao-generator-0.2.0/sqldaogenerator/common/TransactionManager.py`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.1.2/sqldaogenerator/generator/mysql_generator.py` & `sqldao-generator-0.2.0/sqldaogenerator/generator/mysql_generator.py`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.1.2/sqldaogenerator/resources/criterion_template.txt` & `sqldao-generator-0.2.0/sqldaogenerator/resources/criterion_template.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,26 @@
-"""This file is generated by sqldao-generator; don't modify anything. If you need to do it, you should create another class."""
+"""
+This file is generated by sqldao-generator; don't modify anything.
+If you need to do it, you should create another class.
+"""
 from dataclasses import dataclass, field
 from datetime import datetime
 
+from sqlalchemy import BinaryExpression
+
 from {entity_package}.{entity_name} import {entity_name}
 from sqldaogenerator.common.Criterion import Criterion
 from sqldaogenerator.entity.Page import Page
 
 
 @dataclass
 class {entity_name}Criterion:
     page = Page()
-    filters: list[any] = field(default_factory=list)
-    values: dict[any] = field(default_factory=dict)
+    filters: list[BinaryExpression] = field(default_factory=list)
+    values: dict[str, any] = field(default_factory=dict)
 
     @classmethod
     def builder(cls):
         return cls()
 
     def build(self):
         return Criterion(page=self.page, filters=self.filters, values=self.values)
```

### Comparing `sqldao-generator-0.1.2/sqldaogenerator/resources/dao_template.txt` & `sqldao-generator-0.2.0/sqldaogenerator/resources/dao_template.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,53 +1,68 @@
-"""This file is generated by sqldao-generator; don't modify anything. If you need to do it, you should create another class."""
+"""
+This file is generated by sqldao-generator; don't modify anything.
+If you need to do it, you should create another class.
+"""
 from {base_dao_package}.{base_dao_name} import {base_dao_name}
 from {entity_package}.{entity_name} import {entity_name}
 from sqldaogenerator.common.Criterion import Criterion
 from sqldaogenerator.common.TransactionManager import transactional
 
 
 class {entity_name}Dao({base_dao_name}):
 
-    def select_{entity_variable}(self, criterion: Criterion) -> tuple[list[{entity_name}], int]:
+    def select(self, criterion: Criterion) -> tuple[list[{entity_name}], int]:
+        criterion_list = criterion.to_list()
+        assert self.is_in_modules(criterion_list, {entity_name}), \
+            'The expressions must be created by the {entity_name} entity.'
         with self.new_transaction() as session:
-            criterion_list = criterion.to_list()
             page = criterion.page
             orders = page.order_by.split(' ')
-            query = session.query({entity_name}).filter(*criterion_list).order_by(eval(f"{entity_name}.{{orders[0]}}.{{orders[1]}}()"))
+            query = session.query({entity_name}).filter(*criterion_list) \
+                .order_by(eval(f"{entity_name}.{{orders[0]}}.{{orders[1]}}()"))
             total = None
             if page.page_no is not None and page.page_size is not None:
-                query = query.offset((page.page_no - 1) * page.page_size).limit(page.page_size)
+                query = query.offset((page.page_no - 1) * page.page_size) \
+                    .limit(page.page_size)
                 total = session.query({entity_name}).filter(*criterion_list).count()
             entities = query.all()
-        return entities, len(entities) if total is None else total
+        return entities, total or len(entities)
 
     @transactional
-    def insert_{entity_variable}(self, criterion: Criterion):
+    def insert(self, criterion: Criterion):
         session = self.get_transaction()
         entity = {entity_name}(**criterion.values)
         session.add(entity)
         session.flush()
         session.refresh(entity)
         session.expunge(entity)
         return entity
 
     @transactional
-    def update_{entity_variable}(self, criterion: Criterion):
+    def update(self, criterion: Criterion):
         criterion_list = criterion.to_list()
-        assert criterion_list is not None and len(criterion_list) > 0, 'Must have at least one condition in the update.'
+        assert criterion_list is not None and len(criterion_list) > 0, \
+            'Must have at least one condition in the update.'
+        assert self.is_in_modules(criterion_list, {entity_name}), \
+            'The expressions must be created by the {entity_name} entity.'
         session = self.get_transaction()
         entities = session.query({entity_name}).filter(*criterion_list).all()
         for entity in entities:
             for key, value in criterion.items():
-                exec(f"entity.{{key}}=value")
+                setattr(entity, key, value)
+        return len(entities)
 
     @transactional
-    def delete_{entity_variable}(self, criterion: Criterion):
+    def delete(self, criterion: Criterion):
         criterion_list = criterion.to_list()
-        assert criterion_list is not None and len(criterion_list) > 0, 'Must have at least one condition in the delete.'
+        assert criterion_list is not None and len(criterion_list) > 0, \
+            'Must have at least one condition in the delete.'
+        assert self.is_in_modules(criterion_list, {entity_name}), \
+            'The expressions must be created by the {entity_name} entity.'
         session = self.get_transaction()
         entities = session.query({entity_name}).filter(*criterion_list).all()
         for entity in entities:
             session.delete(entity)
+        return len(entities)
 
 
 {entity_variable}_dao = {entity_name}Dao()
```

### Comparing `sqldao-generator-0.1.2/sqldaogenerator/resources/datasource_template.txt` & `sqldao-generator-0.2.0/sqldaogenerator/resources/datasource_template.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,25 @@
-"""This file is generated by sqldao-generator; you can modify connection properties yourself."""
+"""
+This file is generated by sqldao-generator;
+you can modify connection properties yourself.
+"""
 from sqlalchemy import create_engine
 
 from sqldaogenerator.common.Database import Database
 
 
 class {datasource_name}(Database):
 
     def __init__(self):
         user = '{user}'
         password = '{password}'
         host = '{host}'
         port = {port}
         dbname = '{dbname}'
         connection_string = f"mysql+mysqlconnector://{{user}}:{{password}}@{{host}}:{{port}}/{{dbname}}"
-        self.engine = create_engine(connection_string, echo=True, pool_recycle=270)
+        self.engine = create_engine(connection_string,
+                                    echo=True,
+                                    pool_recycle=270)
         super().__init__()
 
 
 datasource = Datasource()
```

