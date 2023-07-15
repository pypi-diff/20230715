# Comparing `tmp/bovine_tool-0.2.6.tar.gz` & `tmp/bovine_tool-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bovine_tool-0.2.6.tar", max compression
+gzip compressed data, was "bovine_tool-0.3.0.tar", max compression
```

## Comparing `bovine_tool-0.2.6.tar` & `bovine_tool-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1327 2023-06-04 18:36:16.378481 bovine_tool-0.2.6/README.md
--rw-r--r--   0        0        0        0 2023-06-04 18:36:16.378481 bovine_tool-0.2.6/bovine_tool/__init__.py
--rw-r--r--   0        0        0      495 2023-06-04 18:36:16.378481 bovine_tool-0.2.6/bovine_tool/cleanup.py
--rw-r--r--   0        0        0      277 2023-06-04 18:36:16.378481 bovine_tool-0.2.6/bovine_tool/create.py
--rw-r--r--   0        0        0     2060 2023-06-04 18:36:16.378481 bovine_tool-0.2.6/bovine_tool/manage.py
--rw-r--r--   0        0        0      770 2023-06-04 18:36:16.378481 bovine_tool-0.2.6/bovine_tool/register.py
--rw-r--r--   0        0        0      557 2023-06-04 18:36:16.378481 bovine_tool-0.2.6/bovine_tool/store.py
--rw-r--r--   0        0        0      520 2023-06-04 18:36:21.138507 bovine_tool-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2044 1970-01-01 00:00:00.000000 bovine_tool-0.2.6/setup.py
--rw-r--r--   0        0        0     1857 1970-01-01 00:00:00.000000 bovine_tool-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1327 2023-07-15 11:45:43.763733 bovine_tool-0.3.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-15 11:45:43.763733 bovine_tool-0.3.0/bovine_tool/__init__.py
+-rw-r--r--   0        0        0      495 2023-07-15 11:45:43.767733 bovine_tool-0.3.0/bovine_tool/cleanup.py
+-rw-r--r--   0        0        0      277 2023-07-15 11:45:43.767733 bovine_tool-0.3.0/bovine_tool/create.py
+-rw-r--r--   0        0        0     2060 2023-07-15 11:45:43.767733 bovine_tool-0.3.0/bovine_tool/manage.py
+-rw-r--r--   0        0        0      770 2023-07-15 11:45:43.767733 bovine_tool-0.3.0/bovine_tool/register.py
+-rw-r--r--   0        0        0      557 2023-07-15 11:45:43.767733 bovine_tool-0.3.0/bovine_tool/store.py
+-rw-r--r--   0        0        0      519 2023-07-15 11:46:38.108131 bovine_tool-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2044 1970-01-01 00:00:00.000000 bovine_tool-0.3.0/setup.py
+-rw-r--r--   0        0        0     1857 1970-01-01 00:00:00.000000 bovine_tool-0.3.0/PKG-INFO
```

### Comparing `bovine_tool-0.2.6/README.md` & `bovine_tool-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.6/bovine_tool/manage.py` & `bovine_tool-0.3.0/bovine_tool/manage.py`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.6/bovine_tool/register.py` & `bovine_tool-0.3.0/bovine_tool/register.py`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.6/bovine_tool/store.py` & `bovine_tool-0.3.0/bovine_tool/store.py`

 * *Files identical despite different names*

### Comparing `bovine_tool-0.2.6/pyproject.toml` & `bovine_tool-0.3.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 [tool.poetry]
 name = "bovine-tool"
-version = "0.2.6"
+version = "0.3.0"
 description = "Basic tools to administrate a bovine herd"
 authors = ["Helge <helge.krueger@gmail.com>"]
 readme = "README.md"
 packages = [{include = "bovine_tool"}]
 repository = "https://codeberg.org/bovine/bovine"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-bovine-store = "^0.2.1"
-
+bovine-store = "^0.3.0"
 
 [tool.poetry.group.dev.dependencies]
 flake8 = "^6.0.0"
 black = "^23.3.0"
 flake8-black = "^0.3.6"
 
 [build-system]
```

### Comparing `bovine_tool-0.2.6/setup.py` & `bovine_tool-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 packages = \
 ['bovine_tool']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['bovine-store>=0.2.1,<0.3.0']
+['bovine-store>=0.3.0,<0.4.0']
 
 setup_kwargs = {
     'name': 'bovine-tool',
-    'version': '0.2.6',
+    'version': '0.3.0',
     'description': 'Basic tools to administrate a bovine herd',
     'long_description': '# bovine_tool\n\nbovine_tool provides a CLI interface to manage bovine.\n\n## Configuration\n\nThe default database connection is "sqlite://bovine.sqlite3". This can be overwridden with the environment variable "BOVINE_DB_URL".\n\n## Quick start\n\nTo register a new user with a FediVerse handle use\n\n```bash\npython -m bovine_tool.register fediverse_handle [--domain DOMAIN]\n```\n\nthe domain must be specified. This creates the account `acct:fediverse_handle@DOMAIN`.\n\n## Managing users\n\n```bash\npython -m bovine_tool.manage bovine_name\n```\n\ndisplays the user.\n\nTo add a did key for [the Moo Client Registration Flow](https://blog.mymath.rocks/2023-03-25/BIN2_Moo_Client_Registration_Flow) with a BovineClient use\n\n```bash\npython -m bovine_tool.manage bovine_name --did_key key_name did_key\n```\n\nFurthermore, using `--properties` the properties can be over written.\n\n## Cleaning the database\n\n```bash\npython -m bovine_tool.cleanup\n```\n\nto delete all remote objects older than 3 days. This should be expanded to make the variables configurable and delete a bunch of other stuff, e.g.\n\n- remove inbox, outbox entries older than 14 days\n- have a "timeline" of outbox entries to display on a public profile\n- remove all local entries not in inbox, outbox, or timeline\n- remove deleted items older than 1 month\n- make time frames configurable\n',
     'author': 'Helge',
     'author_email': 'helge.krueger@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://codeberg.org/bovine/bovine',
```

### Comparing `bovine_tool-0.2.6/PKG-INFO` & `bovine_tool-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: bovine-tool
-Version: 0.2.6
+Version: 0.3.0
 Summary: Basic tools to administrate a bovine herd
 Home-page: https://codeberg.org/bovine/bovine
 Author: Helge
 Author-email: helge.krueger@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: bovine-store (>=0.2.1,<0.3.0)
+Requires-Dist: bovine-store (>=0.3.0,<0.4.0)
 Project-URL: Repository, https://codeberg.org/bovine/bovine
 Description-Content-Type: text/markdown
 
 # bovine_tool
 
 bovine_tool provides a CLI interface to manage bovine.
```

