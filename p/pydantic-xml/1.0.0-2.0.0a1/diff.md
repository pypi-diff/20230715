# Comparing `tmp/pydantic_xml-1.0.0.tar.gz` & `tmp/pydantic_xml-2.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-1.0.0.tar", max compression
+gzip compressed data, was "pydantic_xml-2.0.0a1.tar", max compression
```

## Comparing `pydantic_xml-1.0.0.tar` & `pydantic_xml-2.0.0a1.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1211 2023-07-15 06:45:26.804304 pydantic_xml-1.0.0/LICENSE
--rw-r--r--   0        0        0     3192 2023-07-15 06:45:26.804304 pydantic_xml-1.0.0/README.rst
--rw-r--r--   0        0        0      599 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/config.py
--rw-r--r--   0        0        0       80 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    13330 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      374 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1671 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1173 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      569 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/errors.py
--rw-r--r--   0        0        0    11708 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/model.py
--rw-r--r--   0        0        0        0 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/py.typed
--rw-r--r--   0        0        0       73 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0     1445 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/encoder.py
--rw-r--r--   0        0        0      394 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     1898 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/forwardref.py
--rw-r--r--   0        0        0     4612 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     4337 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0     4894 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0     6903 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     4220 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     6693 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     3292 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0     7364 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0       48 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     2131 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/utils.py
--rw-r--r--   0        0        0     1879 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4697 1970-01-01 00:00:00.000000 pydantic_xml-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-15 07:13:13.144047 pydantic_xml-2.0.0a1/LICENSE
+-rw-r--r--   0        0        0     3335 2023-07-15 07:13:13.144047 pydantic_xml-2.0.0a1/README.rst
+-rw-r--r--   0        0        0      453 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/config.py
+-rw-r--r--   0        0        0       80 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    13335 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      374 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1173 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      712 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    12182 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/model.py
+-rw-r--r--   0        0        0        0 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       36 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0       99 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     3270 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     3174 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0     5289 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0    11102 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     5271 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     1428 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/typed_mapping.py
+-rw-r--r--   0        0        0     4915 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     2543 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0     9374 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0      322 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     2131 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     1876 2023-07-15 07:13:13.148047 pydantic_xml-2.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     4833 1970-01-01 00:00:00.000000 pydantic_xml-2.0.0a1/PKG-INFO
```

### Comparing `pydantic_xml-1.0.0/LICENSE` & `pydantic_xml-2.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-1.0.0/README.rst` & `pydantic_xml-2.0.0a1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -18,53 +18,55 @@
     :target: https://codecov.io/gh/dapper91/pydantic-xml
     :alt: Code coverage
 .. image:: https://readthedocs.org/projects/pydantic-xml/badge/?version=stable&style=flat
    :alt: ReadTheDocs status
    :target: https://pydantic-xml.readthedocs.io/en/stable/
 
 
-``pydantic-xml`` is a `pydantic <https://docs.pydantic.dev/1.10/>`_ extension providing model fields xml binding
+``pydantic-xml`` is a `pydantic <https://docs.pydantic.dev>`_ extension providing model fields xml binding
 and xml serialization / deserialization.
 It is closely integrated with ``pydantic`` which means it supports most of its features.
 
 
 Features
 --------
 
+- pydantic v1 / v2 support
 - flexable attributes, elements and text binding
-- python collection types support (``Dict``, ``List``, ``Set``, ``Tuple``, ...)
+- python collection types support (``Dict``, ``TypedDict``, ``List``, ``Set``, ``Tuple``, ...)
 - ``Union`` type support
-- pydantic `generic <https://docs.pydantic.dev/1.10/usage/models/#generic-models>`_ models support
+- pydantic `generic models <https://docs.pydantic.dev/latest/usage/models/#generic-models>`_ support
+- pydantic `computed fields <https://docs.pydantic.dev/latest/usage/computed_fields/>`_ support
 - `lxml <https://lxml.de/>`_ xml parser support
 - ``xml.etree.ElementTree`` standard library xml parser support
 
 What is not supported?
 ______________________
 
-- `dynamic model creation <https://docs.pydantic.dev/1.10/usage/models/#dynamic-model-creation>`_
-- `dataclasses <https://docs.pydantic.dev/1.10/usage/dataclasses/>`_
-- `discriminated unions <https://docs.pydantic.dev/1.10/usage/types/#discriminated-unions-aka-tagged-unions>`_
+- `dynamic model creation <https://docs.pydantic.dev/usage/models/#dynamic-model-creation>`_
+- `dataclasses <https://docs.pydantic.dev/usage/dataclasses/>`_
+- `discriminated unions <https://docs.pydantic.dev/usage/types/#discriminated-unions-aka-tagged-unions>`_
 
 Getting started
 ---------------
 
 The following model fields binding:
 
 .. code-block:: python
 
    class Product(BaseXmlModel):
        status: Literal['running', 'development'] = attr()  # extracted from the 'status' attribute
-       launched: Optional[int] = attr()  # extracted from the 'launched' attribute
+       launched: Optional[int] = attr(default=None)  # extracted from the 'launched' attribute
        title: str  # extracted from the element text
 
 
    class Company(BaseXmlModel):
        trade_name: str = attr(name='trade-name')  # extracted from the 'trade-name' attribute
        website: HttpUrl = element()  # extracted from the 'website' element text
-       products: List[Product] = element(tag='product')  # extracted from the 'website' element
+       products: List[Product] = element(tag='product', default=[])  # extracted from the 'website' element
 
 defines the XML document:
 
 .. code-block:: xml
 
    <Company trade-name="SpaceX">
        <website>https://www.spacex.com</website>
```

### Comparing `pydantic_xml-1.0.0/pydantic_xml/element/element.py` & `pydantic_xml-2.0.0a1/pydantic_xml/element/element.py`

 * *Files 0% similar despite different names*

```diff
@@ -316,26 +316,26 @@
     """
 
     STRICT = 'strict'
     ORDERED = 'ordered'
     UNORDERED = 'unordered'
 
 
-Searcher = Callable[[XmlElement.State[NativeElement], str, bool], Optional[XmlElement]]
+Searcher = Callable[[XmlElement.State[NativeElement], str, bool], Optional[XmlElement[NativeElement]]]
 
 
 def get_searcher(search_mode: SearchMode) -> Searcher[NativeElement]:
     if search_mode == SearchMode.STRICT:
         return strict_search
     elif search_mode == SearchMode.ORDERED:
         return ordered_search
     elif search_mode == SearchMode.UNORDERED:
         return unordered_search
     else:
-        raise AssertionError('unreachable')
+        raise AssertionError("unreachable")
 
 
 def strict_search(
         state: XmlElement.State[NativeElement],
         tag: str,
         look_behind: bool = False,
 ) -> Optional[XmlElement[NativeElement]]:
@@ -370,15 +370,15 @@
 
     :param state: element state
     :param tag: sub-element tag for be searched for
     :param look_behind: look for a previous element
     :return: found element or `None` if the element not found
     """
 
-    result: Optional[XmlElement[NativeElement]] = None
+    result: Optional[XmlElement[Any]] = None
 
     if look_behind and (result := _look_behind(state, tag)) is not None:
         return result
 
     next_element_idx = state.next_element_idx
     while next_element_idx < len(state.elements):
         element = state.elements[next_element_idx]
```

### Comparing `pydantic_xml-1.0.0/pydantic_xml/element/native/lxml.py` & `pydantic_xml-2.0.0a1/pydantic_xml/element/native/lxml.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-1.0.0/pydantic_xml/element/native/std.py` & `pydantic_xml-2.0.0a1/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-1.0.0/pydantic_xml/model.py` & `pydantic_xml-2.0.0a1/pydantic_xml/model.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,232 +1,246 @@
-import functools as ft
+import dataclasses as dc
 import typing
-from typing import Any, Callable, ClassVar, Dict, Optional, Tuple, Type, TypeVar, Union
+from typing import Any, Callable, ClassVar, Dict, Generic, Optional, Tuple, Type, TypeVar, Union
 
 import pydantic as pd
-import pydantic.fields
-import pydantic.generics
-import pydantic.json
+import pydantic_core as pdc
+from pydantic import BaseModel, RootModel
 
-from . import config, errors, serializers, utils
+from . import config, errors, utils
 from .element import SearchMode
 from .element.native import XmlElement, etree
-from .serializers.factories import ModelSerializerFactory
-from .utils import NsMap, register_nsmap
-
-
-class XmlEntityInfo(pd.fields.FieldInfo):
+from .serializers.factories.model import BaseModelSerializer
+from .serializers.serializer import Serializer, XmlEntityInfoP
+from .typedefs import EntityLocation
+from .utils import NsMap
+
+__all__ = (
+    'attr',
+    'element',
+    'wrapped',
+    'computed_attr',
+    'computed_element',
+    'BaseXmlModel',
+    'RootXmlModel',
+)
+
+
+@dc.dataclass
+class ComputedXmlEntityInfo(pd.fields.ComputedFieldInfo):
+    """
+    Computed field xml meta-information.
+    """
+
+    __slots__ = ('location', 'path', 'ns', 'nsmap', 'wrapped')
+
+    location: Optional[EntityLocation]
+    path: Optional[str]
+    ns: Optional[str]
+    nsmap: Optional[NsMap]
+    wrapped: Optional[XmlEntityInfoP]  # to be compliant with XmlEntityInfoP protocol
+
+    def __post_init__(self) -> None:
+        if config.REGISTER_NS_PREFIXES and self.nsmap:
+            utils.register_nsmap(self.nsmap)
+
+
+PropertyT = typing.TypeVar('PropertyT')
+
+
+def computed_entity(
+        location: EntityLocation,
+        prop: Optional[PropertyT] = None,
+        **kwargs: Any,
+) -> Union[PropertyT, Callable[[PropertyT], PropertyT]]:
+    def decorator(prop: Any) -> Any:
+        path = kwargs.pop('path', None)
+        ns = kwargs.pop('ns', None)
+        nsmap = kwargs.pop('nsmap', None)
+
+        descriptor_proxy = pd.computed_field(**kwargs)(prop)
+        descriptor_proxy.decorator_info = ComputedXmlEntityInfo(
+            location=location,
+            path=path,
+            ns=ns,
+            nsmap=nsmap,
+            wrapped=None,
+            **dc.asdict(descriptor_proxy.decorator_info),
+        )
+
+        return descriptor_proxy
+
+    if prop is None:
+        return decorator
+    else:
+        return decorator(prop)
+
+
+def computed_attr(
+        prop: Optional[PropertyT] = None,
+        *,
+        name: Optional[str] = None,
+        ns: Optional[str] = None,
+        **kwargs: Any,
+) -> Union[PropertyT, Callable[[PropertyT], PropertyT]]:
     """
-    Field xml meta-information.
-    """
-
-
-class XmlAttributeInfo(XmlEntityInfo):
-    """
-    Field xml attribute meta-information.
+    Marks a property as an xml attribute.
 
+    :param prop: decorated property
     :param name: attribute name
     :param ns: attribute xml namespace
-    :param kwargs: pydantic field arguments. See :py:class:`pydantic.Field`
+    :param kwargs: pydantic computed field arguments. See :py:class:`pydantic.computed_field`
     """
 
-    __slots__ = ('_name', '_ns')
-
-    def __init__(
-            self,
-            name: Optional[str] = None,
-            ns: Optional[str] = None,
-            **kwargs: Any,
-    ):
-        super().__init__(**kwargs)
-        self._name = name
-        self._ns = ns
-
-    @property
-    def name(self) -> Optional[str]:
-        return self._name
+    return computed_entity(EntityLocation.ATTRIBUTE, prop, path=name, ns=ns, **kwargs)
 
-    @property
-    def ns(self) -> Optional[str]:
-        return self._ns
 
-
-class XmlElementInfo(XmlEntityInfo):
+def computed_element(
+        prop: Optional[PropertyT] = None,
+        *,
+        tag: Optional[str] = None,
+        ns: Optional[str] = None,
+        nsmap: Optional[NsMap] = None,
+        **kwargs: Any,
+) -> Union[PropertyT, Callable[[PropertyT], PropertyT]]:
     """
-    Field xml element meta-information.
+    Marks a property as an xml element.
 
+    :param prop: decorated property
     :param tag: element tag
     :param ns: element xml namespace
     :param nsmap: element xml namespace map
-    :param kwargs: pydantic field arguments
+    :param kwargs: pydantic computed field arguments. See :py:class:`pydantic.computed_field`
     """
 
-    __slots__ = ('_tag', '_ns', '_nsmap')
+    return computed_entity(EntityLocation.ELEMENT, prop, path=tag, ns=ns, nsmap=nsmap, **kwargs)
 
-    def __init__(
-            self,
-            tag: Optional[str] = None,
-            ns: Optional[str] = None,
-            nsmap: Optional[NsMap] = None,
-            **kwargs: Any,
-    ):
-        super().__init__(**kwargs)
-        self._tag = tag
-        self._ns = ns
-        self._nsmap = nsmap
-
-        if config.REGISTER_NS_PREFIXES and nsmap:
-            register_nsmap(nsmap)
 
-    @property
-    def tag(self) -> Optional[str]:
-        return self._tag
-
-    @property
-    def ns(self) -> Optional[str]:
-        return self._ns
-
-    @property
-    def nsmap(self) -> Optional[NsMap]:
-        return self._nsmap
-
-
-class XmlWrapperInfo(XmlEntityInfo):
+class XmlEntityInfo(pd.fields.FieldInfo):
     """
-    Field xml wrapper meta-information.
-
-    :param entity: wrapped entity
-    :param path: entity path
-    :param ns: element xml namespace
-    :param nsmap: element xml namespace map
-    :param kwargs: pydantic field arguments
+    Field xml meta-information.
     """
 
-    __slots__ = ('_entity', '_path', '_ns', '_nsmap')
+    __slots__ = ('location', 'path', 'ns', 'nsmap', 'wrapped')
 
     def __init__(
             self,
-            path: str,
-            entity: Optional[XmlEntityInfo] = None,
+            location: Optional[EntityLocation],
+            /,
+            path: Optional[str] = None,
             ns: Optional[str] = None,
             nsmap: Optional[NsMap] = None,
+            wrapped: Optional[pd.fields.FieldInfo] = None,
             **kwargs: Any,
     ):
-        if entity is not None:
+        if wrapped is not None:
             # copy arguments from the wrapped entity to let pydantic know how to process the field
-            for entity_field_name in utils.get_slots(entity):
-                kwargs[entity_field_name] = getattr(entity, entity_field_name)
-
-        super().__init__(**kwargs)
-        self._entity = entity
-        self._path = path
-        self._ns = ns
-        self._nsmap = nsmap
-
-        if config.REGISTER_NS_PREFIXES and nsmap:
-            register_nsmap(nsmap)
+            for entity_field_name in utils.get_slots(wrapped):
+                kwargs[entity_field_name] = getattr(wrapped, entity_field_name)
 
-    @property
-    def entity(self) -> Optional[XmlEntityInfo]:
-        return self._entity
+        if kwargs.get('serialization_alias') is None:
+            kwargs['serialization_alias'] = kwargs.get('alias')
 
-    @property
-    def path(self) -> str:
-        return self._path
+        if kwargs.get('validation_alias') is None:
+            kwargs['validation_alias'] = kwargs.get('alias')
 
-    @property
-    def ns(self) -> Optional[str]:
-        return self._ns
+        super().__init__(**kwargs)
+        self.location = location
+        self.path = path
+        self.ns = ns
+        self.nsmap = nsmap
+        self.wrapped: Optional[XmlEntityInfoP] = wrapped if isinstance(wrapped, XmlEntityInfo) else None
 
-    @property
-    def nsmap(self) -> Optional[NsMap]:
-        return self._nsmap
+        if config.REGISTER_NS_PREFIXES and nsmap:
+            utils.register_nsmap(nsmap)
 
 
-def attr(**kwargs: Any) -> Any:
+def attr(name: Optional[str] = None, ns: Optional[str] = None, **kwargs: Any) -> Any:
     """
     Marks a pydantic field as an xml attribute.
 
-    :param kwargs: see :py:class:`pydantic_xml.XmlAttributeInfo`
+    :param name: attribute name
+    :param ns: attribute xml namespace
+    :param kwargs: pydantic field arguments. See :py:class:`pydantic.Field`
     """
 
-    return XmlAttributeInfo(**kwargs)
+    return XmlEntityInfo(EntityLocation.ATTRIBUTE, path=name, ns=ns, **kwargs)
 
 
-def element(**kwargs: Any) -> Any:
+def element(tag: Optional[str] = None, ns: Optional[str] = None, nsmap: Optional[NsMap] = None, **kwargs: Any) -> Any:
     """
     Marks a pydantic field as an xml element.
 
-    :param kwargs: see :py:class:`pydantic_xml.XmlElementInfo`
+    :param tag: element tag
+    :param ns: element xml namespace
+    :param nsmap: element xml namespace map
+    :param kwargs: pydantic field arguments. See :py:class:`pydantic.Field`
     """
 
-    return XmlElementInfo(**kwargs)
+    return XmlEntityInfo(EntityLocation.ELEMENT, path=tag, ns=ns, nsmap=nsmap, **kwargs)
 
 
-def wrapped(*args: Any, **kwargs: Any) -> Any:
+def wrapped(
+        path: str,
+        entity: Optional[pd.fields.FieldInfo] = None,
+        ns: Optional[str] = None,
+        nsmap: Optional[NsMap] = None,
+        **kwargs: Any,
+) -> Any:
     """
     Marks a pydantic field as a wrapped xml entity.
 
-    :param args: see :py:class:`pydantic_xml.XmlWrapperInfo`
-    :param kwargs: see :py:class:`pydantic_xml.XmlWrapperInfo`
+    :param entity: wrapped entity
+    :param path: entity path
+    :param ns: element xml namespace
+    :param nsmap: element xml namespace map
+    :param kwargs: pydantic field arguments. See :py:class:`pydantic.Field`
     """
 
-    return XmlWrapperInfo(*args, **kwargs)
+    return XmlEntityInfo(EntityLocation.WRAPPED, path=path, ns=ns, nsmap=nsmap, wrapped=entity, **kwargs)
 
 
-class XmlModelMeta(pd.main.ModelMetaclass):
+class XmlModelMeta(type(BaseModel)):  # type: ignore[misc]
     """
     Xml model metaclass.
     """
 
-    __is_base_model_defined__ = False
-
-    def __new__(mcls, name: str, bases: Tuple[type], namespace: Dict[str, Any], **kwargs: Any) -> Type['BaseXmlModel']:
-        if mcls.__is_base_model_defined__:
-            mcls._merge_configs(bases, namespace)
+    def __new__(
+            mcls,
+            name: str,
+            bases: Tuple[type],
+            namespace: Dict[str, Any],
+            **kwargs: Any,
+    ) -> Type['BaseXmlModel']:
+        is_abstract: bool = kwargs.pop('__xml_abstract__', False)
 
         cls = super().__new__(mcls, name, bases, namespace, **kwargs)
-        if mcls.__is_base_model_defined__:
-            cls.__init_serializer__()
-        else:
-            mcls.__is_base_model_defined__ = True
+        if not is_abstract:
+            cls.__build_serializer__()
 
         return cls
 
-    @classmethod
-    def _merge_configs(mcls, bases: Tuple[type], namespace: Dict[str, Any]) -> None:
-        xml_encoders: Dict[Type[Any], Callable[[Any], Any]] = {}
-        for base in reversed(bases):
-            if issubclass(base, BaseXmlModel) and base != BaseXmlModel:
-                xml_encoders.update(getattr(base.__config__, 'xml_encoders', {}))
-
-        if self_config := namespace.get('Config'):
-            xml_encoders.update(getattr(self_config, 'xml_encoders', {}))
-            setattr(self_config, 'xml_encoders', xml_encoders)
-
 
 ModelT = TypeVar('ModelT', bound='BaseXmlModel')
 
 
-class BaseXmlModel(pd.BaseModel, metaclass=XmlModelMeta):
+class BaseXmlModel(BaseModel, __xml_abstract__=True, metaclass=XmlModelMeta):
     """
     Base pydantic-xml model.
     """
 
     __xml_tag__: ClassVar[Optional[str]]
     __xml_ns__: ClassVar[Optional[str]]
     __xml_nsmap__: ClassVar[Optional[NsMap]]
     __xml_ns_attrs__: ClassVar[bool]
     __xml_search_mode__: ClassVar[SearchMode]
-    __xml_encoder__: ClassVar[serializers.XmlEncoder]
-    __xml_serializer__: ClassVar[Optional[ModelSerializerFactory.RootSerializer]] = None
+    __xml_serializer__: ClassVar[Optional[BaseModelSerializer]] = None
 
     def __init_subclass__(
             cls,
-            *args: Any,
             tag: Optional[str] = None,
             ns: Optional[str] = None,
             nsmap: Optional[NsMap] = None,
             ns_attrs: Optional[bool] = None,
             search_mode: Optional[SearchMode] = None,
             **kwargs: Any,
     ):
@@ -236,44 +250,60 @@
         :param tag: element tag
         :param ns: element namespace
         :param nsmap: element namespace map
         :param ns_attrs: use namespaced attributes
         :param search_mode: element search mode
         """
 
-        super().__init_subclass__(*args, **kwargs)
+        super().__init_subclass__(**kwargs)
 
         cls.__xml_tag__ = tag if tag is not None else getattr(cls, '__xml_tag__', None)
         cls.__xml_ns__ = ns if ns is not None else getattr(cls, '__xml_ns__', None)
         cls.__xml_nsmap__ = nsmap if nsmap is not None else getattr(cls, '__xml_nsmap__', None)
         cls.__xml_ns_attrs__ = ns_attrs if ns_attrs is not None else getattr(cls, '__xml_ns_attrs__', False)
         cls.__xml_search_mode__ = search_mode if search_mode is not None \
             else getattr(cls, '__xml_search_mode__', SearchMode.STRICT)
 
-        default_xml_encoder: Callable[[Any], Any]
-        if xml_encoders := getattr(cls.Config, 'xml_encoders', None):
-            default_xml_encoder = ft.partial(pd.json.custom_pydantic_encoder, xml_encoders)
-        else:
-            default_xml_encoder = pd.json.pydantic_encoder
+    @classmethod
+    def __build_serializer__(cls) -> None:
+        if cls is BaseXmlModel:
+            return
 
-        cls.__xml_encoder__ = serializers.XmlEncoder(default=default_xml_encoder)
+        if cls.__pydantic_generic_metadata__['parameters']:  # checks that all generic parameters are provided
+            return
 
-    @classmethod
-    def __init_serializer__(cls) -> None:
         if config.REGISTER_NS_PREFIXES and cls.__xml_nsmap__:
-            register_nsmap(cls.__xml_nsmap__)
+            utils.register_nsmap(cls.__xml_nsmap__)
 
-        cls.__xml_serializer__ = ModelSerializerFactory.build_root(cls)
+        if cls.__pydantic_complete__:  # checks that all forward refs are resolved
+            serializer = Serializer.parse_core_schema(
+                schema=cls.__pydantic_core_schema__,
+                ctx=Serializer.Context(
+                    model_name=cls.__name__,
+                    namespaced_attrs=cls.__xml_ns_attrs__,
+                    search_mode=cls.__xml_search_mode__,
+                    entity_info=XmlEntityInfo(
+                        EntityLocation.ELEMENT,
+                        path=cls.__xml_tag__,
+                        ns=cls.__xml_ns__,
+                        nsmap=cls.__xml_nsmap__,
+                    ),
+                ),
+            )
+            assert isinstance(serializer, BaseModelSerializer), "unexpected serializer type"
+            cls.__xml_serializer__ = serializer
+        else:
+            cls.__xml_serializer__ = None
 
     @classmethod
-    def update_forward_refs(cls, **kwargs: Any) -> None:
-        super().update_forward_refs(**kwargs)
+    def model_rebuild(cls, **kwargs: Any) -> None:
+        super().model_rebuild(**kwargs)
 
-        if cls.__xml_serializer__ is not None:
-            cls.__xml_serializer__.resolve_forward_refs()
+        if cls.__xml_serializer__ is None and cls.__pydantic_complete__:
+            cls.__build_serializer__()
 
     @classmethod
     def from_xml_tree(cls: Type[ModelT], root: etree.Element) -> ModelT:
         """
         Deserializes an xml element tree to an object of `cls` type.
 
         :param root: xml element to deserialize the object from
@@ -297,89 +327,55 @@
 
         :param source: xml string
         :return: deserialized object
         """
 
         return cls.from_xml_tree(etree.fromstring(source))
 
-    def to_xml_tree(
-            self,
-            *,
-            encoder: Optional[serializers.XmlEncoder] = None,
-            skip_empty: bool = False,
-    ) -> etree.Element:
+    def to_xml_tree(self, *, skip_empty: bool = False) -> etree.Element:
         """
         Serializes the object to an xml tree.
 
-        :param encoder: xml type encoder
         :param skip_empty: skip empty elements (elements without sub-elements, attributes and text, Nones)
         :return: object xml representation
         """
 
-        encoder = encoder or self.__xml_encoder__
-
         assert self.__xml_serializer__ is not None, f"model {type(self).__name__} is partially initialized"
 
         root = XmlElement(tag=self.__xml_serializer__.element_name, nsmap=self.__xml_serializer__.nsmap)
-        self.__xml_serializer__.serialize(root, self, encoder=encoder, skip_empty=skip_empty)
+        self.__xml_serializer__.serialize(
+            root, self, pdc.to_jsonable_python(self, by_alias=False), skip_empty=skip_empty,
+        )
 
         return root.to_native()
 
-    def to_xml(
-            self,
-            *,
-            encoder: Optional[serializers.XmlEncoder] = None,
-            skip_empty: bool = False,
-            **kwargs: Any,
-    ) -> Union[str, bytes]:
+    def to_xml(self, *, skip_empty: bool = False, **kwargs: Any) -> Union[str, bytes]:
         """
         Serializes the object to an xml string.
 
-        :param encoder: xml type encoder
         :param skip_empty: skip empty elements (elements without sub-elements, attributes and text, Nones)
         :param kwargs: additional xml serialization arguments
         :return: object xml representation
         """
 
-        return etree.tostring(self.to_xml_tree(encoder=encoder, skip_empty=skip_empty), **kwargs)
+        return etree.tostring(self.to_xml_tree(skip_empty=skip_empty), **kwargs)
 
 
-GenericModelT = TypeVar('GenericModelT', bound='BaseGenericXmlModel')
+RootModelRootType = TypeVar('RootModelRootType')
 
 
-class BaseGenericXmlModel(BaseXmlModel, pd.generics.GenericModel):
+class RootXmlModel(  # type: ignore[misc]
+    RootModel[RootModelRootType],
+    BaseXmlModel,
+    Generic[RootModelRootType],
+    __xml_abstract__=True,
+):
     """
-    Base pydantic-xml generic model.
+    Base pydantic-xml root model.
     """
 
-    def __class_getitem__(cls, params: Union[Type[Any], Tuple[Type[Any], ...]]) -> Type[Any]:
-        model = super().__class_getitem__(params)
-        model.__xml_tag__ = cls.__xml_tag__
-        model.__xml_ns__ = cls.__xml_ns__
-        model.__xml_nsmap__ = cls.__xml_nsmap__
-        model.__xml_ns_attrs__ = cls.__xml_ns_attrs__
-        model.__xml_search_mode__ = cls.__xml_search_mode__
-        model.__init_serializer__()
-
-        return model
-
     @classmethod
-    def __init_serializer__(cls) -> None:
-        # checks that the model is not generic
-        if not getattr(cls, '__concrete__', True):
-            cls.__xml_serializer__ = None
-        else:
-            super().__init_serializer__()
-
-    @classmethod
-    def from_xml_tree(cls: Type[GenericModelT], root: etree.Element) -> GenericModelT:
-        """
-        Deserializes an xml element tree to an object of `cls` type.
-
-        :param root: xml element to deserialize the object from
-        :return: deserialized object
-        """
-
-        if cls.__xml_serializer__ is None:
-            raise errors.ModelError(f"{cls.__name__} model is generic")
+    def __build_serializer__(cls) -> None:
+        if cls is RootXmlModel:
+            return
 
-        return super().from_xml_tree(root)
+        super().__build_serializer__()
```

### Comparing `pydantic_xml-1.0.0/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-2.0.0a1/pydantic_xml/serializers/factories/union.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,108 +1,126 @@
-from typing import Any, Optional, Type
+from typing import Any, Dict, List, Optional, Set, Tuple
 
 import pydantic as pd
+from pydantic_core import core_schema as pcs
 
 import pydantic_xml as pxml
+from pydantic_xml import errors
 from pydantic_xml.element import XmlElementReader, XmlElementWriter
-from pydantic_xml.serializers.encoder import XmlEncoder
-from pydantic_xml.serializers.serializer import Location, Serializer
-from pydantic_xml.utils import QName, merge_nsmaps
-
-
-class PrimitiveTypeSerializerFactory:
-    """
-    Primitive type serializer factory.
-    """
-
-    class TextSerializer(Serializer):
-        def serialize(
-                self, element: XmlElementWriter, value: Any, *, encoder: XmlEncoder, skip_empty: bool = False,
-        ) -> Optional[XmlElementWriter]:
-            if value is None and skip_empty:
-                return element
-
-            encoded = encoder.encode(value)
-            element.set_text(encoded)
-            return element
-
-        def deserialize(self, element: Optional[XmlElementReader]) -> Optional[str]:
-            if element is None:
-                return None
-
-            return element.pop_text() or None
-
-    class AttributeSerializer(Serializer):
-        def __init__(
-                self, model: Type['pxml.BaseXmlModel'], model_field: pd.fields.ModelField, ctx: Serializer.Context,
-        ):
-            name, ns, nsmap = self._get_entity_info(model_field)
-            ns_attrs = model.__xml_ns_attrs__
-            name = name or model_field.alias
-            ns = ns or (ctx.parent_ns if ns_attrs else None)
-            nsmap = merge_nsmaps(nsmap, ctx.parent_nsmap)
-
-            self._attr_name = QName.from_alias(tag=name, ns=ns, nsmap=nsmap, is_attr=True).uri
-
-        def serialize(
-                self, element: XmlElementWriter, value: Any, *, encoder: XmlEncoder, skip_empty: bool = False,
-        ) -> Optional[XmlElementWriter]:
-            if value is None and skip_empty:
-                return element
-
-            encoded = encoder.encode(value)
-            element.set_attribute(self._attr_name, encoded)
-
-            return element
-
-        def deserialize(self, element: Optional[XmlElementReader]) -> Optional[str]:
-            if element is None:
-                return None
-
-            return element.pop_attrib(self._attr_name)
-
-    class ElementSerializer(TextSerializer):
-        def __init__(self, model_field: pd.fields.ModelField, ctx: Serializer.Context):
-            name, ns, nsmap = self._get_entity_info(model_field)
-            name = name or model_field.alias
-            ns = ns or ctx.parent_ns
-            self._search_mode = ctx.search_mode
-            self._nsmap = nsmap = merge_nsmaps(nsmap, ctx.parent_nsmap)
-            self._element_name = QName.from_alias(tag=name, ns=ns, nsmap=nsmap).uri
-
-        def serialize(
-                self, element: XmlElementWriter, value: Any, *, encoder: XmlEncoder, skip_empty: bool = False,
-        ) -> Optional[XmlElementWriter]:
-            if value is None and skip_empty:
-                return element
-
-            sub_element = element.make_element(self._element_name, nsmap=self._nsmap)
-            super().serialize(sub_element, value, encoder=encoder, skip_empty=skip_empty)
-            if skip_empty and sub_element.is_empty():
-                return None
-            else:
-                element.append_element(sub_element)
-                return sub_element
-
-        def deserialize(self, element: Optional[XmlElementReader]) -> Any:
-            if element is not None and \
-                    (sub_element := element.pop_element(self._element_name, self._search_mode)) is not None:
-                return super().deserialize(sub_element)
-            else:
-                return None
+from pydantic_xml.serializers.factories.model import ModelProxySerializer
+from pydantic_xml.serializers.serializer import TYPE_FAMILY, SchemaTypeFamily, Serializer
 
+
+class PrimitiveTypeSerializer(Serializer):
+    @classmethod
+    def from_core_schema(cls, schema: pcs.UnionSchema, ctx: Serializer.Context) -> 'PrimitiveTypeSerializer':
+        computed = ctx.field_computed
+        inner_serializers: List[Serializer] = []
+        for choice_schema in schema['choices']:
+            inner_serializers.append(Serializer.parse_core_schema(choice_schema, ctx))
+
+        assert len(inner_serializers) > 0, "union choice is not provided"
+
+        # all union types serializers must be of the same type
+        if len(set(type(s) for s in inner_serializers)) > 1:
+            raise TypeError("unions of different primitive types are not supported")
+
+        return cls(computed, inner_serializers[0])
+
+    def __init__(self, computed: bool, inner_serializer: Serializer):
+        self._computed = computed
+        self._inner_serializer = inner_serializer
+
+    def serialize(
+            self, element: XmlElementWriter, value: Any, encoded: Any, *, skip_empty: bool = False,
+    ) -> Optional[XmlElementWriter]:
+        return self._inner_serializer.serialize(element, value, encoded, skip_empty=skip_empty)
+
+    def deserialize(self, element: Optional[XmlElementReader]) -> Optional[str]:
+        if self._computed:
+            return None
+
+        return self._inner_serializer.deserialize(element)
+
+
+class ModelSerializer(Serializer):
     @classmethod
-    def build(
-            cls,
-            model: Type['pxml.BaseXmlModel'],
-            model_field: pd.fields.ModelField,
-            field_location: Location,
-            ctx: Serializer.Context,
-    ) -> 'Serializer':
-        if field_location is Location.ELEMENT:
-            return cls.ElementSerializer(model_field, ctx)
-        elif field_location is Location.ATTRIBUTE:
-            return cls.AttributeSerializer(model, model_field, ctx)
-        elif field_location is Location.MISSING:
-            return cls.TextSerializer()
-        else:
-            raise AssertionError("unreachable")
+    def from_core_schema(cls, schema: pcs.UnionSchema, ctx: Serializer.Context) -> 'ModelSerializer':
+        computed = ctx.field_computed
+        inner_serializers: List[ModelProxySerializer] = []
+        for choice_schema in schema['choices']:
+            serializer = Serializer.parse_core_schema(choice_schema, ctx)
+            assert isinstance(serializer, ModelProxySerializer), "unexpected serializer type"
+
+            inner_serializers.append(serializer)
+
+        assert len(inner_serializers) > 0, "union choice is not provided"
+
+        return cls(computed, tuple(inner_serializers))
+
+    def __init__(self, computed: bool, inner_serializers: Tuple[ModelProxySerializer, ...]):
+        self._computed = computed
+        self._inner_serializers = inner_serializers
+
+    def serialize(
+            self,
+            element: XmlElementWriter,
+            value: 'pxml.BaseXmlModel',
+            encoded: Dict[str, Any],
+            *,
+            skip_empty: bool = False,
+    ) -> Optional[XmlElementWriter]:
+        for serializer in self._inner_serializers:
+            if serializer.model is type(value):
+                return serializer.serialize(element, value, encoded, skip_empty=skip_empty)
+
+        return None
+
+    def deserialize(self, element: Optional[XmlElementReader]) -> Optional['pxml.BaseXmlModel']:
+        if self._computed:
+            return None
+
+        if element is None:
+            return None
+
+        last_error: Optional[Exception] = None
+        result: Any = None
+        for serializer in self._inner_serializers:
+            snapshot = element.create_snapshot()
+            try:
+                if (result := serializer.deserialize(snapshot)) is None:
+                    continue
+                else:
+                    element.apply_snapshot(snapshot)
+                    return result
+            except pd.ValidationError as e:
+                last_error = e
+
+        if last_error is not None:
+            raise last_error
+
+        return result
+
+
+def from_core_schema(schema: pcs.UnionSchema, ctx: Serializer.Context) -> Serializer:
+    choice_families: Set[SchemaTypeFamily] = set()
+    for choice_schema in schema['choices']:
+        choice_schema, ctx = Serializer.preprocess_schema(choice_schema, ctx)
+        choice_type_family = TYPE_FAMILY.get(choice_schema['type'])
+
+        if choice_type_family not in (SchemaTypeFamily.PRIMITIVE, SchemaTypeFamily.MODEL):
+            raise errors.ModelFieldError(ctx.model_name, ctx.field_name, "union must be of primitive or model type")
+
+        choice_families.add(choice_type_family)
+
+    assert len(choice_families) > 0, "union choices are not provided"
+
+    if len(choice_families) > 1:
+        raise TypeError("unions of combined primitive and model types are not supported")
+
+    choice_family = choice_families.pop()
+    if choice_family is SchemaTypeFamily.MODEL:
+        return ModelSerializer.from_core_schema(schema, ctx)
+    elif choice_family is SchemaTypeFamily.PRIMITIVE:
+        return PrimitiveTypeSerializer.from_core_schema(schema, ctx)
+    else:
+        raise AssertionError("unreachable")
```

### Comparing `pydantic_xml-1.0.0/pydantic_xml/utils.py` & `pydantic_xml-2.0.0a1/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-1.0.0/pyproject.toml` & `pydantic_xml-2.0.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "1.0.0"
+version = "2.0.0a1"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://github.com/dapper91/pydantic-xml"
@@ -22,34 +22,34 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-lxml = {version = "^4.9.1", optional = true}
-pydantic = "^1.9.0"
+lxml = {version = "^4.9.0", optional = true}
+pydantic = "2.0"
 
 furo = {version = "^2022.12.7", optional = true}
 Sphinx = {version = "^5.3.0", optional = true}
 sphinx-copybutton = {version = "^0.5.1", optional = true}
 sphinx_design = {version = "^0.3.0", optional = true}
 toml = {version = "^0.10.2", optional = true}
 
 [tool.poetry.extras]
 lxml = ['lxml']
 docs = ['Sphinx', 'toml', 'sphinx_design', 'furo', 'sphinx-copybutton']
 
 [tool.poetry.dev-dependencies]
 lxml-stubs = "^0.4.0"
 mypy = "^1.4.1"
-pre-commit = "^3.3.3"
+pre-commit = "~3.2.0"
 pytest = "^7.4.0"
 pytest-cov = "^4.1.0"
-xmldiff = "2.5.0"
+xmldiff = "2.5"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 allow_redefinition = true
```

### Comparing `pydantic_xml-1.0.0/PKG-INFO` & `pydantic_xml-2.0.0a1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xml
-Version: 1.0.0
+Version: 2.0.0a1
 Summary: pydantic xml extension
 Home-page: https://github.com/dapper91/pydantic-xml
 License: Unlicense
 Keywords: pydantic,xml,serialization,deserialization,parsing,lxml
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -20,16 +20,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Provides-Extra: lxml
 Requires-Dist: Sphinx (>=5.3.0,<6.0.0) ; extra == "docs"
 Requires-Dist: furo (>=2022.12.7,<2023.0.0) ; extra == "docs"
-Requires-Dist: lxml (>=4.9.1,<5.0.0) ; extra == "lxml"
-Requires-Dist: pydantic (>=1.9.0,<2.0.0)
+Requires-Dist: lxml (>=4.9.0,<5.0.0) ; extra == "lxml"
+Requires-Dist: pydantic (==2.0)
 Requires-Dist: sphinx-copybutton (>=0.5.1,<0.6.0) ; extra == "docs"
 Requires-Dist: sphinx_design (>=0.3.0,<0.4.0) ; extra == "docs"
 Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "docs"
 Project-URL: Documentation, https://github.com/dapper91/pydantic-xml
 Project-URL: Repository, https://github.com/dapper91/pydantic-xml
 Description-Content-Type: text/x-rst
 
@@ -53,53 +53,55 @@
     :target: https://codecov.io/gh/dapper91/pydantic-xml
     :alt: Code coverage
 .. image:: https://readthedocs.org/projects/pydantic-xml/badge/?version=stable&style=flat
    :alt: ReadTheDocs status
    :target: https://pydantic-xml.readthedocs.io/en/stable/
 
 
-``pydantic-xml`` is a `pydantic <https://docs.pydantic.dev/1.10/>`_ extension providing model fields xml binding
+``pydantic-xml`` is a `pydantic <https://docs.pydantic.dev>`_ extension providing model fields xml binding
 and xml serialization / deserialization.
 It is closely integrated with ``pydantic`` which means it supports most of its features.
 
 
 Features
 --------
 
+- pydantic v1 / v2 support
 - flexable attributes, elements and text binding
-- python collection types support (``Dict``, ``List``, ``Set``, ``Tuple``, ...)
+- python collection types support (``Dict``, ``TypedDict``, ``List``, ``Set``, ``Tuple``, ...)
 - ``Union`` type support
-- pydantic `generic <https://docs.pydantic.dev/1.10/usage/models/#generic-models>`_ models support
+- pydantic `generic models <https://docs.pydantic.dev/latest/usage/models/#generic-models>`_ support
+- pydantic `computed fields <https://docs.pydantic.dev/latest/usage/computed_fields/>`_ support
 - `lxml <https://lxml.de/>`_ xml parser support
 - ``xml.etree.ElementTree`` standard library xml parser support
 
 What is not supported?
 ______________________
 
-- `dynamic model creation <https://docs.pydantic.dev/1.10/usage/models/#dynamic-model-creation>`_
-- `dataclasses <https://docs.pydantic.dev/1.10/usage/dataclasses/>`_
-- `discriminated unions <https://docs.pydantic.dev/1.10/usage/types/#discriminated-unions-aka-tagged-unions>`_
+- `dynamic model creation <https://docs.pydantic.dev/usage/models/#dynamic-model-creation>`_
+- `dataclasses <https://docs.pydantic.dev/usage/dataclasses/>`_
+- `discriminated unions <https://docs.pydantic.dev/usage/types/#discriminated-unions-aka-tagged-unions>`_
 
 Getting started
 ---------------
 
 The following model fields binding:
 
 .. code-block:: python
 
    class Product(BaseXmlModel):
        status: Literal['running', 'development'] = attr()  # extracted from the 'status' attribute
-       launched: Optional[int] = attr()  # extracted from the 'launched' attribute
+       launched: Optional[int] = attr(default=None)  # extracted from the 'launched' attribute
        title: str  # extracted from the element text
 
 
    class Company(BaseXmlModel):
        trade_name: str = attr(name='trade-name')  # extracted from the 'trade-name' attribute
        website: HttpUrl = element()  # extracted from the 'website' element text
-       products: List[Product] = element(tag='product')  # extracted from the 'website' element
+       products: List[Product] = element(tag='product', default=[])  # extracted from the 'website' element
 
 defines the XML document:
 
 .. code-block:: xml
 
    <Company trade-name="SpaceX">
        <website>https://www.spacex.com</website>
```

