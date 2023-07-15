# Comparing `tmp/sqldao-generator-0.2.0.tar.gz` & `tmp/sqldao-generator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqldao-generator-0.2.0.tar", last modified: Sat Jul 15 06:40:52 2023, max compression
+gzip compressed data, was "sqldao-generator-0.2.1.tar", last modified: Sat Jul 15 07:46:25 2023, max compression
```

## Comparing `sqldao-generator-0.2.0.tar` & `sqldao-generator-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.830769 sqldao-generator-0.2.0/
--rw-rw-rw-   0        0        0      440 2023-07-15 06:40:52.830769 sqldao-generator-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2059 2023-07-15 06:37:28.000000 sqldao-generator-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-15 06:40:52.830769 sqldao-generator-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-07-15 06:35:31.000000 sqldao-generator-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.815144 sqldao-generator-0.2.0/sqldao_generator.egg-info/
--rw-rw-rw-   0        0        0      440 2023-07-15 06:40:52.000000 sqldao-generator-0.2.0/sqldao_generator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1857 2023-07-15 06:40:52.000000 sqldao-generator-0.2.0/sqldao_generator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 06:40:52.000000 sqldao-generator-0.2.0/sqldao_generator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2023-07-15 06:40:52.000000 sqldao-generator-0.2.0/sqldao_generator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-07-15 06:40:52.000000 sqldao-generator-0.2.0/sqldao_generator.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.783894 sqldao-generator-0.2.0/sqldaogenerator/
-drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.799519 sqldao-generator-0.2.0/sqldaogenerator/common/
--rw-rw-rw-   0        0        0      575 2023-07-15 05:33:46.000000 sqldao-generator-0.2.0/sqldaogenerator/common/Criterion.py
--rw-rw-rw-   0        0        0      263 2023-07-09 05:32:41.000000 sqldao-generator-0.2.0/sqldaogenerator/common/Database.py
--rw-rw-rw-   0        0        0     2045 2023-07-09 05:42:10.000000 sqldao-generator-0.2.0/sqldaogenerator/common/TransactionManager.py
--rw-rw-rw-   0        0        0        0 2023-07-01 05:44:52.000000 sqldao-generator-0.2.0/sqldaogenerator/common/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.799519 sqldao-generator-0.2.0/sqldaogenerator/entity/
--rw-rw-rw-   0        0        0      245 2023-07-04 11:14:21.000000 sqldao-generator-0.2.0/sqldaogenerator/entity/General.py
--rw-rw-rw-   0        0        0      142 2023-07-04 12:50:50.000000 sqldao-generator-0.2.0/sqldaogenerator/entity/Page.py
--rw-rw-rw-   0        0        0        0 2023-07-01 13:43:56.000000 sqldao-generator-0.2.0/sqldaogenerator/entity/__init__.py
--rw-rw-rw-   0        0        0       86 2023-06-30 13:49:06.000000 sqldao-generator-0.2.0/sqldaogenerator/entity/base.py
-drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.799519 sqldao-generator-0.2.0/sqldaogenerator/generator/
--rw-rw-rw-   0        0        0        0 2023-06-28 05:41:54.000000 sqldao-generator-0.2.0/sqldaogenerator/generator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.799519 sqldao-generator-0.2.0/sqldaogenerator/generator/enums/
--rw-rw-rw-   0        0        0      324 2023-07-02 06:41:27.000000 sqldao-generator-0.2.0/sqldaogenerator/generator/enums/MySqlTypeEnum.py
--rw-rw-rw-   0        0        0        0 2023-06-28 06:35:09.000000 sqldao-generator-0.2.0/sqldaogenerator/generator/enums/__init__.py
--rw-rw-rw-   0        0        0     8638 2023-07-08 09:37:34.000000 sqldao-generator-0.2.0/sqldaogenerator/generator/mysql_generator.py
-drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.799519 sqldao-generator-0.2.0/sqldaogenerator/logger/
--rw-rw-rw-   0        0        0        0 2023-06-28 05:41:42.000000 sqldao-generator-0.2.0/sqldaogenerator/logger/__init__.py
--rw-rw-rw-   0        0        0      139 2023-07-02 12:44:00.000000 sqldao-generator-0.2.0/sqldaogenerator/logger/logger.py
-drwxrwxrwx   0        0        0        0 2023-07-15 06:40:52.815144 sqldao-generator-0.2.0/sqldaogenerator/resources/
--rw-rw-rw-   0        0        0        0 2023-07-02 05:38:36.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/__init__.py
--rw-rw-rw-   0        0        0      812 2023-07-15 06:32:45.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/base_dao_template.txt
--rw-rw-rw-   0        0        0     1095 2023-07-15 05:33:47.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/criterion_template.txt
--rw-rw-rw-   0        0        0     3020 2023-07-15 06:32:45.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/dao_template.txt
--rw-rw-rw-   0        0        0      723 2023-07-15 05:28:29.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/datasource_template.txt
--rw-rw-rw-   0        0        0      361 2023-07-15 05:28:29.000000 sqldao-generator-0.2.0/sqldaogenerator/resources/entity_template.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.126779 sqldao-generator-0.2.1/
+-rw-rw-rw-   0        0        0      440 2023-07-15 07:46:25.126779 sqldao-generator-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2556 2023-07-15 06:50:28.000000 sqldao-generator-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 07:46:25.126779 sqldao-generator-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      930 2023-07-15 07:43:56.000000 sqldao-generator-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.126779 sqldao-generator-0.2.1/sqldao_generator.egg-info/
+-rw-rw-rw-   0        0        0      440 2023-07-15 07:46:25.000000 sqldao-generator-0.2.1/sqldao_generator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1857 2023-07-15 07:46:25.000000 sqldao-generator-0.2.1/sqldao_generator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 07:46:25.000000 sqldao-generator-0.2.1/sqldao_generator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-07-15 07:46:25.000000 sqldao-generator-0.2.1/sqldao_generator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-07-15 07:46:25.000000 sqldao-generator-0.2.1/sqldao_generator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.095129 sqldao-generator-0.2.1/sqldaogenerator/
+drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.095129 sqldao-generator-0.2.1/sqldaogenerator/common/
+-rw-rw-rw-   0        0        0      575 2023-07-15 05:33:46.000000 sqldao-generator-0.2.1/sqldaogenerator/common/Criterion.py
+-rw-rw-rw-   0        0        0      263 2023-07-09 05:32:41.000000 sqldao-generator-0.2.1/sqldaogenerator/common/Database.py
+-rw-rw-rw-   0        0        0     2060 2023-07-15 07:37:04.000000 sqldao-generator-0.2.1/sqldaogenerator/common/TransactionManager.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 05:44:52.000000 sqldao-generator-0.2.1/sqldaogenerator/common/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.095129 sqldao-generator-0.2.1/sqldaogenerator/entity/
+-rw-rw-rw-   0        0        0      245 2023-07-04 11:14:21.000000 sqldao-generator-0.2.1/sqldaogenerator/entity/General.py
+-rw-rw-rw-   0        0        0      142 2023-07-04 12:50:50.000000 sqldao-generator-0.2.1/sqldaogenerator/entity/Page.py
+-rw-rw-rw-   0        0        0        0 2023-07-01 13:43:56.000000 sqldao-generator-0.2.1/sqldaogenerator/entity/__init__.py
+-rw-rw-rw-   0        0        0       86 2023-06-30 13:49:06.000000 sqldao-generator-0.2.1/sqldaogenerator/entity/base.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.110138 sqldao-generator-0.2.1/sqldaogenerator/generator/
+-rw-rw-rw-   0        0        0        0 2023-06-28 05:41:54.000000 sqldao-generator-0.2.1/sqldaogenerator/generator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.111144 sqldao-generator-0.2.1/sqldaogenerator/generator/enums/
+-rw-rw-rw-   0        0        0      324 2023-07-02 06:41:27.000000 sqldao-generator-0.2.1/sqldaogenerator/generator/enums/MySqlTypeEnum.py
+-rw-rw-rw-   0        0        0        0 2023-06-28 06:35:09.000000 sqldao-generator-0.2.1/sqldaogenerator/generator/enums/__init__.py
+-rw-rw-rw-   0        0        0     9478 2023-07-15 07:37:04.000000 sqldao-generator-0.2.1/sqldaogenerator/generator/mysql_generator.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.111144 sqldao-generator-0.2.1/sqldaogenerator/logger/
+-rw-rw-rw-   0        0        0        0 2023-06-28 05:41:42.000000 sqldao-generator-0.2.1/sqldaogenerator/logger/__init__.py
+-rw-rw-rw-   0        0        0      139 2023-07-02 12:44:00.000000 sqldao-generator-0.2.1/sqldaogenerator/logger/logger.py
+drwxrwxrwx   0        0        0        0 2023-07-15 07:46:25.111144 sqldao-generator-0.2.1/sqldaogenerator/resources/
+-rw-rw-rw-   0        0        0        0 2023-07-02 05:38:36.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/__init__.py
+-rw-rw-rw-   0        0        0      915 2023-07-15 07:41:08.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/base_dao_template.txt
+-rw-rw-rw-   0        0        0     1095 2023-07-15 05:33:47.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/criterion_template.txt
+-rw-rw-rw-   0        0        0     3283 2023-07-15 07:41:38.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/dao_template.txt
+-rw-rw-rw-   0        0        0      723 2023-07-15 05:28:29.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/datasource_template.txt
+-rw-rw-rw-   0        0        0      361 2023-07-15 05:28:29.000000 sqldao-generator-0.2.1/sqldaogenerator/resources/entity_template.txt
```

### Comparing `sqldao-generator-0.2.0/README.md` & `sqldao-generator-0.2.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -5,14 +5,30 @@
 ## Notice
 
 - Currently, only MySQL and one database are supported.
 
 ## Usage
 
 - See example/test/generator.py, SampleTest.py
+
+- Create a table first
+```sql
+create table t_sample
+(
+    id           bigint unsigned auto_increment comment '主鍵'
+        primary key,
+    col_var      varchar(100)  null comment '字串',
+    col_text     text          null comment '長字串',
+    col_tinyint  tinyint       null comment '微整數',
+    col_int      int           null comment '整數',
+    col_double   double(10, 2) null comment '浮點數',
+    col_datetime datetime      null comment '時間'
+);
+```
+
 - Generate a dao and entity from a table
 
 ```python
 from example import dao, entity
 from sqldaogenerator.generator.mysql_generator import generate
 
 generate('user', 'password', 'host', port, 'database',
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sqldao-generator-0.2.0/setup.py` & `sqldao-generator-0.2.1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='sqldao-generator',
-    version='0.2.0',
+    version='0.2.1',
     author='Daniel Hsu',
     description='SqlAlchemy DAO generator',
     long_description_content_type='text/markdown',
     url='https://github.com/davidhsusl/sqldao-generator',
     keywords='SQLAlchemy, mysql',
     python_requires='>=3.10, <4',
     py_modules=['sqldaogenerator'],  # Name of the python package
     package_dir={'': '.'},  # Directory of the source code of the package
     packages=find_packages(include=['sqldaogenerator.*']),
-    package_data={'': ['*.json', '*.txt']},
+    package_data={'': ['*.json', '*.txt', '*.sql']},
     install_requires=[
         'mysql-connector-python>=8.0.0,<9.0.0',
         'SQLAlchemy>=2.0.0,<3.0.0'
     ],
     author_email='',
     classifiers=[
         'Programming Language :: Python :: 3',
```

### Comparing `sqldao-generator-0.2.0/sqldao_generator.egg-info/SOURCES.txt` & `sqldao-generator-0.2.1/sqldao_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.2.0/sqldaogenerator/common/Criterion.py` & `sqldao-generator-0.2.1/sqldaogenerator/common/Criterion.py`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.2.0/sqldaogenerator/common/TransactionManager.py` & `sqldao-generator-0.2.1/sqldaogenerator/common/TransactionManager.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,16 @@
         return session
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.transaction_thread.session.close()
         self.transaction_thread.is_exists = False
 
     def is_exists(self):
-        return hasattr(self.transaction_thread, 'is_exists') and self.transaction_thread.is_exists
+        return hasattr(self.transaction_thread, 'is_exists') \
+            and self.transaction_thread.is_exists
 
     def get_transaction(self) -> Session:
         if self.is_exists():
             return self.transaction_thread.session
         else:
             raise LookupError('No existing transaction.')
```

### Comparing `sqldao-generator-0.2.0/sqldaogenerator/generator/mysql_generator.py` & `sqldao-generator-0.2.1/sqldaogenerator/generator/mysql_generator.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,59 +32,89 @@
 
 
 def add_set(sets: list[str], column: str, type: str):
     sets.append(set_template.format(column=column, type=type))
 
 
 def add_equal(filters: list[str], column: str, type: str, entity_name: str):
-    filters.append(ifelse_filter_template.format(column=column, suffix='', type=type, entity_name=entity_name,
-                                                 condition='', if_expression=' == value', else_expression=' != value', other=''))
-    filters.append(null_filter_template.format(column=column, suffix='_null', entity_name=entity_name,
-                                               if_expression='.is_(None)', else_expression='.isnot(None)'))
-    filters.append(ifelse_filter_template.format(column=column, suffix='_in', type=f"list[{type}]", entity_name=entity_name,
-                                                 condition=" and len(value) > 0", if_expression='.in_(value)',
-                                                 else_expression='.notin_(value)', other=''))
+    filters.append(ifelse_filter_template
+                   .format(column=column, suffix='', type=type,
+                           entity_name=entity_name,
+                           condition='', if_expression=' == value',
+                           else_expression=' != value', other=''))
+    filters.append(null_filter_template
+                   .format(column=column, suffix='_null',
+                           entity_name=entity_name,
+                           if_expression='.is_(None)',
+                           else_expression='.isnot(None)'))
+    filters.append(ifelse_filter_template
+                   .format(column=column, suffix='_in', type=f"list[{type}]",
+                           entity_name=entity_name,
+                           condition=" and len(value) > 0",
+                           if_expression='.in_(value)',
+                           else_expression='.notin_(value)', other=''))
 
 
 def add_num(filters: list[str], column: str, type: str, entity_name: str):
-    filters.append(filter_template.format(column=column, suffix='_gte', type=type, entity_name=entity_name,
-                                          condition="", expression=' >= value'))
-    filters.append(filter_template.format(column=column, suffix='_lte', type=type, entity_name=entity_name,
-                                          condition="", expression=' <= value'))
+    filters.append(filter_template
+                   .format(column=column, suffix='_gte', type=type,
+                           entity_name=entity_name,
+                           condition="", expression=' >= value'))
+    filters.append(filter_template
+                   .format(column=column, suffix='_lte', type=type,
+                           entity_name=entity_name,
+                           condition="", expression=' <= value'))
 
 
 def add_datetime(filters: list[str], column: str, type: str, entity_name: str):
-    filters.append(filter_template.format(column=column, suffix='_start', type=type, entity_name=entity_name,
-                                          condition='', expression=' >= value'))
-    filters.append(filter_template.format(column=column, suffix='_end', type=type, entity_name=entity_name,
-                                          condition='', expression=' <= value'))
+    filters.append(filter_template
+                   .format(column=column, suffix='_start', type=type,
+                           entity_name=entity_name,
+                           condition='', expression=' >= value'))
+    filters.append(filter_template
+                   .format(column=column, suffix='_end', type=type,
+                           entity_name=entity_name,
+                           condition='', expression=' <= value'))
 
 
 def add_like(filters: list[str], column: str, type: str, entity_name: str):
-    filters.append(ifelse_filter_template.format(column=column, suffix='_like', type=type, entity_name=entity_name,
-                                                 condition=" and value != ''", if_expression='.like(f"{left}{value}{right}")',
-                                                 else_expression='.not_like(f"{left}{value}{right}")', other=", left='%', right='%'"))
+    filters.append(ifelse_filter_template
+                   .format(column=column, suffix='_like', type=type,
+                           entity_name=entity_name,
+                           condition=" and value != ''",
+                           if_expression='.like(f"{left}{value}{right}")',
+                           else_expression='.not_like(f"{left}{value}{right}")',
+                           other=", left='%', right='%'"))
 
 
 def generate(user: str, password: str, host: str, port: int, database: str,
-             datasource_package: ModuleType, datasource_name: str, base_dao_package: ModuleType, base_dao_name: str,
-             dao_package: ModuleType, entity_package: ModuleType, entity_name: str, table: str, override_datasource=False):
+             datasource_package: ModuleType, datasource_name: str,
+             base_dao_package: ModuleType, base_dao_name: str,
+             dao_package: ModuleType, entity_package: ModuleType,
+             entity_name: str, table: str, override_datasource=False):
     # create a Datasource
-    datasource_file = pkg_resources.files(datasource_package).joinpath(f"{datasource_name}.py")
+    datasource_file = pkg_resources.files(datasource_package) \
+        .joinpath(f"{datasource_name}.py")
     if override_datasource or not datasource_file.is_file():
-        template = pkg_resources.files(resources).joinpath('datasource_template.txt').read_text()
-        template = template.format(datasource_name=datasource_name, user=user, password=password, host=host, port=port, dbname=database)
+        template = pkg_resources.files(resources) \
+            .joinpath('datasource_template.txt').read_text()
+        template = template.format(datasource_name=datasource_name,
+                                   user=user, password=password, host=host,
+                                   port=port, dbname=database)
         with datasource_file.open('w', encoding='utf-8') as file:
             file.write(template)
 
     # create a BaseDao
-    base_dao_file = pkg_resources.files(base_dao_package).joinpath(f"{base_dao_name}.py")
-    template = pkg_resources.files(resources).joinpath('base_dao_template.txt').read_text()
+    base_dao_file = pkg_resources.files(base_dao_package) \
+        .joinpath(f"{base_dao_name}.py")
+    template = pkg_resources.files(resources) \
+        .joinpath('base_dao_template.txt').read_text()
     template = template.format(base_dao_name=base_dao_name,
-                               datasource_package=datasource_package.__package__, datasource_name=datasource_name)
+                               datasource_package=datasource_package.__package__,
+                               datasource_name=datasource_name)
     with base_dao_file.open('w', encoding='utf-8') as file:
         file.write(template)
 
     connection_string = f"mysql+mysqlconnector://{user}:{password}@{host}:{port}/{database}"
     engine = create_engine(connection_string, echo=True, pool_recycle=270)
     with engine.connect() as connection:
         results = connection.execute(text(f"""
@@ -98,24 +128,28 @@
     camelcased_word = re.findall('[A-Z][a-z0-9]*', entity_name)
     underlined_word = '_'.join(camelcased_word).lower()
     columns = []
     sets = []
     filters = []
     for result in results:
         column_name = result.COLUMN_NAME.lower()
-        data_type = result.DATA_TYPE.decode() if isinstance(result.DATA_TYPE, bytes) else result.DATA_TYPE
-        comment = result.COLUMN_COMMENT.decode() if isinstance(result.COLUMN_COMMENT, bytes) else result.COLUMN_COMMENT
+        data_type = result.DATA_TYPE.decode() \
+            if isinstance(result.DATA_TYPE, bytes) else result.DATA_TYPE
+        comment = result.COLUMN_COMMENT.decode() \
+            if isinstance(result.COLUMN_COMMENT, bytes) \
+            else result.COLUMN_COMMENT
 
         # column
         if result.COLUMN_KEY == 'PRI':
             template = primary_key_template
         else:
             template = column_template
         columns.append(template.format(
-            column=column_name, comment=comment, type=MySqlTypeEnum[data_type].value))
+            column=column_name, comment=comment,
+            type=MySqlTypeEnum[data_type].value))
 
         # fields, filters
         match [column_name, data_type]:
             case [_, ('varchar' | 'text')]:
                 py_type = 'str'
                 add_set(sets, column_name, py_type)
                 add_equal(filters, column_name, py_type, entity_name)
@@ -130,23 +164,34 @@
                 add_set(sets, column_name, py_type)
                 add_equal(filters, column_name, py_type, entity_name)
                 add_datetime(filters, column_name, py_type, entity_name)
 
     # entity
     tab = '    '
     filter_intent = f"\n\n{tab}"
-    for template_name, file_name in [('entity_template.txt', entity_name), ('criterion_template.txt', f"{entity_name}Criterion")]:
-        template = pkg_resources.files(resources).joinpath(template_name).read_text()
-        template = template.format(entity_name=entity_name, table=table, columns=f'\n{tab}'.join(columns),
-                                   sets=filter_intent.join(sets), filters=filter_intent.join(filters),
+    for template_name, file_name \
+            in [('entity_template.txt', entity_name),
+                ('criterion_template.txt', f"{entity_name}Criterion")]:
+        template = pkg_resources.files(resources) \
+            .joinpath(template_name).read_text()
+        template = template.format(entity_name=entity_name, table=table,
+                                   columns=f'\n{tab}'.join(columns),
+                                   sets=filter_intent.join(sets),
+                                   filters=filter_intent.join(filters),
                                    entity_package=entity_package.__package__)
-        entity_file = pkg_resources.files(entity_package).joinpath(f"{file_name}.py")
+        entity_file = pkg_resources.files(entity_package) \
+            .joinpath(f"{file_name}.py")
         with entity_file.open('w', encoding='utf-8') as file:
             file.write(template)
 
     # dao
-    template = pkg_resources.files(resources).joinpath('dao_template.txt').read_text()
-    template = template.format(base_dao_package=base_dao_package.__package__, base_dao_name=base_dao_name,
-                               entity_package=entity_package.__package__, entity_name=entity_name, entity_variable=underlined_word)
-    entity_file = pkg_resources.files(dao_package).joinpath(f"{entity_name}Dao.py")
+    template = pkg_resources.files(resources) \
+        .joinpath('dao_template.txt').read_text()
+    template = template.format(base_dao_package=base_dao_package.__package__,
+                               base_dao_name=base_dao_name,
+                               entity_package=entity_package.__package__,
+                               entity_name=entity_name,
+                               entity_variable=underlined_word)
+    entity_file = pkg_resources.files(dao_package) \
+        .joinpath(f"{entity_name}Dao.py")
     with entity_file.open('w', encoding='utf-8') as file:
         file.write(template)
```

### Comparing `sqldao-generator-0.2.0/sqldaogenerator/resources/base_dao_template.txt` & `sqldao-generator-0.2.1/sqldaogenerator/resources/base_dao_template.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,14 +8,17 @@
 
 class {base_dao_name}:
     datasource: {datasource_name}
 
     def __init__(self):
         self.datasource = datasource
 
+    def is_transaction_exists(self):
+        return self.datasource.transactionManager.is_exists()
+
     def get_transaction(self):
         return self.datasource.transactionManager.get_transaction()
 
     def new_transaction(self):
         return self.datasource.transactionManager.new_transaction()
 
     @staticmethod
```

### Comparing `sqldao-generator-0.2.0/sqldaogenerator/resources/criterion_template.txt` & `sqldao-generator-0.2.1/sqldaogenerator/resources/criterion_template.txt`

 * *Files identical despite different names*

### Comparing `sqldao-generator-0.2.0/sqldaogenerator/resources/dao_template.txt` & `sqldao-generator-0.2.1/sqldaogenerator/resources/dao_template.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,25 +10,33 @@
 
 class {entity_name}Dao({base_dao_name}):
 
     def select(self, criterion: Criterion) -> tuple[list[{entity_name}], int]:
         criterion_list = criterion.to_list()
         assert self.is_in_modules(criterion_list, {entity_name}), \
             'The expressions must be created by the {entity_name} entity.'
-        with self.new_transaction() as session:
+        is_transaction_exists = self.is_transaction_exists()
+        if is_transaction_exists:
+            session = self.get_transaction()
+        else:
+            session = self.new_transaction()
+        try:
             page = criterion.page
             orders = page.order_by.split(' ')
             query = session.query({entity_name}).filter(*criterion_list) \
                 .order_by(eval(f"{entity_name}.{{orders[0]}}.{{orders[1]}}()"))
             total = None
             if page.page_no is not None and page.page_size is not None:
                 query = query.offset((page.page_no - 1) * page.page_size) \
                     .limit(page.page_size)
                 total = session.query({entity_name}).filter(*criterion_list).count()
             entities = query.all()
+        finally:
+            if not is_transaction_exists:
+                session.close()
         return entities, total or len(entities)
 
     @transactional
     def insert(self, criterion: Criterion):
         session = self.get_transaction()
         entity = {entity_name}(**criterion.values)
         session.add(entity)
```

### Comparing `sqldao-generator-0.2.0/sqldaogenerator/resources/datasource_template.txt` & `sqldao-generator-0.2.1/sqldaogenerator/resources/datasource_template.txt`

 * *Files identical despite different names*

