# Comparing `tmp/todoist_tree-0.2.2.tar.gz` & `tmp/todoist_tree-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "todoist_tree-0.2.2.tar", max compression
+gzip compressed data, was "todoist_tree-0.4.0.tar", max compression
```

## Comparing `todoist_tree-0.2.2.tar` & `todoist_tree-0.4.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rw-r--r--   0        0        0     1360 2023-02-09 14:53:56.488444 todoist_tree-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     1378 2023-02-03 21:30:37.494226 todoist_tree-0.2.2/README.md
--rw-r--r--   0        0        0       43 2023-02-03 21:31:49.703860 todoist_tree-0.2.2/src/todoist_tree/__init__.py
--rw-r--r--   0        0        0      774 2023-02-03 21:30:37.496622 todoist_tree-0.2.2/src/todoist_tree/headers.py
--rw-r--r--   0        0        0        0 2023-02-03 21:30:37.496622 todoist_tree-0.2.2/src/todoist_tree/py.typed
--rw-r--r--   0        0        0     5253 2023-02-09 14:51:38.166720 todoist_tree-0.2.2/src/todoist_tree/read_changes.py
--rw-r--r--   0        0        0     4194 2023-02-03 21:31:49.705470 todoist_tree-0.2.2/src/todoist_tree/task_subsets.py
--rw-r--r--   0        0        0     6473 2023-02-03 21:31:49.705470 todoist_tree-0.2.2/src/todoist_tree/tree.py
--rw-r--r--   0        0        0     3956 2023-02-03 21:31:49.706568 todoist_tree-0.2.2/src/todoist_tree/write_changes.py
--rw-r--r--   0        0        0     2123 1970-01-01 00:00:00.000000 todoist_tree-0.2.2/setup.py
--rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 todoist_tree-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1360 2023-07-15 20:17:05.660444 todoist_tree-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1378 2023-07-15 20:12:50.362623 todoist_tree-0.4.0/README.md
+-rw-r--r--   0        0        0       43 2023-07-15 20:12:50.368683 todoist_tree-0.4.0/src/todoist_tree/__init__.py
+-rw-r--r--   0        0        0      774 2023-07-15 20:12:50.368683 todoist_tree-0.4.0/src/todoist_tree/headers.py
+-rw-r--r--   0        0        0        0 2023-07-15 20:12:50.368683 todoist_tree-0.4.0/src/todoist_tree/py.typed
+-rw-r--r--   0        0        0     5290 2023-07-15 20:15:37.338049 todoist_tree-0.4.0/src/todoist_tree/read_changes.py
+-rw-r--r--   0        0        0     4177 2023-07-15 20:15:37.338049 todoist_tree-0.4.0/src/todoist_tree/task_subsets.py
+-rw-r--r--   0        0        0     6599 2023-07-15 20:15:37.338049 todoist_tree-0.4.0/src/todoist_tree/tree.py
+-rw-r--r--   0        0        0     3956 2023-07-15 20:12:50.368683 todoist_tree-0.4.0/src/todoist_tree/write_changes.py
+-rw-r--r--   0        0        0     1811 1970-01-01 00:00:00.000000 todoist_tree-0.4.0/PKG-INFO
```

### Comparing `todoist_tree-0.2.2/pyproject.toml` & `todoist_tree-0.4.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "todoist-tree"
-version = "0.2.2"
+version = "0.4.0"
 description = "Create a tree from Todoist projects > sections > tasks"
 authors = ["Shay Hill <shay_public@hotmail.com>"]
 readme = "README.md"
 packages = [{include = "todoist_tree", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -16,15 +16,15 @@
 commitizen = "^2.39.1"
 pre-commit = "^2.21.0"
 types-requests = "^2.28.11.8"
 pytest = "^7.2.1"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.2.2"
+version = "0.4.0"
 tag_format = "$version"
 version_files = [
     "pyproject.toml:^version"
 ]
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `todoist_tree-0.2.2/README.md` & `todoist_tree-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `todoist_tree-0.2.2/src/todoist_tree/headers.py` & `todoist_tree-0.4.0/src/todoist_tree/headers.py`

 * *Files identical despite different names*

### Comparing `todoist_tree-0.2.2/src/todoist_tree/read_changes.py` & `todoist_tree-0.4.0/src/todoist_tree/read_changes.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 import requests
 from pydantic import BaseModel
 
 from todoist_tree.headers import SYNC_URL
 
 if TYPE_CHECKING:
-
     from requests.structures import CaseInsensitiveDict
 
 # error codes with special handling
 _UNAUTHORIZED = 401
 _FORBIDDEN = 403
 
 # This is everything this project will look at.
@@ -78,14 +77,15 @@
     """Todoist task (item)."""
 
     added_at: str = ""
     added_by_uid: str = ""
     assigned_by_uid: str | None = None
     child_order: int = 0
     content: str = ""
+    due: dict[str, Any] | None = None
     description: str = ""
     labels: list[str] = []
     parent_id: str | None = None
     priority: int = 0
     project_id: str | None = ""
     section_id: str | None = None
```

### Comparing `todoist_tree-0.2.2/src/todoist_tree/task_subsets.py` & `todoist_tree-0.4.0/src/todoist_tree/task_subsets.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from contextlib import suppress
 from typing import TYPE_CHECKING
 
 from todoist_tree.read_changes import Project, Section
 
 if TYPE_CHECKING:
-    from typing import Iterator
+    from collections.abc import Iterator
 
     from todoist_tree.read_changes import Task
     from todoist_tree.tree import AnyNode
 
     _PST = Project | Section | Task
 
 
@@ -24,15 +24,15 @@
 
     :param elem: a Todoist Project, Section, or Task
     :return: an Automation or None
 
     Projects, Sections, and Tasks don't use the same attribute for the name. Tasks
     use "content", Projects and Sections use "name".
     """
-    name = model.name if isinstance(model, (Project, Section)) else model.content
+    name = model.name if isinstance(model, Project | Section) else model.content
 
     return name.strip().endswith(suffix)
 
 
 def _filter_for_suffix(suffix: str, *model: _PST) -> Iterator[_PST]:
     """Iterate over all elements that have a suffix.
 
@@ -63,15 +63,15 @@
     :param id2node: a mapping from Todoist model IDs to Nodes
     :param suffix: a suffix to identify serial tasks
     :return: a tuple of (selected, rejected) tasks
     """
     selected: dict[str, Task] = {}
 
     for model in _filter_for_suffix(suffix, *projects, *sections, *tasks):
-        with suppress(StopIteration), suppress(StopIteration):
+        with suppress(StopIteration):
             next_task = next(id2node[model.id].iter_childless_tasks())
             selected[next_task.id] = next_task
 
     return list(selected.values()), [x for x in tasks if x.id not in selected]
 
 
 def select_parallel(
```

### Comparing `todoist_tree-0.2.2/src/todoist_tree/tree.py` & `todoist_tree-0.4.0/src/todoist_tree/tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 
 from collections import deque
 from typing import TYPE_CHECKING, Generic, TypeVar
 
 from todoist_tree.read_changes import Project, Section, Task
 
 if TYPE_CHECKING:
-    from typing import Any, Iterator
+    from typing import Any
+    from collections.abc import Iterator
 
 
 _Model = Project | Section | Task
 _ModelT = TypeVar("_ModelT", bound=_Model)
 
 
 def _node_sort_key(node: Node[_ModelT]) -> tuple[int, int]:
@@ -51,15 +52,14 @@
     if node.data.parent_id:
         return 3, node.data.child_order
     msg = f"Unexpected node type: {node.data}"
     raise ValueError(msg)
 
 
 class Node(Generic[_ModelT]):
-
     """A node in a tree of projects, sections, and tasks."""
 
     def __init__(self, model: _ModelT) -> None:
         """Initialize a node.
 
         :param model: the model object that this node represents
         """
@@ -118,15 +118,17 @@
         if isinstance(self.data, Task) and not self._children:
             yield self.data
 
 
 AnyNode = Node[Project] | Node[Section] | Node[Task]
 
 
-def _place_subs(id2node: dict[str, Node[Project]] | dict[str, Node[Task]]) -> None:
+def _place_subs(
+    id2node: dict[str | None, Node[Project]] | dict[str | None, Node[Task]]
+) -> None:
     """Place subtasks or subprojects under their parents.
 
     :param id2node: map of node ids to nodes (includes parents and perhaps children)
     :effect: if there are any subtasks or subprojects, they are will be added to
         their parent element's children attribute.
     :raise AttributeError: if a subtask or subproject is found without a parent
     """
@@ -144,38 +146,39 @@
         if not found_parent:
             msg = f"Could not find parents for nodes {queue}"
             raise AttributeError(msg)
 
 
 def map_id_to_branch(
     projects: list[Project], sections: list[Section], tasks: list[Task]
-) -> dict[str, AnyNode]:
+) -> dict[str | None, AnyNode]:
     """Build a tree of nodes from the API cache.
 
     :param projects: all (sub)project nodes
     :param sections: all section nodes
     :param tasks: all (sub)task nodes
     :return: a map of node ids to nodes. Each node with children will contain
         references to any children, so the branch can be searched downward.
 
     There will not be a root node to this tree, every Project will be a root.
     """
-    project_nodes: dict[str, Node[Project]]
+    project_nodes: dict[str | None, Node[Project]]
     project_nodes = {p.id: Node(p) for p in projects}
     _place_subs(project_nodes)
 
-    section_nodes: dict[str, Node[Section]]
+    section_nodes: dict[str | None, Node[Section]]
     section_nodes = {s.id: Node(s) for s in sections}
     for sect in section_nodes.values():
         project_nodes[sect.data.project_id].add_child(sect)
 
-    task_nodes: dict[str, Node[Task]]
+    task_nodes: dict[str | None, Node[Task]]
     task_nodes = {t.id: Node(t) for t in tasks}
     _place_subs(task_nodes)
 
     for task in (x for x in task_nodes.values() if x.data.parent_id is None):
         if task.data.section_id:
             section_nodes[task.data.section_id].add_child(task)
         else:
             project_nodes[task.data.project_id].add_child(task)
 
-    return {**project_nodes, **section_nodes, **task_nodes}
+    nodes: dict[str | None, AnyNode] = {**project_nodes, **section_nodes, **task_nodes}
+    return nodes
```

### Comparing `todoist_tree-0.2.2/src/todoist_tree/write_changes.py` & `todoist_tree-0.4.0/src/todoist_tree/write_changes.py`

 * *Files identical despite different names*

### Comparing `todoist_tree-0.2.2/setup.py` & `todoist_tree-0.4.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,63 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: todoist-tree
+Version: 0.4.0
+Summary: Create a tree from Todoist projects > sections > tasks
+Author: Shay Hill
+Author-email: shay_public@hotmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pydantic (>=1.10.4,<2.0.0)
+Requires-Dist: requests (>=2.28.2,<3.0.0)
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# todoist_tree
 
-packages = \
-['todoist_tree']
+These are the core functions of [todoist_bot](https://github.com/ShayHill/todoist_bot).
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['pydantic>=1.10.4,<2.0.0', 'requests>=2.28.2,<3.0.0']
-
-setup_kwargs = {
-    'name': 'todoist-tree',
-    'version': '0.2.2',
-    'description': 'Create a tree from Todoist projects > sections > tasks',
-    'long_description': '# todoist_tree\n\nThese are the core functions of [todoist_bot](https://github.com/ShayHill/todoist_bot).\n\nThe reading and writing functions are just (sometimes typeguarded) aliases of Todoist api calls. The differentiating functionality is building a tree with\n\n``` python\nimport time\nfrom todoist_tree import headers\nfrom todoist_tree import read_changes\nfrom todoist_tree import tree\n\nheaders = new_headers(api_token)\ntodoist = None\nsync_token: str = "*"\n\ncomplete = False\n\nwhile not complete:\n\n    todoist = read_changes.read_changes(headers)\n    if todoist is None:\n        # no changes or failure\n        time.sleep(2)\n        continue\n\n    sync_token = todoist.sync_token\n\n    projects = todoist.projects\n    sections = todoist.sections\n    tasks = todoist.tasks\n\n    id2node = tree.map_id_to_branch(\n        todoist.projects,\n        todoist.sections,\n        todoist.tasks\n    )\n\n    # do something here\n\n    time.sleep(5)\n```\n\nThe tree doesn\'t have one root. `map_id_to_branch` maps the id[1] of each project, section, and task to a node. Top-level projects will not have parents, so they are effectively roots of their own trees.\n\nSee [todoist_bot](https://github.com/ShayHill/todoist_bot) for a full example.\n\n[1] where `id` is the value returned in the json dictionary from the Todoist api, *not* the Python object id.\n',
-    'author': 'Shay Hill',
-    'author_email': 'shay_public@hotmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.10,<4.0',
-}
+The reading and writing functions are just (sometimes typeguarded) aliases of Todoist api calls. The differentiating functionality is building a tree with
 
+``` python
+import time
+from todoist_tree import headers
+from todoist_tree import read_changes
+from todoist_tree import tree
+
+headers = new_headers(api_token)
+todoist = None
+sync_token: str = "*"
+
+complete = False
+
+while not complete:
+
+    todoist = read_changes.read_changes(headers)
+    if todoist is None:
+        # no changes or failure
+        time.sleep(2)
+        continue
+
+    sync_token = todoist.sync_token
+
+    projects = todoist.projects
+    sections = todoist.sections
+    tasks = todoist.tasks
+
+    id2node = tree.map_id_to_branch(
+        todoist.projects,
+        todoist.sections,
+        todoist.tasks
+    )
+
+    # do something here
+
+    time.sleep(5)
+```
+
+The tree doesn't have one root. `map_id_to_branch` maps the id[1] of each project, section, and task to a node. Top-level projects will not have parents, so they are effectively roots of their own trees.
+
+See [todoist_bot](https://github.com/ShayHill/todoist_bot) for a full example.
+
+[1] where `id` is the value returned in the json dictionary from the Todoist api, *not* the Python object id.
 
-setup(**setup_kwargs)
```

