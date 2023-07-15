# Comparing `tmp/safrs-3.1.0.tar.gz` & `tmp/safrs-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/safrs-3.1.0.tar", last modified: Tue May 30 18:29:19 2023, max compression
+gzip compressed data, was "safrs-3.1.1.tar", last modified: Sat Jul 15 19:34:01 2023, max compression
```

## Comparing `safrs-3.1.0.tar` & `safrs-3.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 18:29:19.000000 safrs-3.1.0/
--rwxr-xr-x   0 root         (0) root         (0)     1687 2023-05-29 04:14:46.000000 safrs-3.1.0/setup.py
--rw-r--r--   0 root         (0) root         (0)      263 2023-05-30 18:29:19.000000 safrs-3.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs/
--rwxr-xr-x   0 root         (0) root         (0)     4082 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/api_methods.py
--rwxr-xr-x   0 root         (0) root         (0)     7458 2023-02-18 09:01:57.000000 safrs-3.1.0/safrs/safrs_types.py
--rwxr-xr-x   0 root         (0) root         (0)     3349 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/attr_parse.py
--rwxr-xr-x   0 root         (0) root         (0)     5843 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/safrs_init.py
--rwxr-xr-x   0 root         (0) root         (0)    49467 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/base.py
--rwxr-xr-x   0 root         (0) root         (0)    26470 2023-02-18 09:01:57.000000 safrs-3.1.0/safrs/swagger_doc.py
--rwxr-xr-x   0 root         (0) root         (0)     3782 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/errors.py
--rwxr-xr-x   0 root         (0) root         (0)     1401 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/jabase.py
--rwxr-xr-x   0 root         (0) root         (0)     1682 2023-02-14 18:51:37.000000 safrs-3.1.0/safrs/jsonapi_attr.py
--rwxr-xr-x   0 root         (0) root         (0)     5857 2023-02-18 09:01:57.000000 safrs-3.1.0/safrs/jsonapi_filters.py
--rwxr-xr-x   0 root         (0) root         (0)     4047 2023-02-14 18:51:37.000000 safrs-3.1.0/safrs/config.py
--rwxr-xr-x   0 root         (0) root         (0)     1205 2023-02-18 09:01:57.000000 safrs-3.1.0/safrs/util.py
--rwxr-xr-x   0 root         (0) root         (0)    41404 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/jsonapi.py
--rwxr-xr-x   0 root         (0) root         (0)    31418 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/safrs_api.py
--rwxr-xr-x   0 root         (0) root         (0)     1980 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/_safrs_relationship.py
--rwxr-xr-x   0 root         (0) root         (0)     4838 2023-05-30 18:27:13.000000 safrs-3.1.0/safrs/json_encoder.py
--rwxr-xr-x   0 root         (0) root         (0)     1248 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/__init__.py
--rwxr-xr-x   0 root         (0) root         (0)      262 2022-10-24 17:17:14.000000 safrs-3.1.0/safrs/response.py
--rwxr-xr-x   0 root         (0) root         (0)     9866 2023-02-18 09:01:57.000000 safrs-3.1.0/safrs/jsonapi_formatting.py
--rwxr-xr-x   0 root         (0) root         (0)       93 2023-05-29 04:14:46.000000 safrs-3.1.0/safrs/__about__.py
--rwxr-xr-x   0 root         (0) root         (0)     6264 2023-05-28 09:06:48.000000 safrs-3.1.0/safrs/request.py
--rwxr-xr-x   0 root         (0) root         (0)    35120 2023-02-11 18:54:12.000000 safrs-3.1.0/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      522 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      648 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)     2665 2023-05-30 18:29:19.000000 safrs-3.1.0/safrs.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1374 2022-10-24 17:17:13.000000 safrs-3.1.0/README.rst
--rwxr-xr-x   0 root         (0) root         (0)    16881 2023-02-18 09:01:57.000000 safrs-3.1.0/README.md
--rwxr-xr-x   0 root         (0) root         (0)     1422 2023-05-29 04:14:46.000000 safrs-3.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       90 2022-10-24 17:17:13.000000 safrs-3.1.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2665 2023-05-30 18:29:19.000000 safrs-3.1.0/PKG-INFO
--rwxr-xr-x   0 root         (0) root         (0)      433 2023-05-28 09:06:48.000000 safrs-3.1.0/requirements.txt
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2023-07-15 19:34:01.714677 safrs-3.1.1/
+-rwxrwxr-x   0 t         (1000) t         (1000)    35120 2023-05-28 08:17:45.000000 safrs-3.1.1/LICENSE
+-rw-rw-r--   0 t         (1000) t         (1000)       90 2023-05-28 08:17:45.000000 safrs-3.1.1/MANIFEST.in
+-rw-rw-r--   0 t         (1000) t         (1000)     2404 2023-07-15 19:34:01.714677 safrs-3.1.1/PKG-INFO
+-rwxrwxr-x   0 t         (1000) t         (1000)    16881 2023-05-28 08:17:45.000000 safrs-3.1.1/README.md
+-rw-rw-r--   0 t         (1000) t         (1000)     1374 2023-05-28 08:17:45.000000 safrs-3.1.1/README.rst
+-rwxrwxr-x   0 t         (1000) t         (1000)     1448 2023-07-15 19:33:51.000000 safrs-3.1.1/pyproject.toml
+-rwxrwxr-x   0 t         (1000) t         (1000)      433 2023-05-28 08:17:45.000000 safrs-3.1.1/requirements.txt
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2023-07-15 19:34:01.714677 safrs-3.1.1/safrs/
+-rwxrwxr-x   0 t         (1000) t         (1000)       93 2023-07-15 19:33:51.000000 safrs-3.1.1/safrs/__about__.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     1248 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/__init__.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     1980 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/_safrs_relationship.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     4082 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/api_methods.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     3349 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/attr_parse.py
+-rwxrwxr-x   0 t         (1000) t         (1000)    49483 2023-07-15 19:33:51.000000 safrs-3.1.1/safrs/base.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     4047 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/config.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     3782 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/errors.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     1401 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/jabase.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     4838 2023-07-15 19:33:51.000000 safrs-3.1.1/safrs/json_encoder.py
+-rwxrwxr-x   0 t         (1000) t         (1000)    41404 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/jsonapi.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     1682 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/jsonapi_attr.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     5873 2023-07-15 19:33:51.000000 safrs-3.1.1/safrs/jsonapi_filters.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     9866 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/jsonapi_formatting.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     6264 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/request.py
+-rwxrwxr-x   0 t         (1000) t         (1000)      262 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/response.py
+-rwxrwxr-x   0 t         (1000) t         (1000)    31481 2023-07-15 19:33:51.000000 safrs-3.1.1/safrs/safrs_api.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     5843 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/safrs_init.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     7458 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/safrs_types.py
+-rwxrwxr-x   0 t         (1000) t         (1000)    26470 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/swagger_doc.py
+-rwxrwxr-x   0 t         (1000) t         (1000)     1205 2023-05-28 08:17:45.000000 safrs-3.1.1/safrs/util.py
+drwxrwxr-x   0 t         (1000) t         (1000)        0 2023-07-15 19:34:01.714677 safrs-3.1.1/safrs.egg-info/
+-rw-rw-r--   0 t         (1000) t         (1000)     2404 2023-07-15 19:34:01.000000 safrs-3.1.1/safrs.egg-info/PKG-INFO
+-rw-rw-r--   0 t         (1000) t         (1000)      648 2023-07-15 19:34:01.000000 safrs-3.1.1/safrs.egg-info/SOURCES.txt
+-rw-rw-r--   0 t         (1000) t         (1000)        1 2023-07-15 19:34:01.000000 safrs-3.1.1/safrs.egg-info/dependency_links.txt
+-rw-rw-r--   0 t         (1000) t         (1000)      522 2023-07-15 19:34:01.000000 safrs-3.1.1/safrs.egg-info/requires.txt
+-rw-rw-r--   0 t         (1000) t         (1000)        6 2023-07-15 19:34:01.000000 safrs-3.1.1/safrs.egg-info/top_level.txt
+-rw-rw-r--   0 t         (1000) t         (1000)      263 2023-07-15 19:34:01.714677 safrs-3.1.1/setup.cfg
+-rwxrwxr-x   0 t         (1000) t         (1000)     1687 2023-07-15 19:33:51.000000 safrs-3.1.1/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `safrs-3.1.0/setup.py` & `safrs-3.1.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from setuptools import setup, find_packages
 
 
 def safrs_setup():
     with open("requirements.txt", "rt") as fp:
         install_requires = fp.read().strip().split("\n")
 
-    version = "3.1.0"
+    version = "3.1.1"
 
     setup(
         name="safrs",
         packages=find_packages(exclude=['test']),
         version=version,
         license="MIT",
         description="safrs : SqlAlchemy Flask-Restful Swagger2",
```

### Comparing `safrs-3.1.0/safrs/api_methods.py` & `safrs-3.1.1/safrs/api_methods.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/safrs_types.py` & `safrs-3.1.1/safrs/safrs_types.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/attr_parse.py` & `safrs-3.1.1/safrs/attr_parse.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/safrs_init.py` & `safrs-3.1.1/safrs/safrs_init.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/base.py` & `safrs-3.1.1/safrs/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -446,27 +446,27 @@
                     attr_name = "Type"
                 cls._col_attr_name_map[_col_name] = attr_name
                 cls._attr_col_name_map[attr_name] = _col_name
 
         return cls._col_attr_name_map[col_name]
 
     @hybrid_method
-    def _s_check_perm(self, property_name, permission="r"):
+    def _s_check_perm(self, property_name, permission="r") -> bool:
         """
         Check the (instance-level) column permission
         :param column_name: column name
         :param permission: permission string (read/write)
         :return: Boolean indicating whether access is allowed
         """
 
         return self.__class__._s_check_perm(property_name, permission)
 
     @_s_check_perm.expression
     @lru_cache(maxsize=256)
-    def _s_check_perm(cls, property_name, permission="r"):
+    def _s_check_perm(cls, property_name, permission="r") -> bool:
         """
         Check the (class-level) column permission
         :param column_name: column name
         :param permission: permission string (read/write)
         :return: Boolean indicating whether access is allowed
         """
         if property_name.startswith("_"):
```

### Comparing `safrs-3.1.0/safrs/swagger_doc.py` & `safrs-3.1.1/safrs/swagger_doc.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/errors.py` & `safrs-3.1.1/safrs/errors.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/jabase.py` & `safrs-3.1.1/safrs/jabase.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/jsonapi_attr.py` & `safrs-3.1.1/safrs/jsonapi_attr.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/jsonapi_filters.py` & `safrs-3.1.1/safrs/jsonapi_filters.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 JSON:API filtering strategies
 """
 from .config import get_request_param
 import sqlalchemy
 import safrs
 from .jsonapi_attr import is_jsonapi_attr
 from flask import request
-from sqlalchemy.orm import joinedload
+from sqlalchemy.orm import joinedload, Query
+
 
 
 def create_query(cls):
     """
     Create a query for the target collection `cls`.
     If `include=` query parameters are given, the corresponding relationships will be joined loaded if possible
     See: https://docs.sqlalchemy.org/en/13/orm/loading_relationships.html
@@ -41,15 +42,15 @@
         if options:
             query = query.options(options)
 
     return query
 
 
 @classmethod
-def jsonapi_filter(cls):
+def jsonapi_filter(cls) -> Query:
     """
     https://jsonapi.org/recommendations/#filtering
     Apply the request.args filters to the object
 
     :return: sqla query object
     """
 
@@ -95,15 +96,14 @@
         _expressions = []
         for column, val in expressions:
             if hasattr(column, "in_"):
                 _expressions.append(column.in_(val.split(",")))
             else:
                 safrs.log.warning(f"'{cls}.{column}' is not a column ({type(column)})")
         result_query = result_query.filter(*_expressions)
-
     return result_query
 
 
 @classmethod
 def get_swagger_filters(cls):
     """
     :return: JSON:API filters swagger spec
```

### Comparing `safrs-3.1.0/safrs/config.py` & `safrs-3.1.1/safrs/config.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/util.py` & `safrs-3.1.1/safrs/util.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/jsonapi.py` & `safrs-3.1.1/safrs/jsonapi.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/safrs_api.py` & `safrs-3.1.1/safrs/safrs_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     this method creates an API endpoint for the SAFRSBase object and corresponding swagger
     documentation
     """
 
     _operation_ids = {}
     _custom_swagger = {}
     _als_resources = []
+    external_host = None
 
     def __init__(
         self,
         app: Flask,
         host: str = "localhost",
         port: int = 5000,
         prefix: str = "",
@@ -86,14 +87,15 @@
             **kwargs,
         )
         app.json = SAFRSJSONProvider(app)
         app.json_encoder = SAFRSJSONEncoder  # deprecated, but used by the swaggerui blueprint
         self.init_app(app)
         self.representations = OrderedDict(DEFAULT_REPRESENTATIONS)
         self.update_spec()
+        SAFRSAPI.external_host = host
 
     def update_spec(self) -> None:
         """
         :param custom_swagger: swagger spec to be added to the swagger.json
         """
         _swagger_doc = self.get_swagger_doc()
         safrs.dict_merge(_swagger_doc, self._custom_swagger)
```

### Comparing `safrs-3.1.0/safrs/_safrs_relationship.py` & `safrs-3.1.1/safrs/_safrs_relationship.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/json_encoder.py` & `safrs-3.1.1/safrs/json_encoder.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/__init__.py` & `safrs-3.1.1/safrs/__init__.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/jsonapi_formatting.py` & `safrs-3.1.1/safrs/jsonapi_formatting.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs/request.py` & `safrs-3.1.1/safrs/request.py`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/LICENSE` & `safrs-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs.egg-info/requires.txt` & `safrs-3.1.1/safrs.egg-info/requires.txt`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
+Flask-Cors>=3.0.10
+Flask-RESTful>=0.3.9
+Flask-SQLAlchemy>=3.0.3
+Flask>=2.3.2
+Jinja2>=3.1.2
+MarkupSafe>=2.1.2
+PyYAML>=6.0
+SQLAlchemy>=2.0.3
+Werkzeug>=2.2.2
 aniso8601>=9.0.1
 build>=0.10.0
 click>=8.1.3
-Flask>=2.3.2
-Flask-Cors>=3.0.10
-Flask-RESTful>=0.3.9
 flask-restful-swagger-2>=0.35
-Flask-SQLAlchemy>=3.0.3
 flask-swagger-ui>=4.11.1
 greenlet>=2.0.2
 importlib-metadata>=6.0.0
 itsdangerous>=2.1.2
-Jinja2>=3.1.2
-MarkupSafe>=2.1.2
 packaging>=23.0
 pyproject-hooks>=1.0.0
 pytz>=2022.7.1
-PyYAML>=6.0
 six>=1.16.0
-SQLAlchemy>=2.0.3
 tomli>=2.0.1
 typing-extensions>=4.4.0
-Werkzeug>=2.2.2
 zipp>=3.13.0
 
 [admin]
 Flask-Admin>=1.5.8
 Flask-Cors>=3.0.9
 
 [db2api]
-inflect==5.0.2
 Flask-Cors>=3.0.9
+inflect==5.0.2
```

### Comparing `safrs-3.1.0/safrs.egg-info/SOURCES.txt` & `safrs-3.1.1/safrs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/safrs.egg-info/PKG-INFO` & `safrs-3.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,16 @@
 Metadata-Version: 2.1
 Name: safrs
-Version: 3.1.0
+Version: 3.1.1
 Summary: safrs : SqlAlchemy Flask-Restful Swagger2
 Home-page: https://github.com/thomaxxl/safrs
 Author: Thomas Pollet
 Author-email: thomas.pollet@gmail.com
 License: MIT
-Download-URL: https://github.com/thomaxxl/safrs/archive/3.1.0.tar.gz
-Description: SAFRS: Python OpenAPI & JSON:API Framework
-        ==========================================
-        
-        Please check the `GitHub Readme <https://github.com/thomaxxl/safrs>`__ for documentation.
-        
-        Overview
-        --------
-        
-        SAFRS is an acronym for **S**\ ql\ **A**\ lchemy **F**\ lask-\ **R**\ estful **S**\ wagger. The purpose of this framework is to help python developers create a self-documenting JSON API for sqlalchemy database objects and relationships. These objects can be serialized to JSON and can be created, retrieved, updated and deleted through the JSON API.
-        Optionally, custom resource object methods can be exposed and invoked using JSON.
-        Class and method descriptions and examples can be provided in yaml syntax in the code comments. The description is parsed and shown in the swagger web interface.
-        
-        The result is an easy-to-use `swagger/OpenAPI <https://swagger.io/>`_ and `JSON:API <jsonapi.org>`_ compliant API specification.
-        
-        Installation
-        ------------
-        
-        SAFRS can be installed as a `pip package <https://pypi.python.org/pypi/safrs/>`_ or by downloading the latest version from github, for example:
-        
-        .. code-block:: bash
-        
-           git clone https://github.com/thomaxxl/safrs
-           cd safrs
-           pip3 install -r requirements.txt --user
-           python3 setup.py install --user
-        
-        
-        The examples can then be started with
-        
-        .. code-block::
-        
-           python3 examples/demo_relationship.py "your-interface-ip"
-        
-        
-        
+Download-URL: https://github.com/thomaxxl/safrs/archive/3.1.1.tar.gz
 Keywords: SqlAlchemy,Flask,REST,Swagger,JsonAPI,OpenAPI
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Flask
 Classifier: Topic :: Software Development :: Libraries
@@ -54,7 +19,45 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6, !=3.0.*, !=3.1.*, !=3.2.*, <4
 Provides-Extra: admin
 Provides-Extra: db2api
+License-File: LICENSE
+
+SAFRS: Python OpenAPI & JSON:API Framework
+==========================================
+
+Please check the `GitHub Readme <https://github.com/thomaxxl/safrs>`__ for documentation.
+
+Overview
+--------
+
+SAFRS is an acronym for **S**\ ql\ **A**\ lchemy **F**\ lask-\ **R**\ estful **S**\ wagger. The purpose of this framework is to help python developers create a self-documenting JSON API for sqlalchemy database objects and relationships. These objects can be serialized to JSON and can be created, retrieved, updated and deleted through the JSON API.
+Optionally, custom resource object methods can be exposed and invoked using JSON.
+Class and method descriptions and examples can be provided in yaml syntax in the code comments. The description is parsed and shown in the swagger web interface.
+
+The result is an easy-to-use `swagger/OpenAPI <https://swagger.io/>`_ and `JSON:API <jsonapi.org>`_ compliant API specification.
+
+Installation
+------------
+
+SAFRS can be installed as a `pip package <https://pypi.python.org/pypi/safrs/>`_ or by downloading the latest version from github, for example:
+
+.. code-block:: bash
+
+   git clone https://github.com/thomaxxl/safrs
+   cd safrs
+   pip3 install -r requirements.txt --user
+   python3 setup.py install --user
+
+
+The examples can then be started with
+
+.. code-block::
+
+   python3 examples/demo_relationship.py "your-interface-ip"
+
+
+
+
```

### Comparing `safrs-3.1.0/README.rst` & `safrs-3.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/README.md` & `safrs-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `safrs-3.1.0/pyproject.toml` & `safrs-3.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "safrs"
 
-version = "3.1.0"
+version = "3.1.1"
 
 description="SAFRS : SqlAlchemy Flask-Restful Swagger"
 
 readme = "README.md"
 
 requires-python = ">=3.7"
 
@@ -33,15 +33,15 @@
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
 ]
 
-dependencies = [ "Flask-SQLAlchemy", "flask_swagger_ui", "flask-restful-swagger-2", "PyYaml" ]
+dependencies = [ "Flask-SQLAlchemy>=3.0.3", "flask_swagger_ui>=4.11.1", "flask-restful-swagger-2>=0.35", "PyYaml>=6.0" ]
 
 [project.optional-dependencies] # Optional
 dev = ["flask_cors"]
 test = ["flask_cors"]
 
 [project.urls]  # Optional
 "Homepage" = "https://github.com/thomaxxl/safrs"
```

### Comparing `safrs-3.1.0/PKG-INFO` & `safrs-3.1.1/safrs.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,51 +1,16 @@
 Metadata-Version: 2.1
 Name: safrs
-Version: 3.1.0
+Version: 3.1.1
 Summary: safrs : SqlAlchemy Flask-Restful Swagger2
 Home-page: https://github.com/thomaxxl/safrs
 Author: Thomas Pollet
 Author-email: thomas.pollet@gmail.com
 License: MIT
-Download-URL: https://github.com/thomaxxl/safrs/archive/3.1.0.tar.gz
-Description: SAFRS: Python OpenAPI & JSON:API Framework
-        ==========================================
-        
-        Please check the `GitHub Readme <https://github.com/thomaxxl/safrs>`__ for documentation.
-        
-        Overview
-        --------
-        
-        SAFRS is an acronym for **S**\ ql\ **A**\ lchemy **F**\ lask-\ **R**\ estful **S**\ wagger. The purpose of this framework is to help python developers create a self-documenting JSON API for sqlalchemy database objects and relationships. These objects can be serialized to JSON and can be created, retrieved, updated and deleted through the JSON API.
-        Optionally, custom resource object methods can be exposed and invoked using JSON.
-        Class and method descriptions and examples can be provided in yaml syntax in the code comments. The description is parsed and shown in the swagger web interface.
-        
-        The result is an easy-to-use `swagger/OpenAPI <https://swagger.io/>`_ and `JSON:API <jsonapi.org>`_ compliant API specification.
-        
-        Installation
-        ------------
-        
-        SAFRS can be installed as a `pip package <https://pypi.python.org/pypi/safrs/>`_ or by downloading the latest version from github, for example:
-        
-        .. code-block:: bash
-        
-           git clone https://github.com/thomaxxl/safrs
-           cd safrs
-           pip3 install -r requirements.txt --user
-           python3 setup.py install --user
-        
-        
-        The examples can then be started with
-        
-        .. code-block::
-        
-           python3 examples/demo_relationship.py "your-interface-ip"
-        
-        
-        
+Download-URL: https://github.com/thomaxxl/safrs/archive/3.1.1.tar.gz
 Keywords: SqlAlchemy,Flask,REST,Swagger,JsonAPI,OpenAPI
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Intended Audience :: Developers
 Classifier: Framework :: Flask
 Classifier: Topic :: Software Development :: Libraries
@@ -54,7 +19,45 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.6
 Requires-Python: >=3.6, !=3.0.*, !=3.1.*, !=3.2.*, <4
 Provides-Extra: admin
 Provides-Extra: db2api
+License-File: LICENSE
+
+SAFRS: Python OpenAPI & JSON:API Framework
+==========================================
+
+Please check the `GitHub Readme <https://github.com/thomaxxl/safrs>`__ for documentation.
+
+Overview
+--------
+
+SAFRS is an acronym for **S**\ ql\ **A**\ lchemy **F**\ lask-\ **R**\ estful **S**\ wagger. The purpose of this framework is to help python developers create a self-documenting JSON API for sqlalchemy database objects and relationships. These objects can be serialized to JSON and can be created, retrieved, updated and deleted through the JSON API.
+Optionally, custom resource object methods can be exposed and invoked using JSON.
+Class and method descriptions and examples can be provided in yaml syntax in the code comments. The description is parsed and shown in the swagger web interface.
+
+The result is an easy-to-use `swagger/OpenAPI <https://swagger.io/>`_ and `JSON:API <jsonapi.org>`_ compliant API specification.
+
+Installation
+------------
+
+SAFRS can be installed as a `pip package <https://pypi.python.org/pypi/safrs/>`_ or by downloading the latest version from github, for example:
+
+.. code-block:: bash
+
+   git clone https://github.com/thomaxxl/safrs
+   cd safrs
+   pip3 install -r requirements.txt --user
+   python3 setup.py install --user
+
+
+The examples can then be started with
+
+.. code-block::
+
+   python3 examples/demo_relationship.py "your-interface-ip"
+
+
+
+
```

