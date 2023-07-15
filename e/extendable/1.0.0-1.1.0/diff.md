# Comparing `tmp/extendable-1.0.0.tar.gz` & `tmp/extendable-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extendable-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "extendable-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `extendable-1.0.0.tar` & `extendable-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1081 2023-07-14 16:30:24.882046 extendable-1.0.0/LICENSE
--rw-r--r--   0        0        0     3245 2023-07-14 16:30:24.882046 extendable-1.0.0/README.md
--rw-r--r--   0        0        0     1457 2023-07-14 16:30:24.882046 extendable-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      393 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/__init__.py
--rw-r--r--   0        0        0      332 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/context.py
--rw-r--r--   0        0        0       55 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/exceptions.py
--rw-r--r--   0        0        0     9975 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/main.py
--rw-r--r--   0        0        0        0 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/py.typed
--rw-r--r--   0        0        0     8212 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/registry.py
--rw-r--r--   0        0        0     1059 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/utils.py
--rw-r--r--   0        0        0       22 2023-07-14 16:30:24.882046 extendable-1.0.0/src/extendable/version.py
--rw-r--r--   0        0        0     4248 1970-01-01 00:00:00.000000 extendable-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-07-15 16:23:03.710562 extendable-1.1.0/LICENSE
+-rw-r--r--   0        0        0     7477 2023-07-15 16:23:03.710562 extendable-1.1.0/README.md
+-rw-r--r--   0        0        0     1457 2023-07-15 16:23:03.710562 extendable-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      393 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/__init__.py
+-rw-r--r--   0        0        0      332 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/context.py
+-rw-r--r--   0        0        0       55 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/exceptions.py
+-rw-r--r--   0        0        0    10056 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/main.py
+-rw-r--r--   0        0        0        0 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/py.typed
+-rw-r--r--   0        0        0     8212 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/registry.py
+-rw-r--r--   0        0        0     1059 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/utils.py
+-rw-r--r--   0        0        0       22 2023-07-15 16:23:03.710562 extendable-1.1.0/src/extendable/version.py
+-rw-r--r--   0        0        0     8480 1970-01-01 00:00:00.000000 extendable-1.1.0/PKG-INFO
```

### Comparing `extendable-1.0.0/LICENSE` & `extendable-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extendable-1.0.0/pyproject.toml` & `extendable-1.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `extendable-1.0.0/src/extendable/main.py` & `extendable-1.1.0/src/extendable/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,16 @@
     _original_cls: "ExtendableMeta"
 
     @no_type_check
     def __new__(metacls, name, bases, namespace, extends=None, **kwargs):
         """create the expected class and collect the class definition that will be used
         at the end of registry load process to build the final class."""
         class_def = None
+        if isinstance(extends, bool) and extends:
+            extends = bases[0]
         if not _registry_build_mode:
             namespace = metacls._prepare_namespace(
                 name=name, bases=bases, namespace=namespace, extends=extends, **kwargs
             )
             class_def = metacls._collect_class_def(
                 name=name, bases=bases, namespace=namespace, extends=extends, **kwargs
             )
```

### Comparing `extendable-1.0.0/src/extendable/registry.py` & `extendable-1.1.0/src/extendable/registry.py`

 * *Files identical despite different names*

### Comparing `extendable-1.0.0/src/extendable/utils.py` & `extendable-1.1.0/src/extendable/utils.py`

 * *Files identical despite different names*

