# Comparing `tmp/universi-0.3.0.tar.gz` & `tmp/universi-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "universi-0.3.0.tar", max compression
+gzip compressed data, was "universi-0.4.0.tar", max compression
```

## Comparing `universi-0.3.0.tar` & `universi-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.3.0/LICENSE
--rw-r--r--   0        0        0     1111 2023-07-13 19:54:24.646654 universi-0.3.0/README.md
--rw-r--r--   0        0        0     4059 2023-07-12 23:05:34.016074 universi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      453 2023-07-12 22:40:12.864421 universi-0.3.0/universi/__init__.py
--rw-r--r--   0        0        0     2007 2023-07-13 07:28:53.287286 universi-0.3.0/universi/_utils.py
--rw-r--r--   0        0        0    16536 2023-07-12 19:34:22.676522 universi-0.3.0/universi/codegen.py
--rw-r--r--   0        0        0      324 2023-07-10 23:48:56.035792 universi-0.3.0/universi/exceptions.py
--rw-r--r--   0        0        0     2841 2023-07-08 14:21:11.688092 universi-0.3.0/universi/fields.py
--rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.3.0/universi/header.py
--rw-r--r--   0        0        0        0 2023-07-13 08:09:29.390618 universi-0.3.0/universi/py.typed
--rw-r--r--   0        0        0    11467 2023-07-12 19:38:06.375294 universi-0.3.0/universi/routing.py
--rw-r--r--   0        0        0      396 2023-07-08 11:43:06.913473 universi-0.3.0/universi/structure/__init__.py
--rw-r--r--   0        0        0      265 2023-07-08 11:43:06.913473 universi-0.3.0/universi/structure/common.py
--rw-r--r--   0        0        0     4936 2023-07-10 10:22:38.358870 universi-0.3.0/universi/structure/endpoints.py
--rw-r--r--   0        0        0      944 2023-07-08 11:43:06.913473 universi-0.3.0/universi/structure/enums.py
--rw-r--r--   0        0        0     1239 2023-07-12 19:32:07.873928 universi-0.3.0/universi/structure/responses.py
--rw-r--r--   0        0        0     4199 2023-07-11 01:53:10.755842 universi-0.3.0/universi/structure/schemas.py
--rw-r--r--   0        0        0     8670 2023-07-12 19:32:07.877261 universi-0.3.0/universi/structure/versions.py
--rw-r--r--   0        0        0     1858 1970-01-01 00:00:00.000000 universi-0.3.0/setup.py
--rw-r--r--   0        0        0     1771 1970-01-01 00:00:00.000000 universi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-12 19:09:15.569998 universi-0.4.0/LICENSE
+-rw-r--r--   0        0        0    10495 2023-07-14 22:57:30.396654 universi-0.4.0/README.md
+-rw-r--r--   0        0        0     4059 2023-07-14 22:57:44.169987 universi-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      453 2023-07-12 22:40:12.864421 universi-0.4.0/universi/__init__.py
+-rw-r--r--   0        0        0     2821 2023-07-14 12:35:15.746665 universi-0.4.0/universi/_utils.py
+-rw-r--r--   0        0        0    20023 2023-07-14 20:26:25.333325 universi-0.4.0/universi/codegen.py
+-rw-r--r--   0        0        0      324 2023-07-10 23:48:56.035792 universi-0.4.0/universi/exceptions.py
+-rw-r--r--   0        0        0     2841 2023-07-08 14:21:11.688092 universi-0.4.0/universi/fields.py
+-rw-r--r--   0        0        0      903 2023-07-06 22:52:01.148105 universi-0.4.0/universi/header.py
+-rw-r--r--   0        0        0        0 2023-07-13 08:09:29.390618 universi-0.4.0/universi/py.typed
+-rw-r--r--   0        0        0    12278 2023-07-14 12:35:15.899998 universi-0.4.0/universi/routing.py
+-rw-r--r--   0        0        0      396 2023-07-08 11:43:06.913473 universi-0.4.0/universi/structure/__init__.py
+-rw-r--r--   0        0        0      265 2023-07-08 11:43:06.913473 universi-0.4.0/universi/structure/common.py
+-rw-r--r--   0        0        0     4936 2023-07-10 10:22:38.358870 universi-0.4.0/universi/structure/endpoints.py
+-rw-r--r--   0        0        0      944 2023-07-08 11:43:06.913473 universi-0.4.0/universi/structure/enums.py
+-rw-r--r--   0        0        0     1270 2023-07-14 12:35:15.266665 universi-0.4.0/universi/structure/responses.py
+-rw-r--r--   0        0        0     4207 2023-07-14 12:35:03.836665 universi-0.4.0/universi/structure/schemas.py
+-rw-r--r--   0        0        0     8933 2023-07-14 12:35:15.819998 universi-0.4.0/universi/structure/versions.py
+-rw-r--r--   0        0        0    11455 1970-01-01 00:00:00.000000 universi-0.4.0/setup.py
+-rw-r--r--   0        0        0    11155 1970-01-01 00:00:00.000000 universi-0.4.0/PKG-INFO
```

### Comparing `universi-0.3.0/LICENSE` & `universi-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `universi-0.3.0/pyproject.toml` & `universi-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "universi"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/ovsyanka83/universi"
 
 [tool.poetry.dependencies]
```

### Comparing `universi-0.3.0/universi/_utils.py` & `universi-0.4.0/universi/_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,46 +6,78 @@
 from typing import Any
 
 from universi.exceptions import UniversiError
 
 Sentinel: Any = object()
 
 
-def get_another_version_of_cls(cls_from_old_version: type[Any], new_version_dir: Path) -> None:
+def get_another_version_of_cls(
+    cls_from_old_version: type[Any],
+    new_version_dir: Path,
+) -> None:
     # version_dir = /home/myuser/package/companies/v2021_01_01
 
     module_from_old_version = sys.modules[cls_from_old_version.__module__]
     module = get_another_version_of_module(module_from_old_version, new_version_dir)
     return getattr(module, cls_from_old_version.__name__)
 
 
-def get_another_version_of_module(module_from_old_version: ModuleType, new_version_dir: Path):
+def get_another_version_of_module(
+    module_from_old_version: ModuleType,
+    new_version_dir: Path,
+):
+    new_model_module_python_path = get_pythonpath_to_another_version_of_module(
+        module_from_old_version,
+        new_version_dir,
+    )
+    module = importlib.import_module(new_model_module_python_path)
+    return module
+
+
+def get_pythonpath_to_another_version_of_module(
+    module_from_old_version: ModuleType,
+    new_version_dir: Path,
+) -> str:
+    # ['package', 'companies', 'latest', 'schemas']
+    #                           ^^^^^^
+    #                           index = 2
+    index_of_base_schema_dir = get_index_of_base_schema_dir_in_pythonpath(
+        module_from_old_version,
+        new_version_dir,
+    )
+
+    # ['package', 'companies', 'latest', 'schemas']
+    model_split_python_path = module_from_old_version.__name__.split(".")
+    # ['package', 'companies', 'v2021_01_01', 'schemas']
+    model_split_python_path[index_of_base_schema_dir] = new_version_dir.name
+    # package.companies.v2021_01_01.schemas
+    new_model_module_python_path = ".".join(model_split_python_path)
+    return new_model_module_python_path
+
+
+def get_index_of_base_schema_dir_in_pythonpath(
+    module_from_old_version: ModuleType,
+    parallel_dir: Path,
+) -> int:
     file = inspect.getsourcefile(module_from_old_version)
     if file is None:
         # Seems quite unnecessary to cover
-        raise UniversiError(f"Model {module_from_old_version} is not defined in a file")  # pragma: no cover
+        raise UniversiError(
+            f"Model {module_from_old_version} is not defined in a file",
+        )  # pragma: no cover
     # /home/myuser/package/companies/latest/__init__.py
     file = Path(file)
     if file.name == "__init__.py":
         # /home/myuser/package/companies/latest/
         file = file.parent
     # /home/myuser/package/companies
-    root_dir = new_version_dir.parent
+    root_dir = parallel_dir.parent
     # latest/schemas
     relative_file = file.relative_to(root_dir).with_suffix("")
     # ['latest', 'schemas']
     relative_file_parts = relative_file.parts
     # package.companies.latest.schemas.Payable
-    model_python_path = module_from_old_version.__name__
+    module_python_path = module_from_old_version.__name__
     # ['package', 'companies', 'latest', 'schemas']
-    model_split_python_path = model_python_path.split(".")
-
-    # ['package', 'companies', 'latest', 'schemas']
-    #                           ^^^^^^
-    #                           index = -2
+    module_split_python_path = module_python_path.split(".")
 
-    # ['package', 'companies', 'v2021_01_01', 'schemas']
-    model_split_python_path[-len(relative_file_parts)] = new_version_dir.name
-    # package.companies.v2021_01_01.schemas
-    new_model_module_python_path = ".".join(model_split_python_path)
-    module = importlib.import_module(new_model_module_python_path)
-    return module
+    return len(module_split_python_path) - len(relative_file_parts)
```

### Comparing `universi-0.3.0/universi/codegen.py` & `universi-0.4.0/universi/codegen.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import importlib
 import inspect
 import os
 import shutil
 import sys
-from collections.abc import Sequence
+from collections.abc import Generator, Sequence
 from copy import deepcopy
 from datetime import date
 from enum import Enum, auto
 from pathlib import Path
 from types import GenericAlias, LambdaType, ModuleType
 from typing import (
     Any,
@@ -20,24 +20,28 @@
 
 from pydantic import BaseConfig, BaseModel
 from pydantic.fields import FieldInfo as PydanticFieldInfo
 from pydantic.fields import ModelField
 from pydantic.typing import convert_generics
 from typing_extensions import assert_never
 
-from universi.structure.enums import AlterEnumSubInstruction, EnumDidntHaveMembersInstruction, EnumHadMembersInstruction
+from universi.structure.enums import (
+    AlterEnumSubInstruction,
+    EnumDidntHaveMembersInstruction,
+    EnumHadMembersInstruction,
+)
 from universi.structure.schemas import (
     AlterSchemaInstruction,
     OldSchemaDidntHaveField,
     OldSchemaFieldWas,
     OldSchemaHadField,
 )
 from universi.structure.versions import Version, Versions
 
-from ._utils import Sentinel
+from ._utils import Sentinel, get_index_of_base_schema_dir_in_pythonpath
 from .exceptions import CodeGenerationError, InvalidGenerationInstructionError
 from .fields import FieldInfo
 
 LambdaFunctionName = (lambda: None).__name__  # pragma: no branch
 FieldNameT: TypeAlias = str
 dict_of_empty_field_info = {k: getattr(PydanticFieldInfo(), k) for k in PydanticFieldInfo.__slots__}
 
@@ -48,36 +52,107 @@
     enums = {k: (v, {member.name: member.value for member in v}) for k, v in deepcopy(versions.versioned_enums).items()}
 
     for version in versions.versions:
         # NOTE: You'll have to use relative imports
 
         _generate_versioned_directory(template_module, schemas, enums, version.date)
         _apply_migrations(version, schemas, enums)
+    _generate_union_directory(template_module, versions)
 
     current_package = template_module.__name__
     while current_package != "":
         importlib.reload(sys.modules[current_package])
         current_package = ".".join(current_package.split(".")[:-1])
 
 
+def _generate_union_directory(template_module: ModuleType, versions: Versions):
+    template_dir = _get_package_path_from_module(template_module)
+    union_dir = template_dir.with_name("unions")
+    index_of_base_schema_in_pythonpath = get_index_of_base_schema_dir_in_pythonpath(
+        template_module,
+        union_dir,
+    )
+    for (
+        relative_path_to_file,
+        original_module,
+        parallel_file,
+    ) in _generate_parallel_directory(
+        template_module,
+        union_dir,
+    ):
+        new_module_text = _get_unionized_version_of_module(
+            original_module,
+            relative_path_to_file,
+            versions,
+            index_of_base_schema_in_pythonpath,
+        )
+        parallel_file.write_text(new_module_text)
+
+
+def _get_unionized_version_of_module(
+    original_module: ModuleType,
+    relative_path_to_file: Path,
+    versions: Versions,
+    index_of_base_schema_in_pythonpath: int,
+):
+    original_module_parts = original_module.__name__.split(".")
+    original_module_parts[index_of_base_schema_in_pythonpath] = "{}"
+
+    import_pythonpath_template = (".".join(original_module_parts)).removesuffix(".__init__")
+    imported_modules = [
+        import_pythonpath_template.format(_get_version_dir_name(version.date)) for version in versions.versions
+    ]
+
+    parsed_file = _parse_python_module(original_module)
+
+    if original_module.__name__.endswith(".__init__"):
+        module_name = original_module.__name__.removesuffix(".__init__")
+    else:
+        module_name = original_module.__name__
+    body = ast.Module(
+        [
+            ast.ImportFrom(module="universi", names=[ast.alias(name="Field")], level=0),
+            ast.Import(names=[ast.alias(name="typing")], level=0),
+            *[ast.Import(names=[ast.Name(module)]) for module in imported_modules],
+        ]
+        + [
+            ast.Name(
+                f"\n{node.name}Union: typing.TypeAlias = {' | '.join(f'{module}.{node.name}' for module in imported_modules)}",
+            )
+            if isinstance(node, ast.ClassDef)
+            else node
+            for node in parsed_file.body
+        ],
+        [],
+    )
+
+    return ast.unparse(body)
+
+
 def _apply_migrations(
     version: Version,
     schemas: dict[
         str,
         tuple[type[BaseModel], dict[FieldNameT, tuple[type[BaseModel], ModelField]]],
     ],
     enums: dict[str, tuple[type[Enum], dict[str, Any]]],
 ):
     for version_change in version.version_changes:
-        _apply_alter_schema_instructions(schemas, version_change.alter_schema_instructions)
+        _apply_alter_schema_instructions(
+            schemas,
+            version_change.alter_schema_instructions,
+        )
         _apply_alter_enum_instructions(enums, version_change.alter_enum_instructions)
 
 
 def _apply_alter_schema_instructions(
-    schemas: dict[str, tuple[type[BaseModel], dict[FieldNameT, tuple[type[BaseModel], ModelField]]]],
+    schemas: dict[
+        str,
+        tuple[type[BaseModel], dict[FieldNameT, tuple[type[BaseModel], ModelField]]],
+    ],
     alter_schema_instructions: Sequence[AlterSchemaInstruction],
 ):
     for alter_schema_instruction in alter_schema_instructions:
         schema = alter_schema_instruction.schema
         schema_path = schema.__module__ + schema.__name__
         schema_field_info_bundle = schemas[schema_path]
         field_name_to_field_model = schema_field_info_bundle[1]
@@ -152,19 +227,21 @@
                     )
                 else:
                     enum_member_to_value[1][member] = member_value
         else:
             assert_never(alter_enum_instruction)
 
 
-def _get_versioned_schema_dir_name(template_module: ModuleType, version: date) -> Path:
+def _get_version_dir_path(template_module: ModuleType, version: date) -> Path:
     template_dir = _get_package_path_from_module(template_module)
+    return template_dir.with_name(_get_version_dir_name(version))
 
-    version_as_str = version.isoformat().replace("-", "_")
-    return template_dir.with_name("v" + version_as_str)
+
+def _get_version_dir_name(version: date):
+    return "v" + version.isoformat().replace("-", "_")
 
 
 def _get_package_path_from_module(template_module: ModuleType) -> Path:
     file = inspect.getsourcefile(template_module)
 
     # I am too lazy to reproduce this error correctly
     if file is None:  # pragma: no cover
@@ -180,98 +257,134 @@
     schemas: dict[
         str,
         tuple[type[BaseModel], dict[FieldNameT, tuple[type[BaseModel], ModelField]]],
     ],
     enums: dict[str, tuple[type[Enum], dict[str, Any]]],
     version: date,
 ):
+    version_dir = _get_version_dir_path(template_module, version)
+    for (
+        _relative_path_to_file,
+        original_module,
+        parallel_file,
+    ) in _generate_parallel_directory(
+        template_module,
+        version_dir,
+    ):
+        new_module_text = _migrate_module_to_another_version(
+            original_module,
+            schemas,
+            enums,
+        )
+        parallel_file.write_text(new_module_text)
+
+
+def _generate_parallel_directory(
+    template_module: ModuleType,
+    parallel_dir: Path,
+) -> Generator[tuple[Path, ModuleType, Path], Any, None]:
     assert template_module.__file__ is not None
     dir = _get_package_path_from_module(template_module)
-    version_dir = _get_versioned_schema_dir_name(template_module, version)
-    version_dir.mkdir(exist_ok=True)
+    parallel_dir.mkdir(exist_ok=True)
     # [universi, structure, schemas]
     template_module_python_path_parts = template_module.__name__.split(".")
     # [home, foo, bar, universi, structure, schemas]
     template_module_path_parts = Path(template_module.__file__).parent.parts
     # [home, foo, bar] = [home, foo, bar, universi, structure, schemas][:-3]
-    root_module_path = Path(*template_module_path_parts[: -len(template_module_python_path_parts)])
+    root_module_path = Path(
+        *template_module_path_parts[: -len(template_module_python_path_parts)],
+    )
     for subroot, dirnames, filenames in os.walk(dir):
         original_subroot = Path(subroot)
-        versioned_subroot = version_dir / original_subroot.relative_to(dir)
+        parallel_subroot = parallel_dir / original_subroot.relative_to(dir)
         if "__pycache__" in dirnames:
             dirnames.remove("__pycache__")
         for dirname in dirnames:
-            (versioned_subroot / dirname).mkdir(exist_ok=True)
+            (parallel_subroot / dirname).mkdir(exist_ok=True)
         for filename in filenames:
             original_file = (original_subroot / filename).absolute()
-            versioned_file = (versioned_subroot / filename).absolute()
+            parallel_file = (parallel_subroot / filename).absolute()
             print(original_file)
 
             if filename.endswith(".py"):
-                module_path = ".".join(
+                original_module_path = ".".join(
                     original_file.relative_to(root_module_path).with_suffix("").parts,
                 )
-                module = importlib.import_module(module_path)
-                new_module_text = _modify_module(module, schemas, enums)
-                versioned_file.write_text(new_module_text)
+                original_module = importlib.import_module(original_module_path)
+                yield original_subroot.relative_to(dir), original_module, parallel_file
             else:
-                shutil.copyfile(original_file, versioned_file)
+                shutil.copyfile(original_file, parallel_file)
 
 
-def _get_fields_for_model(model: type[BaseModel]) -> dict[FieldNameT, tuple[type[BaseModel], ModelField]]:
+def _get_fields_for_model(
+    model: type[BaseModel],
+) -> dict[FieldNameT, tuple[type[BaseModel], ModelField]]:
     actual_fields: dict[FieldNameT, tuple[type[BaseModel], ModelField]] = {}
     for cls in model.__mro__:
         if cls is BaseModel:
             return actual_fields
         if not issubclass(cls, BaseModel):
             continue
         for field_name, field in cls.__fields__.items():
             if field_name not in actual_fields and field_name in cls.__annotations__:
                 actual_fields[field_name] = (cls, field)
     else:
         raise CodeGenerationError(f"Model {model} is not a subclass of BaseModel")
 
 
-def _modify_module(
-    module,
-    modified_schemas: dict[
-        str,
-        tuple[type[BaseModel], dict[str, tuple[type[BaseModel], ModelField]]],
-    ],
-    modified_enums: dict[str, tuple[type[Enum], dict[str, Any]]],
-) -> str:
+def _parse_python_module(module: ModuleType) -> ast.Module:
     try:
-        parsed_file = ast.parse(inspect.getsource(module))
+        return ast.parse(inspect.getsource(module))
     except OSError as e:
+        if module.__file__ is None:  # pragma: no cover
+            raise CodeGenerationError("Failed to get file path to the module") from e
+
         path = Path(module.__file__)
         if path.is_file() and path.read_text() == "":
-            return ""
+            return ast.Module([])
         # Not sure how to get here so this is just a precaution
         raise CodeGenerationError("Failed to get source code for module") from e  # pragma: no cover
 
+
+def _migrate_module_to_another_version(
+    module,
+    modified_schemas: dict[
+        str,
+        tuple[type[BaseModel], dict[str, tuple[type[BaseModel], ModelField]]],
+    ],
+    modified_enums: dict[str, tuple[type[Enum], dict[str, Any]]],
+) -> str:
+    parsed_file = _parse_python_module(module)
     if module.__name__.endswith(".__init__"):
         module_name = module.__name__.removesuffix(".__init__")
     else:
         module_name = module.__name__
     body = ast.Module(
         [
             ast.ImportFrom(module="universi", names=[ast.alias(name="Field")], level=0),
             ast.Import(names=[ast.alias(name="typing")], level=0),
         ]
         + [
-            _modify_cls(n, module_name, modified_schemas, modified_enums) if isinstance(n, ast.ClassDef) else n
+            _migrate_cls_to_another_version(
+                n,
+                module_name,
+                modified_schemas,
+                modified_enums,
+            )
+            if isinstance(n, ast.ClassDef)
+            else n
             for n in parsed_file.body
         ],
         [],
     )
 
     return ast.unparse(body)
 
 
-def _modify_cls(
+def _migrate_cls_to_another_version(
     cls_node: ast.ClassDef,
     module_python_path: str,
     modified_schemas: dict[
         str,
         tuple[type[BaseModel], dict[str, tuple[type[BaseModel], ModelField]]],
     ],
     modified_enums: dict[str, tuple[type[Enum], dict[str, Any]]],
@@ -302,15 +415,19 @@
                     ast.keyword(
                         arg=attr,
                         value=ast.Name(
                             id=custom_repr(getattr(field[1].field_info, attr)),
                         ),
                     )
                     # TODO: We should lint the code to make sure that the user is not using pydantic.fields.Field instead of universi.Field
-                    for attr in getattr(field[1].field_info, "_universi_field_names", ())
+                    for attr in getattr(
+                        field[1].field_info,
+                        "_universi_field_names",
+                        (),
+                    )
                 ],
             ),
             simple=1,
         )
         for name, field in actual_fields.items()
     ]
     old_body = [n for n in cls_node.body if not isinstance(n, ast.AnnAssign | ast.Pass | ast.Ellipsis)]
@@ -352,15 +469,17 @@
 # The following is based on by Samuel Colvin's devtools
 
 
 def custom_repr(value: Any) -> Any:
     if isinstance(value, list | tuple | set | frozenset):
         return PlainRepr(value.__class__(map(custom_repr, value)))
     if isinstance(value, dict):
-        return PlainRepr(value.__class__((custom_repr(k), custom_repr(v)) for k, v in value.items()))
+        return PlainRepr(
+            value.__class__((custom_repr(k), custom_repr(v)) for k, v in value.items()),
+        )
     if isinstance(value, _BaseGenericAlias | GenericAlias):
         return f"{custom_repr(get_origin(value))}[{', '.join(custom_repr(a) for a in get_args(value))}]"
     if isinstance(value, type):
         return value.__name__
     if isinstance(value, Enum):
         return PlainRepr(f"{value.__class__.__name__}.{value.name}")
     if isinstance(value, auto):
@@ -391,8 +510,10 @@
         return ast.unparse(found_lambdas[0])
     # These two errors are really hard to cover. Not sure if even possible, honestly :)
     elif len(found_lambdas) == 0:  # pragma: no cover
         raise InvalidGenerationInstructionError(
             f"No lambda found in default_factory even though one was passed: {source}",
         )
     else:  # pragma: no cover
-        raise InvalidGenerationInstructionError("More than one lambda found in default_factory. This is not supported.")
+        raise InvalidGenerationInstructionError(
+            "More than one lambda found in default_factory. This is not supported.",
+        )
```

### Comparing `universi-0.3.0/universi/fields.py` & `universi-0.4.0/universi/fields.py`

 * *Files identical despite different names*

### Comparing `universi-0.3.0/universi/header.py` & `universi-0.4.0/universi/header.py`

 * *Files identical despite different names*

### Comparing `universi-0.3.0/universi/routing.py` & `universi-0.4.0/universi/routing.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,39 +2,43 @@
 import functools
 import inspect
 from collections.abc import Callable
 from copy import deepcopy
 from enum import Enum
 from pathlib import Path
 from threading import Lock
-from types import FunctionType, GenericAlias, MappingProxyType, ModuleType
+from types import GenericAlias, MappingProxyType, ModuleType
 from typing import (
     Any,
     TypeVar,
     _BaseGenericAlias,  # pyright: ignore
     cast,
     get_args,
     get_origin,
 )
 
 import fastapi.routing
-from fastapi.dependencies.utils import get_body_field, get_dependant, get_parameterless_sub_dependant
+from fastapi.dependencies.utils import (
+    get_body_field,
+    get_dependant,
+    get_parameterless_sub_dependant,
+)
 from fastapi.params import Depends
 from fastapi.routing import APIRoute
 from pydantic import BaseModel
 from starlette._utils import is_async_callable
 from starlette.routing import (
     BaseRoute,
     request_response,
 )
 from starlette.routing import Mount as Mount  # noqa
 from typing_extensions import Self, assert_never
 
 from universi._utils import Sentinel, get_another_version_of_cls
-from universi.codegen import _get_versioned_schema_dir_name
+from universi.codegen import _get_version_dir_path
 from universi.exceptions import RouterGenerationError
 from universi.structure.common import Endpoint
 from universi.structure.endpoints import (
     EndpointDidntExistInstruction,
     EndpointExistedInstruction,
     EndpointHadInstruction,
 )
@@ -90,33 +94,50 @@
                     raise TypeError(
                         "All versioned endpoints must be asynchronous.",
                     )
                 route.endpoint = versions.versioned()(route.endpoint)
         routers = {}
         for version in versions.versions:
             if latest_schemas_module:
-                version_dir = _get_versioned_schema_dir_name(latest_schemas_module, version.date)
+                version_dir = _get_version_dir_path(latest_schemas_module, version.date)
                 if not version_dir.is_dir():
-                    raise RouterGenerationError(f"Versioned schema directory '{version_dir}' does not exist.")
+                    raise RouterGenerationError(
+                        f"Versioned schema directory '{version_dir}' does not exist.",
+                    )
                 for route in router.routes:
                     if isinstance(route, APIRoute):
                         if route.response_model is not None:
                             route.response_model = _change_versions_of_all_annotations(
                                 route.response_model,
                                 version_dir,
                             )
                         # TODO: Write a test for this line
-                        route.dependencies = _change_versions_of_all_annotations(route.dependencies, version_dir)
-                        route.endpoint = _change_versions_of_all_annotations(route.endpoint, version_dir)
-                        route.dependant = get_dependant(path=route.path_format, call=route.endpoint)
-                        route.body_field = get_body_field(dependant=route.dependant, name=route.unique_id)
+                        route.dependencies = _change_versions_of_all_annotations(
+                            route.dependencies,
+                            version_dir,
+                        )
+                        route.endpoint = _change_versions_of_all_annotations(
+                            route.endpoint,
+                            version_dir,
+                        )
+                        route.dependant = get_dependant(
+                            path=route.path_format,
+                            call=route.endpoint,
+                        )
+                        route.body_field = get_body_field(
+                            dependant=route.dependant,
+                            name=route.unique_id,
+                        )
                         for depends in route.dependencies[::-1]:
                             route.dependant.dependencies.insert(
                                 0,
-                                get_parameterless_sub_dependant(depends=depends, path=route.path_format),
+                                get_parameterless_sub_dependant(
+                                    depends=depends,
+                                    path=route.path_format,
+                                ),
                             )
                         route.app = request_response(route.get_route_handler())
 
             routers[version.date] = router
             router = deepcopy(router)
             for version_change in version.version_changes:
                 for instruction in version_change.alter_endpoint_instructions:
@@ -161,34 +182,45 @@
                         assert_never(instruction)
         return routers
 
 
 def _change_versions_of_all_annotations(annotation: Any, version_dir: Path) -> Any:
     if isinstance(annotation, dict):
         return {
-            _change_versions_of_all_annotations(key, version_dir): _change_versions_of_all_annotations(
+            _change_versions_of_all_annotations(
+                key,
+                version_dir,
+            ): _change_versions_of_all_annotations(
                 value,
                 version_dir,
             )
             for key, value in annotation.items()
         }
 
     elif isinstance(annotation, list | tuple):
-        return type(annotation)(_change_versions_of_all_annotations(v, version_dir) for v in annotation)
+        return type(annotation)(
+            _change_versions_of_all_annotations(v, version_dir) for v in annotation
+        )
     else:
         return _memoized_change_versions_of_all_annotations(annotation, version_dir)
 
 
 # This cache is not here for speeding things up. It's for preventing the creation of copies of the same object
 # because such copies could produce weird behaviors at runtime, especially if you/fastapi do any comparisons.
 @functools.cache
-def _memoized_change_versions_of_all_annotations(annotation: Any, version_dir: Path) -> Any:
+def _memoized_change_versions_of_all_annotations(
+    annotation: Any,
+    version_dir: Path,
+) -> Any:
     if isinstance(annotation, _BaseGenericAlias | GenericAlias):
         return _change_versions_of_all_annotations(get_origin(annotation), version_dir)[
-            tuple(_change_versions_of_all_annotations(arg, version_dir) for arg in get_args(annotation))
+            tuple(
+                _change_versions_of_all_annotations(arg, version_dir)
+                for arg in get_args(annotation)
+            )
         ]
     elif isinstance(annotation, Depends):
         return Depends(
             _change_versions_of_all_annotations(annotation.dependency, version_dir),
             use_cache=annotation.use_cache,
         )
     elif isinstance(annotation, type):
@@ -217,48 +249,65 @@
 
         # Otherwise it will have the same signature as __wrapped__
         del new_callable.__wrapped__
         old_params = inspect.signature(annotation).parameters
         callable_annotations = new_callable.__annotations__
 
         new_callable: Any = cast(Any, new_callable)
-        new_callable.__annotations__ = _change_versions_of_all_annotations(callable_annotations, version_dir)
+        new_callable.__annotations__ = _change_versions_of_all_annotations(
+            callable_annotations,
+            version_dir,
+        )
         new_callable.__defaults__ = _change_versions_of_all_annotations(
-            tuple(p.default for p in old_params.values() if p.default is not inspect.Signature.empty),
+            tuple(
+                p.default
+                for p in old_params.values()
+                if p.default is not inspect.Signature.empty
+            ),
             version_dir=version_dir,
         )
         new_callable.__signature__ = _generate_signature(new_callable, old_params)
         return new_callable
     else:
         return annotation
 
 
-def _generate_signature(new_callable: Callable, old_params: MappingProxyType[str, inspect.Parameter]):
+def _generate_signature(
+    new_callable: Callable,
+    old_params: MappingProxyType[str, inspect.Parameter],
+):
     parameters = []
     default_counter = 0
     for param in old_params.values():
         if param.default is not inspect.Signature.empty:
             default = new_callable.__defaults__[default_counter]
             default_counter += 1
         else:
             default = inspect.Signature.empty
         parameters.append(
             inspect.Parameter(
                 param.name,
                 param.kind,
                 default=default,
-                annotation=new_callable.__annotations__.get(param.name, inspect.Signature.empty),
+                annotation=new_callable.__annotations__.get(
+                    param.name,
+                    inspect.Signature.empty,
+                ),
             ),
         )
     return inspect.Signature(
         parameters=parameters,
-        return_annotation=new_callable.__annotations__.get("return", inspect.Signature.empty),
+        return_annotation=new_callable.__annotations__.get(
+            "return",
+            inspect.Signature.empty,
+        ),
     )
 
 
 def _get_route_index(routes: list[BaseRoute], endpoint: Endpoint):
     for index, route in enumerate(routes):
         if isinstance(route, APIRoute) and (
-            route.endpoint == endpoint or getattr(route.endpoint, "func", None) == endpoint
+            route.endpoint == endpoint
+            or getattr(route.endpoint, "func", None) == endpoint
         ):
             return index
     return None
```

### Comparing `universi-0.3.0/universi/structure/endpoints.py` & `universi-0.4.0/universi/structure/endpoints.py`

 * *Files identical despite different names*

### Comparing `universi-0.3.0/universi/structure/enums.py` & `universi-0.4.0/universi/structure/enums.py`

 * *Files identical despite different names*

### Comparing `universi-0.3.0/universi/structure/responses.py` & `universi-0.4.0/universi/structure/responses.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,17 @@
     endpoints: tuple[Endpoint, ...]
     method: Callable[[type, dict[str, Any]], None]
     owner: type = field(init=False)
 
     def __post_init__(self):
         signature = inspect.signature(self.method)
         if list(signature.parameters) != ["cls", "data"]:
-            raise ValueError(f"Method '{self.method.__name__}' must have 2 parameters: cls and data")
+            raise ValueError(
+                f"Method '{self.method.__name__}' must have 2 parameters: cls and data",
+            )
 
         functools.update_wrapper(self, self.method)
 
     def __set_name__(self, owner, name):
         self.owner = owner
 
     def __call__(self, data: dict[str, Any]) -> None:
```

### Comparing `universi-0.3.0/universi/structure/schemas.py` & `universi-0.4.0/universi/structure/schemas.py`

 * *Files 0% similar despite different names*

```diff
@@ -135,15 +135,17 @@
         return OldSchemaHadField(field_name=self.name, type=type, field=info)
 
 
 def field(name: str, /) -> AlterSchemaSubInstructionFactory:
     return AlterSchemaSubInstructionFactory(name=name)
 
 
-AlterSchemaSubInstruction = OldSchemaFieldWas | OldSchemaDidntHaveField | OldSchemaHadField
+AlterSchemaSubInstruction = (
+    OldSchemaFieldWas | OldSchemaDidntHaveField | OldSchemaHadField
+)
 
 
 @dataclass
 class AlterSchemaInstruction:
     schema: type[BaseModel]
     changes: Sequence[AlterSchemaSubInstruction]
```

### Comparing `universi-0.3.0/universi/structure/versions.py` & `universi-0.4.0/universi/structure/versions.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,46 +16,61 @@
 from .common import Endpoint, VersionedModel
 from .responses import AlterResponseInstruction
 from .schemas import AlterSchemaInstruction
 
 _P = ParamSpec("_P")
 _R = TypeVar("_R")
 VersionDate: TypeAlias = datetime.date
-PossibleInstructions: TypeAlias = AlterSchemaInstruction | AlterEndpointSubInstruction | AlterEnumSubInstruction
+PossibleInstructions: TypeAlias = (
+    AlterSchemaInstruction | AlterEndpointSubInstruction | AlterEnumSubInstruction
+)
 
 
 class AbstractVersionChange:
     side_effects: ClassVar[bool] = False
     description: ClassVar[str] = Sentinel
-    instructions_to_migrate_to_previous_version: ClassVar[Sequence[PossibleInstructions]] = Sentinel
+    instructions_to_migrate_to_previous_version: ClassVar[
+        Sequence[PossibleInstructions]
+    ] = Sentinel
     alter_schema_instructions: ClassVar[Sequence[AlterSchemaInstruction]] = Sentinel
     alter_enum_instructions: ClassVar[Sequence[AlterEnumSubInstruction]] = Sentinel
-    alter_endpoint_instructions: ClassVar[Sequence[AlterEndpointSubInstruction]] = Sentinel
-    alter_response_instructions: ClassVar[dict[Endpoint, AlterResponseInstruction]] = Sentinel
+    alter_endpoint_instructions: ClassVar[
+        Sequence[AlterEndpointSubInstruction]
+    ] = Sentinel
+    alter_response_instructions: ClassVar[
+        dict[Endpoint, AlterResponseInstruction]
+    ] = Sentinel
 
     def __init_subclass__(cls) -> None:
         if not isinstance(cls.side_effects, bool):
-            raise UniversiStructureError(f"Side effects must be bool. Found: {type(cls.side_effects)}")
+            raise UniversiStructureError(
+                f"Side effects must be bool. Found: {type(cls.side_effects)}",
+            )
         if cls.description is Sentinel:
-            raise UniversiStructureError(f"Version change description is not set on '{cls.__name__}' but is required.")
+            raise UniversiStructureError(
+                f"Version change description is not set on '{cls.__name__}' but is required.",
+            )
         if cls.instructions_to_migrate_to_previous_version is Sentinel:
             raise UniversiStructureError(
                 f"Attribute 'instructions_to_migrate_to_previous_version' is not set on '{cls.__name__}' but is required.",
             )
         if not isinstance(cls.instructions_to_migrate_to_previous_version, Sequence):
             raise UniversiStructureError(
                 f"Attribute 'instructions_to_migrate_to_previous_version' must be a sequence in '{cls.__name__}'.",
             )
         for instruction in cls.instructions_to_migrate_to_previous_version:
             if not isinstance(instruction, PossibleInstructions):
                 raise UniversiStructureError(
                     f"Instruction '{instruction}' is not allowed. Please, use the correct instruction types",
                 )
         for attr_name, attr_value in cls.__dict__.items():
-            if not isinstance(attr_value, AlterResponseInstruction) and attr_name not in {
+            if not isinstance(
+                attr_value,
+                AlterResponseInstruction,
+            ) and attr_name not in {
                 "description",
                 "side_effects",
                 "instructions_to_migrate_to_previous_version",
                 "__module__",
                 "__doc__",
             }:
                 raise UniversiStructureError(
@@ -105,26 +120,31 @@
         *version_changes: type[AbstractVersionChange],
     ) -> None:
         self.date = date
         self.version_changes = version_changes
 
 
 class Versions:
-    def __init__(self, *versions: Version, api_version_var: ContextVar[VersionDate | None] = api_version_var) -> None:
+    def __init__(
+        self,
+        *versions: Version,
+        api_version_var: ContextVar[VersionDate | None] = api_version_var,
+    ) -> None:
         self.versions = versions
         self.api_version_var = api_version_var
         if sorted(versions, key=lambda v: v.date, reverse=True) != list(versions):
             raise ValueError(
                 "Versions are not sorted correctly. Please sort them in descending order.",
             )
 
     @functools.cached_property
     def versioned_schemas(self) -> dict[str, type[VersionedModel]]:
         return {
-            instruction.schema.__module__ + instruction.schema.__name__: instruction.schema
+            instruction.schema.__module__
+            + instruction.schema.__name__: instruction.schema
             for version in self.versions
             for version_change in version.version_changes
             for instruction in version_change.alter_schema_instructions
         }
 
     @functools.cached_property
     def versioned_enums(self) -> dict[str, type[Enum]]:
@@ -132,16 +152,22 @@
             instruction.enum.__module__ + instruction.enum.__name__: instruction.enum
             for version in self.versions
             for version_change in version.version_changes
             for instruction in version_change.alter_enum_instructions
         }
 
     @functools.cached_property
-    def _version_changes_to_version_mapping(self) -> dict[type[AbstractVersionChange], VersionDate]:
-        return {version_change: version.date for version in self.versions for version_change in version.version_changes}
+    def _version_changes_to_version_mapping(
+        self,
+    ) -> dict[type[AbstractVersionChange], VersionDate]:
+        return {
+            version_change: version.date
+            for version in self.versions
+            for version_change in version.version_changes
+        }
 
     def is_active(self, version_change: type[AbstractVersionChange]) -> bool:
         api_version = self.api_version_var.get()
         if api_version is None:
             return True
         return self._version_changes_to_version_mapping[version_change] <= api_version
```

