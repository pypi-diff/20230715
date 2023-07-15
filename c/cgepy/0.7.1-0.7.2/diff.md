# Comparing `tmp/cgepy-0.7.1.tar.gz` & `tmp/cgepy-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgepy-0.7.1.tar", max compression
+gzip compressed data, was "cgepy-0.7.2.tar", max compression
```

## Comparing `cgepy-0.7.1.tar` & `cgepy-0.7.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2023-06-29 01:41:56.304652 cgepy-0.7.1/LICENSE.md
--rw-r--r--   0        0        0      508 2023-07-02 20:29:03.422470 cgepy-0.7.1/README.md
--rw-r--r--   0        0        0     4976 2023-07-02 20:34:38.268411 cgepy-0.7.1/cgepy/__init__.py
--rw-r--r--   0        0        0      464 2023-06-24 18:46:51.694033 cgepy-0.7.1/cgepy/colors.py
--rw-r--r--   0        0        0       99 2023-07-02 16:23:21.890637 cgepy-0.7.1/cgepy/ext/__init__.py
--rw-r--r--   0        0        0       22 2023-06-29 01:45:06.356080 cgepy-0.7.1/cgepy/ext/beta/__init__.py
--rw-r--r--   0        0        0     1318 2023-07-02 20:33:33.211943 cgepy-0.7.1/cgepy/ext/text.py
--rw-r--r--   0        0        0      315 2023-06-24 18:46:56.773316 cgepy-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 cgepy-0.7.1/setup.py
--rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 cgepy-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-29 01:41:56.304652 cgepy-0.7.2/LICENSE.md
+-rw-r--r--   0        0        0      508 2023-07-15 01:19:23.115727 cgepy-0.7.2/README.md
+-rw-r--r--   0        0        0     4976 2023-07-15 01:16:57.376599 cgepy-0.7.2/cgepy/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-15 01:18:22.372973 cgepy-0.7.2/cgepy/colors.py
+-rw-r--r--   0        0        0       99 2023-07-15 01:16:54.528052 cgepy-0.7.2/cgepy/ext/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-29 01:45:06.356080 cgepy-0.7.2/cgepy/ext/beta/__init__.py
+-rw-r--r--   0        0        0     1304 2023-07-15 01:16:51.400412 cgepy-0.7.2/cgepy/ext/text.py
+-rw-r--r--   0        0        0      315 2023-07-15 01:18:43.384197 cgepy-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1085 1970-01-01 00:00:00.000000 cgepy-0.7.2/setup.py
+-rw-r--r--   0        0        0     1128 1970-01-01 00:00:00.000000 cgepy-0.7.2/PKG-INFO
```

### Comparing `cgepy-0.7.1/LICENSE.md` & `cgepy-0.7.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cgepy-0.7.1/cgepy/__init__.py` & `cgepy-0.7.2/cgepy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.7.1'
+__version__ = '0.7.2'
 
 try:
 	from cgepy.cgepy.colors import *
 except ModuleNotFoundError:
 	try:
 		from cgePy.cgepy.colors import *
 	except ModuleNotFoundError:
```

### Comparing `cgepy-0.7.1/cgepy/ext/text.py` & `cgepy-0.7.2/cgepy/ext/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '0.7.1'
+__version__ = '0.7.2'
 
 try:
 	from cgePy.cgepy.colors import *
 	from cgePy.cgepy.__init__ import *
 except ModuleNotFoundError:
 	try:
 		from cgepy.cgepy.colors import *
@@ -13,15 +13,15 @@
 
 class empty:
 	'''The name says it all.'''
 	pass
 
 class TextEngine:
 	'''A text engine allowing for text inside grids.'''
-	def __init__(self, grid: Grid) -> TextEngine:
+	def __init__(self, grid: Grid):
 		self.grid = grid
 		self.temp = empty()
 	def Insert(self, content, index=0):
 		self.temp.content = content
 		self.index = index
 		self.temp.contentlen = len(content)
 		if self.temp.contentlen % 2 != 0:
```

### Comparing `cgepy-0.7.1/setup.py` & `cgepy-0.7.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 ['cgepy', 'cgepy.ext', 'cgepy.ext.beta']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'cgepy',
-    'version': '0.7.1',
+    'version': '0.7.2',
     'description': 'Tools for developing graphical programs inside the console.',
-    'long_description': "### cgepy // 0.7.1\n##### A lightweight 8-bit graphics engine\n***\n###### Documentation: https://cgepy.github.io/docs\nLooking for something simple to use? Want to use a reliable package for once?\\\ncgepy's got you covered.\n\nFeaturing a powerful, but easy-to-use system, you can make fun games with cgepy.\\\nThough cgepy lacks many things like mouse support and native keyboard support, it is ever growing and will soon have so many features in place of those, while maintaining that same speed and reliablility.\n",
+    'long_description': "### cgepy // 0.7.2\n##### A lightweight 8-bit graphics engine\n***\n###### Documentation: https://cgepy.github.io/docs\nLooking for something simple to use? Want to use a reliable package for once?\\\ncgepy's got you covered.\n\nFeaturing a powerful, but easy-to-use system, you can make fun games with cgepy.\\\nThough cgepy lacks many things like mouse support and native keyboard support, it is ever growing and will soon have so many features in place of those, while maintaining that same speed and reliablility.\n",
     'author': 'catbox305',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `cgepy-0.7.1/PKG-INFO` & `cgepy-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: cgepy
-Version: 0.7.1
+Version: 0.7.2
 Summary: Tools for developing graphical programs inside the console.
 License: MIT
 Author: catbox305
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
-### cgepy // 0.7.1
+### cgepy // 0.7.2
 ##### A lightweight 8-bit graphics engine
 ***
 ###### Documentation: https://cgepy.github.io/docs
 Looking for something simple to use? Want to use a reliable package for once?\
 cgepy's got you covered.
 
 Featuring a powerful, but easy-to-use system, you can make fun games with cgepy.\
```

