# Comparing `tmp/pydantic_xml-0.7.0.tar.gz` & `tmp/pydantic_xml-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_xml-0.7.0.tar", max compression
+gzip compressed data, was "pydantic_xml-1.0.0.tar", max compression
```

## Comparing `pydantic_xml-0.7.0.tar` & `pydantic_xml-1.0.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1211 2023-06-23 20:11:44.107379 pydantic_xml-0.7.0/LICENSE
--rw-r--r--   0        0        0     3182 2023-06-23 20:11:44.107379 pydantic_xml-0.7.0/README.rst
--rw-r--r--   0        0        0      599 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/__init__.py
--rw-r--r--   0        0        0      489 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/config.py
--rw-r--r--   0        0        0       80 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/element/__init__.py
--rw-r--r--   0        0        0    13091 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/element/element.py
--rw-r--r--   0        0        0      374 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/element/native/__init__.py
--rw-r--r--   0        0        0     1671 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/element/native/lxml.py
--rw-r--r--   0        0        0     1173 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/element/native/std.py
--rw-r--r--   0        0        0      569 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/errors.py
--rw-r--r--   0        0        0    11708 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/model.py
--rw-r--r--   0        0        0        0 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/py.typed
--rw-r--r--   0        0        0       73 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/__init__.py
--rw-r--r--   0        0        0     1445 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/encoder.py
--rw-r--r--   0        0        0      394 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/__init__.py
--rw-r--r--   0        0        0     1898 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/forwardref.py
--rw-r--r--   0        0        0     4612 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/heterogeneous.py
--rw-r--r--   0        0        0     4337 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/homogeneous.py
--rw-r--r--   0        0        0     4732 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/mapping.py
--rw-r--r--   0        0        0     7057 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/model.py
--rw-r--r--   0        0        0     4220 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/primitive.py
--rw-r--r--   0        0        0     6693 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/union.py
--rw-r--r--   0        0        0     3292 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/factories/wrapper.py
--rw-r--r--   0        0        0     7364 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/serializers/serializer.py
--rw-r--r--   0        0        0       48 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/typedefs.py
--rw-r--r--   0        0        0     2131 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pydantic_xml/utils.py
--rw-r--r--   0        0        0     1878 2023-06-23 20:11:44.111379 pydantic_xml-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     4687 1970-01-01 00:00:00.000000 pydantic_xml-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-07-15 06:45:26.804304 pydantic_xml-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3192 2023-07-15 06:45:26.804304 pydantic_xml-1.0.0/README.rst
+-rw-r--r--   0        0        0      599 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/__init__.py
+-rw-r--r--   0        0        0      489 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/config.py
+-rw-r--r--   0        0        0       80 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/element/__init__.py
+-rw-r--r--   0        0        0    13330 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/element/element.py
+-rw-r--r--   0        0        0      374 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/element/native/__init__.py
+-rw-r--r--   0        0        0     1671 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/element/native/lxml.py
+-rw-r--r--   0        0        0     1173 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/element/native/std.py
+-rw-r--r--   0        0        0      569 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/errors.py
+-rw-r--r--   0        0        0    11708 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/model.py
+-rw-r--r--   0        0        0        0 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/py.typed
+-rw-r--r--   0        0        0       73 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/__init__.py
+-rw-r--r--   0        0        0     1445 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/encoder.py
+-rw-r--r--   0        0        0      394 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/__init__.py
+-rw-r--r--   0        0        0     1898 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/forwardref.py
+-rw-r--r--   0        0        0     4612 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/heterogeneous.py
+-rw-r--r--   0        0        0     4337 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/homogeneous.py
+-rw-r--r--   0        0        0     4894 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/mapping.py
+-rw-r--r--   0        0        0     6903 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/model.py
+-rw-r--r--   0        0        0     4220 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/primitive.py
+-rw-r--r--   0        0        0     6693 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/union.py
+-rw-r--r--   0        0        0     3292 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/factories/wrapper.py
+-rw-r--r--   0        0        0     7364 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/serializers/serializer.py
+-rw-r--r--   0        0        0       48 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/typedefs.py
+-rw-r--r--   0        0        0     2131 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pydantic_xml/utils.py
+-rw-r--r--   0        0        0     1879 2023-07-15 06:45:26.808303 pydantic_xml-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     4697 1970-01-01 00:00:00.000000 pydantic_xml-1.0.0/PKG-INFO
```

### Comparing `pydantic_xml-0.7.0/LICENSE` & `pydantic_xml-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/README.rst` & `pydantic_xml-1.0.0/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -18,35 +18,35 @@
     :target: https://codecov.io/gh/dapper91/pydantic-xml
     :alt: Code coverage
 .. image:: https://readthedocs.org/projects/pydantic-xml/badge/?version=stable&style=flat
    :alt: ReadTheDocs status
    :target: https://pydantic-xml.readthedocs.io/en/stable/
 
 
-``pydantic-xml`` is a `pydantic <https://docs.pydantic.dev>`_ extension providing model fields xml binding
+``pydantic-xml`` is a `pydantic <https://docs.pydantic.dev/1.10/>`_ extension providing model fields xml binding
 and xml serialization / deserialization.
 It is closely integrated with ``pydantic`` which means it supports most of its features.
 
 
 Features
 --------
 
 - flexable attributes, elements and text binding
 - python collection types support (``Dict``, ``List``, ``Set``, ``Tuple``, ...)
 - ``Union`` type support
-- pydantic `generic <https://pydantic-docs.helpmanual.io/usage/models/#generic-models>`_ models support
+- pydantic `generic <https://docs.pydantic.dev/1.10/usage/models/#generic-models>`_ models support
 - `lxml <https://lxml.de/>`_ xml parser support
 - ``xml.etree.ElementTree`` standard library xml parser support
 
 What is not supported?
 ______________________
 
-- `dynamic model creation <https://docs.pydantic.dev/usage/models/#dynamic-model-creation>`_
-- `dataclasses <https://docs.pydantic.dev/usage/dataclasses/>`_
-- `discriminated unions <https://docs.pydantic.dev/usage/types/#discriminated-unions-aka-tagged-unions>`_
+- `dynamic model creation <https://docs.pydantic.dev/1.10/usage/models/#dynamic-model-creation>`_
+- `dataclasses <https://docs.pydantic.dev/1.10/usage/dataclasses/>`_
+- `discriminated unions <https://docs.pydantic.dev/1.10/usage/types/#discriminated-unions-aka-tagged-unions>`_
 
 Getting started
 ---------------
 
 The following model fields binding:
 
 .. code-block:: python
@@ -70,8 +70,8 @@
        <website>https://www.spacex.com</website>
        <product status="running" launched="2013">Several launch vehicles</product>
        <product status="running" launched="2019">Starlink</product>
        <product status="development">Starship</product>
    </Company>
 
 
-Check `documentation <https://pydantic-xml.readthedocs.io/en/latest/>`_ for more information.
+See `documentation <https://pydantic-xml.readthedocs.io/en/latest/>`_ for more details.
```

### Comparing `pydantic_xml-0.7.0/pydantic_xml/__init__.py` & `pydantic_xml-1.0.0/pydantic_xml/__init__.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/element/element.py` & `pydantic_xml-1.0.0/pydantic_xml/element/element.py`

 * *Files 2% similar despite different names*

```diff
@@ -269,15 +269,15 @@
 
     def pop_attributes(self) -> Optional[Dict[str, str]]:
         result, self._state.attrib = self._state.attrib, None
 
         return result
 
     def pop_element(self, tag: str, search_mode: 'SearchMode') -> Optional['XmlElement[NativeElement]']:
-        searcher = get_searcher(search_mode)
+        searcher: Searcher[NativeElement] = get_searcher(search_mode)
 
         return searcher(self._state, tag, False)
 
     def find_sub_element(self, path: Sequence[str], search_mode: 'SearchMode') -> Optional['XmlElement[NativeElement]']:
         assert len(path) > 0, "path can't be empty"
 
         root, path = path[0], path[1:]
@@ -297,15 +297,15 @@
             sub_element = self.make_element(tag=tag, nsmap=nsmap)
             self._state.elements.append(sub_element)
             self._state.next_element_idx += 1
 
         return sub_element
 
     def _find_element(self, tag: str, search_mode: 'SearchMode') -> Optional['XmlElement[NativeElement]']:
-        searcher = get_searcher(search_mode)
+        searcher: Searcher[NativeElement] = get_searcher(search_mode)
 
         return searcher(self._state, tag, True)
 
 
 class SearchMode(str, Enum):
     """
     Element search mode.
@@ -316,61 +316,69 @@
     """
 
     STRICT = 'strict'
     ORDERED = 'ordered'
     UNORDERED = 'unordered'
 
 
-Searcher = Callable[[XmlElement.State[Any], str, bool], Optional[XmlElement]]
+Searcher = Callable[[XmlElement.State[NativeElement], str, bool], Optional[XmlElement]]
 
 
-def get_searcher(search_mode: SearchMode) -> Searcher:
+def get_searcher(search_mode: SearchMode) -> Searcher[NativeElement]:
     if search_mode == SearchMode.STRICT:
         return strict_search
     elif search_mode == SearchMode.ORDERED:
         return ordered_search
     elif search_mode == SearchMode.UNORDERED:
         return unordered_search
     else:
         raise AssertionError('unreachable')
 
 
-def strict_search(state: XmlElement.State[Any], tag: str, look_behind: bool = False) -> Optional[XmlElement[Any]]:
+def strict_search(
+        state: XmlElement.State[NativeElement],
+        tag: str,
+        look_behind: bool = False,
+) -> Optional[XmlElement[NativeElement]]:
     """
     Searches for a sub-element sequentially one by one.
 
     :param state: element state
     :param tag: sub-element tag for be searched for
     :param look_behind: look for a previous element
     :return: found element or `None` if the element not found
     """
 
-    result: Optional[XmlElement[Any]] = None
+    result: Optional[XmlElement[NativeElement]] = None
 
     if look_behind and (result := _look_behind(state, tag)) is not None:
         return result
 
     if state.next_element_idx < len(state.elements) and state.elements[state.next_element_idx].tag == tag:
         result = state.elements[state.next_element_idx]
         state.next_element_idx += 1
 
     return result
 
 
-def ordered_search(state: XmlElement.State[Any], tag: str, look_behind: bool = False) -> Optional[XmlElement[Any]]:
+def ordered_search(
+        state: XmlElement.State[NativeElement],
+        tag: str,
+        look_behind: bool = False,
+) -> Optional[XmlElement[NativeElement]]:
     """
     Searches for an element sequentially skipping unmatched ones.
 
     :param state: element state
     :param tag: sub-element tag for be searched for
     :param look_behind: look for a previous element
     :return: found element or `None` if the element not found
     """
 
-    result: Optional[XmlElement[Any]] = None
+    result: Optional[XmlElement[NativeElement]] = None
 
     if look_behind and (result := _look_behind(state, tag)) is not None:
         return result
 
     next_element_idx = state.next_element_idx
     while next_element_idx < len(state.elements):
         element = state.elements[next_element_idx]
@@ -381,28 +389,28 @@
             result = element
             break
 
     return result
 
 
 def unordered_search(
-        state: XmlElement.State[Any],
+        state: XmlElement.State[NativeElement],
         tag: str,
         look_behind: bool = False,
-) -> Optional[XmlElement[Any]]:
+) -> Optional[XmlElement[NativeElement]]:
     """
     Searches search for an element ignoring elements order.
 
     :param state: element state
     :param tag: sub-element tag for be searched for
     :param look_behind: look for a previous element
     :return: found element or `None` if the requested element not found
     """
 
-    result: Optional[XmlElement[Any]] = None
+    result: Optional[XmlElement[NativeElement]] = None
 
     if look_behind and (result := _look_behind(state, tag)) is not None:
         return result
 
     for idx in range(state.next_element_idx, len(state.elements)):
         element = state.elements[idx]
         if element.tag == tag:
@@ -411,14 +419,14 @@
             state.next_element_idx += 1
             result = element
             break
 
     return result
 
 
-def _look_behind(state: XmlElement.State[Any], tag: str) -> Optional[XmlElement[Any]]:
+def _look_behind(state: XmlElement.State[NativeElement], tag: str) -> Optional[XmlElement[NativeElement]]:
     if state.next_element_idx != 0:
         candidate = state.elements[state.next_element_idx - 1]
         if candidate.tag == tag:
             return candidate
 
     return None
```

### Comparing `pydantic_xml-0.7.0/pydantic_xml/element/native/lxml.py` & `pydantic_xml-1.0.0/pydantic_xml/element/native/lxml.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class XmlElement(BaseXmlElement[etree._Element]):
     @classmethod
     def from_native(cls, element: etree._Element) -> 'XmlElement':
         return cls(
             tag=element.tag,
             text=element.text,
             attributes={
-                force_str(name): force_str(value)  # str transformation safe since lxml byte values are ASCII compatible
+                force_str(name): force_str(value)  # transformation is safe since lxml bytes values are ASCII compatible
                 for name, value in element.attrib.items()
             },
             elements=[
                 XmlElement.from_native(sub_element)
                 for sub_element in element
                 if not is_xml_comment(sub_element)
             ],
```

### Comparing `pydantic_xml-0.7.0/pydantic_xml/element/native/std.py` & `pydantic_xml-1.0.0/pydantic_xml/element/native/std.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/errors.py` & `pydantic_xml-1.0.0/pydantic_xml/errors.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/model.py` & `pydantic_xml-1.0.0/pydantic_xml/model.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/serializers/encoder.py` & `pydantic_xml-1.0.0/pydantic_xml/serializers/encoder.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/forwardref.py` & `pydantic_xml-1.0.0/pydantic_xml/serializers/factories/forwardref.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/heterogeneous.py` & `pydantic_xml-1.0.0/pydantic_xml/serializers/factories/heterogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/homogeneous.py` & `pydantic_xml-1.0.0/pydantic_xml/serializers/factories/homogeneous.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/mapping.py` & `pydantic_xml-1.0.0/pydantic_xml/serializers/factories/mapping.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,20 @@
         ):
             name, ns, nsmap = self._get_entity_info(model_field)
             self._ns = ns or ctx.parent_ns
             self._nsmap = merge_nsmaps(nsmap, ctx.parent_nsmap)
             self._ns_attrs = model.__xml_ns_attrs__
 
         def serialize(
-                self, element: XmlElementWriter, value: Dict[str, Any], *, encoder: XmlEncoder, skip_empty: bool = False
+                self,
+                element: XmlElementWriter,
+                value: Dict[str, Any],
+                *,
+                encoder: XmlEncoder,
+                skip_empty: bool = False,
         ) -> Optional[XmlElementWriter]:
             if value is None:
                 return element
 
             ns = self._nsmap.get(self._ns) if self._ns_attrs and self._ns else None
             element.set_attributes({
                 QName(tag=attr, ns=ns).uri: encoder.encode(val)
@@ -58,15 +63,20 @@
 
             name, ns, nsmap = self._get_entity_info(model_field)
             self._name = name or model_field.alias
             self._element_name = QName.from_alias(tag=self._name, ns=self._ns, nsmap=self._nsmap).uri
             self._search_mode = ctx.search_mode
 
         def serialize(
-                self, element: XmlElementWriter, value: Dict[str, Any], *, encoder: XmlEncoder, skip_empty: bool = False
+                self,
+                element: XmlElementWriter,
+                value: Dict[str, Any],
+                *,
+                encoder: XmlEncoder,
+                skip_empty: bool = False,
         ) -> Optional[XmlElementWriter]:
             if skip_empty and len(value) == 0:
                 return element
 
             sub_element = element.make_element(self._element_name, nsmap=self._nsmap)
             super().serialize(sub_element, value, encoder=encoder, skip_empty=skip_empty)
             if skip_empty and sub_element.is_empty():
```

### Comparing `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/model.py` & `pydantic_xml-1.0.0/pydantic_xml/serializers/factories/model.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,17 +167,15 @@
             model: Type['pxml.BaseXmlModel'],
             model_field: pd.fields.ModelField,
             field_location: Location,
             ctx: Serializer.Context,
     ) -> 'Serializer':
         if field_location is Location.ELEMENT:
             return cls.ElementSerializer(model, model_field, ctx)
-        elif not ctx.parent_is_root and field_location is Location.MISSING:
+        elif field_location is Location.MISSING:
             return cls.ElementSerializer(model, model_field, ctx)
-        elif ctx.parent_is_root and field_location is Location.MISSING:
-            return cls.DeferredSerializer(model_field)
         elif field_location is Location.ATTRIBUTE:
             raise errors.ModelFieldError(
                 model.__name__, model_field.name, "attributes of model type are not supported",
             )
         else:
             raise AssertionError("unreachable")
```

### Comparing `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/primitive.py` & `pydantic_xml-1.0.0/pydantic_xml/serializers/factories/primitive.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/union.py` & `pydantic_xml-1.0.0/pydantic_xml/serializers/factories/union.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/serializers/factories/wrapper.py` & `pydantic_xml-1.0.0/pydantic_xml/serializers/factories/wrapper.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/serializers/serializer.py` & `pydantic_xml-1.0.0/pydantic_xml/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pydantic_xml/utils.py` & `pydantic_xml-1.0.0/pydantic_xml/utils.py`

 * *Files identical despite different names*

### Comparing `pydantic_xml-0.7.0/pyproject.toml` & `pydantic_xml-1.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-xml"
-version = "0.7.0"
+version = "1.0.0"
 description = "pydantic xml extension"
 authors = ["Dmitry Pershin <dapper1291@gmail.com>"]
 license = "Unlicense"
 readme = "README.rst"
 homepage = "https://github.com/dapper91/pydantic-xml"
 repository = "https://github.com/dapper91/pydantic-xml"
 documentation = "https://github.com/dapper91/pydantic-xml"
@@ -37,19 +37,19 @@
 
 [tool.poetry.extras]
 lxml = ['lxml']
 docs = ['Sphinx', 'toml', 'sphinx_design', 'furo', 'sphinx-copybutton']
 
 [tool.poetry.dev-dependencies]
 lxml-stubs = "^0.4.0"
-mypy = "^0.971"
-pre-commit = "^2.20.0"
-pytest = "^7.1.2"
-pytest-cov = "^3.0.0"
-xmldiff = "2.5"
+mypy = "^1.4.1"
+pre-commit = "^3.3.3"
+pytest = "^7.4.0"
+pytest-cov = "^4.1.0"
+xmldiff = "2.5.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 allow_redefinition = true
```

### Comparing `pydantic_xml-0.7.0/PKG-INFO` & `pydantic_xml-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-xml
-Version: 0.7.0
+Version: 1.0.0
 Summary: pydantic xml extension
 Home-page: https://github.com/dapper91/pydantic-xml
 License: Unlicense
 Keywords: pydantic,xml,serialization,deserialization,parsing,lxml
 Author: Dmitry Pershin
 Author-email: dapper1291@gmail.com
 Requires-Python: >=3.8,<4.0
@@ -53,35 +53,35 @@
     :target: https://codecov.io/gh/dapper91/pydantic-xml
     :alt: Code coverage
 .. image:: https://readthedocs.org/projects/pydantic-xml/badge/?version=stable&style=flat
    :alt: ReadTheDocs status
    :target: https://pydantic-xml.readthedocs.io/en/stable/
 
 
-``pydantic-xml`` is a `pydantic <https://docs.pydantic.dev>`_ extension providing model fields xml binding
+``pydantic-xml`` is a `pydantic <https://docs.pydantic.dev/1.10/>`_ extension providing model fields xml binding
 and xml serialization / deserialization.
 It is closely integrated with ``pydantic`` which means it supports most of its features.
 
 
 Features
 --------
 
 - flexable attributes, elements and text binding
 - python collection types support (``Dict``, ``List``, ``Set``, ``Tuple``, ...)
 - ``Union`` type support
-- pydantic `generic <https://pydantic-docs.helpmanual.io/usage/models/#generic-models>`_ models support
+- pydantic `generic <https://docs.pydantic.dev/1.10/usage/models/#generic-models>`_ models support
 - `lxml <https://lxml.de/>`_ xml parser support
 - ``xml.etree.ElementTree`` standard library xml parser support
 
 What is not supported?
 ______________________
 
-- `dynamic model creation <https://docs.pydantic.dev/usage/models/#dynamic-model-creation>`_
-- `dataclasses <https://docs.pydantic.dev/usage/dataclasses/>`_
-- `discriminated unions <https://docs.pydantic.dev/usage/types/#discriminated-unions-aka-tagged-unions>`_
+- `dynamic model creation <https://docs.pydantic.dev/1.10/usage/models/#dynamic-model-creation>`_
+- `dataclasses <https://docs.pydantic.dev/1.10/usage/dataclasses/>`_
+- `discriminated unions <https://docs.pydantic.dev/1.10/usage/types/#discriminated-unions-aka-tagged-unions>`_
 
 Getting started
 ---------------
 
 The following model fields binding:
 
 .. code-block:: python
@@ -105,9 +105,9 @@
        <website>https://www.spacex.com</website>
        <product status="running" launched="2013">Several launch vehicles</product>
        <product status="running" launched="2019">Starlink</product>
        <product status="development">Starship</product>
    </Company>
 
 
-Check `documentation <https://pydantic-xml.readthedocs.io/en/latest/>`_ for more information.
+See `documentation <https://pydantic-xml.readthedocs.io/en/latest/>`_ for more details.
```

