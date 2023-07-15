# Comparing `tmp/snap_saas_base-0.1.0.tar.gz` & `tmp/snap_saas_base-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snap_saas_base-0.1.0.tar", max compression
+gzip compressed data, was "snap_saas_base-0.4.0.tar", max compression
```

## Comparing `snap_saas_base-0.1.0.tar` & `snap_saas_base-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     4822 2023-07-08 21:33:39.819647 snap_saas_base-0.1.0/README.md
--rw-r--r--   0        0        0     4202 2023-07-08 21:33:39.823647 snap_saas_base-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       30 2023-07-08 21:33:39.823647 snap_saas_base-0.1.0/src/snap_saas_base/__init__.py
--rw-r--r--   0        0        0       30 2023-07-08 21:33:39.823647 snap_saas_base-0.1.0/src/snap_saas_base/models/__init__.py
--rw-r--r--   0        0        0     2153 2023-07-08 21:33:39.823647 snap_saas_base-0.1.0/src/snap_saas_base/models/base_model_postgres.py
--rw-r--r--   0        0        0     5277 2023-07-08 21:33:39.823647 snap_saas_base-0.1.0/src/snap_saas_base/models/organization.py
--rw-r--r--   0        0        0     3309 2023-07-08 21:33:39.827648 snap_saas_base-0.1.0/src/snap_saas_base/models/user.py
--rw-r--r--   0        0        0     6641 2023-07-08 21:33:39.827648 snap_saas_base-0.1.0/src/snap_saas_base/models/workspace.py
--rw-r--r--   0        0        0        0 2023-07-08 21:33:39.827648 snap_saas_base-0.1.0/src/snap_saas_base/py.typed
--rw-r--r--   0        0        0       38 2023-07-08 21:33:39.827648 snap_saas_base-0.1.0/src/snap_saas_base/schemas/__init__.py
--rw-r--r--   0        0        0     5426 1970-01-01 00:00:00.000000 snap_saas_base-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     4822 2023-07-15 17:02:42.007284 snap_saas_base-0.4.0/README.md
+-rw-r--r--   0        0        0     4202 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       30 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/models/__init__.py
+-rw-r--r--   0        0        0     2153 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/models/base_model.py
+-rw-r--r--   0        0        0     5268 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/models/organization.py
+-rw-r--r--   0        0        0     3300 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/models/user.py
+-rw-r--r--   0        0        0     6632 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/models/workspace.py
+-rw-r--r--   0        0        0        0 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/py.typed
+-rw-r--r--   0        0        0       38 2023-07-15 17:02:42.011284 snap_saas_base-0.4.0/src/snap_saas_base/schemas/__init__.py
+-rw-r--r--   0        0        0     5426 1970-01-01 00:00:00.000000 snap_saas_base-0.4.0/PKG-INFO
```

### Comparing `snap_saas_base-0.1.0/README.md` & `snap_saas_base-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.1.0/pyproject.toml` & `snap_saas_base-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]  # https://python-poetry.org/docs/pyproject/#poetry-and-pep-517
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]  # https://python-poetry.org/docs/pyproject/
 name = "snap-saas-base"
-version = "0.1.0"
+version = "0.4.0"
 description = "Snap Env (https://snapenv.com) Python base module."
 authors = ["Abner G Jacobsen <abner@apoana.com.br>"]
 readme = "README.md"
 repository = "https://github.com/orgs/snapenv/snap-saas-base"
 
 [tool.commitizen]  # https://commitizen-tools.github.io/commitizen/config/
 bump_message = "bump(release): v$current_version → v$new_version"
 tag_format = "v$version"
 update_changelog_on_bump = true
-version = "0.1.0"
+version = "0.4.0"
 version_files = ["pyproject.toml:version"]
 
 [tool.poetry.dependencies]  # https://python-poetry.org/docs/dependency-specification/
 python = ">=3.11,<4.0"
 sqlalchemy = {extras = ["asyncio"], version = "^2.0.18"}
 cuid = "^0.4"
 pydantic = ">=1.0.0,<2.0.0"
```

### Comparing `snap_saas_base-0.1.0/src/snap_saas_base/models/base_model_postgres.py` & `snap_saas_base-0.4.0/src/snap_saas_base/models/base_model.py`

 * *Files identical despite different names*

### Comparing `snap_saas_base-0.1.0/src/snap_saas_base/models/organization.py` & `snap_saas_base-0.4.0/src/snap_saas_base/models/organization.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import cuid
 import sqlalchemy as sa
 import sqlalchemy.orm as so
 
-from snap_saas_base.models.base_model_postgres import AbstractModel
+from snap_saas_base.models.base_model import AbstractModel
 
 # https://github.com/sqlalchemy/sqlalchemy/discussions/6165
 
 
 class Organization(AbstractModel):
     """A class used to represent an Organization in the database.
```

### Comparing `snap_saas_base-0.1.0/src/snap_saas_base/models/user.py` & `snap_saas_base-0.4.0/src/snap_saas_base/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import cuid
 import sqlalchemy as sa
 import sqlalchemy.orm as so
 
-from snap_saas_base.models.base_model_postgres import AbstractModel
+from snap_saas_base.models.base_model import AbstractModel
 
 # https://github.com/sqlalchemy/sqlalchemy/discussions/6165
 
 
 class User(AbstractModel):
     """
     A class used to represent a User in the system.
```

### Comparing `snap_saas_base-0.1.0/src/snap_saas_base/models/workspace.py` & `snap_saas_base-0.4.0/src/snap_saas_base/models/workspace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import cuid
 import sqlalchemy as sa
 import sqlalchemy.orm as so
 from sqlalchemy.dialects.postgresql import JSONB
 
-from snap_saas_base.models.base_model_postgres import AbstractModel
+from snap_saas_base.models.base_model import AbstractModel
 
 # https://github.com/sqlalchemy/sqlalchemy/discussions/6165
 
 
 class Workspace(AbstractModel):
     """A class used to represent a Workspace.
```

### Comparing `snap_saas_base-0.1.0/PKG-INFO` & `snap_saas_base-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snap-saas-base
-Version: 0.1.0
+Version: 0.4.0
 Summary: Snap Env (https://snapenv.com) Python base module.
 Home-page: https://github.com/orgs/snapenv/snap-saas-base
 Author: Abner G Jacobsen
 Author-email: abner@apoana.com.br
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

