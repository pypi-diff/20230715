# Comparing `tmp/universi-0.4.0.tar.gz` & `tmp/universi-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universi-0.4.0.tar", max compression
+gzip compressed data, was "universi-0.5.0.tar", max compression
```

## Comparing `universi-0.4.0.tar` & `universi-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.4.0/LICENSE
--rw-r--r--   0        0        0    10495 2023-07-14 22:57:30.396654 universi-0.4.0/README.md
--rw-r--r--   0        0        0     4059 2023-07-14 22:57:44.169987 universi-0.4.0/pyproject.toml
--rw-r--r--   0        0        0      453 2023-07-12 22:40:12.864421 universi-0.4.0/universi/__init__.py
--rw-r--r--   0        0        0     2821 2023-07-14 12:35:15.746665 universi-0.4.0/universi/_utils.py
--rw-r--r--   0        0        0    20023 2023-07-14 20:26:25.333325 universi-0.4.0/universi/codegen.py
--rw-r--r--   0        0        0      324 2023-07-10 23:48:56.035792 universi-0.4.0/universi/exceptions.py
--rw-r--r--   0        0        0     2841 2023-07-08 14:21:11.688092 universi-0.4.0/universi/fields.py
--rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.4.0/universi/header.py
--rw-r--r--   0        0        0        0 2023-07-13 08:09:29.390618 universi-0.4.0/universi/py.typed
--rw-r--r--   0        0        0    12278 2023-07-14 12:35:15.899998 universi-0.4.0/universi/routing.py
--rw-r--r--   0        0        0      396 2023-07-08 11:43:06.913473 universi-0.4.0/universi/structure/__init__.py
--rw-r--r--   0        0        0      265 2023-07-08 11:43:06.913473 universi-0.4.0/universi/structure/common.py
--rw-r--r--   0        0        0     4936 2023-07-10 10:22:38.358870 universi-0.4.0/universi/structure/endpoints.py
--rw-r--r--   0        0        0      944 2023-07-08 11:43:06.913473 universi-0.4.0/universi/structure/enums.py
--rw-r--r--   0        0        0     1270 2023-07-14 12:35:15.266665 universi-0.4.0/universi/structure/responses.py
--rw-r--r--   0        0        0     4207 2023-07-14 12:35:03.836665 universi-0.4.0/universi/structure/schemas.py
--rw-r--r--   0        0        0     8933 2023-07-14 12:35:15.819998 universi-0.4.0/universi/structure/versions.py
--rw-r--r--   0        0        0    11455 1970-01-01 00:00:00.000000 universi-0.4.0/setup.py
--rw-r--r--   0        0        0    11155 1970-01-01 00:00:00.000000 universi-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.5.0/LICENSE
+-rw-r--r--   0        0        0    10258 2023-07-15 21:13:24.073328 universi-0.5.0/README.md
+-rw-r--r--   0        0        0     4082 2023-07-15 21:13:30.916661 universi-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      453 2023-07-12 22:40:12.864421 universi-0.5.0/universi/__init__.py
+-rw-r--r--   0        0        0     2821 2023-07-14 12:35:15.746665 universi-0.5.0/universi/_utils.py
+-rw-r--r--   0        0        0    21553 2023-07-15 21:13:24.073328 universi-0.5.0/universi/codegen.py
+-rw-r--r--   0        0        0      324 2023-07-10 23:48:56.035792 universi-0.5.0/universi/exceptions.py
+-rw-r--r--   0        0        0     2841 2023-07-08 14:21:11.688092 universi-0.5.0/universi/fields.py
+-rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.5.0/universi/header.py
+-rw-r--r--   0        0        0        0 2023-07-13 08:09:29.390618 universi-0.5.0/universi/py.typed
+-rw-r--r--   0        0        0    12278 2023-07-14 12:35:15.899998 universi-0.5.0/universi/routing.py
+-rw-r--r--   0        0        0      376 2023-07-15 21:13:24.073328 universi-0.5.0/universi/structure/__init__.py
+-rw-r--r--   0        0        0      265 2023-07-08 11:43:06.913473 universi-0.5.0/universi/structure/common.py
+-rw-r--r--   0        0        0     4936 2023-07-10 10:22:38.358870 universi-0.5.0/universi/structure/endpoints.py
+-rw-r--r--   0        0        0      944 2023-07-08 11:43:06.913473 universi-0.5.0/universi/structure/enums.py
+-rw-r--r--   0        0        0     1270 2023-07-14 12:35:15.266665 universi-0.5.0/universi/structure/responses.py
+-rw-r--r--   0        0        0     5909 2023-07-15 21:13:24.073328 universi-0.5.0/universi/structure/schemas.py
+-rw-r--r--   0        0        0     8851 2023-07-15 21:13:24.073328 universi-0.5.0/universi/structure/versions.py
+-rw-r--r--   0        0        0    11197 1970-01-01 00:00:00.000000 universi-0.5.0/setup.py
+-rw-r--r--   0        0        0    10918 1970-01-01 00:00:00.000000 universi-0.5.0/PKG-INFO
```

### Comparing `universi-0.4.0/LICENSE` & `universi-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `universi-0.4.0/README.md` & `universi-0.5.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # universi
 
-Package description
+Modern Stripe-like API versioning
 
 ---
 
 <p align="center">
 <a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">
     <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">
 </a>
@@ -67,15 +67,15 @@
 async def create_user(payload: UserCreateRequest):
     return {
         "id": 83,
         "address": payload.address,
     }
 
 @router.get("/users/{user_id}", response_model=UserResource)
-async def get_user(user_id: UUID):
+async def get_user(user_id: int):
     return {
         "id": user_id,
         "address": "123 Example St",
     }
 ```
 
 ### Turning address into a list
@@ -84,27 +84,26 @@
 
 ```python
 from pydantic import BaseModel
 from universi import Field
 
 
 class UserCreateRequest(BaseModel):
-    id: int
-    addresses: str = Field(min_items=1)
+    addresses: list[str] = Field(min_items=1)
 
 class UserResource(BaseModel):
     id: int
-    addresses: str
+    addresses: list[str]
 ```
 
 ```python
 @router.post("/users", response_model=UserResource)
 async def create_user(payload: UserCreateRequest):
     return {
-        "id": uuid4(),
+        "id": int,
         "addresses": payload.addresses,
     }
 
 @router.get("/users/{user_id}", response_model=UserResource)
 async def get_user(user_id: int):
     return {
         "id": user_id,
@@ -120,66 +119,48 @@
 Universi is heavily inspired by this approach so let's continue our tutorial and now try to combine the two versions we created using versioning.
 
 ### Creating the Migration
 
 We need to create a migration to handle changes between these versions. This migration will convert the list of addresses back to a single address when migrating to the previous version. Yes, migrating **back**: you might be used to database migrations where we write upgrade migration and downgrade migration but here our goal is to have an app of latest version and to describe what older versions looked like in comparison to it. That way the old versions are frozen in migrations and you can **almost** safely forget about them.
 
 ```python
+from universi import Field
 from universi.structure import (
-    field,
     schema,
     AbstractVersionChange,
     convert_response_to_previous_version_for,
-    Field
 )
 
 class ChangeAddressToList(AbstractVersionChange):
     description = (
         "Change user address to a list of strings to "
         "allow the user to specify multiple addresses"
     )
     instructions_to_migrate_to_previous_version = (
-        schema(
-            UserCreateRequest,
-            field("addresses").didnt_exist,
-            field("address").existed_with(type=str, info=Field()),
-        ),
-        schema(
-            UserResource,
-            field("addresses").didnt_exist,
-            field("address").existed_with(type=str, info=Field()),
-        )
+        # You should use schema inheritance if you don't want to repeat yourself in such cases
+        schema(UserCreateRequest).field("addresses").didnt_exist,
+        schema(UserCreateRequest).field("address").existed_with(type=str, info=Field()),
+        schema(UserResource).field("addresses").didnt_exist,
+        schema(UserResource).field("address").existed_with(type=str, info=Field()),
     )
 
     @convert_response_to_previous_version_for(get_user, create_user)
     def change_addresses_to_single_item(cls, data: dict[str, Any]) -> None:
         data["address"] = data.pop("addresses")[0]
+    
+    @schema(UserCreateRequest).had_property("addresses")
+    def addresses_property(parsed_schema):
+        return [parsed_schema.address]
+
 ```
 
+s
 See how we are popping the first address from the list? This is only guaranteed to be possible because we specified earlier that `min_items` for `addresses` must be `1`. If we didn't, then the user would be able to create a user in a newer version that would be impossible to represent in the older version. I.e. If anyone tried to get that user from the older version, they would get a `ResponseValidationError` because the user wouldn't have data for a mandatory `address` field. You need to always keep in mind tht API versioning is only for versioning your **API**, your interface. Your versions must still be completely compatible in terms of data. If they are not, then you are versioning your data and you should really go with a separate app instance. Otherwise, your users will have a hard time migrating back and forth between API versions and so many unexpected errors.
 
-Now that we've made our migration, we are realizing that even though we are migrating data for our response so we don't need to worry about it in our business logic, our user creation function still cannot handle the old version: it will just break when it tries to get `addresses` from `UserCreateRequest` because the old version doesn't have it.
-
-### Accomodating changes in request schemas
-
-```python
-@router.post("/users", response_model=UserResource)
-async def create_user(payload: UserCreateRequest):s
-    if hasattr(payload, "addresses"):
-        addresses = payload.addresses
-    else:
-        addresses = [payload.address]
-    return {
-        "id": uuid4(),
-        "addresses": payload.addresses,
-    }
-
-```
-
-Now we just need to combine everything together and ask universi to generate for us the parts that we would copy-paste in traditional versioning.
+See how we added the `addresses` property? This simple instruction will allow us to use `addresses` even from the old schema, which means that our api route will not need to know anything about versioning. The main goal of universi is to shift the logic of versioning away from your business logic and api endpoints which makes your project easier to navigate and which makes deleting versions a breeze.
 
 ### Grouping Version Changes
 
 Finally, we group the version changes in the `Versions` class. This represents the different versions of your API and the changes between them. You can add any "version changes" to any version. For simplicity, let's use versions 2002 and 2001 which means that we had a single address in API in 2001 and added addresses as a list in 2002's version.
 
 ```python
 from universi.structure import Version, Versions
```

### Comparing `universi-0.4.0/pyproject.toml` & `universi-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "universi"
-version = "0.4.0"
+version = "0.5.0"
 description = ""
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ovsyanka83/universi"
 
 [tool.poetry.dependencies]
@@ -22,20 +22,21 @@
 httpx = ">=0.23.0"
 uvicorn = "*"
 devtools = "*"
 pdbpp = "^0.10.3"
 pytest-pretty = "^1.2.0"
 notebook = "^6.5.4"
 pytest-asyncio = "^0.21.0"
+dirty-equals = "^0.6.0"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.coverage.report]
-fail_under = 100
+fail_under = 99
 skip_covered = true
 skip_empty = true
 # Taken from https://coverage.readthedocs.io/en/7.1.0/excluding.html#advanced-exclusion
 exclude_lines = [
     "pragma: no cover",
     "assert_never\\(",
     "if self.debug:",
```

### Comparing `universi-0.4.0/universi/_utils.py` & `universi-0.5.0/universi/_utils.py`

 * *Files identical despite different names*

### Comparing `universi-0.4.0/universi/codegen.py` & `universi-0.5.0/universi/codegen.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 import ast
+from dataclasses import dataclass, field
 import importlib
 import inspect
 import os
 import shutil
 import sys
 from collections.abc import Generator, Sequence
 from copy import deepcopy
 from datetime import date
 from enum import Enum, auto
 from pathlib import Path
+import textwrap
 from types import GenericAlias, LambdaType, ModuleType
 from typing import (
     Any,
+    Callable,
     TypeAlias,
     _BaseGenericAlias,  # pyright: ignore[reportGeneralTypeIssues]
     get_args,
     get_origin,
 )
 
 from pydantic import BaseConfig, BaseModel
@@ -26,33 +29,42 @@
 
 from universi.structure.enums import (
     AlterEnumSubInstruction,
     EnumDidntHaveMembersInstruction,
     EnumHadMembersInstruction,
 )
 from universi.structure.schemas import (
-    AlterSchemaInstruction,
+    AlterSchemaSubInstruction,
     OldSchemaDidntHaveField,
     OldSchemaFieldWas,
     OldSchemaHadField,
+    SchemaPropertyDefinitionInstruction,
+    SchemaPropertyDidntExistInstruction,
 )
 from universi.structure.versions import Version, Versions
 
 from ._utils import Sentinel, get_index_of_base_schema_dir_in_pythonpath
 from .exceptions import CodeGenerationError, InvalidGenerationInstructionError
 from .fields import FieldInfo
 
-LambdaFunctionName = (lambda: None).__name__  # pragma: no branch
-FieldNameT: TypeAlias = str
-dict_of_empty_field_info = {k: getattr(PydanticFieldInfo(), k) for k in PydanticFieldInfo.__slots__}
+_LambdaFunctionName = (lambda: None).__name__  # pragma: no branch
+_FieldName: TypeAlias = str
+_PropertyName: TypeAlias = str
+_dict_of_empty_field_info = {k: getattr(PydanticFieldInfo(), k) for k in PydanticFieldInfo.__slots__}
+
+
+@dataclass(slots=True)
+class ModelInfo:
+    fields: dict[_FieldName, tuple[type[BaseModel], ModelField]]
+    properties: dict[_PropertyName, Callable[[Any], Any]] = field(default_factory=dict)
 
 
 # TODO: Add enum alteration here
 def regenerate_dir_to_all_versions(template_module: ModuleType, versions: Versions):
-    schemas = {k: (v, _get_fields_for_model(v)) for k, v in deepcopy(versions.versioned_schemas).items()}
+    schemas = {k: ModelInfo(_get_fields_for_model(v)) for k, v in deepcopy(versions.versioned_schemas).items()}
     enums = {k: (v, {member.name: member.value for member in v}) for k, v in deepcopy(versions.versioned_enums).items()}
 
     for version in versions.versions:
         # NOTE: You'll have to use relative imports
 
         _generate_versioned_directory(template_module, schemas, enums, version.date)
         _apply_migrations(version, schemas, enums)
@@ -67,51 +79,41 @@
 def _generate_union_directory(template_module: ModuleType, versions: Versions):
     template_dir = _get_package_path_from_module(template_module)
     union_dir = template_dir.with_name("unions")
     index_of_base_schema_in_pythonpath = get_index_of_base_schema_dir_in_pythonpath(
         template_module,
         union_dir,
     )
-    for (
-        relative_path_to_file,
-        original_module,
-        parallel_file,
-    ) in _generate_parallel_directory(
+    for _, original_module, parallel_file in _generate_parallel_directory(
         template_module,
         union_dir,
     ):
         new_module_text = _get_unionized_version_of_module(
             original_module,
-            relative_path_to_file,
             versions,
             index_of_base_schema_in_pythonpath,
         )
         parallel_file.write_text(new_module_text)
 
 
 def _get_unionized_version_of_module(
     original_module: ModuleType,
-    relative_path_to_file: Path,
     versions: Versions,
     index_of_base_schema_in_pythonpath: int,
 ):
     original_module_parts = original_module.__name__.split(".")
     original_module_parts[index_of_base_schema_in_pythonpath] = "{}"
 
     import_pythonpath_template = (".".join(original_module_parts)).removesuffix(".__init__")
     imported_modules = [
         import_pythonpath_template.format(_get_version_dir_name(version.date)) for version in versions.versions
     ]
 
     parsed_file = _parse_python_module(original_module)
 
-    if original_module.__name__.endswith(".__init__"):
-        module_name = original_module.__name__.removesuffix(".__init__")
-    else:
-        module_name = original_module.__name__
     body = ast.Module(
         [
             ast.ImportFrom(module="universi", names=[ast.alias(name="Field")], level=0),
             ast.Import(names=[ast.alias(name="typing")], level=0),
             *[ast.Import(names=[ast.Name(module)]) for module in imported_modules],
         ]
         + [
@@ -128,84 +130,93 @@
     return ast.unparse(body)
 
 
 def _apply_migrations(
     version: Version,
     schemas: dict[
         str,
-        tuple[type[BaseModel], dict[FieldNameT, tuple[type[BaseModel], ModelField]]],
+        ModelInfo,
     ],
     enums: dict[str, tuple[type[Enum], dict[str, Any]]],
 ):
     for version_change in version.version_changes:
         _apply_alter_schema_instructions(
             schemas,
             version_change.alter_schema_instructions,
         )
         _apply_alter_enum_instructions(enums, version_change.alter_enum_instructions)
 
 
 def _apply_alter_schema_instructions(
-    schemas: dict[
-        str,
-        tuple[type[BaseModel], dict[FieldNameT, tuple[type[BaseModel], ModelField]]],
-    ],
-    alter_schema_instructions: Sequence[AlterSchemaInstruction],
+    schema_infos: dict[str, ModelInfo],
+    alter_schema_instructions: Sequence[AlterSchemaSubInstruction],
 ):
     for alter_schema_instruction in alter_schema_instructions:
         schema = alter_schema_instruction.schema
         schema_path = schema.__module__ + schema.__name__
-        schema_field_info_bundle = schemas[schema_path]
-        field_name_to_field_model = schema_field_info_bundle[1]
-        for field_change in alter_schema_instruction.changes:
-            if isinstance(field_change, OldSchemaDidntHaveField):
-                # TODO: Check that the user doesn't pop it and change it at the same time
-                # TODO: Add a check that field actually exists (it's very necessary!)
-                field_name_to_field_model.pop(field_change.field_name)
-
-            elif isinstance(field_change, OldSchemaFieldWas):
-                # TODO: Add a check that field actually exists (it's very necessary!)
-                model_field = field_name_to_field_model[field_change.field_name][1]
-                if field_change.type is not Sentinel:
-                    if model_field.annotation == field_change.type:
-                        raise InvalidGenerationInstructionError(
-                            f"You tried to change the type of field '{field_change.field_name}' to '{field_change.type}' in {schema.__name__} but it already has type '{model_field.annotation}'",
-                        )
-                    model_field.annotation = field_change.type
-                    model_field.type_ = convert_generics(field_change.type)
-                    model_field.outer_type_ = field_change.type
-                field_info = model_field.field_info
-
-                if not isinstance(field_info, FieldInfo):
-                    dict_of_field_info = {k: getattr(field_info, k) for k in field_info.__slots__}
-                    if dict_of_field_info == dict_of_empty_field_info:
-                        field_info = FieldInfo()
-                        model_field.field_info = field_info
-                    else:
-                        raise InvalidGenerationInstructionError(
-                            f"You have defined a Field using pydantic.fields.Field but you must use universi.Field in {schema.__name__}",
-                        )
-                for attr_name in field_change.field_changes.__dataclass_fields__:
-                    attr_value = getattr(field_change.field_changes, attr_name)
-                    if attr_value is not Sentinel:
-                        setattr(field_info, attr_name, attr_value)
-                        field_info._universi_field_names.add(attr_name)
-            elif isinstance(field_change, OldSchemaHadField):
-                field_name_to_field_model[field_change.field_name] = (
-                    schema,
-                    ModelField(
-                        name=field_change.field_name,
-                        type_=field_change.type,
-                        field_info=field_change.field,
-                        class_validators=None,
-                        model_config=BaseConfig,
-                    ),
+        field_name_to_field_model = schema_infos[schema_path].fields
+        if isinstance(alter_schema_instruction, OldSchemaDidntHaveField):
+            # TODO: Check that the user doesn't pop it and change it at the same time
+            # TODO: Add a check that field actually exists (it's necessary!)
+            field_name_to_field_model.pop(alter_schema_instruction.field_name)
+
+        elif isinstance(alter_schema_instruction, OldSchemaFieldWas):
+            # TODO: Add a check that field actually exists (it's necessary!)
+            model_field = field_name_to_field_model[alter_schema_instruction.field_name][1]
+            if alter_schema_instruction.type is not Sentinel:
+                if model_field.annotation == alter_schema_instruction.type:
+                    raise InvalidGenerationInstructionError(
+                        f"You tried to change the type of field '{alter_schema_instruction.field_name}' to '{alter_schema_instruction.type}' in {schema.__name__} but it already has type '{model_field.annotation}'",
+                    )
+                model_field.annotation = alter_schema_instruction.type
+                model_field.type_ = convert_generics(alter_schema_instruction.type)
+                model_field.outer_type_ = alter_schema_instruction.type
+            field_info = model_field.field_info
+
+            if not isinstance(field_info, FieldInfo):
+                dict_of_field_info = {k: getattr(field_info, k) for k in field_info.__slots__}
+                if dict_of_field_info == _dict_of_empty_field_info:
+                    field_info = FieldInfo()
+                    model_field.field_info = field_info
+                else:
+                    raise InvalidGenerationInstructionError(
+                        f"You have defined a Field using pydantic.fields.Field but you must use universi.Field in {schema.__name__}",
+                    )
+            for attr_name in alter_schema_instruction.field_changes.__dataclass_fields__:
+                attr_value = getattr(alter_schema_instruction.field_changes, attr_name)
+                if attr_value is not Sentinel:
+                    setattr(field_info, attr_name, attr_value)
+                    field_info._universi_field_names.add(attr_name)
+        elif isinstance(alter_schema_instruction, OldSchemaHadField):
+            field_name_to_field_model[alter_schema_instruction.field_name] = (
+                schema,
+                ModelField(
+                    name=alter_schema_instruction.field_name,
+                    type_=alter_schema_instruction.type,
+                    field_info=alter_schema_instruction.field,
+                    class_validators=None,
+                    model_config=BaseConfig,
+                ),
+            )
+        elif isinstance(alter_schema_instruction, SchemaPropertyDefinitionInstruction):
+            if alter_schema_instruction.name in field_name_to_field_model:
+                raise InvalidGenerationInstructionError(
+                    f"You tried to define a property '{alter_schema_instruction.name}' in '{schema.__name__}' "
+                    "but there is already a field with that name."
                 )
-            else:
-                assert_never(field_change)
+            schema_infos[schema_path].properties[alter_schema_instruction.name] = alter_schema_instruction.function
+        elif isinstance(alter_schema_instruction, SchemaPropertyDidntExistInstruction):
+            if alter_schema_instruction.name not in schema_infos[schema_path].properties:
+                raise InvalidGenerationInstructionError(
+                    f"You tried to delete a property '{alter_schema_instruction.name}' in '{schema.__name__}' "
+                    "but there is no such property defined in any of the migrations."
+                )
+            schema_infos[schema_path].properties.pop(alter_schema_instruction.name)
+        else:
+            assert_never(alter_schema_instruction)
 
 
 def _apply_alter_enum_instructions(
     enums: dict[str, tuple[type[Enum], dict[str, Any]]],
     alter_enum_instructions: Sequence[AlterEnumSubInstruction],
 ):
     for alter_enum_instruction in alter_enum_instructions:
@@ -250,18 +261,15 @@
     if not file.name == "__init__.py":
         raise CodeGenerationError(f"Module {template_module} is not a package")
     return file.parent
 
 
 def _generate_versioned_directory(
     template_module: ModuleType,
-    schemas: dict[
-        str,
-        tuple[type[BaseModel], dict[FieldNameT, tuple[type[BaseModel], ModelField]]],
-    ],
+    schemas: dict[str, ModelInfo],
     enums: dict[str, tuple[type[Enum], dict[str, Any]]],
     version: date,
 ):
     version_dir = _get_version_dir_path(template_module, version)
     for (
         _relative_path_to_file,
         original_module,
@@ -313,16 +321,16 @@
                 yield original_subroot.relative_to(dir), original_module, parallel_file
             else:
                 shutil.copyfile(original_file, parallel_file)
 
 
 def _get_fields_for_model(
     model: type[BaseModel],
-) -> dict[FieldNameT, tuple[type[BaseModel], ModelField]]:
-    actual_fields: dict[FieldNameT, tuple[type[BaseModel], ModelField]] = {}
+) -> dict[_FieldName, tuple[type[BaseModel], ModelField]]:
+    actual_fields: dict[_FieldName, tuple[type[BaseModel], ModelField]] = {}
     for cls in model.__mro__:
         if cls is BaseModel:
             return actual_fields
         if not issubclass(cls, BaseModel):
             continue
         for field_name, field in cls.__fields__.items():
             if field_name not in actual_fields and field_name in cls.__annotations__:
@@ -343,29 +351,28 @@
             return ast.Module([])
         # Not sure how to get here so this is just a precaution
         raise CodeGenerationError("Failed to get source code for module") from e  # pragma: no cover
 
 
 def _migrate_module_to_another_version(
     module,
-    modified_schemas: dict[
-        str,
-        tuple[type[BaseModel], dict[str, tuple[type[BaseModel], ModelField]]],
-    ],
+    modified_schemas: dict[str, ModelInfo],
     modified_enums: dict[str, tuple[type[Enum], dict[str, Any]]],
 ) -> str:
     parsed_file = _parse_python_module(module)
     if module.__name__.endswith(".__init__"):
         module_name = module.__name__.removesuffix(".__init__")
     else:
         module_name = module.__name__
+
     body = ast.Module(
         [
             ast.ImportFrom(module="universi", names=[ast.alias(name="Field")], level=0),
             ast.Import(names=[ast.alias(name="typing")], level=0),
+            ast.ImportFrom(module="typing", names=[ast.alias(name="Any")], level=0),
         ]
         + [
             _migrate_cls_to_another_version(
                 n,
                 module_name,
                 modified_schemas,
                 modified_enums,
@@ -379,73 +386,81 @@
 
     return ast.unparse(body)
 
 
 def _migrate_cls_to_another_version(
     cls_node: ast.ClassDef,
     module_python_path: str,
-    modified_schemas: dict[
-        str,
-        tuple[type[BaseModel], dict[str, tuple[type[BaseModel], ModelField]]],
-    ],
+    modified_schemas: dict[str, ModelInfo],
     modified_enums: dict[str, tuple[type[Enum], dict[str, Any]]],
 ) -> ast.ClassDef:
     cls_python_path = module_python_path + cls_node.name
     if cls_python_path in modified_schemas:
-        cls_node = _modify_schema_cls(cls_node, modified_schemas[cls_python_path][1])
+        cls_node = _modify_schema_cls(cls_node, modified_schemas[cls_python_path])
     if cls_python_path in modified_enums:
         cls_node = _modify_enum_cls(cls_node, modified_enums[cls_python_path][1])
 
     if not cls_node.body:
         cls_node.body = [ast.Pass()]
     return cls_node
 
 
 def _modify_schema_cls(
     cls_node: ast.ClassDef,
-    actual_fields: dict[str, tuple[type[BaseModel], ModelField]],
+    model_info: ModelInfo,
 ) -> ast.ClassDef:
-    body = [
+    field_definitions = [
         ast.AnnAssign(
-            target=ast.Name(id=name, ctx=ast.Store()),
-            annotation=ast.Name(id=custom_repr(field[1].annotation), ctx=ast.Load()),
+            target=ast.Name(name, ctx=ast.Store()),
+            annotation=ast.Name(custom_repr(field[1].annotation)),
             value=ast.Call(
-                func=ast.Name(id="Field", ctx=ast.Load()),
+                func=ast.Name("Field"),
                 args=[],
                 keywords=[
                     ast.keyword(
                         arg=attr,
-                        value=ast.Name(
-                            id=custom_repr(getattr(field[1].field_info, attr)),
-                        ),
+                        value=ast.Name(custom_repr(getattr(field[1].field_info, attr))),
                     )
                     # TODO: We should lint the code to make sure that the user is not using pydantic.fields.Field instead of universi.Field
                     for attr in getattr(
                         field[1].field_info,
                         "_universi_field_names",
                         (),
                     )
                 ],
             ),
             simple=1,
         )
-        for name, field in actual_fields.items()
+        for name, field in model_info.fields.items()
     ]
+    property_definitions = [_make_property_ast(name, func) for name, func in model_info.properties.items()]
     old_body = [n for n in cls_node.body if not isinstance(n, ast.AnnAssign | ast.Pass | ast.Ellipsis)]
     docstring = _pop_docstring_from_cls_body(old_body)
-    cls_node.body = docstring + body + old_body
+    cls_node.body = docstring + field_definitions + old_body + property_definitions
 
     return cls_node
 
 
+# TODO: Type hint these func definitions everywhere
+def _make_property_ast(name: str, func: Callable):
+    func_source = inspect.getsource(func)
+
+    func_ast = ast.parse(textwrap.dedent(func_source)).body[0]
+    # TODO: What if it's a lambda?
+    assert isinstance(func_ast, ast.FunctionDef)
+    func_ast.decorator_list = [ast.Name("property")]
+    func_ast.name = name
+    return func_ast
+
+
 def _modify_enum_cls(cls_node: ast.ClassDef, enum_info: dict[str, Any]) -> ast.ClassDef:
     new_body = [
         ast.Assign(
-            targets=[ast.Name(id=member, ctx=ast.Store())],
-            value=ast.Name(id=custom_repr(member_value)),
+            targets=[ast.Name(member, ctx=ast.Store())],
+            value=ast.Name(custom_repr(member_value)),
             lineno=0,
         )
         for member, member_value in enum_info.items()
     ]
 
     old_body = [n for n in cls_node.body if not isinstance(n, ast.AnnAssign | ast.Assign | ast.Pass | ast.Ellipsis)]
     docstring = _pop_docstring_from_cls_body(old_body)
@@ -475,20 +490,25 @@
     if isinstance(value, dict):
         return PlainRepr(
             value.__class__((custom_repr(k), custom_repr(v)) for k, v in value.items()),
         )
     if isinstance(value, _BaseGenericAlias | GenericAlias):
         return f"{custom_repr(get_origin(value))}[{', '.join(custom_repr(a) for a in get_args(value))}]"
     if isinstance(value, type):
+        # TODO: Add tests for constrained types
+        # TODO: Be wary of this hack when migrating to pydantic v2
+        # This is a hack for pydantic's Constrained types
+        if value.__name__.startswith("Constrained") and hasattr(value, "__origin__") and hasattr(value, "__args__"):
+            return custom_repr(value.__origin__[value.__args__])
         return value.__name__
     if isinstance(value, Enum):
         return PlainRepr(f"{value.__class__.__name__}.{value.name}")
     if isinstance(value, auto):
         return PlainRepr("auto()")
-    if isinstance(value, LambdaType) and LambdaFunctionName == value.__name__:
+    if isinstance(value, LambdaType) and _LambdaFunctionName == value.__name__:
         return _find_a_lambda(inspect.getsource(value).strip())
     if inspect.isfunction(value):
         return PlainRepr(value.__name__)
     else:
         return PlainRepr(repr(value))
```

### Comparing `universi-0.4.0/universi/fields.py` & `universi-0.5.0/universi/fields.py`

 * *Files identical despite different names*

### Comparing `universi-0.4.0/universi/header.py` & `universi-0.5.0/universi/header.py`

 * *Files identical despite different names*

### Comparing `universi-0.4.0/universi/routing.py` & `universi-0.5.0/universi/routing.py`

 * *Files identical despite different names*

### Comparing `universi-0.4.0/universi/structure/endpoints.py` & `universi-0.5.0/universi/structure/endpoints.py`

 * *Files identical despite different names*

### Comparing `universi-0.4.0/universi/structure/enums.py` & `universi-0.5.0/universi/structure/enums.py`

 * *Files identical despite different names*

### Comparing `universi-0.4.0/universi/structure/responses.py` & `universi-0.5.0/universi/structure/responses.py`

 * *Files identical despite different names*

### Comparing `universi-0.4.0/universi/structure/schemas.py` & `universi-0.5.0/universi/structure/schemas.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from collections.abc import Callable, Sequence
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any
+import functools
+from typing import TYPE_CHECKING, Any, Generic, ParamSpec, TypeAlias, TypeVar, cast
 
 from pydantic import BaseModel
 
 from universi.fields import FieldInfo
 
 from .._utils import Sentinel
 
 if TYPE_CHECKING:
     from pydantic.typing import AbstractSetIntStr, MappingIntStrAny
 
+_SchemaInstance = TypeVar("_SchemaInstance", bound=Any)
+_R = TypeVar("_R")
+_P = ParamSpec("_P")
+
 
 @dataclass
 class FieldChanges:
     default: Any
     default_factory: Any
     alias: str
     title: str
@@ -39,33 +44,37 @@
     regex: str
     discriminator: str
     repr: bool
 
 
 @dataclass
 class OldSchemaFieldWas:
+    schema: type[BaseModel]
     field_name: str
     type: type
     field_changes: FieldChanges
 
 
 @dataclass
 class OldSchemaDidntHaveField:
+    schema: type[BaseModel]
     field_name: str
 
 
 @dataclass
 class OldSchemaHadField:
+    schema: type[BaseModel]
     field_name: str
     type: type
     field: FieldInfo
 
 
 @dataclass(slots=True)
-class AlterSchemaSubInstructionFactory:
+class AlterFieldInstructionFactory:
+    schema: type[BaseModel]
     name: str
     # TODO: Add a validation  to check that field actually changed
 
     def had(
         self,
         *,
         type: Any = Sentinel,
@@ -92,14 +101,15 @@
         max_length: int = Sentinel,
         allow_mutation: bool = Sentinel,
         regex: str = Sentinel,
         discriminator: str = Sentinel,
         repr: bool = Sentinel,
     ) -> OldSchemaFieldWas:
         return OldSchemaFieldWas(
+            schema=self.schema,
             field_name=self.name,
             type=type,
             field_changes=FieldChanges(
                 default=default,
                 default_factory=default_factory,
                 alias=alias,
                 title=title,
@@ -125,34 +135,73 @@
                 discriminator=discriminator,
                 repr=repr,
             ),
         )
 
     @property
     def didnt_exist(self) -> OldSchemaDidntHaveField:
-        return OldSchemaDidntHaveField(field_name=self.name)
+        return OldSchemaDidntHaveField(self.schema, field_name=self.name)
 
     def existed_with(self, *, type: type, info: FieldInfo) -> OldSchemaHadField:
-        return OldSchemaHadField(field_name=self.name, type=type, field=info)
+        return OldSchemaHadField(self.schema, field_name=self.name, type=type, field=info)
+
+
+@dataclass(slots=True)
+class SchemaPropertyDidntExistInstruction:
+    schema: type[BaseModel]
+    name: str
+
+
+# TODO: Validate that the function has the correct definition
+@dataclass
+class SchemaPropertyDefinitionInstruction:
+    schema: type[BaseModel]
+    name: str
+    function: Callable
+
+    # TODO: Only allow one argument and disallow type hints on it to make sure that the type checker
+    # is making sure that the produced properties are valid.
+    def __post_init__(self):
+        functools.update_wrapper(self, self.function)
+
+    def __call__(self, __parsed_schema: BaseModel):
+        return self.function(__parsed_schema)
+
+
+@dataclass(slots=True)
+class AlterPropertyInstructionFactory:
+    schema: type[BaseModel]
+    name: str
 
+    def __call__(self, function: Callable) -> SchemaPropertyDefinitionInstruction:
+        return SchemaPropertyDefinitionInstruction(self.schema, self.name, function)
 
-def field(name: str, /) -> AlterSchemaSubInstructionFactory:
-    return AlterSchemaSubInstructionFactory(name=name)
+    @property
+    def didnt_exist(self) -> SchemaPropertyDidntExistInstruction:
+        return SchemaPropertyDidntExistInstruction(self.schema, self.name)
 
 
 AlterSchemaSubInstruction = (
-    OldSchemaFieldWas | OldSchemaDidntHaveField | OldSchemaHadField
+    OldSchemaFieldWas
+    | OldSchemaDidntHaveField
+    | OldSchemaHadField
+    | SchemaPropertyDidntExistInstruction
+    | SchemaPropertyDefinitionInstruction
 )
 
 
 @dataclass
-class AlterSchemaInstruction:
+class AlterSchemaSubInstructionFactory:
     schema: type[BaseModel]
-    changes: Sequence[AlterSchemaSubInstruction]
+
+    def field(self, name: str, /) -> AlterFieldInstructionFactory:
+        return AlterFieldInstructionFactory(self.schema, name)
+
+    def had_property(self, name: str, /) -> type[staticmethod]:
+        return cast(type[staticmethod], AlterPropertyInstructionFactory(self.schema, name))
+
+    def property(self, name: str, /) -> AlterPropertyInstructionFactory:
+        return AlterPropertyInstructionFactory(self.schema, name)
 
 
-def schema(
-    model: type[BaseModel],
-    /,
-    *changes: AlterSchemaSubInstruction,
-) -> AlterSchemaInstruction:
-    return AlterSchemaInstruction(schema=model, changes=changes)
+def schema(model: type[BaseModel], /) -> AlterSchemaSubInstructionFactory:
+    return AlterSchemaSubInstructionFactory(model)
```

### Comparing `universi-0.4.0/universi/structure/versions.py` & `universi-0.5.0/universi/structure/versions.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,38 +11,30 @@
 from universi.header import api_version_var
 from universi.structure.endpoints import AlterEndpointSubInstruction
 from universi.structure.enums import AlterEnumSubInstruction
 
 from .._utils import Sentinel
 from .common import Endpoint, VersionedModel
 from .responses import AlterResponseInstruction
-from .schemas import AlterSchemaInstruction
+from .schemas import AlterSchemaSubInstruction, SchemaPropertyDefinitionInstruction
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 VersionDate: TypeAlias = datetime.date
-PossibleInstructions: TypeAlias = (
-    AlterSchemaInstruction | AlterEndpointSubInstruction | AlterEnumSubInstruction
-)
+PossibleInstructions: TypeAlias = AlterSchemaSubInstruction | AlterEndpointSubInstruction | AlterEnumSubInstruction
 
 
 class AbstractVersionChange:
     side_effects: ClassVar[bool] = False
     description: ClassVar[str] = Sentinel
-    instructions_to_migrate_to_previous_version: ClassVar[
-        Sequence[PossibleInstructions]
-    ] = Sentinel
-    alter_schema_instructions: ClassVar[Sequence[AlterSchemaInstruction]] = Sentinel
+    instructions_to_migrate_to_previous_version: ClassVar[Sequence[PossibleInstructions]] = Sentinel
+    alter_schema_instructions: ClassVar[Sequence[AlterSchemaSubInstruction]] = Sentinel
     alter_enum_instructions: ClassVar[Sequence[AlterEnumSubInstruction]] = Sentinel
-    alter_endpoint_instructions: ClassVar[
-        Sequence[AlterEndpointSubInstruction]
-    ] = Sentinel
-    alter_response_instructions: ClassVar[
-        dict[Endpoint, AlterResponseInstruction]
-    ] = Sentinel
+    alter_endpoint_instructions: ClassVar[Sequence[AlterEndpointSubInstruction]] = Sentinel
+    alter_response_instructions: ClassVar[dict[Endpoint, AlterResponseInstruction]] = Sentinel
 
     def __init_subclass__(cls) -> None:
         if not isinstance(cls.side_effects, bool):
             raise UniversiStructureError(
                 f"Side effects must be bool. Found: {type(cls.side_effects)}",
             )
         if cls.description is Sentinel:
@@ -61,50 +53,46 @@
             if not isinstance(instruction, PossibleInstructions):
                 raise UniversiStructureError(
                     f"Instruction '{instruction}' is not allowed. Please, use the correct instruction types",
                 )
         for attr_name, attr_value in cls.__dict__.items():
             if not isinstance(
                 attr_value,
-                AlterResponseInstruction,
+                (AlterResponseInstruction, SchemaPropertyDefinitionInstruction),
             ) and attr_name not in {
                 "description",
                 "side_effects",
                 "instructions_to_migrate_to_previous_version",
                 "__module__",
                 "__doc__",
             }:
                 raise UniversiStructureError(
-                    f"Found: '{attr_name}' attribute in {cls.__name__}. Only migration instructions are allowed in version change classes.",
+                    f"Found: '{attr_name}' attribute of type '{type(attr_value)}' in '{cls.__name__}'. Only migration instructions and schema properties are allowed in version change class body.",
                 )
 
         cls.alter_schema_instructions = []
         cls.alter_enum_instructions = []
         cls.alter_endpoint_instructions = []
         for alter_instruction in cls.instructions_to_migrate_to_previous_version:
-            if isinstance(alter_instruction, AlterSchemaInstruction):
+            if isinstance(alter_instruction, AlterSchemaSubInstruction):
                 cls.alter_schema_instructions.append(alter_instruction)
             elif isinstance(alter_instruction, AlterEnumSubInstruction):
                 cls.alter_enum_instructions.append(alter_instruction)
-            else:
+            elif isinstance(alter_instruction, AlterEndpointSubInstruction):
                 cls.alter_endpoint_instructions.append(alter_instruction)
+        for value in cls.__dict__.values():
+            if isinstance(value, SchemaPropertyDefinitionInstruction):
+                cls.alter_schema_instructions.append(value)
+        # TODO: You can include it in a for loop over dict above. Do so
         cls.alter_response_instructions = {
             endpoint: instruction
             for instruction in cls.__dict__.values()
             if isinstance(instruction, AlterResponseInstruction)
             for endpoint in instruction.endpoints
         }
-        repetitions = set()
-        for alter_instruction in cls.alter_schema_instructions:
-            if alter_instruction.schema in repetitions:
-                raise UniversiStructureError(
-                    f"'{alter_instruction.schema.__name__}' got repeated in multiple instructions. "
-                    "Please, merge these instructions.",
-                )
-            repetitions.add(alter_instruction.schema)
 
         if cls.mro() != [cls, AbstractVersionChange, object]:
             raise TypeError(
                 f"Can't subclass {cls.__name__} as it was never meant to be subclassed.",
             )
 
     def __init__(self) -> None:
@@ -135,16 +123,15 @@
             raise ValueError(
                 "Versions are not sorted correctly. Please sort them in descending order.",
             )
 
     @functools.cached_property
     def versioned_schemas(self) -> dict[str, type[VersionedModel]]:
         return {
-            instruction.schema.__module__
-            + instruction.schema.__name__: instruction.schema
+            instruction.schema.__module__ + instruction.schema.__name__: instruction.schema
             for version in self.versions
             for version_change in version.version_changes
             for instruction in version_change.alter_schema_instructions
         }
 
     @functools.cached_property
     def versioned_enums(self) -> dict[str, type[Enum]]:
@@ -155,19 +142,15 @@
             for instruction in version_change.alter_enum_instructions
         }
 
     @functools.cached_property
     def _version_changes_to_version_mapping(
         self,
     ) -> dict[type[AbstractVersionChange], VersionDate]:
-        return {
-            version_change: version.date
-            for version in self.versions
-            for version_change in version.version_changes
-        }
+        return {version_change: version.date for version in self.versions for version_change in version.version_changes}
 
     def is_active(self, version_change: type[AbstractVersionChange]) -> bool:
         api_version = self.api_version_var.get()
         if api_version is None:
             return True
         return self._version_changes_to_version_mapping[version_change] <= api_version
```

### Comparing `universi-0.4.0/setup.py` & `universi-0.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 ['fastapi>=0.96.1',
  'type-inspector>=1.2.2,<2.0.0',
  'typer[all]',
  'typing-extensions']
 
 setup_kwargs = {
     'name': 'universi',
-    'version': '0.4.0',
+    'version': '0.5.0',
     'description': '',
-    'long_description': '# universi\n\nPackage description\n\n---\n\n<p align="center">\n<a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://codecov.io/gh/ovsyanka83/universi" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/universi?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/universi?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/universi?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Installation\n\n```bash\npip install universi\n```\n\n<!---\n# TODO: Note that we don\'t handle "from .schemas import Schema as OtherSchema" case\n# TODO: Need to validate that the user doesn\'t use versioned schemas instead of the latest ones\n-->\n\n## Tutorial\n\nThis guide provides a step-by-step tutorial for setting up automatic API versioning using Universi library. I will illustrate this with an example of a User API, where we will be implementing changes to a User\'s address.\n\n### A dummy setup\n\nHere is an initial API setup where the User has a single address. We will be implementing two routes - one for creating a user and another for retrieving user details. We\'ll be using "int" for ID for simplicity.\n\nThe first API you come up with usually doesn\'t require more than one address -- why bother?\n\nSo we create our file with schemas:\n\n```python\nfrom pydantic import BaseModel\n\n\nclass UserCreateRequest(BaseModel):\n    id: int\n    address: str\n\nclass UserResource(BaseModel):\n    id: int\n    address: str\n```\n\nAnd we create our file with routes:\n\n```python\nfrom versions.latest.users import UserCreateRequest, UserResource\nfrom universi import VersionedAPIRouter\n\nrouter = VersionedAPIRouter()\n\n@router.post("/users", response_model=UserResource)\nasync def create_user(payload: UserCreateRequest):\n    return {\n        "id": 83,\n        "address": payload.address,\n    }\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def get_user(user_id: UUID):\n    return {\n        "id": user_id,\n        "address": "123 Example St",\n    }\n```\n\n### Turning address into a list\n\nDuring our development, we have realized that the initial API design was wrong and that addresses should have always been a list because the user wants to have multiple addresses to choose from so now we have to change the type of the "address" field to the list of strings.\n\n```python\nfrom pydantic import BaseModel\nfrom universi import Field\n\n\nclass UserCreateRequest(BaseModel):\n    id: int\n    addresses: str = Field(min_items=1)\n\nclass UserResource(BaseModel):\n    id: int\n    addresses: str\n```\n\n```python\n@router.post("/users", response_model=UserResource)\nasync def create_user(payload: UserCreateRequest):\n    return {\n        "id": uuid4(),\n        "addresses": payload.addresses,\n    }\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def get_user(user_id: int):\n    return {\n        "id": user_id,\n        "addresses": ["123 Example St", "456 Main St"],\n    }\n\n```\n\nBut every user of ours will now have their API integration broken. To prevent that, we have to introduce API versioning. There aren\'t many methods of doing that. Most of them force you to either duplicate your schemas, your endpoints, or your entire app instance. And it makes sense, really: duplication is the only way to make sure that you will not break old versions with your new versions; the bigger the piece you duplicating -- the safer. Of course, the safest being duplicating the entire app instance and even having a separate database. But that is expensive and makes it either impossible to make breaking changes often or to support many versions. As a result, either you need infinite resources, very long development cycles, or your users will need to often migrate from version to version.\n\nStripe has come up [with a solution](https://stripe.com/blog/api-versioning): let\'s have one latest app version whose responses get migrated to older versions and let\'s describe changes between these versions using migrations. This approach allows them to keep versions for **years** without dropping them. Obviously, each breaking change is still bad and each version still makes our system more complex and expensive, but their approach gives us a chance to minimize that. Additionally, it allows us backport features and bugfixes to older versions. However, you will also be backporting bugs, which is a sad consequence of eliminating duplication.\n\nUniversi is heavily inspired by this approach so let\'s continue our tutorial and now try to combine the two versions we created using versioning.\n\n### Creating the Migration\n\nWe need to create a migration to handle changes between these versions. This migration will convert the list of addresses back to a single address when migrating to the previous version. Yes, migrating **back**: you might be used to database migrations where we write upgrade migration and downgrade migration but here our goal is to have an app of latest version and to describe what older versions looked like in comparison to it. That way the old versions are frozen in migrations and you can **almost** safely forget about them.\n\n```python\nfrom universi.structure import (\n    field,\n    schema,\n    AbstractVersionChange,\n    convert_response_to_previous_version_for,\n    Field\n)\n\nclass ChangeAddressToList(AbstractVersionChange):\n    description = (\n        "Change user address to a list of strings to "\n        "allow the user to specify multiple addresses"\n    )\n    instructions_to_migrate_to_previous_version = (\n        schema(\n            UserCreateRequest,\n            field("addresses").didnt_exist,\n            field("address").existed_with(type=str, info=Field()),\n        ),\n        schema(\n            UserResource,\n            field("addresses").didnt_exist,\n            field("address").existed_with(type=str, info=Field()),\n        )\n    )\n\n    @convert_response_to_previous_version_for(get_user, create_user)\n    def change_addresses_to_single_item(cls, data: dict[str, Any]) -> None:\n        data["address"] = data.pop("addresses")[0]\n```\n\nSee how we are popping the first address from the list? This is only guaranteed to be possible because we specified earlier that `min_items` for `addresses` must be `1`. If we didn\'t, then the user would be able to create a user in a newer version that would be impossible to represent in the older version. I.e. If anyone tried to get that user from the older version, they would get a `ResponseValidationError` because the user wouldn\'t have data for a mandatory `address` field. You need to always keep in mind tht API versioning is only for versioning your **API**, your interface. Your versions must still be completely compatible in terms of data. If they are not, then you are versioning your data and you should really go with a separate app instance. Otherwise, your users will have a hard time migrating back and forth between API versions and so many unexpected errors.\n\nNow that we\'ve made our migration, we are realizing that even though we are migrating data for our response so we don\'t need to worry about it in our business logic, our user creation function still cannot handle the old version: it will just break when it tries to get `addresses` from `UserCreateRequest` because the old version doesn\'t have it.\n\n### Accomodating changes in request schemas\n\n```python\n@router.post("/users", response_model=UserResource)\nasync def create_user(payload: UserCreateRequest):s\n    if hasattr(payload, "addresses"):\n        addresses = payload.addresses\n    else:\n        addresses = [payload.address]\n    return {\n        "id": uuid4(),\n        "addresses": payload.addresses,\n    }\n\n```\n\nNow we just need to combine everything together and ask universi to generate for us the parts that we would copy-paste in traditional versioning.\n\n### Grouping Version Changes\n\nFinally, we group the version changes in the `Versions` class. This represents the different versions of your API and the changes between them. You can add any "version changes" to any version. For simplicity, let\'s use versions 2002 and 2001 which means that we had a single address in API in 2001 and added addresses as a list in 2002\'s version.\n\n```python\nfrom universi.structure import Version, Versions\nfrom datetime import date\n\nversions = Versions(\n    Version(date(2002, 1, 1), ChangeAddressToList),\n    Version(date(2001, 1, 1)),\n)\n```\n\nThat\'s it. You\'re done with describing things. Now you just gotta ask universi to do the rest for you. We\'ll need the VersionedAPIRouter we used previously, our API versions, and the module representing the latest versions of our schemas.\n\n```python\nfrom versions import latest\nfrom universi import regenerate_dir_to_all_versions, api_version_var\n\nregenerate_dir_to_all_versions(latest, versions)\nrouter_versions = router.create_versioned_copies(\n    versions,\n    latest_schemas_module=latest,\n)\napi_version_var.set(date(2002, 1, 1))\nuvicorn.run(router_versions[date(2002, 1, 1)])\n```\n\nUniversi has generated multiple things in this code:\n\n* Three versions of our schemas: one for each API version and one that includes definitions of unions of all versions for each schema which will be useful when you want to type check that you are using requests of different versions correctly. For example, we\'ll have `UserCreateRequestUnion` defined there which is a `TypeAlias` pointing to the union of 2002 version and 2001 version of `UserCreateRequest`.\n* Two versions of our API router: one for each API version\n\nYou can now just pick a router by its version and run it separately or use a parent router/app to specify the logic by which you\'d like to pick a version. I recommend using a header-based router with version dates as headers. And yes, that\'s how Stripe does it.\n\nNote that universi migrates your response data based on the api_version_var context variable so you must set it with each request. `universi.header` has a dependency that does that for you.\n\nObviously, this was just a simple example and universi has a lot more features so if you\'re interested -- take a look at the reference\n\n## Reference\n\nTBD\n',
+    'long_description': '# universi\n\nModern Stripe-like API versioning\n\n---\n\n<p align="center">\n<a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">\n    <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">\n</a>\n<a href="https://codecov.io/gh/ovsyanka83/universi" target="_blank">\n    <img src="https://img.shields.io/codecov/c/github/ovsyanka83/universi?color=%2334D058" alt="Coverage">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img alt="PyPI" src="https://img.shields.io/pypi/v/universi?color=%2334D058&label=pypi%20package" alt="Package version">\n</a>\n<a href="https://pypi.org/project/universi/" target="_blank">\n    <img src="https://img.shields.io/pypi/pyversions/universi?color=%2334D058" alt="Supported Python versions">\n</a>\n</p>\n\n## Installation\n\n```bash\npip install universi\n```\n\n<!---\n# TODO: Note that we don\'t handle "from .schemas import Schema as OtherSchema" case\n# TODO: Need to validate that the user doesn\'t use versioned schemas instead of the latest ones\n-->\n\n## Tutorial\n\nThis guide provides a step-by-step tutorial for setting up automatic API versioning using Universi library. I will illustrate this with an example of a User API, where we will be implementing changes to a User\'s address.\n\n### A dummy setup\n\nHere is an initial API setup where the User has a single address. We will be implementing two routes - one for creating a user and another for retrieving user details. We\'ll be using "int" for ID for simplicity.\n\nThe first API you come up with usually doesn\'t require more than one address -- why bother?\n\nSo we create our file with schemas:\n\n```python\nfrom pydantic import BaseModel\n\n\nclass UserCreateRequest(BaseModel):\n    id: int\n    address: str\n\nclass UserResource(BaseModel):\n    id: int\n    address: str\n```\n\nAnd we create our file with routes:\n\n```python\nfrom versions.latest.users import UserCreateRequest, UserResource\nfrom universi import VersionedAPIRouter\n\nrouter = VersionedAPIRouter()\n\n@router.post("/users", response_model=UserResource)\nasync def create_user(payload: UserCreateRequest):\n    return {\n        "id": 83,\n        "address": payload.address,\n    }\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def get_user(user_id: int):\n    return {\n        "id": user_id,\n        "address": "123 Example St",\n    }\n```\n\n### Turning address into a list\n\nDuring our development, we have realized that the initial API design was wrong and that addresses should have always been a list because the user wants to have multiple addresses to choose from so now we have to change the type of the "address" field to the list of strings.\n\n```python\nfrom pydantic import BaseModel\nfrom universi import Field\n\n\nclass UserCreateRequest(BaseModel):\n    addresses: list[str] = Field(min_items=1)\n\nclass UserResource(BaseModel):\n    id: int\n    addresses: list[str]\n```\n\n```python\n@router.post("/users", response_model=UserResource)\nasync def create_user(payload: UserCreateRequest):\n    return {\n        "id": int,\n        "addresses": payload.addresses,\n    }\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def get_user(user_id: int):\n    return {\n        "id": user_id,\n        "addresses": ["123 Example St", "456 Main St"],\n    }\n\n```\n\nBut every user of ours will now have their API integration broken. To prevent that, we have to introduce API versioning. There aren\'t many methods of doing that. Most of them force you to either duplicate your schemas, your endpoints, or your entire app instance. And it makes sense, really: duplication is the only way to make sure that you will not break old versions with your new versions; the bigger the piece you duplicating -- the safer. Of course, the safest being duplicating the entire app instance and even having a separate database. But that is expensive and makes it either impossible to make breaking changes often or to support many versions. As a result, either you need infinite resources, very long development cycles, or your users will need to often migrate from version to version.\n\nStripe has come up [with a solution](https://stripe.com/blog/api-versioning): let\'s have one latest app version whose responses get migrated to older versions and let\'s describe changes between these versions using migrations. This approach allows them to keep versions for **years** without dropping them. Obviously, each breaking change is still bad and each version still makes our system more complex and expensive, but their approach gives us a chance to minimize that. Additionally, it allows us backport features and bugfixes to older versions. However, you will also be backporting bugs, which is a sad consequence of eliminating duplication.\n\nUniversi is heavily inspired by this approach so let\'s continue our tutorial and now try to combine the two versions we created using versioning.\n\n### Creating the Migration\n\nWe need to create a migration to handle changes between these versions. This migration will convert the list of addresses back to a single address when migrating to the previous version. Yes, migrating **back**: you might be used to database migrations where we write upgrade migration and downgrade migration but here our goal is to have an app of latest version and to describe what older versions looked like in comparison to it. That way the old versions are frozen in migrations and you can **almost** safely forget about them.\n\n```python\nfrom universi import Field\nfrom universi.structure import (\n    schema,\n    AbstractVersionChange,\n    convert_response_to_previous_version_for,\n)\n\nclass ChangeAddressToList(AbstractVersionChange):\n    description = (\n        "Change user address to a list of strings to "\n        "allow the user to specify multiple addresses"\n    )\n    instructions_to_migrate_to_previous_version = (\n        # You should use schema inheritance if you don\'t want to repeat yourself in such cases\n        schema(UserCreateRequest).field("addresses").didnt_exist,\n        schema(UserCreateRequest).field("address").existed_with(type=str, info=Field()),\n        schema(UserResource).field("addresses").didnt_exist,\n        schema(UserResource).field("address").existed_with(type=str, info=Field()),\n    )\n\n    @convert_response_to_previous_version_for(get_user, create_user)\n    def change_addresses_to_single_item(cls, data: dict[str, Any]) -> None:\n        data["address"] = data.pop("addresses")[0]\n    \n    @schema(UserCreateRequest).had_property("addresses")\n    def addresses_property(parsed_schema):\n        return [parsed_schema.address]\n\n```\n\ns\nSee how we are popping the first address from the list? This is only guaranteed to be possible because we specified earlier that `min_items` for `addresses` must be `1`. If we didn\'t, then the user would be able to create a user in a newer version that would be impossible to represent in the older version. I.e. If anyone tried to get that user from the older version, they would get a `ResponseValidationError` because the user wouldn\'t have data for a mandatory `address` field. You need to always keep in mind tht API versioning is only for versioning your **API**, your interface. Your versions must still be completely compatible in terms of data. If they are not, then you are versioning your data and you should really go with a separate app instance. Otherwise, your users will have a hard time migrating back and forth between API versions and so many unexpected errors.\n\nSee how we added the `addresses` property? This simple instruction will allow us to use `addresses` even from the old schema, which means that our api route will not need to know anything about versioning. The main goal of universi is to shift the logic of versioning away from your business logic and api endpoints which makes your project easier to navigate and which makes deleting versions a breeze.\n\n### Grouping Version Changes\n\nFinally, we group the version changes in the `Versions` class. This represents the different versions of your API and the changes between them. You can add any "version changes" to any version. For simplicity, let\'s use versions 2002 and 2001 which means that we had a single address in API in 2001 and added addresses as a list in 2002\'s version.\n\n```python\nfrom universi.structure import Version, Versions\nfrom datetime import date\n\nversions = Versions(\n    Version(date(2002, 1, 1), ChangeAddressToList),\n    Version(date(2001, 1, 1)),\n)\n```\n\nThat\'s it. You\'re done with describing things. Now you just gotta ask universi to do the rest for you. We\'ll need the VersionedAPIRouter we used previously, our API versions, and the module representing the latest versions of our schemas.\n\n```python\nfrom versions import latest\nfrom universi import regenerate_dir_to_all_versions, api_version_var\n\nregenerate_dir_to_all_versions(latest, versions)\nrouter_versions = router.create_versioned_copies(\n    versions,\n    latest_schemas_module=latest,\n)\napi_version_var.set(date(2002, 1, 1))\nuvicorn.run(router_versions[date(2002, 1, 1)])\n```\n\nUniversi has generated multiple things in this code:\n\n* Three versions of our schemas: one for each API version and one that includes definitions of unions of all versions for each schema which will be useful when you want to type check that you are using requests of different versions correctly. For example, we\'ll have `UserCreateRequestUnion` defined there which is a `TypeAlias` pointing to the union of 2002 version and 2001 version of `UserCreateRequest`.\n* Two versions of our API router: one for each API version\n\nYou can now just pick a router by its version and run it separately or use a parent router/app to specify the logic by which you\'d like to pick a version. I recommend using a header-based router with version dates as headers. And yes, that\'s how Stripe does it.\n\nNote that universi migrates your response data based on the api_version_var context variable so you must set it with each request. `universi.header` has a dependency that does that for you.\n\nObviously, this was just a simple example and universi has a lot more features so if you\'re interested -- take a look at the reference\n\n## Reference\n\nTBD\n',
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ovsyanka83/universi',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['universi',
 'universi.structure'] package_data = \ {'': ['*']} install_requires = \
 ['fastapi>=0.96.1', 'type-inspector>=1.2.2,<2.0.0', 'typer[all]', 'typing-
-extensions'] setup_kwargs = { 'name': 'universi', 'version': '0.4.0',
-'description': '', 'long_description': '# universi\n\nPackage description\n\n--
--\n\n
+extensions'] setup_kwargs = { 'name': 'universi', 'version': '0.5.0',
+'description': '', 'long_description': '# universi\n\nModern Stripe-like API
+versioning\n\n---\n\n
 \n\n_[Test]\n\n\n_[Coverage]\n\n\n_[PyPI]\n\n\n_[Supported_Python_versions]\n\n
 \n\n## Installation\n\n```bash\npip install universi\n```\n\n\n\n##
 Tutorial\n\nThis guide provides a step-by-step tutorial for setting up
 automatic API versioning using Universi library. I will illustrate this with an
 example of a User API, where we will be implementing changes to a User\'s
 address.\n\n### A dummy setup\n\nHere is an initial API setup where the User
 has a single address. We will be implementing two routes - one for creating a
@@ -19,91 +19,89 @@
 int\n address: str\n```\n\nAnd we create our file with routes:
 \n\n```python\nfrom versions.latest.users import UserCreateRequest,
 UserResource\nfrom universi import VersionedAPIRouter\n\nrouter =
 VersionedAPIRouter()\n\n@router.post("/users",
 response_model=UserResource)\nasync def create_user(payload:
 UserCreateRequest):\n return {\n "id": 83,\n "address": payload.address,\n
 }\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def
-get_user(user_id: UUID):\n return {\n "id": user_id,\n "address": "123 Example
+get_user(user_id: int):\n return {\n "id": user_id,\n "address": "123 Example
 St",\n }\n```\n\n### Turning address into a list\n\nDuring our development, we
 have realized that the initial API design was wrong and that addresses should
 have always been a list because the user wants to have multiple addresses to
 choose from so now we have to change the type of the "address" field to the
 list of strings.\n\n```python\nfrom pydantic import BaseModel\nfrom universi
-import Field\n\n\nclass UserCreateRequest(BaseModel):\n id: int\n addresses:
-str = Field(min_items=1)\n\nclass UserResource(BaseModel):\n id: int\n
-addresses: str\n```\n\n```python\n@router.post("/users",
+import Field\n\n\nclass UserCreateRequest(BaseModel):\n addresses: list[str] =
+Field(min_items=1)\n\nclass UserResource(BaseModel):\n id: int\n addresses:
+list[str]\n```\n\n```python\n@router.post("/users",
 response_model=UserResource)\nasync def create_user(payload:
-UserCreateRequest):\n return {\n "id": uuid4(),\n "addresses":
-payload.addresses,\n }\n\n@router.get("/users/{user_id}",
-response_model=UserResource)\nasync def get_user(user_id: int):\n return {\n
-"id": user_id,\n "addresses": ["123 Example St", "456 Main St"],\n
-}\n\n```\n\nBut every user of ours will now have their API integration broken.
-To prevent that, we have to introduce API versioning. There aren\'t many
-methods of doing that. Most of them force you to either duplicate your schemas,
-your endpoints, or your entire app instance. And it makes sense, really:
-duplication is the only way to make sure that you will not break old versions
-with your new versions; the bigger the piece you duplicating -- the safer. Of
-course, the safest being duplicating the entire app instance and even having a
-separate database. But that is expensive and makes it either impossible to make
-breaking changes often or to support many versions. As a result, either you
-need infinite resources, very long development cycles, or your users will need
-to often migrate from version to version.\n\nStripe has come up [with a
-solution](https://stripe.com/blog/api-versioning): let\'s have one latest app
-version whose responses get migrated to older versions and let\'s describe
-changes between these versions using migrations. This approach allows them to
-keep versions for **years** without dropping them. Obviously, each breaking
-change is still bad and each version still makes our system more complex and
-expensive, but their approach gives us a chance to minimize that. Additionally,
-it allows us backport features and bugfixes to older versions. However, you
-will also be backporting bugs, which is a sad consequence of eliminating
-duplication.\n\nUniversi is heavily inspired by this approach so let\'s
-continue our tutorial and now try to combine the two versions we created using
-versioning.\n\n### Creating the Migration\n\nWe need to create a migration to
-handle changes between these versions. This migration will convert the list of
-addresses back to a single address when migrating to the previous version. Yes,
-migrating **back**: you might be used to database migrations where we write
-upgrade migration and downgrade migration but here our goal is to have an app
-of latest version and to describe what older versions looked like in comparison
-to it. That way the old versions are frozen in migrations and you can
-**almost** safely forget about them.\n\n```python\nfrom universi.structure
-import (\n field,\n schema,\n AbstractVersionChange,\n
-convert_response_to_previous_version_for,\n Field\n)\n\nclass
-ChangeAddressToList(AbstractVersionChange):\n description = (\n "Change user
-address to a list of strings to "\n "allow the user to specify multiple
-addresses"\n )\n instructions_to_migrate_to_previous_version = (\n schema(\n
-UserCreateRequest,\n field("addresses").didnt_exist,\n field
-("address").existed_with(type=str, info=Field()),\n ),\n schema(\n
-UserResource,\n field("addresses").didnt_exist,\n field("address").existed_with
-(type=str, info=Field()),\n )\n )\n\n @convert_response_to_previous_version_for
-(get_user, create_user)\n def change_addresses_to_single_item(cls, data: dict
-[str, Any]) -> None:\n data["address"] = data.pop("addresses")[0]\n```\n\nSee
-how we are popping the first address from the list? This is only guaranteed to
-be possible because we specified earlier that `min_items` for `addresses` must
-be `1`. If we didn\'t, then the user would be able to create a user in a newer
-version that would be impossible to represent in the older version. I.e. If
-anyone tried to get that user from the older version, they would get a
+UserCreateRequest):\n return {\n "id": int,\n "addresses": payload.addresses,\n
+}\n\n@router.get("/users/{user_id}", response_model=UserResource)\nasync def
+get_user(user_id: int):\n return {\n "id": user_id,\n "addresses": ["123
+Example St", "456 Main St"],\n }\n\n```\n\nBut every user of ours will now have
+their API integration broken. To prevent that, we have to introduce API
+versioning. There aren\'t many methods of doing that. Most of them force you to
+either duplicate your schemas, your endpoints, or your entire app instance. And
+it makes sense, really: duplication is the only way to make sure that you will
+not break old versions with your new versions; the bigger the piece you
+duplicating -- the safer. Of course, the safest being duplicating the entire
+app instance and even having a separate database. But that is expensive and
+makes it either impossible to make breaking changes often or to support many
+versions. As a result, either you need infinite resources, very long
+development cycles, or your users will need to often migrate from version to
+version.\n\nStripe has come up [with a solution](https://stripe.com/blog/api-
+versioning): let\'s have one latest app version whose responses get migrated to
+older versions and let\'s describe changes between these versions using
+migrations. This approach allows them to keep versions for **years** without
+dropping them. Obviously, each breaking change is still bad and each version
+still makes our system more complex and expensive, but their approach gives us
+a chance to minimize that. Additionally, it allows us backport features and
+bugfixes to older versions. However, you will also be backporting bugs, which
+is a sad consequence of eliminating duplication.\n\nUniversi is heavily
+inspired by this approach so let\'s continue our tutorial and now try to
+combine the two versions we created using versioning.\n\n### Creating the
+Migration\n\nWe need to create a migration to handle changes between these
+versions. This migration will convert the list of addresses back to a single
+address when migrating to the previous version. Yes, migrating **back**: you
+might be used to database migrations where we write upgrade migration and
+downgrade migration but here our goal is to have an app of latest version and
+to describe what older versions looked like in comparison to it. That way the
+old versions are frozen in migrations and you can **almost** safely forget
+about them.\n\n```python\nfrom universi import Field\nfrom universi.structure
+import (\n schema,\n AbstractVersionChange,\n
+convert_response_to_previous_version_for,\n)\n\nclass ChangeAddressToList
+(AbstractVersionChange):\n description = (\n "Change user address to a list of
+strings to "\n "allow the user to specify multiple addresses"\n )\n
+instructions_to_migrate_to_previous_version = (\n # You should use schema
+inheritance if you don\'t want to repeat yourself in such cases\n schema
+(UserCreateRequest).field("addresses").didnt_exist,\n schema
+(UserCreateRequest).field("address").existed_with(type=str, info=Field()),\n
+schema(UserResource).field("addresses").didnt_exist,\n schema
+(UserResource).field("address").existed_with(type=str, info=Field()),\n )\n\n
+@convert_response_to_previous_version_for(get_user, create_user)\n def
+change_addresses_to_single_item(cls, data: dict[str, Any]) -> None:\n data
+["address"] = data.pop("addresses")[0]\n \n @schema
+(UserCreateRequest).had_property("addresses")\n def addresses_property
+(parsed_schema):\n return [parsed_schema.address]\n\n```\n\ns\nSee how we are
+popping the first address from the list? This is only guaranteed to be possible
+because we specified earlier that `min_items` for `addresses` must be `1`. If
+we didn\'t, then the user would be able to create a user in a newer version
+that would be impossible to represent in the older version. I.e. If anyone
+tried to get that user from the older version, they would get a
 `ResponseValidationError` because the user wouldn\'t have data for a mandatory
 `address` field. You need to always keep in mind tht API versioning is only for
 versioning your **API**, your interface. Your versions must still be completely
 compatible in terms of data. If they are not, then you are versioning your data
 and you should really go with a separate app instance. Otherwise, your users
 will have a hard time migrating back and forth between API versions and so many
-unexpected errors.\n\nNow that we\'ve made our migration, we are realizing that
-even though we are migrating data for our response so we don\'t need to worry
-about it in our business logic, our user creation function still cannot handle
-the old version: it will just break when it tries to get `addresses` from
-`UserCreateRequest` because the old version doesn\'t have it.\n\n###
-Accomodating changes in request schemas\n\n```python\n@router.post("/users",
-response_model=UserResource)\nasync def create_user(payload:
-UserCreateRequest):s\n if hasattr(payload, "addresses"):\n addresses =
-payload.addresses\n else:\n addresses = [payload.address]\n return {\n "id":
-uuid4(),\n "addresses": payload.addresses,\n }\n\n```\n\nNow we just need to
-combine everything together and ask universi to generate for us the parts that
-we would copy-paste in traditional versioning.\n\n### Grouping Version
+unexpected errors.\n\nSee how we added the `addresses` property? This simple
+instruction will allow us to use `addresses` even from the old schema, which
+means that our api route will not need to know anything about versioning. The
+main goal of universi is to shift the logic of versioning away from your
+business logic and api endpoints which makes your project easier to navigate
+and which makes deleting versions a breeze.\n\n### Grouping Version
 Changes\n\nFinally, we group the version changes in the `Versions` class. This
 represents the different versions of your API and the changes between them. You
 can add any "version changes" to any version. For simplicity, let\'s use
 versions 2002 and 2001 which means that we had a single address in API in 2001
 and added addresses as a list in 2002\'s version.\n\n```python\nfrom
 universi.structure import Version, Versions\nfrom datetime import
 date\n\nversions = Versions(\n Version(date(2002, 1, 1),
```

### Comparing `universi-0.4.0/PKG-INFO` & `universi-0.5.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: universi
-Version: 0.4.0
+Version: 0.5.0
 Summary: 
 Home-page: https://github.com/ovsyanka83/universi
 License: MIT
 Author: Stanislav Zmiev
 Author-email: szmiev2000@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -16,15 +16,15 @@
 Requires-Dist: typer[all]
 Requires-Dist: typing-extensions
 Project-URL: Repository, https://github.com/ovsyanka83/universi
 Description-Content-Type: text/markdown
 
 # universi
 
-Package description
+Modern Stripe-like API versioning
 
 ---
 
 <p align="center">
 <a href="https://github.com/ovsyanka83/universi/actions?query=workflow%3ATests+event%3Apush+branch%3Amain" target="_blank">
     <img src="https://github.com/Ovsyanka83/universi/actions/workflows/test.yaml/badge.svg?branch=main&event=push" alt="Test">
 </a>
@@ -87,15 +87,15 @@
 async def create_user(payload: UserCreateRequest):
     return {
         "id": 83,
         "address": payload.address,
     }
 
 @router.get("/users/{user_id}", response_model=UserResource)
-async def get_user(user_id: UUID):
+async def get_user(user_id: int):
     return {
         "id": user_id,
         "address": "123 Example St",
     }
 ```
 
 ### Turning address into a list
@@ -104,27 +104,26 @@
 
 ```python
 from pydantic import BaseModel
 from universi import Field
 
 
 class UserCreateRequest(BaseModel):
-    id: int
-    addresses: str = Field(min_items=1)
+    addresses: list[str] = Field(min_items=1)
 
 class UserResource(BaseModel):
     id: int
-    addresses: str
+    addresses: list[str]
 ```
 
 ```python
 @router.post("/users", response_model=UserResource)
 async def create_user(payload: UserCreateRequest):
     return {
-        "id": uuid4(),
+        "id": int,
         "addresses": payload.addresses,
     }
 
 @router.get("/users/{user_id}", response_model=UserResource)
 async def get_user(user_id: int):
     return {
         "id": user_id,
@@ -140,66 +139,48 @@
 Universi is heavily inspired by this approach so let's continue our tutorial and now try to combine the two versions we created using versioning.
 
 ### Creating the Migration
 
 We need to create a migration to handle changes between these versions. This migration will convert the list of addresses back to a single address when migrating to the previous version. Yes, migrating **back**: you might be used to database migrations where we write upgrade migration and downgrade migration but here our goal is to have an app of latest version and to describe what older versions looked like in comparison to it. That way the old versions are frozen in migrations and you can **almost** safely forget about them.
 
 ```python
+from universi import Field
 from universi.structure import (
-    field,
     schema,
     AbstractVersionChange,
     convert_response_to_previous_version_for,
-    Field
 )
 
 class ChangeAddressToList(AbstractVersionChange):
     description = (
         "Change user address to a list of strings to "
         "allow the user to specify multiple addresses"
     )
     instructions_to_migrate_to_previous_version = (
-        schema(
-            UserCreateRequest,
-            field("addresses").didnt_exist,
-            field("address").existed_with(type=str, info=Field()),
-        ),
-        schema(
-            UserResource,
-            field("addresses").didnt_exist,
-            field("address").existed_with(type=str, info=Field()),
-        )
+        # You should use schema inheritance if you don't want to repeat yourself in such cases
+        schema(UserCreateRequest).field("addresses").didnt_exist,
+        schema(UserCreateRequest).field("address").existed_with(type=str, info=Field()),
+        schema(UserResource).field("addresses").didnt_exist,
+        schema(UserResource).field("address").existed_with(type=str, info=Field()),
     )
 
     @convert_response_to_previous_version_for(get_user, create_user)
     def change_addresses_to_single_item(cls, data: dict[str, Any]) -> None:
         data["address"] = data.pop("addresses")[0]
+    
+    @schema(UserCreateRequest).had_property("addresses")
+    def addresses_property(parsed_schema):
+        return [parsed_schema.address]
+
 ```
 
+s
 See how we are popping the first address from the list? This is only guaranteed to be possible because we specified earlier that `min_items` for `addresses` must be `1`. If we didn't, then the user would be able to create a user in a newer version that would be impossible to represent in the older version. I.e. If anyone tried to get that user from the older version, they would get a `ResponseValidationError` because the user wouldn't have data for a mandatory `address` field. You need to always keep in mind tht API versioning is only for versioning your **API**, your interface. Your versions must still be completely compatible in terms of data. If they are not, then you are versioning your data and you should really go with a separate app instance. Otherwise, your users will have a hard time migrating back and forth between API versions and so many unexpected errors.
 
-Now that we've made our migration, we are realizing that even though we are migrating data for our response so we don't need to worry about it in our business logic, our user creation function still cannot handle the old version: it will just break when it tries to get `addresses` from `UserCreateRequest` because the old version doesn't have it.
-
-### Accomodating changes in request schemas
-
-```python
-@router.post("/users", response_model=UserResource)
-async def create_user(payload: UserCreateRequest):s
-    if hasattr(payload, "addresses"):
-        addresses = payload.addresses
-    else:
-        addresses = [payload.address]
-    return {
-        "id": uuid4(),
-        "addresses": payload.addresses,
-    }
-
-```
-
-Now we just need to combine everything together and ask universi to generate for us the parts that we would copy-paste in traditional versioning.
+See how we added the `addresses` property? This simple instruction will allow us to use `addresses` even from the old schema, which means that our api route will not need to know anything about versioning. The main goal of universi is to shift the logic of versioning away from your business logic and api endpoints which makes your project easier to navigate and which makes deleting versions a breeze.
 
 ### Grouping Version Changes
 
 Finally, we group the version changes in the `Versions` class. This represents the different versions of your API and the changes between them. You can add any "version changes" to any version. For simplicity, let's use versions 2002 and 2001 which means that we had a single address in API in 2001 and added addresses as a list in 2002's version.
 
 ```python
 from universi.structure import Version, Versions
```

