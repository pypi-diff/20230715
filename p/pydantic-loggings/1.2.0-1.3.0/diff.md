# Comparing `tmp/pydantic-loggings-1.2.0.tar.gz` & `tmp/pydantic-loggings-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic-loggings-1.2.0.tar", last modified: Fri Jul 14 17:57:06 2023, max compression
+gzip compressed data, was "pydantic-loggings-1.3.0.tar", last modified: Sat Jul 15 07:37:12 2023, max compression
```

## Comparing `pydantic-loggings-1.2.0.tar` & `pydantic-loggings-1.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/
--rw-r--r--   0 root         (0) root         (0)     3119 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2313 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/README.md
--rw-r--r--   0 root         (0) root         (0)     2508 2023-07-14 17:56:56.000000 pydantic-loggings-1.2.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.846429 pydantic-loggings-1.2.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.846429 pydantic-loggings-1.2.0/src/pydantic_loggings/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/src/pydantic_loggings/base/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/__init__.py
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/filters.py
--rw-r--r--   0 root         (0) root         (0)      404 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/formatters.py
--rw-r--r--   0 root         (0) root         (0)      392 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/handlers.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/loggers.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/base/loggings.py
--rw-r--r--   0 root         (0) root         (0)     3706 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/mixins.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/
--rw-r--r--   0 root         (0) root         (0)      241 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/__init__.py
--rw-r--r--   0 root         (0) root         (0)      419 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/filters.py
--rw-r--r--   0 root         (0) root         (0)     1417 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/formatters.py
--rw-r--r--   0 root         (0) root         (0)      894 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/handlers.py
--rw-r--r--   0 root         (0) root         (0)      706 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/loggers.py
--rw-r--r--   0 root         (0) root         (0)     2649 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/loggings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.850429 pydantic-loggings-1.2.0/src/pydantic_loggings/rich/
--rw-r--r--   0 root         (0) root         (0)      148 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/rich/__init__.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/rich/handlers.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/rich/loggers.py
--rw-r--r--   0 root         (0) root         (0)      405 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/rich/loggings.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/types_.py
--rw-r--r--   0 root         (0) root         (0)       91 2023-07-14 17:56:55.000000 pydantic-loggings-1.2.0/src/pydantic_loggings/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 17:57:06.846429 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3119 2023-07-14 17:57:06.000000 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1018 2023-07-14 17:57:06.000000 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 17:57:06.000000 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-07-14 17:57:06.000000 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-07-14 17:57:06.000000 pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2313 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     2508 2023-07-15 07:37:02.000000 pydantic-loggings-1.3.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.626620 pydantic-loggings-1.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.626620 pydantic-loggings-1.3.0/src/pydantic_loggings/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/src/pydantic_loggings/base/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/filters.py
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      392 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      650 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/base/loggings.py
+-rw-r--r--   0 root         (0) root         (0)     3706 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/mixins.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/
+-rw-r--r--   0 root         (0) root         (0)      241 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      419 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/filters.py
+-rw-r--r--   0 root         (0) root         (0)     1417 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/formatters.py
+-rw-r--r--   0 root         (0) root         (0)      894 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      706 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/loggers.py
+-rw-r--r--   0 root         (0) root         (0)     2710 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/loggings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/src/pydantic_loggings/rich/
+-rw-r--r--   0 root         (0) root         (0)      148 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/rich/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/rich/handlers.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/rich/loggers.py
+-rw-r--r--   0 root         (0) root         (0)      454 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/rich/loggings.py
+-rw-r--r--   0 root         (0) root         (0)      391 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/types_.py
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-15 07:37:01.000000 pydantic-loggings-1.3.0/src/pydantic_loggings/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 07:37:12.630620 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3119 2023-07-15 07:37:12.000000 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-07-15 07:37:12.000000 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 07:37:12.000000 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-07-15 07:37:12.000000 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-07-15 07:37:12.000000 pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/top_level.txt
```

### Comparing `pydantic-loggings-1.2.0/PKG-INFO` & `pydantic-loggings-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 1.2.0
+Version: 1.3.0
 Summary: Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-loggings
 Project-URL: Source, https://github.com/m9810223/pydantic-loggings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pydantic-loggings-1.2.0/README.md` & `pydantic-loggings-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.2.0/pyproject.toml` & `pydantic-loggings-1.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project.urls]
 Homepage = "https://github.com/m9810223/pydantic-loggings"
 Source = "https://github.com/m9810223/pydantic-loggings"
 
 [project]
 name = "pydantic-loggings"
 description = "Configure 🎁 Your 🤗 Python 🐍 Logging 📝"
-version = "1.2.0"
+version = "1.3.0"
 authors = [
   { name = "m9810223", email = "m9810223@gmail.com" },
 ]
 requires-python = ">=3.9"
 readme = "README.md"
 
 classifiers = [
```

### Comparing `pydantic-loggings-1.2.0/src/pydantic_loggings/mixins.py` & `pydantic-loggings-1.3.0/src/pydantic_loggings/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/formatters.py` & `pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/formatters.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/handlers.py` & `pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/loggers.py` & `pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/loggers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.2.0/src/pydantic_loggings/not_set/loggings.py` & `pydantic-loggings-1.3.0/src/pydantic_loggings/not_set/loggings.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 from pydantic import field_validator
 from pydantic_core.core_schema import FieldValidationInfo
 from pydantic_settings import BaseSettings
 from pydantic_settings import SettingsConfigDict
 
 from .. import mixins
+from ..types_ import OptionalModel
+from ..types_ import OptionalModelDict
 from .filters import Filter
 from .formatters import Formatter
 from .handlers import Handler
 from .loggers import Logger
 
 
 class Logging(
@@ -26,19 +28,19 @@
         env_prefix='log__',
         env_nested_delimiter='__',
         extra='ignore',
     )
     # https://docs.python.org/3/library/logging.config.html#configuration-dictionary-schema
     # https://docs.python.org/3/howto/logging-cookbook.html#an-example-dictionary-based-configuration
     version: int = 1  # ok
-    formatters: t.Optional[dict[str, Formatter]] = None
-    filters: t.Optional[dict[str, Filter]] = None
-    handlers: t.Optional[dict[str, Handler]] = None
-    loggers: t.Optional[dict[str, Logger]] = None
-    root: t.Optional[Logger] = None
+    formatters: OptionalModelDict[Formatter] = None
+    filters: OptionalModelDict[Filter] = None
+    handlers: OptionalModelDict[Handler] = None
+    loggers: OptionalModelDict[Logger] = None
+    root: OptionalModel[Logger] = None
     incremental: t.Optional[bool] = None
     disable_existing_loggers: t.Optional[bool] = None
 
     configurator: t.ClassVar = DictConfigurator
 
     @field_validator(
         'formatters',
```

### Comparing `pydantic-loggings-1.2.0/src/pydantic_loggings/rich/handlers.py` & `pydantic-loggings-1.3.0/src/pydantic_loggings/rich/handlers.py`

 * *Files identical despite different names*

### Comparing `pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/PKG-INFO` & `pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-loggings
-Version: 1.2.0
+Version: 1.3.0
 Summary: Configure 🎁 Your 🤗 Python 🐍 Logging 📝
 Author-email: m9810223 <m9810223@gmail.com>
 Project-URL: Homepage, https://github.com/m9810223/pydantic-loggings
 Project-URL: Source, https://github.com/m9810223/pydantic-loggings
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pydantic-loggings-1.2.0/src/pydantic_loggings.egg-info/SOURCES.txt` & `pydantic-loggings-1.3.0/src/pydantic_loggings.egg-info/SOURCES.txt`

 * *Files identical despite different names*

