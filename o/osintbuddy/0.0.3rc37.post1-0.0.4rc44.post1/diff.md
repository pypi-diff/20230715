# Comparing `tmp/osintbuddy-0.0.3rc37.post1.tar.gz` & `tmp/osintbuddy-0.0.4rc44.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osintbuddy-0.0.3rc37.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "osintbuddy-0.0.4rc44.post1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `osintbuddy-0.0.3rc37.post1.tar` & `osintbuddy-0.0.4rc44.post1.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0      447 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.github/workflows/CI.yml
--rw-r--r--   0        0        0      263 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      314 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.github/workflows/semantic-pr-check.yml
--rw-r--r--   0        0        0     1807 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.gitignore
--rw-r--r--   0        0        0     1540 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      158 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/.pypirc
--rw-r--r--   0        0        0        5 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0      316 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/Dockerfile
--rw-r--r--   0        0        0     1059 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/LICENSE
--rw-r--r--   0        0        0     3407 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/README.md
--rw-r--r--   0        0        0       47 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/docs/developer.md
--rw-r--r--   0        0        0      471 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/docs/pre-commit-config.md
--rw-r--r--   0        0        0    16088 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/docs/pylint.md
--rw-r--r--   0        0        0      497 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/docs/pyproject.md
--rw-r--r--   0        0        0      208 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/docs/workflows.md
--rw-r--r--   0        0        0     6844 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/pyproject.toml
--rw-r--r--   0        0        0      522 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/requirements.txt
--rw-r--r--   0        0        0     2958 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/README.md
--rw-r--r--   0        0        0      435 2023-06-16 12:38:31.479757 osintbuddy-0.0.3rc37.post1/src/osintbuddy/__init__.py
--rw-r--r--   0        0        0      370 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/__init__.py
--rw-r--r--   0        0        0     1302 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/base.py
--rw-r--r--   0        0        0     2993 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/displays.py
--rw-r--r--   0        0        0     4103 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/inputs.py
--rw-r--r--   0        0        0       62 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/entities/INDEX.md
--rw-r--r--   0        0        0      151 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/errors.py
--rw-r--r--   0        0        0     6431 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/plugins.py
--rw-r--r--   0        0        0     1301 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/src/osintbuddy/utils.py
--rw-r--r--   0        0        0      964 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/tests/conftest.py
--rw-r--r--   0        0        0      590 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/tests/plugins.py
--rw-r--r--   0        0        0      530 2023-06-16 12:38:28.647799 osintbuddy-0.0.3rc37.post1/tests/test_methods.py
--rw-r--r--   0        0        0     5861 1970-01-01 00:00:00.000000 osintbuddy-0.0.3rc37.post1/PKG-INFO
+-rw-r--r--   0        0        0      359 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/.github/workflows/CI.yml
+-rw-r--r--   0        0        0      284 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1807 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/.gitignore
+-rw-r--r--   0        0        0     1540 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      158 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/.pypirc
+-rw-r--r--   0        0        0        5 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0      316 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/Dockerfile
+-rw-r--r--   0        0        0     1059 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/LICENSE
+-rw-r--r--   0        0        0     4493 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/README.md
+-rw-r--r--   0        0        0       47 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/docs/developer.md
+-rw-r--r--   0        0        0      471 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/docs/pre-commit-config.md
+-rw-r--r--   0        0        0    16088 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/docs/pylint.md
+-rw-r--r--   0        0        0      497 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/docs/pyproject.md
+-rw-r--r--   0        0        0      208 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/docs/workflows.md
+-rw-r--r--   0        0        0     6639 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/pyproject.toml
+-rw-r--r--   0        0        0      166 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/requirements.txt
+-rw-r--r--   0        0        0     4413 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/README.md
+-rw-r--r--   0        0        0      465 2023-07-15 03:47:10.910524 osintbuddy-0.0.4rc44.post1/src/osintbuddy/__init__.py
+-rw-r--r--   0        0        0      396 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/__init__.py
+-rw-r--r--   0        0        0     1314 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/base.py
+-rw-r--r--   0        0        0     2993 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/displays.py
+-rw-r--r--   0        0        0     4116 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/inputs.py
+-rw-r--r--   0        0        0       62 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/entities/INDEX.md
+-rw-r--r--   0        0        0      151 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/errors.py
+-rw-r--r--   0        0        0     8551 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/plugins.py
+-rw-r--r--   0        0        0     1301 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/src/osintbuddy/utils.py
+-rw-r--r--   0        0        0      964 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/tests/conftest.py
+-rw-r--r--   0        0        0      590 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/tests/plugins.py
+-rw-r--r--   0        0        0      530 2023-07-15 03:47:07.930484 osintbuddy-0.0.4rc44.post1/tests/test_methods.py
+-rw-r--r--   0        0        0     6790 1970-01-01 00:00:00.000000 osintbuddy-0.0.4rc44.post1/PKG-INFO
```

### Comparing `osintbuddy-0.0.3rc37.post1/.gitignore` & `osintbuddy-0.0.4rc44.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc37.post1/.pre-commit-config.yaml` & `osintbuddy-0.0.4rc44.post1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc37.post1/LICENSE` & `osintbuddy-0.0.4rc44.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc37.post1/docs/pylint.md` & `osintbuddy-0.0.4rc44.post1/docs/pylint.md`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc37.post1/pyproject.toml` & `osintbuddy-0.0.4rc44.post1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,67 +1,64 @@
 [build-system]
 requires = ["flit"]
 build-backend = "flit.buildapi"
 
 [project]
 name =  "osintbuddy"
 authors = [
-    {name = "jerlendds", email = "jerlendsdev@proton.me"},
+    {name = "jerlendds", email = "theosintbuddyproject@openinfolabs.com"},
 ]
 description = "OSINTBuddy - mine, merge, and map data for novel insights"
 readme = "README.md"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
-    "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
-    "Programming Language :: Python :: 3 :: Only",
-    "Programming Language :: Python :: 3.7",
-    "Programming Language :: Python :: 3.8",
-    "Programming Language :: Python :: 3.9",
-    "Programming Language :: Python :: 3.10"
+    "License :: OSI Approved :: GNU Affero General Public License v3",
+    "Programming Language :: Python :: 3.11"
 ]
 requires-python = ">=3.7"
 dynamic = ["version"]
 dependencies = [
-  "selenium==4.9.0",
-  "pydantic==1.10.7",
-  "httpx==0.24.1"
+  "selenium>=4.9.0",
+  "pydantic>=1.10.8",
+  "httpx>=0.24.1",
+  "SQLAlchemy>=2.0.12",
 ]
 [project.optional-dependencies]
 test = [
-    "astroid==2.15.4",
-    "colorama==0.4.6",
-    "dill==0.3.6",
-    "eradicate==2.2.0",
-    "exceptiongroup==1.1.1",
-    "iniconfig==2.0.0",
-    "isort==5.12.0",
-    "lazy-object-proxy==1.9.0",
-    "mando==0.7.1",
-    "mccabe==0.7.0",
-    "mypy==1.3.0",
-    "mypy-extensions==1.0.0",
-    "packaging==23.1",
-    "platformdirs==3.5.1",
-    "pluggy==1.0.0",
-    "pycodestyle==2.10.0",
-    "pydocstyle==6.3.0",
-    "pyflakes==3.0.1",
-    "pylama==8.4.1",
-    "pylint==2.17.4",
-    "pytest==7.3.1",
-    "radon==6.0.1",
-    "six==1.16.0",
-    "snowballstemmer==2.2.0",
-    "toml==0.10.2",
-    "tomli==2.0.1",
-    "tomlkit==0.11.8",
-    "typing-extensions==4.5.0",
-    "vulture==2.7",
-    "wrapt==1.15.0"
+  "astroid==2.15.4",
+  "colorama==0.4.6",
+  "dill==0.3.6",
+  "eradicate==2.2.0",
+  "exceptiongroup==1.1.1",
+  "iniconfig==2.0.0",
+  "isort==5.12.0",
+  "lazy-object-proxy==1.9.0",
+  "mando==0.7.1",
+  "mccabe==0.7.0",
+  "mypy==1.3.0",
+  "mypy-extensions==1.0.0",
+  "packaging==23.1",
+  "platformdirs==3.5.1",
+  "pluggy==1.0.0",
+  "pycodestyle==2.10.0",
+  "pydocstyle==6.3.0",
+  "pyflakes==3.0.1",
+  "pylama==8.4.1",
+  "pylint==2.17.4",
+  "pytest==7.3.1",
+  "radon==6.0.1",
+  "six==1.16.0",
+  "snowballstemmer==2.2.0",
+  "toml==0.10.2",
+  "tomli==2.0.1",
+  "tomlkit==0.11.8",
+  "typing-extensions==4.5.0",
+  "vulture==2.7",
+  "wrapt==1.15.0",
 ]
 
 [project.urls]
 Documentation = "https://docs.osintbuddy.com/"
 Source = "https://github.com/jerlendds/osintbuddy-plugins"
 Tracker = "https://github.com/jerlendds/osintbuddy/issues"
```

### Comparing `osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/base.py` & `osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-class BaseNode(object):
+class BaseElement(object):
     """
-    The BaseNode class represents a basic building block used in OsintBuddy
+    The BaseElement class represents a basic building block used in OsintBuddy
     plugins. It is designed to implement the base styles used
     in other nodes that can render a nodes element
     with a specific element type, label, and style on the OSINTbuddy UI.
 
     label : str
         A string representing the label for the node.
     style : dict
@@ -31,13 +31,13 @@
             'type': self.node_type,
             'label': self.label,
             'placeholder': self.placeholder,
             'style': self.style
         }
 
 
-class BaseInput(BaseNode):
+class BaseInput(BaseElement):
     pass
 
 
-class BaseDisplay(BaseNode):
+class BaseDisplay(BaseElement):
     pass
```

### Comparing `osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/displays.py` & `osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/displays.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc37.post1/src/osintbuddy/elements/inputs.py` & `osintbuddy-0.0.4rc44.post1/src/osintbuddy/elements/inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -77,15 +77,15 @@
                 options=[{'label': 'Option 1', 'tooltip': 'Hello on hover!'}],
                 value='Option 1'
             )
         ]
     """
     node_type: str = "dropdown"
 
-    def __init__(self, options=[], value={'label': '', 'tooltip': ''}, **kwargs):
+    def __init__(self, options=[], value={'label': '', 'tooltip': '', 'value': ''}, **kwargs):
         super().__init__(**kwargs)
         self.options: List[any] = options
         self.value: dict = value
 
     def json(self):
         node = self._base_blueprint()
         node["options"] = self.options
```

### Comparing `osintbuddy-0.0.3rc37.post1/src/osintbuddy/plugins.py` & `osintbuddy-0.0.4rc44.post1/src/osintbuddy/plugins.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,26 @@
 import os
 import importlib
-from typing import List, Any
+from typing import List, Any, Callable
 from collections import defaultdict
+from pydantic import create_model, BaseModel
+import undetected_chromedriver as uc
 # from osintbuddy.utils import slugify
-from osintbuddy.elements.base import BaseNode
+from osintbuddy.elements.base import BaseElement
 from osintbuddy.errors import OBPluginError
 from osintbuddy.utils import to_snake_case
 
+def driver() -> uc.Chrome:
+    pass
+
+# @todo add permission system and display what parts of system plugin can access
+class OBAuthorUse(BaseModel):
+    get_driver: Callable[[], uc.Chrome]
+    get_graph: Callable[[], None]  # @todo
+
 
 class OBRegistry(type):
     plugins = []
     labels = []
     ui_labels = []
 
     def __init__(cls, name, bases, attrs):
@@ -33,15 +43,15 @@
         Returns the corresponding plugin class for a given plugin_label or
         'None' if not found.
 
         :param plugin_label: The label of the plugin to be returned.
         :return: The plugin class or None if not found.
         """
         for idx, label in enumerate(cls.labels):
-            if label == plugin_label:
+            if to_snake_case(label) == to_snake_case(plugin_label):
                 return cls.plugins[idx]
         return None
 
     def __getitem__(self, i):
         return self.get_plugin[i]
 
 
@@ -67,15 +77,15 @@
                     importlib.import_module(f'{modpath}{modname}')
                 except ImportError as e:
                     print(f"Error importing plugin '{modpath}{modname}': {e}")
 
     return OBRegistry.plugins
 
 
-def transform(label, icon='list', prompt=None):
+def transform(label, icon='list', prompt=None, edge_label='transformed_to'):
     """
     A decorator add transforms to an osintbuddy plugin.
 
     Usage:
     @transform(label=<label_text>, icon=<tabler_react_icon_name>)
     def transform_to_ip(self, node, **kwargs):
         # Method implementation
@@ -87,50 +97,49 @@
     :return: A decorator for the plugin transform method.
     """
     def decorator_transform(func):
         async def wrapper(self, node, **kwargs):
             return await func(self=self, node=node, **kwargs)
         wrapper.label = label
         wrapper.icon = icon
+        wrapper.edge_label = edge_label
         if prompt is not None:
             wrapper.prompt = prompt
 
         return wrapper
     return decorator_transform
 
 
 class OBPlugin(object, metaclass=OBRegistry):
     """
     OBPlugin is the base class for all plugin classes in this application.
     It provides the required structure and methods for a plugin.
     """
-    node: List[BaseNode]
-    name: str = 'Plugin Node'
+    node: List[BaseElement]
     color: str = '#145070'
     label: str = ''
     icon: str = 'atom-2'
-    transform_icons: dict = {}
     show_label = True
     style: dict = {}
 
     def __init__(self):
         transforms = self.__class__.__dict__.values()
         self.transforms = {
-            func.label: func for func in transforms if hasattr(func, 'label')
+            to_snake_case(func.label): func for func in transforms if hasattr(func, 'label')
         }
         self.transform_labels = [
             {'label': func.label, 'icon': func.icon} for func in transforms
             if hasattr(func, 'icon') and hasattr(func, 'label')
         ]
 
     def __call__(self):
         return self.blueprint()
 
     @staticmethod
-    def _map_node_elements(element, kwargs):
+    def _map_graph_data_labels(element, kwargs):
         label = to_snake_case(element['label'])
         for passed_label in kwargs:
             if passed_label == label:
                 if type(kwargs[label]) is str:
                     element['value'] = kwargs[label]
                 elif type(kwargs[label]) is dict:
                     for t in kwargs[label]:
@@ -142,44 +151,83 @@
         """
         Generate and return a dictionary representing the plugins node.
         Includes label, name, color, icon, and a list of all elements
         for the node/plugin.
         """
         node = defaultdict(None)
         node['label'] = cls.label
-        node['name'] = cls.name
-        node['color'] = cls.color
+        node['color'] = cls.color if cls.color else '#145070'
         node['icon'] = cls.icon
         node['style'] = cls.style
         node['elements'] = []
         for element in cls.node:
-            if type(element) is list:
-                e = []
-                for elm in element:
-                    e.append(cls._map_node_elements(elm.json(), kwargs))
-                node['elements'].append(e)
+            if isinstance(element, list):
+                node['elements'].append([
+                    cls._map_graph_data_labels(elm.json(), kwargs)
+                    for elm in element
+                ])
             else:
-                e = cls._map_node_elements(element.json(), kwargs)
-                node['elements'].append(e)
+                element_row = cls._map_graph_data_labels(element.json(), kwargs)
+                node['elements'].append(element_row)
         return node
 
-    async def _get_transform(self, transform_type: str, node, **kwargs) -> Any:
+    async def get_transform(self, transform_type: str, node, use: OBAuthorUse) -> Any:
         """ Return output from a function accepting node data.
             The function will be called with a single argument, the node data
             from when a node context menu action is taken - and should return
             a list of Nodes.
             None if the plugin doesn't provide a transform
             for the transform_type.
         """
+        transform_type = to_snake_case(transform_type)
+        print('transform_type', transform_type)
+        print('transforms', self.transforms)
         if self.transforms and self.transforms[transform_type]:
             try:
                 transform = await self.transforms[transform_type](
                     self=self,
-                    node=node,
-                    **kwargs
+                    node=self._map_to_transform_data(node),
+                    use=use
                 )
-                if type(transform) != list:
+                edge_label = self.transforms[transform_type].edge_label
+                if not isinstance(transform, list):
+                    transform['edge_label'] = edge_label
                     return [transform]
+                [
+                    n.__setitem__('edge_label', edge_label)
+                    for n in transform
+                ]
                 return transform
-            except OBPluginError as e:
-                raise OBPluginError(e)
+            except (Exception, OBPluginError) as e:
+                if isinstance(e, OBPluginError):
+                    raise OBPluginError(e)
+                raise OBPluginError(f'This plugin has run into an unhandled error: {e}')
         return None
+
+    @staticmethod
+    def _map_element(transform_map: dict, element: dict):
+        label = to_snake_case(element.pop('label', None))
+        transform_map[label] = {}
+        type = element.pop('type', None)
+        element.pop('icon', None)
+        element.pop('placeholder', None)
+        element.pop('style', None)
+        element.pop('options', None)
+        for k, v in element.items():
+            if (isinstance(v, str) and len(element.values()) == 1) or type == 'dropdown':
+                transform_map[label] = v
+            else:
+                transform_map[label][k] = v
+
+    @classmethod
+    def _map_to_transform_data(cls, node: dict):
+        transform_map = {}
+        data = node.get('data', {})
+        model_label = data.get('label')
+        elements = data.get('elements', [])
+        for element in elements:
+            if isinstance(element, list):
+                [cls._map_element(transform_map, elm) for elm in element]
+            else:
+                cls._map_element(transform_map, element)
+        model = create_model(model_label, **transform_map)
+        return model()
```

### Comparing `osintbuddy-0.0.3rc37.post1/src/osintbuddy/utils.py` & `osintbuddy-0.0.4rc44.post1/src/osintbuddy/utils.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc37.post1/tests/conftest.py` & `osintbuddy-0.0.4rc44.post1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc37.post1/tests/plugins.py` & `osintbuddy-0.0.4rc44.post1/tests/plugins.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc37.post1/tests/test_methods.py` & `osintbuddy-0.0.4rc44.post1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `osintbuddy-0.0.3rc37.post1/PKG-INFO` & `osintbuddy-0.0.4rc44.post1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: osintbuddy
-Version: 0.0.3rc37.post1
+Version: 0.0.4rc44.post1
 Summary: OSINTBuddy - mine, merge, and map data for novel insights
-Author-email: jerlendds <jerlendsdev@proton.me>
+Author-email: jerlendds <theosintbuddyproject@openinfolabs.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: selenium==4.9.0
-Requires-Dist: pydantic==1.10.7
-Requires-Dist: httpx==0.24.1
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: selenium>=4.9.0
+Requires-Dist: pydantic>=1.10.8
+Requires-Dist: httpx>=0.24.1
+Requires-Dist: SQLAlchemy>=2.0.12
 Requires-Dist: astroid==2.15.4 ; extra == "test"
 Requires-Dist: colorama==0.4.6 ; extra == "test"
 Requires-Dist: dill==0.3.6 ; extra == "test"
 Requires-Dist: eradicate==2.2.0 ; extra == "test"
 Requires-Dist: exceptiongroup==1.1.1 ; extra == "test"
 Requires-Dist: iniconfig==2.0.0 ; extra == "test"
 Requires-Dist: isort==5.12.0 ; extra == "test"
@@ -47,85 +44,107 @@
 Requires-Dist: vulture==2.7 ; extra == "test"
 Requires-Dist: wrapt==1.15.0 ; extra == "test"
 Project-URL: Documentation, https://docs.osintbuddy.com/
 Project-URL: Source, https://github.com/jerlendds/osintbuddy-plugins
 Project-URL: Tracker, https://github.com/jerlendds/osintbuddy/issues
 Provides-Extra: test
 
-[![Total Downloads](https://static.pepy.tech/badge/osintbuddy)](https://pepy.tech/project/osintbuddy)
-[![Downloads](https://static.pepy.tech/badge/osintbuddy/week)](https://pepy.tech/project/osintbuddy)
+# OSINTBuddy plugins and extensions
 
-# Extending OSINTBuddy with plugins
+The plugins library for [jerlendds/osintbuddy](https://github.com/jerlendds/osintbuddy).
 
-The plugins library for [osintbuddy](https://github.com/jerlendds/osintbuddy)
-![osintbuddy-demo](https://github.com/jerlendds/osintbuddy/assets/29207058/c01357a9-9e55-44e3-9734-c84130bd110b)
 
-This project follows the Python Standards declared in PEP 621. It uses a pyproject.yaml file to configure the project and Flit to simplify the build process and publish to PyPI.
+![ob-demo 2023-07-14 20-51](https://github.com/jerlendds/osintbuddy/assets/29207058/b69e08f3-ac2a-4cef-9a85-713e7df6b12f)
 
 
-## Creating your first plugin
+***Please note:** [OSINTBuddy plugins](https://github.com/jerlendds/osintbuddy-plugins) are still in early alpha and breaking changes may occasionally occur in the API. That said, if you remain on the `main` branch and avoid accessing protected methods we will try our best to avoid introducing breaking changes.*
 
-In this guide, we will dive into creating a custom plugin for OSINTBuddy that extends its capabilities. This will enable you to incorporate additional sources and transformations into the OSINTBuddy toolbox. We will use the provided code example as a reference to build our plugin.
+### **NOTICE:** There has been a major update to plugins, any created plugins will have to be updated to use the new, and more convenient data access method:
+  - Remove `name` from any `ob.Plugin`
+  - Update `node['data']` access to be `node.label_defined_in_node`
+    - Please see the introduction to the plugin system below
 
-### Step-by-step guide to create a new plugin
 
-Start by importing the necessary modules:
+The osintbuddy plugin system at its core is very simple. An `OBRegistry` class holds all registered `OBPlugin` classes within the application. This registry is loaded into the [osintbuddy application](https://github.com/jerlendds/osintbuddy/) where it is then used to load the available entities for the user when they access a project graph, load transforms when a user opens the context menu of a node, and perform transformations which expect a `Plugin.blueprint()` to be returned. The returned data of a transform decorated method will be automatically mapped to a [JanusGraph](https://janusgraph.org/) database through [gremlin](https://tinkerpop.apache.org/) according to the labels *(as snakecase)* you previously set in the classes `node` for whatever `Plugin.blueprint()`
+you return.
+ 
+To make this a bit more clear please see the below example...
 
 ```py
-import socket
-import osintbuddy as ob
-```
+from pydantic import BaseModel
+import osintbuddy import transform, Plugin
+from osintbuddy.elements import TextInput, DropdownInput, Title, CopyText
+from osintbuddy.errors import OBPluginError
 
-Define a class for your plugin, inheriting from `ob.Plugin`. Set the required attributes such as `label`, and optionally set an `icon` like `world-www` (using [tabler-icon](https://tabler-icons.io/) names), and a `node` which contains a list of elements used as a blueprint for creating the node displayed on the OSINTBuddy UI.
 
-```py
-class WebsitePlugin(ob.Plugin):
-    label = 'Website'
-    name = 'Website'
-    color = '#1D1DB8'
-    icon = 'world-www'
+class CSESearchResults(Plugin):
+    label = "CSE Result"
+    name = "CSE result"
+    show_label = False  # do not show this on the entities dialog 
+    # the user sees on the left of the project graph screen
+    color = "#058F63"
     node = [
-        ob.elements.TextInput(label='Domain', icon='world-www'),
+        Title(label="Result"),
+        CopyText(label="URL"),
+        CopyText(label="Cache URL"),
     ]
-```
-
-Now, define a transformation method to gather and transform the data from the input node. In this case, the transform_to_ip function uses the `socket.gethostbyname()` Python module to obtain the IP address for a given domain. Decorate the method with `@transform()` and set the metadata attributes such as `label` and `icon`.
-
-```py
-@transform(label='To IP', icon='building-broadcast-tower')
-def transform_to_ip(self, node, **kwargs):
-    blueprint = IPAddressPlugin.blueprint(
-        ip_address=socket.gethostbyname(node['data'][0])
-    )
-    return blueprint
-```
-## Using the new plugin
 
-To use the new plugin, simply add it to the existing OSINTBuddy plugins folder inside the application, in development mode it will be detected automatically and loaded by the platform. Once added, you can access your 'Website' plugin and use the 'To IP' transformation.
 
-Creating a custom plugin for OSINTBuddy is an easy and effective way to enhance the capabilities of the tool, allowing you to fetch information from additional sources or transform the data in new ways. By following this guide and using the provided code example as a reference, you'll be able to create your own unique plugins to extend the functionality of OSINTBuddy to fit your specific needs.
-
-
-### Full example
-
-```py
-import socket
-import osintbuddy as ob
-
-class WebsitePlugin(ob.Plugin):
-    label = 'Website'
-    name = 'Website'
-    color = '#1D1DB8'
-    icon = 'world-www'
+class CSESearchPlugin(Plugin):
+    label = "CSE Search"
+    name = "CSE search"
+    color = "#2C7237"
     node = [
-        ob.elements.TextInput(label='Domain', icon='world-www'),
+        [
+            TextInput(label="Query", icon="search"),
+            TextInput(label="Pages", icon="123", default="1"),
+        ],
+        DropdownInput(label="CSE Categories", options=cse_link_options)
     ]
 
-    @ob.transform(label='To IP', icon='building-broadcast-tower')
-    async def transform_to_ip(self, node, **kwargs):
-        blueprint = IPAddressPlugin.blueprint(
-            ip_address=socket.gethostbyname(node['data'][0])
-        )
-        return blueprint
+    @transform(label="To cse results", icon="search")
+    async def transform_to_cse_results(
+      self,
+      node: BaseModel,  # dynamically generated pydantic model 
+      # that is mapped from the above labels contained within `node`
+      use  # a pydantic model allowing you to access a selenium instance
+      # (and eventually a gremlin graph and settings api) 
+    ):
+        results = []
+
+        if not node.query:
+          raise OBPluginError((
+            'You can send error messages to the user here'
+            'if they forget to submit data or if some other error occurs'
+          ))
+
+        # notice how you can access data returned from the context menu
+        # of this node; using the label name in snake case
+        print(node.cse_categories, node.query, node.pages) 
+
+        ... # (removed code for clarity)
+
+        if resp:
+            for result in resp["results"]:
+                url = result.get("breadcrumbUrl", {})
+                # some elements you can store more than just a string,
+                # (these elements storing dicts are mapped 
+                # to janusgraph as properties with the names
+                # result_title, result_subtitle, and result_text)
+                blueprint = CSESearchResults.blueprint(
+                    result={
+                        "title": result.get("titleNoFormatting"),
+                        "subtitle": url.get("host") + url.get("crumbs"),
+                        "text": result.get("contentNoFormatting"),
+                    },
+                    url=result.get("unescapedUrl"),
+                    cache_url=result.get("cacheUrl"),
+                )
+                results.append(blueprint)
+        # here we return a list of blueprints (blueprints are dicts)
+        # but you can also return a single blueprint without a list
+        return results
+
 ```
 
 
+
```

