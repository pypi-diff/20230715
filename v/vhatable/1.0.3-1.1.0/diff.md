# Comparing `tmp/vhatable-1.0.3.tar.gz` & `tmp/vhatable-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vhatable-1.0.3.tar", last modified: Sun May 21 13:03:57 2023, max compression
+gzip compressed data, was "vhatable-1.1.0.tar", last modified: Sat Jul 15 11:29:55 2023, max compression
```

## Comparing `vhatable-1.0.3.tar` & `vhatable-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,33 @@
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-05-21 13:03:57.401244 vhatable-1.0.3/
--rw-r--r--   0 fred      (1000) fred      (1000)    35138 2022-01-30 18:20:55.000000 vhatable-1.0.3/LICENSE.txt
--rw-r--r--   0 fred      (1000) fred      (1000)      609 2023-05-21 13:03:57.401244 vhatable-1.0.3/PKG-INFO
--rw-r--r--   0 fred      (1000) fred      (1000)      336 2022-01-30 18:20:55.000000 vhatable-1.0.3/README.rst
--rw-r--r--   0 fred      (1000) fred      (1000)       38 2023-05-21 13:03:57.401244 vhatable-1.0.3/setup.cfg
--rwxr-xr-x   0 fred      (1000) fred      (1000)     2840 2022-01-15 02:09:48.000000 vhatable-1.0.3/setup.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-05-21 13:03:57.401244 vhatable-1.0.3/vhatable/
--rw-r--r--   0 fred      (1000) fred      (1000)      958 2023-05-21 12:57:47.000000 vhatable-1.0.3/vhatable/__init__.py
--rw-r--r--   0 fred      (1000) fred      (1000)     9318 2023-04-23 15:34:41.000000 vhatable-1.0.3/vhatable/cell.py
--rw-r--r--   0 fred      (1000) fred      (1000)    23251 2023-05-21 13:01:34.000000 vhatable-1.0.3/vhatable/core.py
--rw-r--r--   0 fred      (1000) fred      (1000)     6758 2023-04-23 15:39:49.000000 vhatable-1.0.3/vhatable/filters.py
--rw-r--r--   0 fred      (1000) fred      (1000)    20587 2023-04-23 15:37:15.000000 vhatable-1.0.3/vhatable/sample.py
-drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-05-21 13:03:57.401244 vhatable-1.0.3/vhatable.egg-info/
--rwxr-xr-x   0 fred      (1000) fred      (1000)      609 2023-05-21 13:03:57.000000 vhatable-1.0.3/vhatable.egg-info/PKG-INFO
--rwxr-xr-x   0 fred      (1000) fred      (1000)      319 2023-05-21 13:03:57.000000 vhatable-1.0.3/vhatable.egg-info/SOURCES.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)        1 2023-05-21 13:03:57.000000 vhatable-1.0.3/vhatable.egg-info/dependency_links.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)       67 2023-05-21 13:03:57.000000 vhatable-1.0.3/vhatable.egg-info/entry_points.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)       84 2023-05-21 13:03:57.000000 vhatable-1.0.3/vhatable.egg-info/requires.txt
--rwxr-xr-x   0 fred      (1000) fred      (1000)        9 2023-05-21 13:03:57.000000 vhatable-1.0.3/vhatable.egg-info/top_level.txt
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 11:29:55.890906 vhatable-1.1.0/
+-rw-r--r--   0 fred      (1000) fred      (1000)    35138 2022-01-30 18:20:55.000000 vhatable-1.1.0/LICENSE.txt
+-rw-r--r--   0 fred      (1000) fred      (1000)      636 2023-07-15 11:29:55.890906 vhatable-1.1.0/PKG-INFO
+-rw-r--r--   0 fred      (1000) fred      (1000)      336 2022-01-30 18:20:55.000000 vhatable-1.1.0/README.rst
+-rw-r--r--   0 fred      (1000) fred      (1000)       38 2023-07-15 11:29:55.890906 vhatable-1.1.0/setup.cfg
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     3061 2023-06-12 21:44:16.000000 vhatable-1.1.0/setup.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 11:29:55.887573 vhatable-1.1.0/tests/
+-rw-r--r--   0 fred      (1000) fred      (1000)     8453 2023-06-10 11:01:04.000000 vhatable-1.1.0/tests/test_cellv2.py
+-rwxr-xr-x   0 fred      (1000) fred      (1000)     3166 2022-01-15 02:09:48.000000 vhatable-1.1.0/tests/test_commands.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    10593 2023-07-15 10:18:27.000000 vhatable-1.1.0/tests/test_factory.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    11653 2023-07-15 10:18:27.000000 vhatable-1.1.0/tests/test_filters.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    12798 2023-07-15 10:18:27.000000 vhatable-1.1.0/tests/test_processors.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7469 2023-07-15 10:18:27.000000 vhatable-1.1.0/tests/test_units.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 11:29:55.887573 vhatable-1.1.0/vhatable/
+-rw-r--r--   0 fred      (1000) fred      (1000)      958 2023-07-15 11:28:16.000000 vhatable-1.1.0/vhatable/__init__.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9351 2023-05-28 10:43:18.000000 vhatable-1.1.0/vhatable/cell.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6735 2023-06-12 21:44:47.000000 vhatable-1.1.0/vhatable/cellv2.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    23356 2023-06-11 17:38:31.000000 vhatable-1.1.0/vhatable/core.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     9302 2023-07-15 10:18:27.000000 vhatable-1.1.0/vhatable/corev2.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    12333 2023-07-15 10:18:27.000000 vhatable-1.1.0/vhatable/demo.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     7106 2023-07-15 10:18:27.000000 vhatable-1.1.0/vhatable/filters.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     3956 2023-07-15 10:18:27.000000 vhatable-1.1.0/vhatable/filtersv2.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    21643 2023-07-15 10:18:27.000000 vhatable-1.1.0/vhatable/processors.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    20643 2023-06-11 17:38:31.000000 vhatable-1.1.0/vhatable/sample.py
+-rw-r--r--   0 fred      (1000) fred      (1000)     6377 2023-07-15 10:18:27.000000 vhatable-1.1.0/vhatable/samplev2.py
+-rw-r--r--   0 fred      (1000) fred      (1000)    12950 2023-07-15 11:28:20.000000 vhatable-1.1.0/vhatable/units.py
+drwxr-xr-x   0 fred      (1000) fred      (1000)        0 2023-07-15 11:29:55.890906 vhatable-1.1.0/vhatable.egg-info/
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      636 2023-07-15 11:29:55.000000 vhatable-1.1.0/vhatable.egg-info/PKG-INFO
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      591 2023-07-15 11:29:55.000000 vhatable-1.1.0/vhatable.egg-info/SOURCES.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)        1 2023-07-15 11:29:55.000000 vhatable-1.1.0/vhatable.egg-info/dependency_links.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      162 2023-07-15 11:29:55.000000 vhatable-1.1.0/vhatable.egg-info/entry_points.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)      129 2023-07-15 11:29:55.000000 vhatable-1.1.0/vhatable.egg-info/requires.txt
+-rwxr-xr-x   0 fred      (1000) fred      (1000)        9 2023-07-15 11:29:55.000000 vhatable-1.1.0/vhatable.egg-info/top_level.txt
```

### Comparing `vhatable-1.0.3/LICENSE.txt` & `vhatable-1.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vhatable-1.0.3/PKG-INFO` & `vhatable-1.1.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: vhatable
-Version: 1.0.3
+Version: 1.1.0
 Summary: vhatable.
 Home-page: https://github.com/fred49/vhatable
 Author: Frederic MARTIN
 Author-email: frederic.martin.fma@gmail.com
 License: GPL3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: SAMPLE
+Provides-Extra: SAMPLEV2
+Provides-Extra: DEMO
 Provides-Extra: DEV
 License-File: LICENSE.txt
 
 long_description
-
```

### Comparing `vhatable-1.0.3/setup.py` & `vhatable-1.1.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,24 +72,30 @@
     # simple. Or you can use find_packages.
     packages=find_packages(exclude=["contrib", "docs", "tests*"]),
 
     # List run-time dependencies here.  These will be installed by pip when your
     # project is installed.
     install_requires=[
         'veryprettytable==0.8.1',
+        'prettytable==3.7.0',
         'humanfriendly==9.0'
     ],
     extras_require={
         "SAMPLE": [],
+        "SAMPLEV2": [],
+        "DEMO": [],
         'DEV': [
             'pytest',
             'flake8',
             'tox',
+            'twine',
             'pylint',
         ]
     },
     entry_points={
         "console_scripts": [
-            "vhatable-sample = vhatable.sample:main [SAMPLE]"
+            "vhatable-sample = vhatable.sample:main [SAMPLE]",
+            "vhatable-samplev2 = vhatable.samplev2:main [SAMPLEV2]",
+            "vhatable-demo = vhatable.demo:main [DEMO]"
         ],
     },
 )
```

### Comparing `vhatable-1.0.3/vhatable/__init__.py` & `vhatable-1.1.0/vhatable/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,12 +21,12 @@
 # Copyright 2014-2016 Frédéric MARTIN
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
-__version__ = '1.0.3'
+__version__ = '1.1.0'
 # from .core import *
 from . import core
 from . import cell
 from . import filters
```

### Comparing `vhatable-1.0.3/vhatable/cell.py` & `vhatable-1.1.0/vhatable/cell.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
 
-
 import datetime
 import logging
 
 from humanfriendly import format_size
 
 
 class CellFactory:
@@ -50,15 +49,15 @@
             "expirationDate",
             "uploadDate"
         ]
         self.size_cells = ["size"]
         self.custom_cells = {}
 
     def __call__(self, name, value, row=None):
-        if name in list(self.custom_cells.keys()):
+        if name in self.custom_cells:
             clazz = self.custom_cells.get(name)
         elif name in self.date_cells:
             clazz = DateCell
         elif name in self.size_cells:
             clazz = SizeCell
         elif isinstance(value, bool):
             clazz = BCell
@@ -223,40 +222,44 @@
 class DateCell(BaseCell):
     """TODO"""
 
     millisecond = True
 
     # pylint: disable=too-few-public-methods
     def __init__(self, value):
-        super(DateCell, self).__init__(value)
-        self._d_formatt = "{da:%Y-%m-%d %H:%M:%S}"
+        super().__init__(value)
+        fmt = "{da:%Y-%m-%d %H:%M:%S}"
+        self._format = fmt
+        self._format_vertical = fmt
+        # self._format_filter = fmt
 
     def __unicode__(self):
         if self.raw:
             return str(self.value)
         if self.value is not None:
-            # if self.vertical:
-            #     self._d_formatt = "{da:%Y-%m-%d}"
+            fmt = self._format
+            if self.vertical:
+                fmt = self._format_vertical
             div = 1
             if self.millisecond:
                 div = 1000
-            return self._d_formatt.format(
+            return fmt.format(
                 da=datetime.datetime.fromtimestamp(self.value / div))
         return self.none
 
     def __div__(self, value):
         return self.value / value
 
 
 class ICell(int, BaseCell):
     """TODO"""
     # pylint: disable=too-few-public-methods
 
     def __init__(self, value):
-        super(ICell, self).__init__(value)
+        super().__init__(value)
         self.value = value
 
     def __unicode__(self):
         if self.raw:
             return str(self.value)
         return str(self.value)
 
@@ -341,8 +344,8 @@
 
 
 class ComplexCellBuilder(CellBuilder):
     """wrapper to build a ComplexCell with extra parameters."""
     # pylint: disable=too-few-public-methods
 
     def __init__(self, formatt, formatv=None, formatf=None):
-        super(ComplexCellBuilder, self).__init__(formatt, formatv, formatf, cell=ComplexCell)
+        super().__init__(formatt, formatv, formatf, cell=ComplexCell)
```

### Comparing `vhatable-1.0.3/vhatable/core.py` & `vhatable-1.1.0/vhatable/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
 
+# pylint: skip-file
+# flake8: noqa
+# Deprecated module
+
 import json
 import time
 import logging
 import logging.handlers
 
 from collections import OrderedDict
 from functools import wraps
@@ -53,14 +57,16 @@
         def time_wrapper(*args, **kwargs):
             self.log.debug("args: %s", args)
             self.log.debug("kwargs: %s", kwargs)
             start = time.time()
             res = original_func(*args, **kwargs)
             end = time.time()
             diff = end - start
+            # enforce string length to avoid random length
+            diff = f'{diff:.15f}'
             if len(args) > 0:
                 first_arg = args[0]
                 self.enabled = getattr(first_arg, "verbose", self.enabled)
             self.log.debug(self.label, {'time': diff})
             if self.enabled:
                 print(self.label % {'time': diff})
             return res
@@ -105,22 +111,20 @@
                             matches += 1
                 self.log.debug("matches: %s", matches)
                 self.log.debug("enabled_filters: %s", enabled_filters)
                 if enabled_filters == 0:
                     return True
                 if matches == enabled_filters:
                     return True
-            else:
-                if filters.is_enable():
-                    if filters(row):
-                        return True
-                else:
+                return False
+            if filters.is_enable():
+                if filters(row):
                     return True
-        else:
-            return True
+                return False
+        return True
 
     def get_raw(self):
         """TODO"""
         raise NotImplementedError()
 
     def get_json(self):
         """TODO"""
```

### Comparing `vhatable-1.0.3/vhatable/filters.py` & `vhatable-1.1.0/vhatable/filters.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with Vhatable cli.  If not, see <http://www.gnu.org/licenses/>.
 #
-# Copyright 2014 Frédéric MARTIN
+# Copyright 2023 Frédéric MARTIN
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
 
@@ -68,16 +68,16 @@
             return vals
         return self._get_val(row, self.prop)
 
     def _get_val(self, row, prop):
         val = row.get(prop)
         if val is None:
             raise ValueError("missing key : " + self.prop)
-        self.log.debug("type: %s", type(val))
-        self.log.debug("value: '%s'", val)
+        # self.log.debug("type: %s", type(val))
+        # self.log.debug("value: '%s'", val)
         return val
 
 
 class PartialOr(Filter):
     """Get the current property into the current row, and match the result with
      a list of values"""
 
@@ -167,25 +167,27 @@
         if self.is_enable():
             pattern = r"^.*" + value + ".*$"
             self.regex = re.compile(pattern)
 
     def __call__(self, row):
         if not self.is_enable():
             return True
-        vals = self.get_val(row)
-        if isinstance(vals, dict):
-            for val in list(vals.values()):
+        val = self.get_val(row)
+        if isinstance(val, dict):
+            # no idea how it is possible
+            for val in list(val.values()):
                 if self.regex.match(val):
                     return True
         else:
             formatt = "{da:%Y-%m-%d %H:%M:%S}"
-            vals = formatt.format(
-                da=datetime.datetime.fromtimestamp(vals / 1000))
-            self.log.debug("type of values: %s", vals)
-            if self.regex.match(vals):
+            val = formatt.format(
+                da=datetime.datetime.fromtimestamp(val / 1000))
+            self.log.debug("type of value: %s", type(val))
+            self.log.debug("value: %s", val)
+            if self.regex.match(val):
                 return True
         return False
 
 
 class Equal(Filter):
     """Get the current property into the current row, and test equality.
     Only one value is possible"""
@@ -196,17 +198,23 @@
         val = self.get_val(row)
         if val == self.values:
             return True
         return False
 
 
 class Equals(Filter):
-    """Get the current property into the current row, and test equality.
-    A list of values will be test"""
+    """Deprecated. Use EqualMultipleOr.
+    Get the current property into the current row, and test equality.
+    A list of values will be tested"""
 
     def __call__(self, row):
         if not self.is_enable():
             return True
         val = self.get_val(row)
+        self.log.debug("type of value: %s", type(val))
+        self.log.debug("value: %s", val)
+        for v in self.values:
+            self.log.debug("comp: %s", v)
+            self.log.debug("comp type: %s", type(v))
         if val in self.values:
             return True
         return False
```

### Comparing `vhatable-1.0.3/vhatable/sample.py` & `vhatable-1.1.0/vhatable/sample.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,18 @@
 #
 # Contributors list :
 #
 #  Frédéric MARTIN frederic.martin.fma@gmail.com
 #
 
 
+# pylint: skip-file
+# flake8: noqa
+# Deprecated module
+
 import sys
 import time
 import inspect
 import argparse
 import logging
 
 from linshareapi.core import ResourceBuilder
```

### Comparing `vhatable-1.0.3/vhatable.egg-info/PKG-INFO` & `vhatable-1.1.0/vhatable.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: vhatable
-Version: 1.0.3
+Version: 1.1.0
 Summary: vhatable.
 Home-page: https://github.com/fred49/vhatable
 Author: Frederic MARTIN
 Author-email: frederic.martin.fma@gmail.com
 License: GPL3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Provides-Extra: SAMPLE
+Provides-Extra: SAMPLEV2
+Provides-Extra: DEMO
 Provides-Extra: DEV
 License-File: LICENSE.txt
 
 long_description
-
```

