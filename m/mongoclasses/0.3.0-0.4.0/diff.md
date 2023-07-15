# Comparing `tmp/mongoclasses-0.3.0.tar.gz` & `tmp/mongoclasses-0.4.0.tar.gz`

## Comparing `mongoclasses-0.3.0.tar` & `mongoclasses-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,27 @@
--rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/.python-version
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/docs/apiref.md
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/docs/index.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/__about__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/__init__.py
--rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/asyncio.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/asyncio.pyi
--rw-r--r--   0        0        0     1879 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/dataclass.py
--rw-r--r--   0        0        0      825 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/dataclass.pyi
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/sync.py
--rw-r--r--   0        0        0      966 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/src/mongoclasses/sync.pyi
--rw-r--r--   0        0        0     2884 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/tests/test_asyncio.py
--rw-r--r--   0        0        0     5585 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/tests/test_dataclass.py
--rw-r--r--   0        0        0     2555 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/tests/test_sync.py
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/.gitignore
--rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/README.md
--rw-r--r--   0        0        0     1239 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     1390 2020-02-02 00:00:00.000000 mongoclasses-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/.python-version
+-rw-r--r--   0        0        0      974 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/mkdocs.yml
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/docs/apiref.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/docs/conversions.md
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/docs/index.md
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/__about__.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/__init__.py
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/asyncio.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/asyncio.pyi
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/converters.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/converters.pyi
+-rw-r--r--   0        0        0      706 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/cursors.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/cursors.pyi
+-rw-r--r--   0        0        0      998 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/mongoclasses.py
+-rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/mongoclasses.pyi
+-rw-r--r--   0        0        0     3677 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/sync.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/src/mongoclasses/sync.pyi
+-rw-r--r--   0        0        0     3174 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     3082 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/tests/test_converters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/tests/test_cursors.py
+-rw-r--r--   0        0        0     2823 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/tests/test_mongoclasses.py
+-rw-r--r--   0        0        0     3539 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/tests/test_sync.py
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/.gitignore
+-rw-r--r--   0        0        0     1100 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/LICENSE.txt
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/README.md
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 mongoclasses-0.4.0/PKG-INFO
```

### Comparing `mongoclasses-0.3.0/docs/index.md` & `mongoclasses-0.4.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `mongoclasses-0.3.0/src/mongoclasses/asyncio.pyi` & `mongoclasses-0.4.0/src/mongoclasses/asyncio.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,14 @@
-from typing import Any, Callable, TypeAlias, TYPE_CHECKING
+from typing import Any
 from pymongo.results import DeleteResult, InsertOneResult, UpdateResult
-from .dataclass import MongoclassInstance, Data
-
-if TYPE_CHECKING:
-    from _typeshed import DataclassInstance
-
-DictFactory: TypeAlias = Callable[[list[tuple[str, Any]]], Data]
-
-
-async def insert_one(
-    obj: MongoclassInstance, /, dict_factory: DictFactory
-) -> InsertOneResult:
-    ...
-
+from .mongoclasses import MongoclassInstance
 
+async def insert_one(obj: MongoclassInstance, /) -> InsertOneResult: ...
 async def update_one(
-    obj: MongoclassInstance, /, dict_factory: DictFactory
-) -> UpdateResult:
-    ...
-
-
-async def delete_one(obj: MongoclassInstance, /) -> DeleteResult:
-    ...
-
-
+    obj: MongoclassInstance, /, fields: list[str] | None
+) -> UpdateResult: ...
+async def delete_one(obj: MongoclassInstance, /) -> DeleteResult: ...
 async def find_one(
     cls: type[MongoclassInstance],
     /,
-    query: Data,
-    fromdict: Callable[[type[DataclassInstance], Data], DataclassInstance],
-) -> MongoclassInstance | None:
-    ...
+    filter: dict[str, Any] | None,
+) -> MongoclassInstance | None: ...
```

### Comparing `mongoclasses-0.3.0/tests/test_asyncio.py` & `mongoclasses-0.4.0/tests/test_asyncio.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,28 @@
     await update_one(f)
 
     doc = await Foo.collection.find_one({"_id": f._id})
     assert doc["name"] == "Fred"
 
 
 @pytest.mark.asyncio
+async def test_update_one_with_fields(Foo):
+    f = Foo()
+    await insert_one(f)
+
+    f.name = "Fred"
+    f.description = "Hello World"
+    await update_one(f, fields=["name"])
+
+    doc = await Foo.collection.find_one({"_id": f._id})
+    assert doc["name"] == "Fred"
+    assert doc["description"] == ""
+
+
+@pytest.mark.asyncio
 async def test_delete_one(Foo):
     f = Foo()
     await insert_one(f)
     await delete_one(f)
 
     assert await Foo.collection.find_one({"_id": f._id}) is None
 
@@ -103,31 +117,28 @@
 
     f3 = Foo(name="Charlie")
     await insert_one(f3)
 
     cursor = find(Foo, {})
     objects = [foo async for foo in cursor]
     assert len(objects) == 3
+    for obj in objects:
+        assert isinstance(obj, Foo)
 
 
 @pytest.mark.asyncio
-async def test_non_mongoclasses_in_mongoclass_functions():
+async def test_not_a_mongoclass():
+    @dataclass
     class Foo:
         ...
-
+    
     with pytest.raises(TypeError):
-        f = Foo()
-        await insert_one(f)
-
+        await insert_one(Foo())
+    
     with pytest.raises(TypeError):
-        f = Foo()
-        await update_one(f)
-
+        await update_one(Foo())
+    
     with pytest.raises(TypeError):
-        f = Foo()
-        await delete_one(f)
+        await delete_one(Foo())
 
     with pytest.raises(TypeError):
         await find_one(Foo, {})
-
-    with pytest.raises(TypeError):
-        find(Foo, {})
```

### Comparing `mongoclasses-0.3.0/.gitignore` & `mongoclasses-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `mongoclasses-0.3.0/LICENSE.txt` & `mongoclasses-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mongoclasses-0.3.0/pyproject.toml` & `mongoclasses-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "mongoclasses"
 dynamic = ["version"]
-description = ''
+description = "A lightweight tool for performing MongoDB operations on python dataclasses."
 readme = "README.md"
 requires-python = ">=3.8"
 license = "MIT"
 keywords = []
 authors = [
   { name = "Ryan Kroon", email = "rykroon.tech@gmail.com" },
 ]
@@ -20,14 +20,15 @@
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = [
+  "cattrs==23.1.2, <24",
   "motor>=3.1.1, <4"
 ]
 
 [project.urls]
 Documentation = "https://github.com/rykroon/mongoclasses#readme"
 Issues = "https://github.com/rykroon/mongoclasses/issues"
 Source = "https://github.com/rykroon/mongoclasses"
@@ -43,7 +44,26 @@
 ]
 [tool.hatch.envs.test.scripts]
 test = "coverage run -m pytest"
 cov-report = "coverage report -m"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["3.8", "3.9", "3.10", "3.11"]
+
+[tool.hatch.envs.mypy]
+python="3.11"
+dependencies = [
+  "mypy"
+]
+[tool.hatch.envs.mypy.scripts]
+strict = "mypy --strict src/mongoclasses"
+
+[tool.hatch.envs.docs]
+python="3.11"
+dependencies = [
+  "mkdocs",
+  "mkdocs-material",
+  "mkdocstrings[python]",
+]
+[tool.hatch.envs.docs.scripts]
+build = "mkdocs build --clean --strict"
+serve = "mkdocs serve"
```

