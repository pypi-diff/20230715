# Comparing `tmp/django_registries-0.0.1rc0.tar.gz` & `tmp/django_registries-0.0.2.tar.gz`

## Comparing `django_registries-0.0.1rc0.tar` & `django_registries-0.0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 django_registries-0.0.1rc0/django_registries/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_registries-0.0.1rc0/django_registries/__init__.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 django_registries-0.0.1rc0/django_registries/apps.py
--rw-r--r--   0        0        0     2445 2020-02-02 00:00:00.000000 django_registries-0.0.1rc0/django_registries/registry.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 django_registries-0.0.1rc0/.gitignore
--rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 django_registries-0.0.1rc0/LICENSE.txt
--rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 django_registries-0.0.1rc0/README.md
--rw-r--r--   0        0        0     2911 2020-02-02 00:00:00.000000 django_registries-0.0.1rc0/pyproject.toml
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 django_registries-0.0.1rc0/PKG-INFO
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 django_registries-0.0.2/django_registries/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_registries-0.0.2/django_registries/__init__.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 django_registries-0.0.2/django_registries/apps.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 django_registries-0.0.2/django_registries/py.typed
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 django_registries-0.0.2/django_registries/registry.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 django_registries-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1110 2020-02-02 00:00:00.000000 django_registries-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0     1260 2020-02-02 00:00:00.000000 django_registries-0.0.2/README.md
+-rw-r--r--   0        0        0     2960 2020-02-02 00:00:00.000000 django_registries-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 django_registries-0.0.2/PKG-INFO
```

### Comparing `django_registries-0.0.1rc0/LICENSE.txt` & `django_registries-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django_registries-0.0.1rc0/README.md` & `django_registries-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `django_registries-0.0.1rc0/pyproject.toml` & `django_registries-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,23 +2,24 @@
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "django-registries"
 description = 'django-registries is a structured way to create registries of implementations.'
 readme = "README.md"
-requires-python = ">=3.10"
+requires-python = ">=3.9"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Víðir Valberg Guðmundsson", email = "valberg@orn.li" },
 ]
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Programming Language :: Python",
+  "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
   "Django>=3.2",
@@ -45,15 +46,15 @@
   "pytest-cov",
   "pytest-django==4.5.2",
   "mypy==1.1.1",
   "django-stubs==1.16.0",
 ]
 
 [[tool.hatch.envs.tests.matrix]]
-python = ["3.10", "3.11"]
+python = ["3.9", "3.10", "3.11"]
 django = ["3.2", "4.0", "4.1", "4.2"]
 
 [tool.hatch.envs.tests.overrides]
 matrix.django.dependencies = [
     { value = "django~={matrix:django}" },
 ]
 matrix.python.dependencies = [
```

### Comparing `django_registries-0.0.1rc0/PKG-INFO` & `django_registries-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-registries
-Version: 0.0.1rc0
+Version: 0.0.2
 Summary: django-registries is a structured way to create registries of implementations.
 Project-URL: Documentation, https://django-registries.readthedocs.io/
 Project-URL: Issues, https://github.com/valberg/django-registries/issues
 Project-URL: Source, https://github.com/valberg/django-registries
 Author-email: Víðir Valberg Guðmundsson <valberg@orn.li>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
-Requires-Python: >=3.10
+Requires-Python: >=3.9
 Requires-Dist: django>=3.2
 Description-Content-Type: text/markdown
 
 # Django Registries
 
 [![Tests](https://github.com/valberg/django-registries/actions/workflows/test.yml/badge.svg)](https://github.com/valberg/django-registries/actions/workflows/test.yml)
 [![Documentation](https://readthedocs.org/projects/django-registries/badge/?version=latest)](https://django-registries.readthedocs.io/en/latest/?badge=latest)
```

