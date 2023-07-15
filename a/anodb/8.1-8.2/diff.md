# Comparing `tmp/anodb-8.1.tar.gz` & `tmp/anodb-8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anodb-8.1.tar", last modified: Fri Jun 16 06:22:42 2023, max compression
+gzip compressed data, was "anodb-8.2.tar", last modified: Sat Jul 15 09:54:09 2023, max compression
```

## Comparing `anodb-8.1.tar` & `anodb-8.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 06:22:42.046711 anodb-8.1/
--rw-------   0 fabien    (1001) fabien    (1001)       33 2023-05-14 12:33:50.000000 anodb-8.1/LICENSE
--rw-------   0 fabien    (1001) fabien    (1001)       49 2023-05-14 12:33:50.000000 anodb-8.1/MANIFEST.in
--rw-------   0 fabien    (1001) fabien    (1001)     1178 2023-06-16 05:51:21.000000 anodb-8.1/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)     4703 2023-06-16 06:22:42.046711 anodb-8.1/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)     3753 2023-06-15 13:10:50.000000 anodb-8.1/README.md
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 06:22:42.046711 anodb-8.1/anodb.egg-info/
--rw-------   0 fabien    (1001) fabien    (1001)     4703 2023-06-16 06:22:42.000000 anodb-8.1/anodb.egg-info/PKG-INFO
--rw-------   0 fabien    (1001) fabien    (1001)      239 2023-06-16 06:22:42.000000 anodb-8.1/anodb.egg-info/SOURCES.txt
--rw-------   0 fabien    (1001) fabien    (1001)        1 2023-06-16 06:22:42.000000 anodb-8.1/anodb.egg-info/dependency_links.txt
--rw-------   0 fabien    (1001) fabien    (1001)      213 2023-06-16 06:22:42.000000 anodb-8.1/anodb.egg-info/requires.txt
--rw-------   0 fabien    (1001) fabien    (1001)        6 2023-06-16 06:22:42.000000 anodb-8.1/anodb.egg-info/top_level.txt
--rwx------   0 fabien    (1001) fabien    (1001)     8820 2023-06-16 06:02:12.000000 anodb-8.1/anodb.py
--rw-------   0 fabien    (1001) fabien    (1001)     1269 2023-06-16 06:21:14.000000 anodb-8.1/pyproject.toml
--rw-------   0 fabien    (1001) fabien    (1001)       38 2023-06-16 06:22:42.046711 anodb-8.1/setup.cfg
-drwx------   0 fabien    (1001) fabien    (1001)        0 2023-06-16 06:22:42.046711 anodb-8.1/test/
--rw-------   0 fabien    (1001) fabien    (1001)      399 2023-06-15 09:59:54.000000 anodb-8.1/test/Makefile
--rw-------   0 fabien    (1001) fabien    (1001)     8943 2023-06-15 09:43:43.000000 anodb-8.1/test/test_anodb.py
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-15 09:54:09.350700 anodb-8.2/
+-rw-------   0 fabien    (1001) fabien    (1001)       33 2023-05-14 12:33:50.000000 anodb-8.2/LICENSE
+-rw-------   0 fabien    (1001) fabien    (1001)       49 2023-05-14 12:33:50.000000 anodb-8.2/MANIFEST.in
+-rw-------   0 fabien    (1001) fabien    (1001)     1187 2023-07-15 09:46:27.000000 anodb-8.2/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     5724 2023-07-15 09:54:09.350700 anodb-8.2/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)     4773 2023-07-15 09:52:46.000000 anodb-8.2/README.md
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-15 09:54:09.350700 anodb-8.2/anodb.egg-info/
+-rw-------   0 fabien    (1001) fabien    (1001)     5724 2023-07-15 09:54:09.000000 anodb-8.2/anodb.egg-info/PKG-INFO
+-rw-------   0 fabien    (1001) fabien    (1001)      239 2023-07-15 09:54:09.000000 anodb-8.2/anodb.egg-info/SOURCES.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        1 2023-07-15 09:54:09.000000 anodb-8.2/anodb.egg-info/dependency_links.txt
+-rw-------   0 fabien    (1001) fabien    (1001)      213 2023-07-15 09:54:09.000000 anodb-8.2/anodb.egg-info/requires.txt
+-rw-------   0 fabien    (1001) fabien    (1001)        6 2023-07-15 09:54:09.000000 anodb-8.2/anodb.egg-info/top_level.txt
+-rwx------   0 fabien    (1001) fabien    (1001)     8820 2023-06-16 06:02:12.000000 anodb-8.2/anodb.py
+-rw-------   0 fabien    (1001) fabien    (1001)     1270 2023-07-15 09:51:52.000000 anodb-8.2/pyproject.toml
+-rw-------   0 fabien    (1001) fabien    (1001)       38 2023-07-15 09:54:09.350700 anodb-8.2/setup.cfg
+drwx------   0 fabien    (1001) fabien    (1001)        0 2023-07-15 09:54:09.350700 anodb-8.2/test/
+-rw-------   0 fabien    (1001) fabien    (1001)      399 2023-06-15 09:59:54.000000 anodb-8.2/test/Makefile
+-rw-------   0 fabien    (1001) fabien    (1001)     8943 2023-06-15 09:43:43.000000 anodb-8.2/test/test_anodb.py
```

### Comparing `anodb-8.1/Makefile` & `anodb-8.2/Makefile`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 check.coverage: venv
 	source venv/bin/activate
 	$(MAKE) -C test coverage
 
 check.pymarkdown: venv
 	source venv/bin/activate
-	pymarkdown scan *.md
+	pymarkdown -d MD013 scan *.md
 
 .PHONY: clean clean.venv
 clean:
 	$(RM) -r __pycache__ */__pycache__ dist build .mypy_cache .pytest_cache
 	$(MAKE) -C test clean
 
 clean.venv: clean
```

### Comparing `anodb-8.1/PKG-INFO` & `anodb-8.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,7 @@
-Metadata-Version: 2.1
-Name: anodb
-Version: 8.1
-Summary: Convenient Wrapper around AioSQL and a Database Connection
-Author-email: Fabien Coelho <ano.db@coelho.net>
-License: CC0
-Project-URL: repository, https://github.com/zx80/anodb
-Project-URL: documentation, https://zx80.github.io/anodb/
-Project-URL: issues, https://github.com/zx80/anodb/issues
-Project-URL: package, https://pypi.org/project/anodb/
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: SQL
-Classifier: Topic :: Database :: Front-Ends
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-Provides-Extra: pub
-Provides-Extra: postgres
-Provides-Extra: mysql
-License-File: LICENSE
-
 # AnoDB
 
 Convenient Wrapper around [aiosql](https://github.com/nackjicholson/aiosql)
 and a [Database Connection](https://www.python.org/dev/peps/pep-0249).
 
 ![Status](https://github.com/zx80/anodb/actions/workflows/anodb-package.yml/badge.svg?branch=master&style=flat)
 ![Tests](https://img.shields.io/badge/tests-11%20✓-success)
@@ -85,45 +60,57 @@
 
 ## Documentation
 
 The `anodb` module provides the `DB` class which embeds both a
 [PEP 249](https://peps.python.org/pep-0249/) database connection
 (providing methods `commit`, `rollback`, `cursor`, `close` and
 its `connect` counterpart to re-connect) *and* SQL queries wrapped
-into dynamically generated functions by [aiosql](https://pypi.org/project/aiosql/).
+into dynamically generated functions by
+[aiosql](https://pypi.org/project/aiosql/).
 Such functions may be loaded from a string (`add_queries_from_str`) or a
 path (`add_queries_from_path`).
 
 The `DB` constructor parameters are:
 
-- `db` the name of the database driver: `sqlite3`, `psycopg`, `pymysql`,
-  see [aiosql documentation](https://nackjicholson.github.io/aiosql/database-driver-adapters.html)
+- `db` the name of the database driver: `sqlite3`, `psycopg`, `pymysql`, see
+  [aiosql documentation](https://nackjicholson.github.io/aiosql/database-driver-adapters.html)
   for a list of supported drivers.
-- `conn` an optional connection string used to initiate a connection with the driver.
+- `conn` an optional connection string used to initiate a connection with the
+  driver.
   For instance, `psycopg` accepts a
   [libpq connection string](https://www.postgresql.org/docs/current/libpq-connect.html#LIBPQ-CONNSTRING)
   such as: `"host=db1.my.org port=5432 dbname=acme user=calvin …"`.
-- `queries` a path name or list of path names from which to read query definitions.
+- `queries` a path name or list of path names from which to read query
+   definitions.
 - `options` a dictionary or string to pass additional connection parameters.
 - `auto_reconnect` whether to attempt a reconnection if the connection is lost.
   Default is `True`.
 - `debug` whether to generate debugging messages.
   Default is `False`.
 - other named parameters are passed as additional connection parameters.
 
 ```python
 import anodb
 
-db = anodb.DB("sqlite3", ":memory:", "acme-queries.sql")
+db = anodb.DB("sqlite3", "acme.db", "acme-queries.sql")
+db = anodb.DB("duckdb", "acme.db", "acme-queries.sql")
 db = anodb.DB("psycopg", "host=localhost dbname=acme", "acme-queries.sql")
+db = anodb.DB("psycopg", None, "acme-queries.sql", host="localhost", user="calvin", password="...", dbname="acme")
+db = anodb.DB("psycopg2", "host=localhost dbname=acme", "acme-queries.sql")
+db = anodb.DB("pygresql", None, "acme-queries.sql", host="localhost:5432", user="calvin", password="...", database="acme")
+db = anodb.DB("pg8000", None, "acme-queries.sql", host="localhost", port=5432, user="calvin", password="...", database="acme")
+db = anodb.DB("MySQLdb", None, "acme-queries.sql", host="localhost", port=3306, user="calvin", password="...", database="acme")
+db = anodb.DB("pymysql", None, "acme-queries.sql", host="localhost", port=3306, user="calvin", password="...", database="acme")
+db = anodb.DB("mysql-connector", None, "acme-queries.sql", host="localhost", port=3306, user="calvin", password="...", database="acme")
+db = anodb.DB("mariadb", None, "acme-queries.sql", host="localhost", port=3306, user="calvin", password="...", database="acme")
 ```
 
 ## Versions
 
 [Sources](https://github.com/zx80/anodb),
 [documentation](https://zx80.github.io/anodb/) and
 [issues](https://github.com/zx80/anodb/issues)
 are available on [GitHub](https://github.com/).
 
-Latest version is *7.3* on 2023-01-21.
+Latest version is *8.2* on 2023-07-15.
 
 See [all versions](VERSIONS.md)
```

### Comparing `anodb-8.1/anodb.py` & `anodb-8.2/anodb.py`

 * *Files identical despite different names*

### Comparing `anodb-8.1/pyproject.toml` & `anodb-8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "anodb"
-version = "8.1"
+version = "8.2"
 authors = [ { name = "Fabien Coelho", email = "ano.db@coelho.net" } ]
 description = "Convenient Wrapper around AioSQL and a Database Connection"
 readme = "README.md"
 license = { text = "CC0" }
-requires-python = ">= 3.8"
+requires-python = ">= 3.10"
 dependencies = [ "aiosql >= 8.0" ]
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Intended Audience :: Developers",
   "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
   "Programming Language :: Python",
   "Programming Language :: SQL",
```

### Comparing `anodb-8.1/test/test_anodb.py` & `anodb-8.2/test/test_anodb.py`

 * *Files identical despite different names*

