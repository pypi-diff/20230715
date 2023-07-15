# Comparing `tmp/pysucculent-0.0.0.tar.gz` & `tmp/pysucculent-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysucculent-0.0.0.tar", last modified: Fri Jul 14 16:24:13 2023, max compression
+gzip compressed data, was "pysucculent-1.0.0.tar", last modified: Sat Jul 15 01:21:38 2023, max compression
```

## Comparing `pysucculent-0.0.0.tar` & `pysucculent-1.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-07-14 16:24:13.478526 pysucculent-0.0.0/
--rw-rw-rw-   0        0        0        0 2023-07-14 12:44:03.000000 pysucculent-0.0.0/LICENSE
--rw-rw-rw-   0        0        0      492 2023-07-14 16:24:13.477525 pysucculent-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-07-14 12:44:32.000000 pysucculent-0.0.0/README.md
--rw-rw-rw-   0        0        0       86 2023-07-14 12:47:41.000000 pysucculent-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-14 16:24:13.478526 pysucculent-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      822 2023-07-14 16:23:24.000000 pysucculent-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-14 16:24:13.458536 pysucculent-0.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-07-14 16:24:13.470529 pysucculent-0.0.0/src/pysucculent/
--rw-rw-rw-   0        0        0     7631 2023-07-14 16:03:12.000000 pysucculent-0.0.0/src/pysucculent/MysqlDB.py
--rw-rw-rw-   0        0        0       33 2023-07-14 16:06:41.000000 pysucculent-0.0.0/src/pysucculent/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-14 16:24:13.476527 pysucculent-0.0.0/src/pysucculent.egg-info/
--rw-rw-rw-   0        0        0      492 2023-07-14 16:24:13.000000 pysucculent-0.0.0/src/pysucculent.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-07-14 16:24:13.000000 pysucculent-0.0.0/src/pysucculent.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-14 16:24:13.000000 pysucculent-0.0.0/src/pysucculent.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-07-14 16:24:13.000000 pysucculent-0.0.0/src/pysucculent.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 01:21:38.216404 pysucculent-1.0.0/
+-rw-rw-rw-   0        0        0        0 2023-07-14 12:44:03.000000 pysucculent-1.0.0/LICENSE
+-rw-rw-rw-   0        0        0      492 2023-07-15 01:21:38.216404 pysucculent-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-07-14 12:44:32.000000 pysucculent-1.0.0/README.md
+-rw-rw-rw-   0        0        0       86 2023-07-14 12:47:41.000000 pysucculent-1.0.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 01:21:38.217402 pysucculent-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      822 2023-07-15 01:20:20.000000 pysucculent-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:21:38.200550 pysucculent-1.0.0/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 01:21:38.210408 pysucculent-1.0.0/src/pysucculent/
+-rw-rw-rw-   0        0        0     7613 2023-07-14 16:28:41.000000 pysucculent-1.0.0/src/pysucculent/MysqlDB.py
+-rw-rw-rw-   0        0        0       33 2023-07-14 16:06:41.000000 pysucculent-1.0.0/src/pysucculent/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 01:21:38.215403 pysucculent-1.0.0/src/pysucculent.egg-info/
+-rw-rw-rw-   0        0        0      492 2023-07-15 01:21:38.000000 pysucculent-1.0.0/src/pysucculent.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-07-15 01:21:38.000000 pysucculent-1.0.0/src/pysucculent.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 01:21:38.000000 pysucculent-1.0.0/src/pysucculent.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-07-15 01:21:38.000000 pysucculent-1.0.0/src/pysucculent.egg-info/top_level.txt
```

### Comparing `pysucculent-0.0.0/setup.py` & `pysucculent-1.0.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from time import time
 import setuptools
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="pysucculent",
-    version="0.0.0",
+    version="1.0.0",
     author="duer",
     author_email="1186969412@qq.com",
     description="mysql crud exends",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pypa/sampleproject",
     project_urls={
```

### Comparing `pysucculent-0.0.0/src/pysucculent/MysqlDB.py` & `pysucculent-1.0.0/src/pysucculent/MysqlDB.py`

 * *Files 0% similar despite different names*

```diff
@@ -224,10 +224,8 @@
     def exec(self, sql):
         try:
             self.cursor.execute(sql)
             self.conn.commit()
             return True
         except Exception as e:
             self.conn.rollback()
-        return False
-
-BDB = baseDB()
+        return False
```

