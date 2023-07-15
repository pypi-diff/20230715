# Comparing `tmp/pylinsql-0.1.17.tar.gz` & `tmp/pylinsql-0.1.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylinsql-0.1.17.tar", last modified: Tue Apr 26 16:09:09 2022, max compression
+gzip compressed data, was "pylinsql-0.1.18.tar", last modified: Sat Jul 15 15:07:25 2023, max compression
```

## Comparing `pylinsql-0.1.17.tar` & `pylinsql-0.1.18.tar`

### file list

```diff
@@ -1,15 +1,41 @@
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2022-04-26 16:09:09.361810 pylinsql-0.1.17/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1085 2021-11-19 09:11:20.000000 pylinsql-0.1.17/LICENSE
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18993 2022-04-26 16:09:09.361322 pylinsql-0.1.17/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18440 2022-02-19 21:48:03.000000 pylinsql-0.1.17/README.md
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2022-04-26 16:09:09.357915 pylinsql-0.1.17/pylinsql/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2021-11-19 09:11:20.000000 pylinsql-0.1.17/pylinsql/__init__.py
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11536 2022-02-20 09:38:19.000000 pylinsql-0.1.17/pylinsql/async_database.py
-drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2022-04-26 16:09:09.360700 pylinsql-0.1.17/pylinsql.egg-info/
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18993 2022-04-26 16:09:08.000000 pylinsql-0.1.17/pylinsql.egg-info/PKG-INFO
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      233 2022-04-26 16:09:09.000000 pylinsql-0.1.17/pylinsql.egg-info/SOURCES.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2022-04-26 16:09:08.000000 pylinsql-0.1.17/pylinsql.egg-info/dependency_links.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       27 2022-04-26 16:09:09.000000 pylinsql-0.1.17/pylinsql.egg-info/requires.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)        9 2022-04-26 16:09:09.000000 pylinsql-0.1.17/pylinsql.egg-info/top_level.txt
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)       38 2022-04-26 16:09:09.361987 pylinsql-0.1.17/setup.cfg
--rw-r--r--   0 levente.hunyadi   (503) staff       (20)      970 2022-04-26 16:08:31.000000 pylinsql-0.1.17/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-15 15:07:25.087772 pylinsql-0.1.18/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1085 2021-11-19 09:11:20.000000 pylinsql-0.1.18/LICENSE
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19021 2023-07-15 15:07:25.087072 pylinsql-0.1.18/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    18440 2022-02-19 21:48:03.000000 pylinsql-0.1.18/README.md
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-15 15:07:25.066554 pylinsql-0.1.18/pylinsql/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2021-11-19 09:11:20.000000 pylinsql-0.1.18/pylinsql/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    11536 2022-02-20 09:38:19.000000 pylinsql-0.1.18/pylinsql/async_database.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-15 15:07:25.070587 pylinsql-0.1.18/pylinsql/connection/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-07-15 15:05:15.000000 pylinsql-0.1.18/pylinsql/connection/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4985 2022-02-19 21:46:26.000000 pylinsql-0.1.18/pylinsql/connection/async_database.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-15 15:07:25.077859 pylinsql-0.1.18/pylinsql/generator/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-07-15 15:05:20.000000 pylinsql-0.1.18/pylinsql/generator/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    25116 2022-10-03 08:23:26.000000 pylinsql-0.1.18/pylinsql/generator/code_generator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8775 2023-07-04 11:53:32.000000 pylinsql-0.1.18/pylinsql/generator/conversion.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1246 2023-02-05 14:02:41.000000 pylinsql-0.1.18/pylinsql/generator/database_traits.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4100 2023-02-04 10:22:38.000000 pylinsql-0.1.18/pylinsql/generator/dbml_generator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     4644 2022-05-16 18:50:02.000000 pylinsql-0.1.18/pylinsql/generator/inspection.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1201 2022-02-20 09:46:42.000000 pylinsql-0.1.18/pylinsql/generator/schema.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     7805 2023-02-05 14:48:40.000000 pylinsql-0.1.18/pylinsql/generator/sql_generator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      942 2022-02-19 20:54:28.000000 pylinsql-0.1.18/pylinsql/generator/timing.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-15 15:07:25.085237 pylinsql-0.1.18/pylinsql/query/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        0 2023-07-15 15:05:32.000000 pylinsql-0.1.18/pylinsql/query/__init__.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9674 2022-02-19 20:42:50.000000 pylinsql-0.1.18/pylinsql/query/ast.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     2034 2022-02-19 20:51:27.000000 pylinsql-0.1.18/pylinsql/query/base.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    29179 2022-02-20 20:15:20.000000 pylinsql-0.1.18/pylinsql/query/builder.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     5247 2022-02-19 20:49:55.000000 pylinsql-0.1.18/pylinsql/query/core.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    13624 2022-02-19 20:42:44.000000 pylinsql-0.1.18/pylinsql/query/decompiler.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     9969 2022-02-19 20:42:42.000000 pylinsql-0.1.18/pylinsql/query/evaluator.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    17842 2022-02-19 20:50:12.000000 pylinsql-0.1.18/pylinsql/query/node.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1387 2022-02-19 20:42:43.000000 pylinsql-0.1.18/pylinsql/query/plot.py
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     3084 2022-02-20 20:15:16.000000 pylinsql-0.1.18/pylinsql/query/query.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-15 15:07:25.069388 pylinsql-0.1.18/pylinsql.egg-info/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)    19021 2023-07-15 15:07:25.000000 pylinsql-0.1.18/pylinsql.egg-info/PKG-INFO
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)      883 2023-07-15 15:07:25.000000 pylinsql-0.1.18/pylinsql.egg-info/SOURCES.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        1 2023-07-15 15:07:25.000000 pylinsql-0.1.18/pylinsql.egg-info/dependency_links.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       27 2023-07-15 15:07:25.000000 pylinsql-0.1.18/pylinsql.egg-info/requires.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)        9 2023-07-15 15:07:25.000000 pylinsql-0.1.18/pylinsql.egg-info/top_level.txt
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)       38 2023-07-15 15:07:25.087964 pylinsql-0.1.18/setup.cfg
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     1016 2023-07-15 15:01:42.000000 pylinsql-0.1.18/setup.py
+drwxr-xr-x   0 levente.hunyadi   (503) staff       (20)        0 2023-07-15 15:07:25.086032 pylinsql-0.1.18/tests/
+-rw-r--r--   0 levente.hunyadi   (503) staff       (20)     8456 2022-02-19 20:42:54.000000 pylinsql-0.1.18/tests/test_async_database.py
```

### Comparing `pylinsql-0.1.17/LICENSE` & `pylinsql-0.1.18/LICENSE`

 * *Files identical despite different names*

### Comparing `pylinsql-0.1.17/PKG-INFO` & `pylinsql-0.1.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pylinsql
-Version: 0.1.17
+Version: 0.1.18
 Summary: Language-Integrated SQL Queries in Python
 Home-page: https://github.com/hunyadi/pylinsql
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 7 - Inactive
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Language-Integrated SQL Queries in Python
 
 *pylinsql* helps you write SQL queries in Python that integrate with the type checker and produce standard SQL query strings as an end result. The main idea is to take a Python generator expression such as
 ```python
@@ -379,8 +379,7 @@
 
     *pylinsql* checks if the expression is well-formed, e.g. whether you join objects along existing properties (e.g. `Person` has `given_name`).
 
 7. Emit an SQL statement.
 
     *pylinsql* maps Python function calls into SQL statement equivalents, e.g. `asc()` becomes `ORDER BY`, `inner_join()` maps to an `INNER JOIN` in a `FROM` clause, a condition on a `min()` becomes part of `HAVING`, `GROUP BY` is generated based on the result expressions in the original Python generator expression, etc.
     
-
```

### Comparing `pylinsql-0.1.17/README.md` & `pylinsql-0.1.18/README.md`

 * *Files identical despite different names*

### Comparing `pylinsql-0.1.17/pylinsql/async_database.py` & `pylinsql-0.1.18/pylinsql/async_database.py`

 * *Files identical despite different names*

### Comparing `pylinsql-0.1.17/pylinsql.egg-info/PKG-INFO` & `pylinsql-0.1.18/pylinsql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pylinsql
-Version: 0.1.17
+Version: 0.1.18
 Summary: Language-Integrated SQL Queries in Python
 Home-page: https://github.com/hunyadi/pylinsql
 Author: Levente Hunyadi
 Author-email: hunyadi@gmail.com
 License: MIT
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Development Status :: 7 - Inactive
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Language-Integrated SQL Queries in Python
 
 *pylinsql* helps you write SQL queries in Python that integrate with the type checker and produce standard SQL query strings as an end result. The main idea is to take a Python generator expression such as
 ```python
@@ -379,8 +379,7 @@
 
     *pylinsql* checks if the expression is well-formed, e.g. whether you join objects along existing properties (e.g. `Person` has `given_name`).
 
 7. Emit an SQL statement.
 
     *pylinsql* maps Python function calls into SQL statement equivalents, e.g. `asc()` becomes `ORDER BY`, `inner_join()` maps to an `INNER JOIN` in a `FROM` clause, a condition on a `min()` becomes part of `HAVING`, `GROUP BY` is generated based on the result expressions in the original Python generator expression, etc.
     
-
```

### Comparing `pylinsql-0.1.17/setup.py` & `pylinsql-0.1.18/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,27 @@
 
 # the text of the README file
 with open(os.path.join(ROOT, "README.md"), "r") as f:
     README = f.read()
 
 setup(
     name="pylinsql",
-    version="0.1.17",
+    version="0.1.18",
     description="Language-Integrated SQL Queries in Python",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/hunyadi/pylinsql",
     author="Levente Hunyadi",
     author_email="hunyadi@gmail.com",
     license="MIT",
     classifiers=[
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Development Status :: 7 - Inactive",
     ],
     packages=find_packages(exclude=("tests",)),
     include_package_data=True,
     install_requires=["asyncpg", "json_strong_typing"],
 )
```

