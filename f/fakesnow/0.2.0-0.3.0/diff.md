# Comparing `tmp/fakesnow-0.2.0.tar.gz` & `tmp/fakesnow-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fakesnow-0.2.0.tar", last modified: Sat Jun 24 05:20:28 2023, max compression
+gzip compressed data, was "fakesnow-0.3.0.tar", last modified: Sat Jul 15 01:02:08 2023, max compression
```

## Comparing `fakesnow-0.2.0.tar` & `fakesnow-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:20:28.764951 fakesnow-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-24 05:20:18.000000 fakesnow-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-24 05:20:18.000000 fakesnow-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-24 05:20:28.764951 fakesnow-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-06-24 05:20:18.000000 fakesnow-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:20:28.764951 fakesnow-0.2.0/fakesnow/
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    19502 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    18172 2023-06-24 05:20:18.000000 fakesnow-0.2.0/fakesnow/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:20:28.764951 fakesnow-0.2.0/fakesnow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-06-24 05:20:28.000000 fakesnow-0.2.0/fakesnow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-24 05:20:28.000000 fakesnow-0.2.0/fakesnow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 05:20:28.000000 fakesnow-0.2.0/fakesnow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-24 05:20:28.000000 fakesnow-0.2.0/fakesnow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-24 05:20:28.000000 fakesnow-0.2.0/fakesnow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-06-24 05:20:18.000000 fakesnow-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 05:20:28.764951 fakesnow-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-24 05:20:18.000000 fakesnow-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 05:20:28.764951 fakesnow-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-06-24 05:20:18.000000 fakesnow-0.2.0/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-06-24 05:20:18.000000 fakesnow-0.2.0/tests/test_expr.py
--rw-r--r--   0 runner    (1001) docker     (123)    25787 2023-06-24 05:20:18.000000 fakesnow-0.2.0/tests/test_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-06-24 05:20:18.000000 fakesnow-0.2.0/tests/test_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-06-24 05:20:18.000000 fakesnow-0.2.0/tests/test_transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:02:08.483699 fakesnow-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-15 01:01:57.000000 fakesnow-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-07-15 01:01:57.000000 fakesnow-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-15 01:02:08.483699 fakesnow-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-07-15 01:01:57.000000 fakesnow-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:02:08.479699 fakesnow-0.3.0/fakesnow/
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22362 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    21842 2023-07-15 01:01:57.000000 fakesnow-0.3.0/fakesnow/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:02:08.479699 fakesnow-0.3.0/fakesnow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-07-15 01:02:08.000000 fakesnow-0.3.0/fakesnow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-15 01:02:08.000000 fakesnow-0.3.0/fakesnow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 01:02:08.000000 fakesnow-0.3.0/fakesnow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-07-15 01:02:08.000000 fakesnow-0.3.0/fakesnow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-15 01:02:08.000000 fakesnow-0.3.0/fakesnow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2212 2023-07-15 01:01:57.000000 fakesnow-0.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 01:02:08.483699 fakesnow-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-15 01:01:57.000000 fakesnow-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 01:02:08.479699 fakesnow-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1801 2023-07-15 01:01:57.000000 fakesnow-0.3.0/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-15 01:01:57.000000 fakesnow-0.3.0/tests/test_expr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28884 2023-07-15 01:01:57.000000 fakesnow-0.3.0/tests/test_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-15 01:01:57.000000 fakesnow-0.3.0/tests/test_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-07-15 01:01:57.000000 fakesnow-0.3.0/tests/test_transforms.py
```

### Comparing `fakesnow-0.2.0/LICENSE` & `fakesnow-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fakesnow-0.2.0/PKG-INFO` & `fakesnow-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.2.0
+Version: 0.3.0
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -30,14 +30,18 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: notebook
 License-File: LICENSE
 
 # fakesnow ❄️
 
+[![ci](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml)
+[![release](https://github.com/tekumara/fakesnow/actions/workflows/release.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/release.yml)
+[![PyPI](https://img.shields.io/pypi/v/fakesnow?color=violet)](https://pypi.org/project/fakesnow/)
+
 Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run and mock Snowflake DB locally.
 
 ## Install
 
 ```
 pip install fakesnow
 ```
```

### Comparing `fakesnow-0.2.0/README.md` & `fakesnow-0.3.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # fakesnow ❄️
 
+[![ci](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml)
+[![release](https://github.com/tekumara/fakesnow/actions/workflows/release.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/release.yml)
+[![PyPI](https://img.shields.io/pypi/v/fakesnow?color=violet)](https://pypi.org/project/fakesnow/)
+
 Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run and mock Snowflake DB locally.
 
 ## Install
 
 ```
 pip install fakesnow
 ```
```

### Comparing `fakesnow-0.2.0/fakesnow/__init__.py` & `fakesnow-0.3.0/fakesnow/__init__.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.2.0/fakesnow/checks.py` & `fakesnow-0.3.0/fakesnow/checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.2.0/fakesnow/expr.py` & `fakesnow-0.3.0/fakesnow/expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.2.0/fakesnow/fakes.py` & `fakesnow-0.3.0/fakesnow/fakes.py`

 * *Files 12% similar despite different names*

```diff
@@ -33,14 +33,42 @@
     ext_table_schema varchar,
     ext_table_name varchar,
     comment varchar,
     PRIMARY KEY(ext_table_catalog, ext_table_schema, ext_table_name)
 )
 """
 )
+SQL_CREATE_INFORMATION_SCHEMA_COLUMNS_EXT = Template(
+    """
+create table ${catalog}.information_schema.columns_ext (
+    ext_table_catalog varchar,
+    ext_table_schema varchar,
+    ext_table_name varchar,
+    ext_column_name varchar,
+    ext_character_maximum_length integer,
+    ext_character_octet_length integer,
+    PRIMARY KEY(ext_table_catalog, ext_table_schema, ext_table_name, ext_column_name)
+)
+"""
+)
+# only include fields applicable to snowflake (as mentioned by describe table information_schema.columns)
+
+SQL_CREATE_INFORMATION_SCHEMA_COLUMNS_VIEW = Template(
+    """
+create view ${catalog}.information_schema.columns_snowflake AS
+select table_catalog, table_schema, table_name, column_name, ordinal_position, column_default, is_nullable, data_type,
+ext_character_maximum_length as character_maximum_length, ext_character_octet_length as character_octet_length,
+numeric_precision, numeric_precision_radix, numeric_scale,
+collation_name, is_identity, identity_generation, identity_cycle
+from ${catalog}.information_schema.columns
+left join ${catalog}.information_schema.columns_ext ext
+on ext_table_catalog = table_catalog AND ext_table_schema = table_schema
+AND ext_table_name = table_name AND ext_column_name = column_name
+"""
+)
 
 
 class FakeSnowflakeCursor:
     def __init__(
         self,
         conn: FakeSnowflakeConnection,
         duck_conn: DuckDBPyConnection,
@@ -130,69 +158,90 @@
             ) from None
 
         transformed = (
             expression.transform(transforms.upper_case_unquoted_identifiers)
             .transform(transforms.set_schema, current_database=self._conn.database)
             .transform(transforms.create_database)
             .transform(transforms.extract_comment)
-            .transform(transforms.join_information_schema_ext)
+            .transform(transforms.information_schema_columns_snowflake)
+            .transform(transforms.information_schema_tables_ext)
             .transform(transforms.drop_schema_cascade)
             .transform(transforms.tag)
             .transform(transforms.regex)
             .transform(transforms.semi_structured_types)
             .transform(transforms.parse_json)
             .transform(transforms.indices_to_array)
             .transform(transforms.indices_to_object)
             .transform(transforms.values_columns)
             .transform(transforms.to_date)
             .transform(transforms.object_construct)
+            .transform(transforms.timestamp_ntz_ns)
+            .transform(transforms.float_to_double)
+            .transform(transforms.integer_precision)
+            .transform(transforms.extract_text_length)
         )
-
         sql = transformed.sql(dialect="duckdb")
 
-        if cmd != "COMMENT TABLE":
-            try:
-                self._last_sql = sql
-                self._last_params = params
-                self._duck_conn.execute(sql, params)
-            except duckdb.BinderException as e:
-                msg = e.args[0]
-                raise snowflake.connector.errors.ProgrammingError(msg=msg, errno=2043, sqlstate="02000") from None
-            except duckdb.CatalogException as e:
-                # minimal processing to make it look like a snowflake exception, message content may differ
-                msg = cast(str, e.args[0]).split("\n")[0]
-                raise snowflake.connector.errors.ProgrammingError(msg=msg, errno=2003, sqlstate="42S02") from None
+        try:
+            self._last_sql = sql
+            self._last_params = params
+            self._duck_conn.execute(sql, params)
+        except duckdb.BinderException as e:
+            msg = e.args[0]
+            raise snowflake.connector.errors.ProgrammingError(msg=msg, errno=2043, sqlstate="02000") from None
+        except duckdb.CatalogException as e:
+            # minimal processing to make it look like a snowflake exception, message content may differ
+            msg = cast(str, e.args[0]).split("\n")[0]
+            raise snowflake.connector.errors.ProgrammingError(msg=msg, errno=2003, sqlstate="42S02") from None
 
         if cmd == "USE DATABASE" and (ident := expression.find(exp.Identifier)) and isinstance(ident.this, str):
             self._conn.database = ident.this.upper()
             self._conn.database_set = True
 
         if cmd == "USE SCHEMA" and (ident := expression.find(exp.Identifier)) and isinstance(ident.this, str):
             self._conn.schema = ident.this.upper()
             self._conn.schema_set = True
 
-        if cmd == "CREATE DATABASE":
-            # make sure every database has the info schema extension table
-            catalog = transformed.args["db_name"] or self._conn.database
-            self._duck_conn.execute(SQL_CREATE_INFORMATION_SCHEMA_TABLES_EXT.substitute(catalog=catalog))
+        if create_db_name := transformed.args.get("create_db_name"):
+            # we created a new database, so create the info schema extensions
+            self._conn._create_info_schema_ext(create_db_name)  # noqa: SLF001
 
         if table_comment := transformed.args.get("table_comment"):
-            # store table comment, if any
-            assert (table := transformed.find(exp.Table)), "Cannot find table"
+            # record table comment
+            table, comment = table_comment
             catalog = table.catalog or self._conn.database
             schema = table.db or self._conn.schema
             self._duck_conn.execute(
                 f"""
-                INSERT INTO information_schema.tables_ext
-                values ('{catalog}', '{schema}', '{table.name}', '{table_comment}')
+                INSERT INTO {catalog}.information_schema.tables_ext
+                values ('{catalog}', '{schema}', '{table.name}', '{comment}')
                 ON CONFLICT (ext_table_catalog, ext_table_schema, ext_table_name)
                 DO UPDATE SET comment = excluded.comment
                 """
             )
 
+        if (text_lengths := transformed.args.get("text_lengths")) and (table := transformed.find(exp.Table)):
+            # record text lengths
+            catalog = table.catalog or self._conn.database
+            schema = table.db or self._conn.schema
+            values = ", ".join(
+                f"('{catalog}', '{schema}', '{table.name}', '{col_name}', {size}, {min(size*4,16777216)})"
+                for (col_name, size) in text_lengths
+            )
+
+            self._duck_conn.execute(
+                f"""
+                INSERT INTO {catalog}.information_schema.columns_ext
+                values {values}
+                ON CONFLICT (ext_table_catalog, ext_table_schema, ext_table_name, ext_column_name)
+                DO UPDATE SET ext_character_maximum_length = excluded.ext_character_maximum_length,
+                                ext_character_octet_length = excluded.ext_character_octet_length
+                """
+            )
+
         return self
 
     def executemany(
         self,
         command: str,
         seqparams: Sequence[Any] | dict[str, Any],
         **kwargs: Any,
@@ -226,15 +275,15 @@
         if not self._arrow_table:
             self._arrow_table = self._duck_conn.fetch_arrow_table()
             self._arrow_table_fetch_one_index = -1
 
         self._arrow_table_fetch_one_index += 1
 
         try:
-            return self._arrow_table.take([self._arrow_table_fetch_one_index]).to_pylist()
+            return self._arrow_table.take([self._arrow_table_fetch_one_index]).to_pylist()[0]
         except pyarrow.lib.ArrowIndexError:
             return None
 
     def get_result_batches(self) -> list[ResultBatch] | None:
         # rows_per_batch is approximate
         # see https://github.com/duckdb/duckdb/issues/4755
         reader = self._duck_conn.fetch_record_batch(rows_per_batch=1000)
@@ -270,15 +319,15 @@
                     name=column_name, type_code=0, display_size=None, internal_size=None, precision=precision, scale=scale, is_nullable=True # type: ignore # noqa: E501
                 )
             elif column_type == "VARCHAR":
                 # TODO: fetch internal_size from varchar size
                 return ResultMetadata(
                     name=column_name, type_code=2, display_size=None, internal_size=16777216, precision=None, scale=None, is_nullable=True   # type: ignore # noqa: E501
                 )
-            elif column_type == "FLOAT":
+            elif column_type == "DOUBLE":
                 return ResultMetadata(
                     name=column_name, type_code=1, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True       # type: ignore # noqa: E501
                 )
             elif column_type == "BOOLEAN":
                 return ResultMetadata(
                     name=column_name, type_code=13, display_size=None, internal_size=None, precision=None, scale=None, is_nullable=True      # type: ignore # noqa: E501
                 )
@@ -325,14 +374,15 @@
         database: Optional[str] = None,
         schema: Optional[str] = None,
         create_database: bool = True,
         create_schema: bool = True,
         *args: Any,
         **kwargs: Any,
     ):
+        self._duck_conn = duck_conn
         # upper case database and schema like snowflake
         self.database = database and database.upper()
         self.schema = schema and schema.upper()
         self.database_set = False
         self.schema_set = False
         self._paramstyle = "pyformat"
 
@@ -342,15 +392,15 @@
             and self.database
             and not duck_conn.execute(
                 f"""select * from information_schema.schemata
                 where catalog_name = '{self.database}'"""
             ).fetchone()
         ):
             duck_conn.execute(f"ATTACH DATABASE ':memory:' AS {self.database}")
-            duck_conn.execute(SQL_CREATE_INFORMATION_SCHEMA_TABLES_EXT.substitute(catalog=self.database))
+            self._create_info_schema_ext(self.database)
 
         # create schema if needed
         if (
             create_schema
             and self.database
             and self.schema
             and not duck_conn.execute(
@@ -379,15 +429,16 @@
                 f"""select * from information_schema.schemata
                 where catalog_name = '{self.database}'"""
             ).fetchone()
         ):
             duck_conn.execute(f"SET schema='{self.database}.main'")
             self.database_set = True
 
-        self._duck_conn = duck_conn
+        # use UTC instead of local time zone for consistent testing
+        duck_conn.execute("SET TimeZone = 'UTC'")
 
     def __enter__(self) -> Self:
         return self
 
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]] = ...,
@@ -427,14 +478,20 @@
         # whereas duckdb loads them as a struct, so we convert them to json here
         cols = [f"TO_JSON({c})" if isinstance(df[c][0], dict) else c for c in df.columns]
         cols = ",".join(cols)
 
         self._duck_conn.execute(f"INSERT INTO {table_name}({','.join(df.columns.to_list())}) SELECT {cols} FROM df")
         return self._duck_conn.fetchall()[0][0]
 
+    def _create_info_schema_ext(self, catalog: str) -> None:
+        """Create the info schema extension tables/views used for storing snowflake metadata not captured by duckdb."""
+        self._duck_conn.execute(SQL_CREATE_INFORMATION_SCHEMA_TABLES_EXT.substitute(catalog=catalog))
+        self._duck_conn.execute(SQL_CREATE_INFORMATION_SCHEMA_COLUMNS_EXT.substitute(catalog=catalog))
+        self._duck_conn.execute(SQL_CREATE_INFORMATION_SCHEMA_COLUMNS_VIEW.substitute(catalog=catalog))
+
 
 class FakeResultBatch(ResultBatch):
     def __init__(self, use_dict_result: bool, batch: pyarrow.RecordBatch):
         self._use_dict_result = use_dict_result
         self._batch = batch
 
     def create_iter(
```

### Comparing `fakesnow-0.2.0/fakesnow/transforms.py` & `fakesnow-0.3.0/fakesnow/transforms.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from typing import cast
 
 import sqlglot
 from sqlglot import exp
 
 MISSING_DATABASE = "missing_database"
-SUCCESS_NO_OP = sqlglot.parse_one("SELECT 'Statement executed successfully.'")
+SUCCESS_NOP = sqlglot.parse_one("SELECT 'Statement executed successfully.'")
 
 
 def as_describe(expression: exp.Expression) -> exp.Expression:
     """Prepend describe to the expression.
 
     Example:
         >>> import sqlglot
@@ -34,24 +34,24 @@
         >>> import sqlglot
         >>> sqlglot.parse_one("CREATE database foo").transform(create_database).sql()
         'ATTACH DATABASE ':memory:' as foo'
     Args:
         expression (exp.Expression): the expression that will be transformed.
 
     Returns:
-        exp.Expression: The transformed expression, with the database name stored in the db_name arg.
+        exp.Expression: The transformed expression, with the database name stored in the create_db_name arg.
     """
 
     if isinstance(expression, exp.Create) and str(expression.args.get("kind")).upper() == "DATABASE":
         assert (ident := expression.find(exp.Identifier)), f"No identifier in {expression.sql}"
         db_name = ident.this
         return exp.Command(
             this="ATTACH",
             expression=exp.Literal(this=f"DATABASE ':memory:' AS {db_name}", is_string=True),
-            db_name=db_name,
+            create_db_name=db_name,
         )
 
     return expression
 
 
 def drop_schema_cascade(expression: exp.Expression) -> exp.Expression:
     """Drop schema cascade.
@@ -83,50 +83,110 @@
     return new
 
 
 def extract_comment(expression: exp.Expression) -> exp.Expression:
     """Extract table comment, removing it from the Expression.
 
     duckdb doesn't support comments. So we remove them from the expression and store them in the table_comment arg.
+    We also replace the transform the expression to NOP if the statement can't be executed by duckdb.
 
-    Example:
-        >>> import sqlglot
-        >>> sqlglot.parse_one("CREATE TABLE table1 (id int) COMMENT = 'comment1'").transform(extract_comment).sql()
-        'CREATE TABLE table1 (id int)'
-        >>> sqlglot.parse_one("COMMENT ON TABLE table1 IS 'comment1'").transform(extract_comment).arg('table_comment')
-        'comment1'
     Args:
         expression (exp.Expression): the expression that will be transformed.
 
     Returns:
         exp.Expression: The transformed expression, with any comment stored in the new 'table_comment' arg.
     """
 
-    if isinstance(expression, exp.Create):
+    if isinstance(expression, exp.Create) and (table := expression.find(exp.Table)):
         comment = None
         if props := cast(exp.Properties, expression.args.get("properties")):
             other_props = []
             for p in props.expressions:
                 if isinstance(p, exp.SchemaCommentProperty) and (isinstance(p.this, (exp.Literal, exp.Identifier))):
                     comment = p.this.this
                 else:
                     other_props.append(p)
 
             new = expression.copy()
             new_props: exp.Properties = new.args["properties"]
-            new_props.args["expressions"] = other_props
-            new.args["table_comment"] = comment
+            new_props.set("expressions", other_props)
+            new.args["table_comment"] = (table, comment)
             return new
     elif (
         isinstance(expression, exp.Comment)
         and (cexp := expression.args.get("expression"))
         and isinstance(cexp, exp.Literal)
+        and (table := expression.find(exp.Table))
+    ):
+        new = SUCCESS_NOP.copy()
+        new.args["table_comment"] = (table, cexp.this)
+        return new
+    elif (
+        isinstance(expression, exp.AlterTable)
+        and (sexp := expression.find(exp.Set))
+        and not sexp.args["tag"]
+        and (eq := sexp.find(exp.EQ))
+        and (id := eq.find(exp.Identifier))
+        and isinstance(id.this, str)
+        and id.this.upper() == "COMMENT"
+        and (lit := eq.find(exp.Literal))
+        and (table := expression.find(exp.Table))
     ):
+        new = SUCCESS_NOP.copy()
+        new.args["table_comment"] = (table, lit.this)
+        return new
+
+    return expression
+
+
+def extract_text_length(expression: exp.Expression) -> exp.Expression:
+    """Extract length of text columns.
+
+    duckdb doesn't have fixed-sized text types. So we capture the size of text types and store that in the
+    character_maximum_length arg.
+
+    Args:
+        expression (exp.Expression): the expression that will be transformed.
+
+    Returns:
+        exp.Expression: The original expression, with any comment stored in the new 'table_comment' arg.
+    """
+
+    if isinstance(expression, (exp.Create, exp.AlterTable)):
+        text_lengths = []
+        for dt in expression.find_all(exp.DataType):
+            if dt.this in (exp.DataType.Type.VARCHAR, exp.DataType.Type.TEXT):
+                col_name = dt.parent and dt.parent.this and dt.parent.this.this
+                if dt_size := dt.find(exp.DataTypeSize):
+                    size = (
+                        isinstance(dt_size.this, exp.Literal)
+                        and isinstance(dt_size.this.this, str)
+                        and int(dt_size.this.this)
+                    )
+                else:
+                    size = 16777216
+                text_lengths.append((col_name, size))
+
+        if text_lengths:
+            expression.args["text_lengths"] = text_lengths
+
+    return expression
+
+
+def float_to_double(expression: exp.Expression) -> exp.Expression:
+    """Convert float to double for 64 bit precision.
+
+    Snowflake floats are all 64 bit (ie: double)
+    see https://docs.snowflake.com/en/sql-reference/data-types-numeric#float-float4-float8
+    """
+
+    if isinstance(expression, exp.DataType) and expression.this == exp.DataType.Type.FLOAT:
+        # TODO don't copy!
         new = expression.copy()
-        new.args["table_comment"] = cexp.this
+        new.args["this"] = exp.DataType.Type.DOUBLE
         return new
 
     return expression
 
 
 def indices_to_array(expression: exp.Expression) -> exp.Expression:
     """Convert to 1-based list indices.
@@ -189,33 +249,37 @@
     ):
         # use sql() to handle quoting
         ident_sql = ident.sql()
         return sqlglot.parse_one(f"{ident_sql} -> '$.{index.this}'", read="duckdb")
     return expression
 
 
-def join_information_schema_ext(expression: exp.Expression) -> exp.Expression:
-    """Join to information_schema_ext to access additional metadata columns (eg: comment).
-
-    Example:
-        >>> import sqlglot
-        >>> sqlglot.parse_one("SELECT * FROM INFORMATION_SCHEMA.TABLES").transform(join_information_schema_ext).sql()
-        'SELECT * FROM INFORMATION_SCHEMA.TABLES
-         LEFT JOIN information_schema.tables_ext ON tables.table_catalog = tables_ext.ext_table_catalog AND
-         tables.table_schema = tables_ext.ext_table_schema AND tables.table_name = tables_ext.ext_table_name'
-    Args:
-        expression (exp.Expression): the expression that will be transformed.
+def information_schema_columns_snowflake(expression: exp.Expression) -> exp.Expression:
+    """Redirect to the information_schema.columns_snowflake view which has metadata that matches snowflake.
 
-    Returns:
-        exp.Expression: The transformed expression.
+    Because duckdb doesn't store character_maximum_length or character_octet_length.
     """
 
     if (
         isinstance(expression, exp.Select)
         and (tbl_exp := expression.find(exp.Table))
+        and tbl_exp.name.upper() == "COLUMNS"
+        and tbl_exp.db.upper() == "INFORMATION_SCHEMA"
+    ):
+        tbl_exp.set("this", exp.Identifier(this="COLUMNS_SNOWFLAKE", quoted=False))
+
+    return expression
+
+
+def information_schema_tables_ext(expression: exp.Expression) -> exp.Expression:
+    """Join to information_schema.tables_ext to access additional metadata columns (eg: comment)."""
+
+    if (
+        isinstance(expression, exp.Select)
+        and (tbl_exp := expression.find(exp.Table))
         and tbl_exp.name.upper() == "TABLES"
         and tbl_exp.db.upper() == "INFORMATION_SCHEMA"
     ):
         return expression.join(
             "information_schema.tables_ext",
             on=(
                 """
@@ -226,14 +290,41 @@
             ),
             join_type="left",
         )
 
     return expression
 
 
+def integer_precision(expression: exp.Expression) -> exp.Expression:
+    """Snowflake integers are 38 digits.
+
+    See https://docs.snowflake.com/en/sql-reference/data-types-numeric
+    """
+
+    decimal_38_0 = exp.DataType(
+        this=exp.DataType.Type.DECIMAL,
+        expressions=[
+            exp.DataTypeSize(this=exp.Literal(this="38", is_string=False)),
+            exp.DataTypeSize(this=exp.Literal(this="0", is_string=False)),
+        ],
+        nested=False,
+        prefix=False,
+    )
+
+    if (
+        isinstance(expression, exp.DataType)
+        and (expression.this == exp.DataType.Type.DECIMAL and not expression.expressions)
+        or expression.this
+        in (exp.DataType.Type.BIGINT, exp.DataType.Type.INT, exp.DataType.Type.SMALLINT, exp.DataType.Type.TINYINT)
+    ):
+        return decimal_38_0
+
+    return expression
+
+
 def object_construct(expression: exp.Expression) -> exp.Expression:
     """Convert object_construct to return a json string
 
     Because internally snowflake stores OBJECT types as a json string.
 
     Example:
         >>> import sqlglot
@@ -313,15 +404,15 @@
         if len(new_args) == 2:
             # if no replacement string, the snowflake default is ''
             new_args.append(exp.Literal(this="", is_string=True))
 
         # snowflake regex replacements are global
         new_args.append(exp.Literal(this="g", is_string=True))
 
-        new.args["expressions"] = new_args
+        new.set("expressions", new_args)
 
         return new
 
     return expression
 
 
 # TODO: move this into a Dialect as a transpilation
@@ -372,39 +463,39 @@
 
     return expression
 
 
 def tag(expression: exp.Expression) -> exp.Expression:
     """Handle tags. Transfer tags into upserts of the tag table.
 
-    duckdb doesn't support tags. In lieu of a full implementation, for now we make it the SUCCESS_NO_OP.
+    duckdb doesn't support tags. In lieu of a full implementation, for now we make it a NOP.
 
     Example:
         >>> import sqlglot
         >>> sqlglot.parse_one("ALTER TABLE table1 SET TAG foo='bar'").transform(tag).sql()
         "SELECT 'Statement executed successfully.'"
     Args:
         expression (exp.Expression): the expression that will be transformed.
 
     Returns:
         exp.Expression: The transformed expression.
     """
 
     if isinstance(expression, exp.AlterTable) and (actions := expression.args.get("actions")):
         for a in actions:
-            if isinstance(a, exp.SetTag):
-                return SUCCESS_NO_OP
+            if isinstance(a, exp.Set) and a.args["tag"]:
+                return SUCCESS_NOP
     elif (
         isinstance(expression, exp.Command)
         and (cexp := expression.args.get("expression"))
         and isinstance(cexp, str)
         and "SET TAG" in cexp.upper()
     ):
         # alter table modify column set tag
-        return SUCCESS_NO_OP
+        return SUCCESS_NOP
 
     return expression
 
 
 def to_date(expression: exp.Expression) -> exp.Expression:
     """Convert to_date() to a cast.
 
@@ -431,14 +522,33 @@
             # and avoid https://github.com/duckdb/duckdb/issues/7672
             this=exp.DateTrunc(unit=exp.Literal(this="day", is_string=True), this=expression.expressions[0]),
             to=exp.DataType(this=exp.DataType.Type.DATE, nested=False, prefix=False),
         )
     return expression
 
 
+def timestamp_ntz_ns(expression: exp.Expression) -> exp.Expression:
+    """Convert timestamp_ntz(9) to timestamp_ntz.
+
+    To compensate for https://github.com/duckdb/duckdb/issues/7980
+    """
+
+    if (
+        isinstance(expression, exp.DataType)
+        and expression.this == exp.DataType.Type.TIMESTAMP
+        and exp.DataTypeSize(this=exp.Literal(this="9", is_string=False)) in expression.expressions
+    ):
+        new = expression.copy()
+        del new.args["expressions"]
+        return new
+
+    return expression
+
+
+# sqlglot.parse_one("create table example(date TIMESTAMP_NTZ(9));", read="snowflake")
 def semi_structured_types(expression: exp.Expression) -> exp.Expression:
     """Convert OBJECT, ARRAY, and VARIANT types to duckdb compatible types.
 
     Example:
         >>> import sqlglot
         >>> sqlglot.parse_one("CREATE TABLE table1 (name object)").transform(semi_structured_types).sql()
         "CREATE TABLE table1 (name JSON)"
@@ -452,15 +562,15 @@
     if isinstance(expression, exp.DataType):
         if expression.this in [exp.DataType.Type.OBJECT, exp.DataType.Type.VARIANT]:
             new = expression.copy()
             new.args["this"] = exp.DataType.Type.JSON
             return new
         elif expression.this == exp.DataType.Type.ARRAY:
             new = expression.copy()
-            new.args["expressions"] = [exp.DataType(this=exp.DataType.Type.JSON)]
+            new.set("expressions", [exp.DataType(this=exp.DataType.Type.JSON)])
             return new
 
     return expression
 
 
 def upper_case_unquoted_identifiers(expression: exp.Expression) -> exp.Expression:
     """Upper case unquoted identifiers.
@@ -477,15 +587,15 @@
 
     Returns:
         exp.Expression: The transformed expression.
     """
 
     if isinstance(expression, exp.Identifier) and not expression.quoted and isinstance(expression.this, str):
         new = expression.copy()
-        new.args["this"] = expression.this.upper()
+        new.set("this", expression.this.upper())
         return new
 
     return expression
 
 
 def values_columns(expression: exp.Expression) -> exp.Expression:
     """Support column1, column2 expressions in VALUES.
@@ -509,11 +619,11 @@
         and not expression.alias
         and expression.find_ancestor(exp.Select)
         and (values := expression.find(exp.Tuple))
     ):
         new = expression.copy()
         num_columns = len(values.expressions)
         columns = [exp.Identifier(this=f"column{i + 1}", quoted=True) for i in range(num_columns)]
-        new.args["alias"] = exp.TableAlias(this=exp.Identifier(this="_", quoted=False), columns=columns)
+        new.set("alias", exp.TableAlias(this=exp.Identifier(this="_", quoted=False), columns=columns))
         return new
 
     return expression
```

### Comparing `fakesnow-0.2.0/fakesnow.egg-info/PKG-INFO` & `fakesnow-0.3.0/fakesnow.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fakesnow
-Version: 0.2.0
+Version: 0.3.0
 Summary: Fake Snowflake Connector for Python. Run Snowflake DB locally.
 License: MIT License
         
         Copyright (c) 2023 Oliver Mannion
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
@@ -30,14 +30,18 @@
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: notebook
 License-File: LICENSE
 
 # fakesnow ❄️
 
+[![ci](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/ci.yml)
+[![release](https://github.com/tekumara/fakesnow/actions/workflows/release.yml/badge.svg)](https://github.com/tekumara/fakesnow/actions/workflows/release.yml)
+[![PyPI](https://img.shields.io/pypi/v/fakesnow?color=violet)](https://pypi.org/project/fakesnow/)
+
 Fake [Snowflake Connector for Python](https://docs.snowflake.com/en/user-guide/python-connector). Run and mock Snowflake DB locally.
 
 ## Install
 
 ```
 pip install fakesnow
 ```
```

### Comparing `fakesnow-0.2.0/pyproject.toml` & `fakesnow-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [project]
 name = "fakesnow"
 description = "Fake Snowflake Connector for Python. Run Snowflake DB locally."
-version = "0.2.0"
+version = "0.3.0"
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = ["License :: OSI Approved :: MIT License"]
 keywords = ["snowflake", "snowflakedb", "fake", "local", "mock", "testing"]
 requires-python = ">=3.9"
 dependencies = [
     "duckdb~=0.8.0",
     "pyarrow",
     "snowflake-connector-python",
-    "sqlglot~=16.4.2",
+    "sqlglot~=16.8.1",
 ]
 
 [project.urls]
 homepage = "https://github.com/tekumara/fakesnow"
 
 [project.optional-dependencies]
 dev = [
```

### Comparing `fakesnow-0.2.0/tests/test_checks.py` & `fakesnow-0.3.0/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.2.0/tests/test_expr.py` & `fakesnow-0.3.0/tests/test_expr.py`

 * *Files identical despite different names*

### Comparing `fakesnow-0.2.0/tests/test_fakes.py` & `fakesnow-0.3.0/tests/test_fakes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 import datetime
 import json
 
 import pandas as pd
 import pytest
+import pytz
 import snowflake.connector
 import snowflake.connector.cursor
 import snowflake.connector.pandas_tools
 from pandas.testing import assert_frame_equal
 
 
+def test_alter_table(cur: snowflake.connector.cursor.SnowflakeCursor):
+    cur.execute("create table table1 (id int)")
+    cur.execute("alter table table1 add column name varchar(20)")
+    cur.execute("select name from table1")
+
+
 def test_binding_default_paramstyle(conn: snowflake.connector.SnowflakeConnection):
     assert conn._paramstyle == "pyformat"  # noqa: SLF001
     with conn.cursor() as cur:
         cur.execute("create table customers (ID int, FIRST_NAME varchar, ACTIVE boolean)")
         cur.execute("insert into customers values (%s, %s, %s)", (1, "Jenny", True))
         cur.execute("select * from customers")
         assert cur.fetchall() == [(1, "Jenny", True)]
@@ -316,20 +323,16 @@
 def test_fetchone_dict_cursor(conn: snowflake.connector.SnowflakeConnection):
     with conn.cursor(snowflake.connector.cursor.DictCursor) as cur:
         cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
         cur.execute("insert into customers values (1, 'Jenny', 'P')")
         cur.execute("insert into customers values (2, 'Jasper', 'M')")
         cur.execute("select id, first_name, last_name from customers")
 
-        assert cur.fetchone() == [
-            {"ID": 1, "FIRST_NAME": "Jenny", "LAST_NAME": "P"},
-        ]
-        assert cur.fetchone() == [
-            {"ID": 2, "FIRST_NAME": "Jasper", "LAST_NAME": "M"},
-        ]
+        assert cur.fetchone() == {"ID": 1, "FIRST_NAME": "Jenny", "LAST_NAME": "P"}
+        assert cur.fetchone() == {"ID": 2, "FIRST_NAME": "Jasper", "LAST_NAME": "M"}
         assert not cur.fetchone()
 
 
 def test_fetch_pandas_all(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
     cur.execute("insert into customers values (1, 'Jenny', 'P')")
     cur.execute("insert into customers values (2, 'Jasper', 'M')")
@@ -340,14 +343,22 @@
             {"ID": 1, "FIRST_NAME": "Jenny", "LAST_NAME": "P"},
             {"ID": 2, "FIRST_NAME": "Jasper", "LAST_NAME": "M"},
         ]
     )
     assert_frame_equal(cur.fetch_pandas_all(), expected_df, check_dtype=False)
 
 
+def test_floats_are_64bit(cur: snowflake.connector.cursor.SnowflakeCursor):
+    cur.execute("create or replace table example (f float, f4 float4, f8 float8, d double, r real)")
+    cur.execute("insert into example values (1.23, 1.23, 1.23, 1.23, 1.23)")
+    cur.execute("select * from example")
+    # 32 bit floats will return 1.2300000190734863 rather than 1.23
+    assert cur.fetchall() == [(1.23, 1.23, 1.23, 1.23, 1.23)]
+
+
 def test_get_result_batches(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("create table customers (ID int, FIRST_NAME varchar, LAST_NAME varchar)")
     cur.execute("insert into customers values (1, 'Jenny', 'P')")
     cur.execute("insert into customers values (2, 'Jasper', 'M')")
     cur.execute("select id, first_name, last_name from customers")
     batches = cur.get_result_batches()
     assert batches
@@ -370,14 +381,70 @@
         assert rows == [
             {"ID": 1, "FIRST_NAME": "Jenny", "LAST_NAME": "P"},
             {"ID": 2, "FIRST_NAME": "Jasper", "LAST_NAME": "M"},
         ]
         assert sum(batch.rowcount for batch in batches) == 2
 
 
+def test_information_schema_columns_numeric(cur: snowflake.connector.cursor.SnowflakeCursor):
+    # see https://docs.snowflake.com/en/sql-reference/data-types-numeric
+    cur.execute(
+        """
+        create table example (
+            XNUMBER20 NUMBER(2,0), XNUMBER NUMBER, XDECIMAL DECIMAL, XNUMERIC NUMERIC,
+            XINT INT, XINTEGER INTEGER, XBIGINT BIGINT, XSMALLINT SMALLINT, XTINYINT TINYINT, XBYTEINT BYTEINT
+        )
+        """
+    )
+
+    cur.execute(
+        """
+        select column_name,numeric_precision,numeric_precision_radix,numeric_scale
+        from information_schema.columns where table_name = 'EXAMPLE' order by ordinal_position
+        """
+    )
+
+    assert cur.fetchall() == [
+        ("XNUMBER20", 2, 10, 0),
+        ("XNUMBER", 38, 10, 0),
+        ("XDECIMAL", 38, 10, 0),
+        ("XNUMERIC", 38, 10, 0),
+        ("XINT", 38, 10, 0),
+        ("XINTEGER", 38, 10, 0),
+        ("XBIGINT", 38, 10, 0),
+        ("XSMALLINT", 38, 10, 0),
+        ("XTINYINT", 38, 10, 0),
+        ("XBYTEINT", 38, 10, 0),
+    ]
+
+
+def test_information_schema_columns_text(cur: snowflake.connector.cursor.SnowflakeCursor):
+    # see https://docs.snowflake.com/en/sql-reference/data-types-text
+    cur.execute(
+        """
+        create table example (
+            XVARCHAR20 VARCHAR(20), XVARCHAR VARCHAR, XTEXT TEXT
+        )
+        """
+    )
+
+    cur.execute(
+        """
+        select column_name,character_maximum_length,character_octet_length
+        from information_schema.columns where table_name = 'EXAMPLE' order by ordinal_position
+        """
+    )
+
+    assert cur.fetchall() == [
+        ("XVARCHAR20", 20, 80),
+        ("XVARCHAR", 16777216, 16777216),
+        ("XTEXT", 16777216, 16777216),
+    ]
+
+
 def test_non_existent_table_throws_snowflake_exception(cur: snowflake.connector.cursor.SnowflakeCursor):
     with pytest.raises(snowflake.connector.errors.ProgrammingError) as _:
         cur.execute("select * from this_table_does_not_exist")
 
 
 def test_object_construct(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("SELECT OBJECT_CONSTRUCT('a',1,'b','BBBB', 'c',null)")
@@ -440,14 +507,16 @@
 
     cur.execute("CREATE TABLE ingredients (id int) COMMENT = 'cheese'")
     assert read_comment() == "cheese"
     cur.execute("COMMENT ON TABLE ingredients IS 'pepperoni'")
     assert read_comment() == "pepperoni"
     cur.execute("COMMENT IF EXISTS ON TABLE schema1.ingredients IS 'mushrooms'")
     assert read_comment() == "mushrooms"
+    cur.execute("ALTER TABLE ingredients SET comment = 'pineapple'")
+    assert read_comment() == "pineapple"
 
 
 def test_tags_noop(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("CREATE TABLE table1 (id int)")
     cur.execute("ALTER TABLE table1 SET TAG foo='bar'")
     cur.execute("ALTER TABLE table1 MODIFY COLUMN name1 SET TAG foo='bar'")
 
@@ -458,14 +527,29 @@
 
 
 def test_timestamp_to_date(cur: snowflake.connector.cursor.SnowflakeCursor):
     cur.execute("SELECT to_date(to_timestamp(0)), to_date(cast(to_timestamp(0) as timestamp(9)))")
     assert cur.fetchall() == [(datetime.date(1970, 1, 1), datetime.date(1970, 1, 1))]
 
 
+def test_write_pandas_timestamp_ntz(conn: snowflake.connector.SnowflakeConnection):
+    # compensate for https://github.com/duckdb/duckdb/issues/7980
+    with conn.cursor() as cur:
+        cur.execute("create table example (UPDATE_AT_NTZ timestamp_ntz(9))")
+        # cur.execute("create table example (UPDATE_AT_NTZ timestamp)")
+
+        now_utc = datetime.datetime.now(pytz.utc)
+        df = pd.DataFrame([(now_utc,)], columns=["UPDATE_AT_NTZ"])
+        snowflake.connector.pandas_tools.write_pandas(conn, df, "EXAMPLE")
+
+        cur.execute("select * from example")
+
+        assert cur.fetchall() == [(now_utc.replace(tzinfo=None),)]
+
+
 def test_transactions(conn: snowflake.connector.SnowflakeConnection):
     conn.execute_string(
         """CREATE TABLE table1 (i int);
             BEGIN TRANSACTION;
             INSERT INTO table1 (i) VALUES (1);"""
     )
     conn.rollback()
```

### Comparing `fakesnow-0.2.0/tests/test_patch.py` & `fakesnow-0.3.0/tests/test_patch.py`

 * *Files identical despite different names*

