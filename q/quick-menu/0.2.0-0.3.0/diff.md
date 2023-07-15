# Comparing `tmp/quick_menu-0.2.0.tar.gz` & `tmp/quick_menu-0.3.0.tar.gz`

## Comparing `quick_menu-0.2.0.tar` & `quick_menu-0.3.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 quick_menu-0.2.0/mkdocs.yml
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 quick_menu-0.2.0/.vscode/settings.json
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 quick_menu-0.2.0/docs/index.md
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 quick_menu-0.2.0/src/quick_menu/__about__.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 quick_menu-0.2.0/src/quick_menu/__init__.py
--rw-r--r--   0        0        0     4769 2020-02-02 00:00:00.000000 quick_menu-0.2.0/src/quick_menu/menu.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 quick_menu-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 quick_menu-0.2.0/tests/test_menu.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 quick_menu-0.2.0/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 quick_menu-0.2.0/LICENSE.txt
--rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 quick_menu-0.2.0/README.md
--rw-r--r--   0        0        0     3426 2020-02-02 00:00:00.000000 quick_menu-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 quick_menu-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1201 2020-02-02 00:00:00.000000 quick_menu-0.3.0/mkdocs.yml
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 quick_menu-0.3.0/.vscode/settings.json
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 quick_menu-0.3.0/docs/index.md
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 quick_menu-0.3.0/src/quick_menu/__about__.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 quick_menu-0.3.0/src/quick_menu/__init__.py
+-rw-r--r--   0        0        0     4649 2020-02-02 00:00:00.000000 quick_menu-0.3.0/src/quick_menu/menu.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 quick_menu-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 quick_menu-0.3.0/tests/test_menu.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 quick_menu-0.3.0/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 quick_menu-0.3.0/LICENSE.txt
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 quick_menu-0.3.0/README.md
+-rw-r--r--   0        0        0     3408 2020-02-02 00:00:00.000000 quick_menu-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 quick_menu-0.3.0/PKG-INFO
```

### Comparing `quick_menu-0.2.0/mkdocs.yml` & `quick_menu-0.3.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `quick_menu-0.2.0/src/quick_menu/menu.py` & `quick_menu-0.3.0/src/quick_menu/menu.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,41 +22,37 @@
             .add(MenuItem("S", "Submenu", action=submenu.run))
             .add(MenuItem("X", "Exit", is_exit=True))
         )
 
         menu.run()
 """
 import os
-from dataclasses import KW_ONLY, dataclass, field
+from dataclasses import dataclass, field
 from typing import Callable, Optional
 
 from typing_extensions import Self
 
 
 @dataclass
 class MenuItem:
     """A menu item to add to a menu.
 
     The menu item can optionally call a function or start a submenu. A menu item can
     also be an exit item which exits the curren menu.
 
-    Note:
-        The `action`, `kwargs`, and `is_exit` parameters are keyword only arguments.
-
     Parameters:
         choice:  The string used to select the menu item.
         label:   The text label displayed for the menu item.
         action:  An optional function to be called when the menu item is selected.
         kwargs:  Arguments to pass to a menu item action.
         is_exit: Whether or not this menu item exits the current menu
     """
 
     choice: str
     label: str
-    _: KW_ONLY
     action: Optional[Callable[..., None]] = None
     kwargs: dict = field(default_factory=dict)
     is_exit: bool = False
 
     def select(self):
         """Select the menu item.
```

### Comparing `quick_menu-0.2.0/tests/test_menu.py` & `quick_menu-0.3.0/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `quick_menu-0.2.0/.gitignore` & `quick_menu-0.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `quick_menu-0.2.0/LICENSE.txt` & `quick_menu-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `quick_menu-0.2.0/pyproject.toml` & `quick_menu-0.3.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 dynamic = ["version"]
 description = ''
 readme = "README.md"
 requires-python = ">=3.7"
 license = "MIT"
 keywords = []
 authors = [
-  { name = "Stephan Poole (e122785)", email = "yqbear@gmail.com" },
+  { name = "Stephan Poole", email = "yqbear@gmail.com" },
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
@@ -23,15 +23,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 dependencies = ["typing_extensions"]
 
 [project.urls]
-Documentation = "https://github.com/yqbear/quick-menu#readme"
+Documentation = "https://yqbear.github.io/quick-menu"
 Issues = "https://github.com/yqbear/quick-menu/issues"
 Source = "https://github.com/yqbear/quick-menu"
 
 [tool.hatch.version]
 path = "src/quick_menu/__about__.py"
 
 [tool.hatch.envs.default]
```

### Comparing `quick_menu-0.2.0/PKG-INFO` & `quick_menu-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: quick-menu
-Version: 0.2.0
-Project-URL: Documentation, https://github.com/yqbear/quick-menu#readme
+Version: 0.3.0
+Project-URL: Documentation, https://yqbear.github.io/quick-menu
 Project-URL: Issues, https://github.com/yqbear/quick-menu/issues
 Project-URL: Source, https://github.com/yqbear/quick-menu
-Author-email: "Stephan Poole (e122785)" <yqbear@gmail.com>
+Author-email: Stephan Poole <yqbear@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,18 +23,19 @@
 # quick-menu
 
 [![PyPI - Version](https://img.shields.io/pypi/v/quick-menu.svg)](https://pypi.org/project/quick-menu)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/quick-menu.svg)](https://pypi.org/project/quick-menu)
 
 -----
 
-**Table of Contents**
+This is a simple package to create text menus for use in console applications.
 
-- [Installation](#installation)
-- [License](#license)
+## Documentation
+
+The [documentation](https://yqbear.github.io/quick-menu) is made with [Material for MkDocs](https://github.com/squidfunk/mkdocs-material) and is hosted by [GitHub Pages](https://docs.github.com/en/pages).
 
 ## Installation
 
 ```console
 pip install quick-menu
 ```
```

