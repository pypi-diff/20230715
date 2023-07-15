# Comparing `tmp/py3make-1.0.1.tar.gz` & `tmp/py3make-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3make-1.0.1.tar", last modified: Sat Jul 15 16:18:04 2023, max compression
+gzip compressed data, was "py3make-1.0.3.tar", last modified: Sat Jul 15 16:32:13 2023, max compression
```

## Comparing `py3make-1.0.1.tar` & `py3make-1.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.022978 py3make-1.0.1/
--rw-rw-rw-   0        0        0     6890 2023-07-15 16:17:11.000000 py3make-1.0.1/CONTRIBUTE
--rw-rw-rw-   0        0        0     2087 2023-07-15 16:17:11.000000 py3make-1.0.1/LICENCE
--rw-rw-rw-   0        0        0      245 2023-07-15 16:17:11.000000 py3make-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4620 2023-07-15 16:17:11.000000 py3make-1.0.1/Makefile
--rw-rw-rw-   0        0        0     9735 2023-07-15 16:18:04.022978 py3make-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7194 2023-07-15 16:17:11.000000 py3make-1.0.1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.007405 py3make-1.0.1/examples/
--rw-rw-rw-   0        0        0      355 2023-07-15 16:17:11.000000 py3make-1.0.1/examples/Makefile
--rw-rw-rw-   0        0        0      463 2023-07-15 16:17:11.000000 py3make-1.0.1/examples/simple_examples.py
--rw-rw-rw-   0        0        0     5577 2023-07-15 16:17:11.000000 py3make-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 16:18:04.022978 py3make-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      459 2023-07-15 16:17:11.000000 py3make-1.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.007405 py3make-1.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.022978 py3make-1.0.1/src/py3make/
--rw-rw-rw-   0        0        0      241 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/__init__.py
--rw-rw-rw-   0        0        0       33 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/__main__.py
--rw-rw-rw-   0        0        0     3380 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/_main.py
--rw-rw-rw-   0        0        0     4806 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/_pymake.py
--rw-rw-rw-   0        0        0     1819 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/_utils.py
--rw-rw-rw-   0        0        0      996 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.022978 py3make-1.0.1/src/py3make.egg-info/
--rw-rw-rw-   0        0        0     9735 2023-07-15 16:18:03.000000 py3make-1.0.1/src/py3make.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-07-15 16:18:04.000000 py3make-1.0.1/src/py3make.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 16:18:03.000000 py3make-1.0.1/src/py3make.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-15 16:18:03.000000 py3make-1.0.1/src/py3make.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      126 2023-07-15 16:18:03.000000 py3make-1.0.1/src/py3make.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-15 16:18:03.000000 py3make-1.0.1/src/py3make.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.022978 py3make-1.0.1/tests/
--rw-rw-rw-   0        0        0     2003 2023-07-15 16:17:11.000000 py3make-1.0.1/tests/test_main.py
--rw-rw-rw-   0        0        0      169 2023-07-15 16:17:11.000000 py3make-1.0.1/tests/test_pymake.py
--rw-rw-rw-   0        0        0      302 2023-07-15 16:17:11.000000 py3make-1.0.1/tests/test_version.py
--rw-rw-rw-   0        0        0      816 2023-07-15 16:17:11.000000 py3make-1.0.1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.703621 py3make-1.0.3/
+-rw-rw-rw-   0        0        0     6890 2023-07-15 16:30:55.000000 py3make-1.0.3/CONTRIBUTE
+-rw-rw-rw-   0        0        0     2087 2023-07-15 16:30:55.000000 py3make-1.0.3/LICENCE
+-rw-rw-rw-   0        0        0      245 2023-07-15 16:30:55.000000 py3make-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4620 2023-07-15 16:30:55.000000 py3make-1.0.3/Makefile
+-rw-rw-rw-   0        0        0     9752 2023-07-15 16:32:13.687985 py3make-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     7211 2023-07-15 16:30:55.000000 py3make-1.0.3/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.687985 py3make-1.0.3/examples/
+-rw-rw-rw-   0        0        0      355 2023-07-15 16:30:55.000000 py3make-1.0.3/examples/Makefile
+-rw-rw-rw-   0        0        0      463 2023-07-15 16:30:55.000000 py3make-1.0.3/examples/simple_examples.py
+-rw-rw-rw-   0        0        0     5577 2023-07-15 16:30:55.000000 py3make-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:32:13.703621 py3make-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      459 2023-07-15 16:30:55.000000 py3make-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.672391 py3make-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.687985 py3make-1.0.3/src/py3make/
+-rw-rw-rw-   0        0        0      241 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/__main__.py
+-rw-rw-rw-   0        0        0     3380 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/_main.py
+-rw-rw-rw-   0        0        0     4806 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/_pymake.py
+-rw-rw-rw-   0        0        0     1819 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/_utils.py
+-rw-rw-rw-   0        0        0      996 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.687985 py3make-1.0.3/src/py3make.egg-info/
+-rw-rw-rw-   0        0        0     9752 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      126 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.687985 py3make-1.0.3/tests/
+-rw-rw-rw-   0        0        0     2003 2023-07-15 16:30:55.000000 py3make-1.0.3/tests/test_main.py
+-rw-rw-rw-   0        0        0      169 2023-07-15 16:30:55.000000 py3make-1.0.3/tests/test_pymake.py
+-rw-rw-rw-   0        0        0      302 2023-07-15 16:30:55.000000 py3make-1.0.3/tests/test_version.py
+-rw-rw-rw-   0        0        0      816 2023-07-15 16:30:55.000000 py3make-1.0.3/tox.ini
```

### Comparing `py3make-1.0.1/CONTRIBUTE` & `py3make-1.0.3/CONTRIBUTE`

 * *Files identical despite different names*

### Comparing `py3make-1.0.1/LICENCE` & `py3make-1.0.3/LICENCE`

 * *Files identical despite different names*

### Comparing `py3make-1.0.1/Makefile` & `py3make-1.0.3/Makefile`

 * *Files identical despite different names*

### Comparing `py3make-1.0.1/PKG-INFO` & `py3make-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3make
-Version: 1.0.1
+Version: 1.0.3
 Summary: Makefile execution powered by pure Python
 Author-email: Stephen Karl Larroque <LRQ3000@gmail.com>, Casper da Costa-Luis <casper.dcl@physics.org>
 Maintainer-email: tqdm developers <python.tqdm@gmail.com>
 License: Mozilla Public License 2.0
 Project-URL: Homepage, https://github.com/lrq3000/py3make
 Project-URL: Documentation, https://github.com/lrq3000/py3make/blob/master/README.md
 Project-URL: Source, https://github.com/lrq3000/py3make
@@ -49,15 +49,15 @@
 Provides-Extra: test
 Provides-Extra: testmeta
 License-File: LICENCE
 
 py3make
 =======
 
-|PyPI-Status| |PyPI-Versions|
+|PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
 
 |Build-Status| |Coverage-Status| |Branch-Coverage-Status| |Codacy-Grade| |Libraries-Rank|
 
 |LICENCE|
 
 
 Bring basic ``Makefile`` support to any system with Python.
@@ -222,18 +222,18 @@
    :target: https://github.com/lrq3000/py3make/pulls
 .. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/lrq3000/py3make.svg?logo=github&logoColor=white
    :target: https://github.com/lrq3000/py3make/graphs/contributors
 .. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/lrq3000/py3make/master.svg?logo=github&logoColor=white&label=pushed
    :target: https://github.com/lrq3000/py3make/pulse
 .. |PyPI-Status| image:: https://img.shields.io/pypi/v/py3make.svg
    :target: https://pypi.org/project/py3make
-.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/py3make.svg?label=pypi%20downloads&logo=python&logoColor=white
-   :target: https://pypi.org/project/py3make
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/py3make.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/py3make
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/py3make.svg?label=pypi%20downloads&logo=python&logoColor=white
+   :target: https://pypi.org/project/py3make
 .. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/py3make.svg?logo=koding&logoColor=white
    :target: https://libraries.io/pypi/py3make
 .. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/py3make.svg?logo=koding&logoColor=white
     :target: https://github.com/lrq3000/py3make/network/dependents
 .. |LICENCE| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
 .. |LICENCEAUTO| image:: https://img.shields.io/pypi/l/py3make.svg
```

### Comparing `py3make-1.0.1/README.rst` & `py3make-1.0.3/README.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 py3make
 =======
 
-|PyPI-Status| |PyPI-Versions|
+|PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
 
 |Build-Status| |Coverage-Status| |Branch-Coverage-Status| |Codacy-Grade| |Libraries-Rank|
 
 |LICENCE|
 
 
 Bring basic ``Makefile`` support to any system with Python.
@@ -170,18 +170,18 @@
    :target: https://github.com/lrq3000/py3make/pulls
 .. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/lrq3000/py3make.svg?logo=github&logoColor=white
    :target: https://github.com/lrq3000/py3make/graphs/contributors
 .. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/lrq3000/py3make/master.svg?logo=github&logoColor=white&label=pushed
    :target: https://github.com/lrq3000/py3make/pulse
 .. |PyPI-Status| image:: https://img.shields.io/pypi/v/py3make.svg
    :target: https://pypi.org/project/py3make
-.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/py3make.svg?label=pypi%20downloads&logo=python&logoColor=white
-   :target: https://pypi.org/project/py3make
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/py3make.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/py3make
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/py3make.svg?label=pypi%20downloads&logo=python&logoColor=white
+   :target: https://pypi.org/project/py3make
 .. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/py3make.svg?logo=koding&logoColor=white
    :target: https://libraries.io/pypi/py3make
 .. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/py3make.svg?logo=koding&logoColor=white
     :target: https://github.com/lrq3000/py3make/network/dependents
 .. |LICENCE| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
 .. |LICENCEAUTO| image:: https://img.shields.io/pypi/l/py3make.svg
```

### Comparing `py3make-1.0.1/pyproject.toml` & `py3make-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py3make-1.0.1/src/py3make/_main.py` & `py3make-1.0.3/src/py3make/_main.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.1/src/py3make/_pymake.py` & `py3make-1.0.3/src/py3make/_pymake.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.1/src/py3make/_utils.py` & `py3make-1.0.3/src/py3make/_utils.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.1/src/py3make/_version.py` & `py3make-1.0.3/src/py3make/_version.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 except:  # pragma: no cover
     _sh = None
 
 from subprocess import STDOUT
 __all__ = ["__version__"]
 
 # major, minor, patch, -extra
-version_info = 1, 0, 1
+version_info = 1, 0, 3
 
 # Nice string for the version
 __version__ = '.'.join(map(str, version_info))
 
 
 # auto -extra based on commit hash (if not tagged as release)
 if (_sh is not None) and (len(version_info) < 4):  # pragma: no cover
```

### Comparing `py3make-1.0.1/src/py3make.egg-info/PKG-INFO` & `py3make-1.0.3/src/py3make.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py3make
-Version: 1.0.1
+Version: 1.0.3
 Summary: Makefile execution powered by pure Python
 Author-email: Stephen Karl Larroque <LRQ3000@gmail.com>, Casper da Costa-Luis <casper.dcl@physics.org>
 Maintainer-email: tqdm developers <python.tqdm@gmail.com>
 License: Mozilla Public License 2.0
 Project-URL: Homepage, https://github.com/lrq3000/py3make
 Project-URL: Documentation, https://github.com/lrq3000/py3make/blob/master/README.md
 Project-URL: Source, https://github.com/lrq3000/py3make
@@ -49,15 +49,15 @@
 Provides-Extra: test
 Provides-Extra: testmeta
 License-File: LICENCE
 
 py3make
 =======
 
-|PyPI-Status| |PyPI-Versions|
+|PyPI-Status| |PyPI-Versions| |PyPI-Downloads|
 
 |Build-Status| |Coverage-Status| |Branch-Coverage-Status| |Codacy-Grade| |Libraries-Rank|
 
 |LICENCE|
 
 
 Bring basic ``Makefile`` support to any system with Python.
@@ -222,18 +222,18 @@
    :target: https://github.com/lrq3000/py3make/pulls
 .. |GitHub-Contributions| image:: https://img.shields.io/github/contributors/lrq3000/py3make.svg?logo=github&logoColor=white
    :target: https://github.com/lrq3000/py3make/graphs/contributors
 .. |GitHub-Updated| image:: https://img.shields.io/github/last-commit/lrq3000/py3make/master.svg?logo=github&logoColor=white&label=pushed
    :target: https://github.com/lrq3000/py3make/pulse
 .. |PyPI-Status| image:: https://img.shields.io/pypi/v/py3make.svg
    :target: https://pypi.org/project/py3make
-.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/py3make.svg?label=pypi%20downloads&logo=python&logoColor=white
-   :target: https://pypi.org/project/py3make
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/py3make.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/py3make
+.. |PyPI-Downloads| image:: https://img.shields.io/pypi/dm/py3make.svg?label=pypi%20downloads&logo=python&logoColor=white
+   :target: https://pypi.org/project/py3make
 .. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/py3make.svg?logo=koding&logoColor=white
    :target: https://libraries.io/pypi/py3make
 .. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/py3make.svg?logo=koding&logoColor=white
     :target: https://github.com/lrq3000/py3make/network/dependents
 .. |LICENCE| image:: https://img.shields.io/badge/License-MIT-yellow.svg
    :target: https://opensource.org/licenses/MIT
 .. |LICENCEAUTO| image:: https://img.shields.io/pypi/l/py3make.svg
```

### Comparing `py3make-1.0.1/src/py3make.egg-info/SOURCES.txt` & `py3make-1.0.3/src/py3make.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3make-1.0.1/tests/test_main.py` & `py3make-1.0.3/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.1/tox.ini` & `py3make-1.0.3/tox.ini`

 * *Files identical despite different names*

