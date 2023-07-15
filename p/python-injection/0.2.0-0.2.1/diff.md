# Comparing `tmp/python_injection-0.2.0.tar.gz` & `tmp/python_injection-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_injection-0.2.0.tar", max compression
+gzip compressed data, was "python_injection-0.2.1.tar", max compression
```

## Comparing `python_injection-0.2.0.tar` & `python_injection-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0     2538 2023-07-14 21:21:08.690746 python_injection-0.2.0/README.md
--rw-r--r--   0        0        0       38 2023-07-14 21:21:08.690746 python_injection-0.2.0/injection/__init__.py
--rw-r--r--   0        0        0     3621 2023-07-14 21:21:08.690746 python_injection-0.2.0/injection/core.py
--rw-r--r--   0        0        0      381 2023-07-14 21:21:08.690746 python_injection-0.2.0/injection/core.pyi
--rw-r--r--   0        0        0      461 2023-07-14 21:21:08.690746 python_injection-0.2.0/injection/utils.py
--rw-r--r--   0        0        0       81 2023-07-14 21:21:08.690746 python_injection-0.2.0/injection/utils.pyi
--rw-r--r--   0        0        0      561 2023-07-14 21:21:33.231213 python_injection-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 python_injection-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2538 2023-07-15 13:17:13.335254 python_injection-0.2.1/README.md
+-rw-r--r--   0        0        0       38 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/__init__.py
+-rw-r--r--   0        0        0     3657 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/core.py
+-rw-r--r--   0        0        0      340 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/core.pyi
+-rw-r--r--   0        0        0       39 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/exceptions.py
+-rw-r--r--   0        0        0      461 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/utils.py
+-rw-r--r--   0        0        0       81 2023-07-15 13:17:13.335254 python_injection-0.2.1/injection/utils.pyi
+-rw-r--r--   0        0        0      561 2023-07-15 13:17:34.087188 python_injection-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 python_injection-0.2.1/PKG-INFO
```

### Comparing `python_injection-0.2.0/README.md` & `python_injection-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -108,18 +108,18 @@
 Useful for put in memory injectables hidden deep within a package. Example:
 
 ```
 package
 ├── sub_package
 │   ├── __init__.py
 │   └── module2.py
-│       └── class Injectable1
+│       └── class Injectable2
 ├── __init__.py
 └── module1.py
-    └── class Injectable2
+    └── class Injectable1
 ```
 
 To load Injectable1 and Injectable2 into memory you can do the following:
 
 ```python
 from injection.utils import load_package
```

### Comparing `python_injection-0.2.0/injection/core.py` & `python_injection-0.2.1/injection/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import inspect
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from functools import cached_property, wraps
 from inspect import Parameter
-from typing import Callable, Generic, NamedTuple, TypeVar
+from typing import Callable, Generic, TypeVar
+
+from injection.exceptions import NoInjectable
 
 T = TypeVar("T")
 
 
 @dataclass(repr=False, frozen=True, slots=True)
 class Injectable(Generic[T], ABC):
     __constructor: Callable[..., T]
@@ -30,18 +32,14 @@
     def __instance(self) -> T:
         return self.factory()
 
     def get_instance(self) -> T:
         return self.__instance
 
 
-class NoInjectable(Exception):
-    ...
-
-
 @dataclass(repr=False, frozen=True, slots=True)
 class InjectionManager:
     __container: dict[type, Injectable] = field(default_factory=dict, init=False)
 
     def __getitem__(self, reference: type) -> Injectable:
         try:
             return self.__container[reference]
@@ -59,23 +57,24 @@
 
 
 _manager = InjectionManager()
 
 del InjectionManager
 
 
-class Decorator(NamedTuple):
-    injectable_class: type[Injectable]
+@dataclass(repr=False, frozen=True, slots=True)
+class Decorator:
+    __injectable_class: type[Injectable]
 
     def __repr__(self) -> str:
-        return f"<{self.injectable_class.__name__} decorator>"  # pragma: no cover
+        return f"<{self.__injectable_class.__name__} decorator>"  # pragma: no cover
 
     def __call__(self, wp=None, /, **kwargs):
         def decorator(wrapped):
-            injectable = self.injectable_class(wrapped)
+            injectable = self.__injectable_class(wrapped)
 
             if isinstance(wrapped, type):
                 _manager[wrapped] = injectable
 
             if reference := kwargs.pop("reference", None):
                 _manager[reference] = injectable
```

### Comparing `python_injection-0.2.0/pyproject.toml` & `python_injection-0.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-injection"
-version = "0.2.0"
+version = "0.2.1"
 description = "Fast and easy dependency injection framework."
 authors = ["remimd"]
 keywords = ["dependencies", "inject", "injection"]
 license = "MIT"
 packages = [{ include = "injection" }]
 readme = "README.md"
 repository = "https://github.com/soon-app/injection"
```

### Comparing `python_injection-0.2.0/PKG-INFO` & `python_injection-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-injection
-Version: 0.2.0
+Version: 0.2.1
 Summary: Fast and easy dependency injection framework.
 Home-page: https://github.com/soon-app/injection
 License: MIT
 Keywords: dependencies,inject,injection
 Author: remimd
 Requires-Python: >=3.10,<4
 Classifier: License :: OSI Approved :: MIT License
@@ -124,18 +124,18 @@
 Useful for put in memory injectables hidden deep within a package. Example:
 
 ```
 package
 ├── sub_package
 │   ├── __init__.py
 │   └── module2.py
-│       └── class Injectable1
+│       └── class Injectable2
 ├── __init__.py
 └── module1.py
-    └── class Injectable2
+    └── class Injectable1
 ```
 
 To load Injectable1 and Injectable2 into memory you can do the following:
 
 ```python
 from injection.utils import load_package
```

