# Comparing `tmp/valcheck-0.3.8.tar.gz` & `tmp/valcheck-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valcheck-0.3.8.tar", last modified: Thu Jul 13 15:49:04 2023, max compression
+gzip compressed data, was "valcheck-0.3.9.tar", last modified: Sat Jul 15 05:52:38 2023, max compression
```

## Comparing `valcheck-0.3.8.tar` & `valcheck-0.3.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-13 15:49:04.879855 valcheck-0.3.8/
--rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-0.3.8/LICENSE
--rw-rw-rw-   0        0        0      760 2023-07-13 15:49:04.878024 valcheck-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     2674 2023-07-13 15:45:46.000000 valcheck-0.3.8/README.md
--rw-rw-rw-   0        0        0       42 2023-07-13 15:49:04.879855 valcheck-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1568 2023-07-13 15:44:55.000000 valcheck-0.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-13 15:49:04.857757 valcheck-0.3.8/valcheck/
--rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-0.3.8/valcheck/__init__.py
--rw-rw-rw-   0        0        0     1270 2023-07-02 09:39:38.000000 valcheck-0.3.8/valcheck/exceptions.py
--rw-rw-rw-   0        0        0    18170 2023-07-10 06:29:50.000000 valcheck-0.3.8/valcheck/fields.py
--rw-rw-rw-   0        0        0     2574 2023-07-10 06:29:50.000000 valcheck-0.3.8/valcheck/models.py
--rw-rw-rw-   0        0        0     2490 2023-07-09 19:22:10.000000 valcheck-0.3.8/valcheck/utils.py
--rw-rw-rw-   0        0        0     5322 2023-07-10 06:29:50.000000 valcheck-0.3.8/valcheck/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-13 15:49:04.877022 valcheck-0.3.8/valcheck.egg-info/
--rw-rw-rw-   0        0        0      760 2023-07-13 15:49:04.000000 valcheck-0.3.8/valcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-13 15:49:04.000000 valcheck-0.3.8/valcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-13 15:49:04.000000 valcheck-0.3.8/valcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-13 15:49:04.000000 valcheck-0.3.8/valcheck.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 05:52:38.775278 valcheck-0.3.9/
+-rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-0.3.9/LICENSE
+-rw-rw-rw-   0        0        0      760 2023-07-15 05:52:38.771305 valcheck-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     2674 2023-07-13 15:45:46.000000 valcheck-0.3.9/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 05:52:38.775278 valcheck-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2023-07-15 05:51:54.000000 valcheck-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 05:52:38.752382 valcheck-0.3.9/valcheck/
+-rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-0.3.9/valcheck/__init__.py
+-rw-rw-rw-   0        0        0     1270 2023-07-02 09:39:38.000000 valcheck-0.3.9/valcheck/exceptions.py
+-rw-rw-rw-   0        0        0    19874 2023-07-15 05:51:54.000000 valcheck-0.3.9/valcheck/fields.py
+-rw-rw-rw-   0        0        0     2694 2023-07-15 05:51:54.000000 valcheck-0.3.9/valcheck/models.py
+-rw-rw-rw-   0        0        0     2485 2023-07-15 05:51:54.000000 valcheck-0.3.9/valcheck/utils.py
+-rw-rw-rw-   0        0        0     5394 2023-07-15 05:51:54.000000 valcheck-0.3.9/valcheck/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-15 05:52:38.771305 valcheck-0.3.9/valcheck.egg-info/
+-rw-rw-rw-   0        0        0      760 2023-07-15 05:52:38.000000 valcheck-0.3.9/valcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-15 05:52:38.000000 valcheck-0.3.9/valcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 05:52:38.000000 valcheck-0.3.9/valcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-15 05:52:38.000000 valcheck-0.3.9/valcheck.egg-info/top_level.txt
```

### Comparing `valcheck-0.3.8/LICENSE` & `valcheck-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `valcheck-0.3.8/PKG-INFO` & `valcheck-0.3.9/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `valcheck-0.3.8/README.md` & `valcheck-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `valcheck-0.3.8/setup.py` & `valcheck-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import find_packages, setup
 
 # Constants
 PACKAGE_NAME = "valcheck"
-PACKAGE_VERSION = "0.3.8"
+PACKAGE_VERSION = "0.3.9"
 AUTHOR_NAME = "Nishant Rao"
 AUTHOR_EMAIL_ID = "nishant.rao173@gmail.com"
 FILEPATH_TO_README = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
 FILEPATH_TO_REQUIREMENTS = os.path.join(os.path.abspath(os.path.dirname(__file__)), "requirements.txt")
 REPOSITORY_URL = "https://github.com/Nishant173/valcheck"
 
 # Requirements
```

### Comparing `valcheck-0.3.8/valcheck/exceptions.py` & `valcheck-0.3.9/valcheck/exceptions.py`

 * *Files identical despite different names*

### Comparing `valcheck-0.3.8/valcheck/fields.py` & `valcheck-0.3.9/valcheck/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from copy import deepcopy
 from typing import Any, Callable, Iterable, List, Optional, Type, Union
 
 from valcheck.models import Error
 from valcheck.utils import (
     Empty,
     dict_has_any_keys,
     is_empty,
@@ -12,38 +13,42 @@
     is_list_of_instances_of_type,
     is_valid_datetime_string,
     is_valid_email_id,
     is_valid_json_string,
     is_valid_object_of_type,
     is_valid_uuid_string,
     set_as_empty,
+    wrap_in_quotes_if_string,
 )
 
 
 class ValidatedField:
     """Class that represents a validated field"""
 
     def __init__(
             self,
             *,
+            field_identifier: str,
             field_name: str,
             field_value: Union[Any, Empty],
             errors: List[Error],
         ) -> None:
+        assert isinstance(field_identifier, str), "Param `field_identifier` must be of type 'str'"
         assert isinstance(field_name, str), "Param `field_name` must be of type 'str'"
         assert is_list_of_instances_of_type(errors, type_=Error, allow_empty=True), (
             "Param `errors` must be a list where each item is of type `valcheck.models.Error`"
         )
 
+        self.field_identifier = field_identifier
         self.field_name = field_name
         self._field_value = field_value
         self._errors = errors
 
     def __str__(self) -> str:
-        return f"{self.__class__.__name__}(field_name='{self.field_name}')"
+        return f"{self.__class__.__name__}(field_identifier='{self.field_identifier}', field_name='{self.field_name}')"
 
     @property
     def field_value(self) -> Union[Any, Empty]:
         return self._field_value
 
     @field_value.setter
     def field_value(self, value: Union[Any, Empty]) -> None:
@@ -63,33 +68,38 @@
 
 class Field:
     """Class that represents a field (that needs to be validated)"""
 
     def __init__(
             self,
             *,
+            alias: Optional[str] = None,
             required: Optional[bool] = True,
             nullable: Optional[bool] = False,
             default_factory: Optional[Callable] = None,
             converter_factory: Optional[Callable] = None,
             validators: Optional[List[Callable]] = None,
             error: Optional[Error] = None,
         ) -> None:
         """
         Parameters:
+            - alias (str): Alias for the field's name (optional)
             - required (bool): True if the field is required, else False. Default: True
             - nullable (bool): True if the field is nullable, else False. Default: False
             - default_factory (callable): Callable that returns the default value to set for the field
             if `required=False` and the field is missing.
             - converter_factory (callable): Callable that takes in the validated value (of the field), and returns
             the converted value (for the field).
             - validators (list of callables): List of callables that each return a boolean (takes the field value as a param).
             The callable returns True if validation is successful, else False.
             - error (Error instance): Instance of type `valcheck.models.Error`.
         """
+        assert alias is None or is_valid_object_of_type(alias, type_=str, allow_empty=False), (
+            "Param `alias` must be of type 'str' and must be non-empty"
+        )
         assert isinstance(required, bool), "Param `required` must be of type 'bool'"
         assert isinstance(nullable, bool), "Param `nullable` must be of type 'bool'"
         assert default_factory is None or callable(default_factory), (
             "Param `default_factory` must be a callable that returns the default value if the field is missing when `required=False`"
         )
         assert converter_factory is None or callable(converter_factory), (
             "Param `converter_factory` must be a callable that takes in the validated value (of the field), and returns"
@@ -97,23 +107,50 @@
         )
         assert validators is None or isinstance(validators, list), "Param `validators` must be of type 'list'"
         if isinstance(validators, list):
             for validator in validators:
                 assert callable(validator), "Param `validators` must be a list of callables"
         assert error is None or isinstance(error, Error), "Param `error` must be of type `valcheck.models.Error`"
 
+        self._field_identifier = set_as_empty()
         self._field_name = set_as_empty()
         self._field_value = set_as_empty()
+        self.alias = alias
         self.required = required
         self.nullable = nullable
         self.default_factory = default_factory
         self.converter_factory = converter_factory
         self.validators = validators or []
         self.error = error or Error()
 
+    def copy(self) -> Field:
+        """Returns deep-copy of current `Field` object"""
+        return deepcopy(self)
+
+    def __str__(self) -> str:
+        kwargs_list = [
+            f"field_identifier={wrap_in_quotes_if_string(self.field_identifier)}",
+            f"field_name={wrap_in_quotes_if_string(self.field_name)}",
+            f"field_value={wrap_in_quotes_if_string(self.field_value)}",
+            f"alias={wrap_in_quotes_if_string(self.alias)}",
+            f"required={self.required}",
+            f"nullable={self.nullable}",
+        ]
+        kwargs_string = "(" + ", ".join(kwargs_list) + ")"
+        return f"{self.__class__.__name__}{kwargs_string}"
+
+    @property
+    def field_identifier(self) -> str:
+        return self._field_identifier
+
+    @field_identifier.setter
+    def field_identifier(self, value: str) -> None:
+        assert isinstance(value, str), "Param `field_identifier` must be of type 'str'"
+        self._field_identifier = value
+
     @property
     def field_name(self) -> str:
         return self._field_name
 
     @field_name.setter
     def field_name(self, value: str) -> None:
         assert isinstance(value, str), "Param `field_name` must be of type 'str'"
@@ -148,14 +185,15 @@
         """Returns list of errors (each of type `valcheck.models.Error`)"""
         raise NotImplementedError()
 
     def run_validations(self) -> ValidatedField:
         if is_empty(self.field_value) and not self.required and self.default_factory:
             self.field_value = self.default_factory()
         validated_field = ValidatedField(
+            field_identifier=self.field_identifier,
             field_name=self.field_name,
             field_value=self.field_value,
             errors=[],
         )
         if is_empty(self.field_value) and not self.required and not self.default_factory:
             return validated_field
         if self._can_be_set_to_null():
```

### Comparing `valcheck-0.3.8/valcheck/models.py` & `valcheck-0.3.9/valcheck/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -47,33 +47,35 @@
 
     def append_to_field_path(
             self,
             s: str,
             /,
             *,
             at_beginning: Optional[bool] = True,
-            separator: Optional[str] = ".",
+            separator: Optional[str] = " --> ",
         ) -> None:
         """Appends the given string `s` to the `field_path` (in-place)"""
         if not self.field_path:
             self.field_path += s
             return
         self.field_path = (
             s + separator + self.field_path
             if at_beginning else
             self.field_path + separator + s
         )
 
-    def as_dict(self) -> Dict[str, Any]:
-        return {
+    def as_dict(self, *, include_validator_info: Optional[bool] = True) -> Dict[str, Any]:
+        dict_ = {
             "description": self.description,
             "code": self.code,
             "details": self.details,
-            "validator_info": {
+        }
+        if include_validator_info:
+            dict_["validator_info"] = {
                 "validator_message": self.validator_message,
                 "field_path": self.field_path,
-            },
-        }
+            }
+        return dict_
 
     def __str__(self) -> str:
         return f"{self.__class__.__name__}({self.as_dict()})"
```

### Comparing `valcheck-0.3.8/valcheck/utils.py` & `valcheck-0.3.9/valcheck/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,11 +81,11 @@
     return isinstance(obj, Empty)
 
 
 def is_instance_of_any(obj: Any, types: List[Type]) -> bool:
     return any((isinstance(obj, type_) for type_ in types))
 
 
-def wrap_in_quotes_if_string(obj: Any, /) -> str:
+def wrap_in_quotes_if_string(obj: Any, /) -> Any:
     if isinstance(obj, str):
         return f"'{obj}'"
-    return f"{obj}"
+    return obj
```

### Comparing `valcheck-0.3.8/valcheck/validator.py` & `valcheck-0.3.9/valcheck/validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,16 +47,16 @@
     def _clear_errors(self) -> None:
         """Clears out the list of errors"""
         self._errors.clear()
 
     def _register_errors(self, *, errors: List[Error]) -> None:
         self._errors.extend(errors)
 
-    def _register_validated_data(self, *, field_name: str, field_value: Any) -> None:
-        self._validated_data[field_name] = field_value
+    def _register_validated_data(self, *, key: str, value: Any) -> None:
+        self._validated_data[key] = value
 
     @property
     def validated_data(self) -> Dict[str, Any]:
         return self._validated_data
 
     def _clear_validated_data(self) -> None:
         """Clears out the dictionary having validated data"""
@@ -76,15 +76,15 @@
     def _perform_field_validation_checks(self, *, field: Field) -> None:
         """Performs validation checks for the given field, and registers errors (if any) and validated-data"""
         validated_field = field.run_validations()
         if validated_field.errors:
             self._register_errors(errors=validated_field.errors)
             return
         if not is_empty(validated_field.field_value):
-            self._register_validated_data(field_name=validated_field.field_name, field_value=validated_field.field_value)
+            self._register_validated_data(key=validated_field.field_identifier, value=validated_field.field_value)
 
     def _perform_model_validation_checks(self) -> None:
         """Performs model validation checks, and registers errors (if any)"""
         errors = self.model_validator()
         assert is_list_of_instances_of_type(errors, type_=Error, allow_empty=True), (
             "The output of the model validator method must be a list of errors (each of type `valcheck.models.Error`)."
             " Must be an empty list if there are no errors."
@@ -105,17 +105,18 @@
     def run_validations(self, *, raise_exception: Optional[bool] = False) -> List[Error]:
         """
         Runs validations and registers errors/validated-data. Returns list of errors.
         If `raise_exception=True` and validations fail, raises `valcheck.exceptions.ValidationException`.
         """
         self._clear_errors()
         self._clear_validated_data()
-        for field_name, field in self._field_info.items():
-            field.field_name = field_name
-            field.field_value = self.data.get(field_name, set_as_empty())
+        for field_identifier, field in self._field_info.items():
+            field.field_identifier = field_identifier
+            field.field_name = field.alias if field.alias else field_identifier
+            field.field_value = self.data.get(field.field_name, set_as_empty())
             self._perform_field_validation_checks(field=field)
         # Perform model validation checks only if there are no errors in field validation checks
         if not self._errors:
             self._perform_model_validation_checks()
         if self._errors:
             self._clear_validated_data()
         if raise_exception and self._errors:
```

### Comparing `valcheck-0.3.8/valcheck.egg-info/PKG-INFO` & `valcheck-0.3.9/valcheck.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 0.3.8
+Version: 0.3.9
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

