# Comparing `tmp/py3make-1.0.0b1.tar.gz` & `tmp/py3make-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3make-1.0.0b1.tar", last modified: Sat Jul 15 15:40:45 2023, max compression
+gzip compressed data, was "py3make-1.0.1.tar", last modified: Sat Jul 15 16:18:04 2023, max compression
```

## Comparing `py3make-1.0.0b1.tar` & `py3make-1.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 15:40:45.938534 py3make-1.0.0b1/
--rw-rw-rw-   0        0        0     6890 2023-07-15 15:39:36.000000 py3make-1.0.0b1/CONTRIBUTE
--rw-rw-rw-   0        0        0     2099 2023-07-15 15:39:36.000000 py3make-1.0.0b1/LICENCE
--rw-rw-rw-   0        0        0      245 2023-07-15 15:39:36.000000 py3make-1.0.0b1/MANIFEST.in
--rw-rw-rw-   0        0        0     4620 2023-07-15 15:39:36.000000 py3make-1.0.0b1/Makefile
--rw-rw-rw-   0        0        0     9602 2023-07-15 15:40:45.938534 py3make-1.0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     7034 2023-07-15 15:39:36.000000 py3make-1.0.0b1/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-15 15:40:45.938534 py3make-1.0.0b1/examples/
--rw-rw-rw-   0        0        0      355 2023-07-15 15:39:36.000000 py3make-1.0.0b1/examples/Makefile
--rw-rw-rw-   0        0        0      463 2023-07-15 15:39:36.000000 py3make-1.0.0b1/examples/simple_examples.py
--rw-rw-rw-   0        0        0     5586 2023-07-15 15:39:36.000000 py3make-1.0.0b1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 15:40:45.938534 py3make-1.0.0b1/setup.cfg
--rw-rw-rw-   0        0        0      459 2023-07-15 15:39:36.000000 py3make-1.0.0b1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 15:40:45.938534 py3make-1.0.0b1/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 15:40:45.938534 py3make-1.0.0b1/src/py3make/
--rw-rw-rw-   0        0        0      241 2023-07-15 15:39:36.000000 py3make-1.0.0b1/src/py3make/__init__.py
--rw-rw-rw-   0        0        0       33 2023-07-15 15:39:36.000000 py3make-1.0.0b1/src/py3make/__main__.py
--rw-rw-rw-   0        0        0     3380 2023-07-15 15:39:36.000000 py3make-1.0.0b1/src/py3make/_main.py
--rw-rw-rw-   0        0        0     4806 2023-07-15 15:39:36.000000 py3make-1.0.0b1/src/py3make/_pymake.py
--rw-rw-rw-   0        0        0     1819 2023-07-15 15:39:36.000000 py3make-1.0.0b1/src/py3make/_utils.py
--rw-rw-rw-   0        0        0     1002 2023-07-15 15:39:36.000000 py3make-1.0.0b1/src/py3make/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-15 15:40:45.938534 py3make-1.0.0b1/src/py3make.egg-info/
--rw-rw-rw-   0        0        0     9602 2023-07-15 15:40:45.000000 py3make-1.0.0b1/src/py3make.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-07-15 15:40:45.000000 py3make-1.0.0b1/src/py3make.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 15:40:45.000000 py3make-1.0.0b1/src/py3make.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-15 15:40:45.000000 py3make-1.0.0b1/src/py3make.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      126 2023-07-15 15:40:45.000000 py3make-1.0.0b1/src/py3make.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-15 15:40:45.000000 py3make-1.0.0b1/src/py3make.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 15:40:45.938534 py3make-1.0.0b1/tests/
--rw-rw-rw-   0        0        0     2003 2023-07-15 15:39:36.000000 py3make-1.0.0b1/tests/test_main.py
--rw-rw-rw-   0        0        0      169 2023-07-15 15:39:36.000000 py3make-1.0.0b1/tests/test_pymake.py
--rw-rw-rw-   0        0        0      302 2023-07-15 15:39:36.000000 py3make-1.0.0b1/tests/test_version.py
--rw-rw-rw-   0        0        0      816 2023-07-15 15:39:36.000000 py3make-1.0.0b1/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.022978 py3make-1.0.1/
+-rw-rw-rw-   0        0        0     6890 2023-07-15 16:17:11.000000 py3make-1.0.1/CONTRIBUTE
+-rw-rw-rw-   0        0        0     2087 2023-07-15 16:17:11.000000 py3make-1.0.1/LICENCE
+-rw-rw-rw-   0        0        0      245 2023-07-15 16:17:11.000000 py3make-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4620 2023-07-15 16:17:11.000000 py3make-1.0.1/Makefile
+-rw-rw-rw-   0        0        0     9735 2023-07-15 16:18:04.022978 py3make-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7194 2023-07-15 16:17:11.000000 py3make-1.0.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.007405 py3make-1.0.1/examples/
+-rw-rw-rw-   0        0        0      355 2023-07-15 16:17:11.000000 py3make-1.0.1/examples/Makefile
+-rw-rw-rw-   0        0        0      463 2023-07-15 16:17:11.000000 py3make-1.0.1/examples/simple_examples.py
+-rw-rw-rw-   0        0        0     5577 2023-07-15 16:17:11.000000 py3make-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 16:18:04.022978 py3make-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      459 2023-07-15 16:17:11.000000 py3make-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.007405 py3make-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.022978 py3make-1.0.1/src/py3make/
+-rw-rw-rw-   0        0        0      241 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/__main__.py
+-rw-rw-rw-   0        0        0     3380 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/_main.py
+-rw-rw-rw-   0        0        0     4806 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/_pymake.py
+-rw-rw-rw-   0        0        0     1819 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/_utils.py
+-rw-rw-rw-   0        0        0      996 2023-07-15 16:17:11.000000 py3make-1.0.1/src/py3make/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.022978 py3make-1.0.1/src/py3make.egg-info/
+-rw-rw-rw-   0        0        0     9735 2023-07-15 16:18:03.000000 py3make-1.0.1/src/py3make.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-07-15 16:18:04.000000 py3make-1.0.1/src/py3make.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 16:18:03.000000 py3make-1.0.1/src/py3make.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-15 16:18:03.000000 py3make-1.0.1/src/py3make.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      126 2023-07-15 16:18:03.000000 py3make-1.0.1/src/py3make.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-15 16:18:03.000000 py3make-1.0.1/src/py3make.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 16:18:04.022978 py3make-1.0.1/tests/
+-rw-rw-rw-   0        0        0     2003 2023-07-15 16:17:11.000000 py3make-1.0.1/tests/test_main.py
+-rw-rw-rw-   0        0        0      169 2023-07-15 16:17:11.000000 py3make-1.0.1/tests/test_pymake.py
+-rw-rw-rw-   0        0        0      302 2023-07-15 16:17:11.000000 py3make-1.0.1/tests/test_version.py
+-rw-rw-rw-   0        0        0      816 2023-07-15 16:17:11.000000 py3make-1.0.1/tox.ini
```

### Comparing `py3make-1.0.0b1/CONTRIBUTE` & `py3make-1.0.1/CONTRIBUTE`

 * *Files identical despite different names*

### Comparing `py3make-1.0.0b1/LICENCE` & `py3make-1.0.1/LICENCE`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,25 @@
-`py-make` is a product of collaborative work.
+`py3make` is a product of collaborative work.
 Unless otherwise stated, all authors (see commit logs) retain copyright
-for their respective work, and release the work under the MPLv2.0 licence.
+for their respective work, and release the work under the MIT licence.
 
 Exceptions or notable authors are listed below
-in reverse chronological order:
+in chronological order:
 
-* lines of code last modified by Casper da Costa-Luis:
-  MPLv2.0 2016-2019 (c) Casper da Costa-Luis
-  [casperdcl](https://github.com/casperdcl).
 * lines of code last modified by Stephen Karl Larroque:
   MIT 2015-2023 (c) Stephen Karl Larroque
   [LRQ3000](https://github.com/LRQ3000).
+* lines of code last modified by Casper da Costa-Luis:
+  MPLv2.0 2016-2019 (c) Casper da Costa-Luis
+  [casperdcl](https://github.com/casperdcl).
 
 Note: the git history does not reflect the true last author of each LOC,
 instead, look at the https://github.com/tqdm/tqdm history.
 
-Mozilla Public Licence (MPL) v. 2.0 - Exhibit A
------------------------------------------------
-
-This Source Code Form is subject to the terms of the
-Mozilla Public License, v. 2.0.
-If a copy of the MPL was not distributed with this file,
-You can obtain one at https://mozilla.org/MPL/2.0/.
-
-MIT License - Exhibit B
+MIT License - Exhibit A
 -----------------------
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
@@ -38,7 +30,15 @@
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
+
+Mozilla Public Licence (MPL) v. 2.0 - Exhibit B
+-----------------------------------------------
+
+This Source Code Form is subject to the terms of the
+Mozilla Public License, v. 2.0.
+If a copy of the MPL was not distributed with this file,
+You can obtain one at https://mozilla.org/MPL/2.0/.
```

### Comparing `py3make-1.0.0b1/Makefile` & `py3make-1.0.1/Makefile`

 * *Files identical despite different names*

### Comparing `py3make-1.0.0b1/PKG-INFO` & `py3make-1.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: py3make
-Version: 1.0.0b1
+Version: 1.0.1
 Summary: Makefile execution powered by pure Python
 Author-email: Stephen Karl Larroque <LRQ3000@gmail.com>, Casper da Costa-Luis <casper.dcl@physics.org>
 Maintainer-email: tqdm developers <python.tqdm@gmail.com>
 License: Mozilla Public License 2.0
 Project-URL: Homepage, https://github.com/lrq3000/py3make
 Project-URL: Documentation, https://github.com/lrq3000/py3make/blob/master/README.md
 Project-URL: Source, https://github.com/lrq3000/py3make
 Project-URL: Tracker, https://github.com/lrq3000/py3make/issues
 Project-URL: Download, https://github.com/lrq3000/py3make/releases
 Project-URL: Changelog, https://allmychanges.com/p/python/py3make/
 Keywords: make,makefile,gnumake,gnu,console,terminal,cli,py3make,pymake,py-make
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Classifier: Operating System :: POSIX :: Linux
@@ -198,17 +198,17 @@
 - Stephen Karl Larroque (`lrq3000 <https://github.com/lrq3000>`__, core logic & maintenance Py3)
 - Casper da Costa-Luis (`casperdcl <https://github.com/casperdcl>`__, modularization & self-referential aliases & ironing out edge cases & documentation)
 
 We are grateful for all |GitHub-Contributions|!
 
 .. |Build-Status| image:: https://github.com/lrq3000/py3make/actions/workflows/ci-build.yml/badge.svg?event=push
     :target: https://github.com/lrq3000/py3make/actions/workflows/ci-build.yml
-.. |Coverage-Status| image:: https://coveralls.io/repos/lrq3000/py3make/badge.svg?branch=master
-   :target: https://coveralls.io/github/lrq3000/py3make
-.. |Branch-Coverage-Status| image:: https://codecov.io/gh/lrq3000/py3make/branch/master/graph/badge.svg
+.. |Coverage-Status| image:: https://coveralls.io/repos/github/lrq3000/py3make/badge.svg?branch=main
+   :target: https://coveralls.io/github/lrq3000/py3make?branch=main
+.. |Branch-Coverage-Status| image:: https://codecov.io/gh/lrq3000/py3make/branch/main/graph/badge.svg?token=JCKB7CEBCC 
    :target: https://codecov.io/gh/lrq3000/py3make
 .. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/64b870375f664419b5f2a0a956006db7
    :target: https://app.codacy.com/gh/lrq3000/py3make/dashboard
 .. |GitHub-Status| image:: https://img.shields.io/github/tag/lrq3000/py3make.svg?maxAge=86400&logo=github&logoColor=white
    :target: https://github.com/lrq3000/py3make/releases
 .. |GitHub-Forks| image:: https://img.shields.io/github/forks/lrq3000/py3make.svg?logo=github&logoColor=white
    :target: https://github.com/lrq3000/py3make/network
@@ -230,9 +230,11 @@
    :target: https://pypi.org/project/py3make
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/py3make.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/py3make
 .. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/py3make.svg?logo=koding&logoColor=white
    :target: https://libraries.io/pypi/py3make
 .. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/py3make.svg?logo=koding&logoColor=white
     :target: https://github.com/lrq3000/py3make/network/dependents
-.. |LICENCE| image:: https://img.shields.io/pypi/l/py3make.svg
+.. |LICENCE| image:: https://img.shields.io/badge/License-MIT-yellow.svg
+   :target: https://opensource.org/licenses/MIT
+.. |LICENCEAUTO| image:: https://img.shields.io/pypi/l/py3make.svg
    :target: https://raw.githubusercontent.com/lrq3000/py3make/master/LICENCE
```

### Comparing `py3make-1.0.0b1/README.rst` & `py3make-1.0.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -146,17 +146,17 @@
 - Stephen Karl Larroque (`lrq3000 <https://github.com/lrq3000>`__, core logic & maintenance Py3)
 - Casper da Costa-Luis (`casperdcl <https://github.com/casperdcl>`__, modularization & self-referential aliases & ironing out edge cases & documentation)
 
 We are grateful for all |GitHub-Contributions|!
 
 .. |Build-Status| image:: https://github.com/lrq3000/py3make/actions/workflows/ci-build.yml/badge.svg?event=push
     :target: https://github.com/lrq3000/py3make/actions/workflows/ci-build.yml
-.. |Coverage-Status| image:: https://coveralls.io/repos/lrq3000/py3make/badge.svg?branch=master
-   :target: https://coveralls.io/github/lrq3000/py3make
-.. |Branch-Coverage-Status| image:: https://codecov.io/gh/lrq3000/py3make/branch/master/graph/badge.svg
+.. |Coverage-Status| image:: https://coveralls.io/repos/github/lrq3000/py3make/badge.svg?branch=main
+   :target: https://coveralls.io/github/lrq3000/py3make?branch=main
+.. |Branch-Coverage-Status| image:: https://codecov.io/gh/lrq3000/py3make/branch/main/graph/badge.svg?token=JCKB7CEBCC 
    :target: https://codecov.io/gh/lrq3000/py3make
 .. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/64b870375f664419b5f2a0a956006db7
    :target: https://app.codacy.com/gh/lrq3000/py3make/dashboard
 .. |GitHub-Status| image:: https://img.shields.io/github/tag/lrq3000/py3make.svg?maxAge=86400&logo=github&logoColor=white
    :target: https://github.com/lrq3000/py3make/releases
 .. |GitHub-Forks| image:: https://img.shields.io/github/forks/lrq3000/py3make.svg?logo=github&logoColor=white
    :target: https://github.com/lrq3000/py3make/network
@@ -178,9 +178,11 @@
    :target: https://pypi.org/project/py3make
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/py3make.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/py3make
 .. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/py3make.svg?logo=koding&logoColor=white
    :target: https://libraries.io/pypi/py3make
 .. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/py3make.svg?logo=koding&logoColor=white
     :target: https://github.com/lrq3000/py3make/network/dependents
-.. |LICENCE| image:: https://img.shields.io/pypi/l/py3make.svg
+.. |LICENCE| image:: https://img.shields.io/badge/License-MIT-yellow.svg
+   :target: https://opensource.org/licenses/MIT
+.. |LICENCEAUTO| image:: https://img.shields.io/pypi/l/py3make.svg
    :target: https://raw.githubusercontent.com/lrq3000/py3make/master/LICENCE
```

### Comparing `py3make-1.0.0b1/pyproject.toml` & `py3make-1.0.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     {name = "tqdm developers", email = "python.tqdm@gmail.com"},
     ]
 requires-python = ">=3.7"
 license = {text = "Mozilla Public License 2.0"} # { file = "LICENSE" }
 keywords = ["make", "makefile", "gnumake", "gnu", "console", "terminal", "cli", "py3make", "pymake", "py-make"]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
-    'License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)',
+    'License :: OSI Approved :: MIT License',
     'Environment :: Console',
 	'Operating System :: MacOS :: MacOS X',
 	'Operating System :: Microsoft :: Windows',
 	'Operating System :: POSIX',
 	'Operating System :: POSIX :: BSD',
 	'Operating System :: POSIX :: BSD :: FreeBSD',
 	'Operating System :: POSIX :: Linux',
@@ -120,24 +120,24 @@
 ]
 required_plugins = "pytest-cov"
 
 [tool.coverage.run]
 branch = true
 relative_files = true
 include = [
-    "*/*.py",
+    "*/py3make/*.py",
     ]
 
 [tool.coverage.paths]
 source = ["src"]
 
 [tool.coverage.report]  # Beware: you need to delete .coveragerc if you have one, otherwise .coveragerc will take precedence!
 show_missing = true
 include = [
-    "*/*.py",
+    "*/py3make/*.py",
 ]
 omit = [
     "*/python?.?/*",
     "*/site-packages/nose/*",
     "*/opt/python/pypy*",
     "*/tests/*",
 ]
```

### Comparing `py3make-1.0.0b1/src/py3make/_main.py` & `py3make-1.0.1/src/py3make/_main.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.0b1/src/py3make/_pymake.py` & `py3make-1.0.1/src/py3make/_pymake.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.0b1/src/py3make/_utils.py` & `py3make-1.0.1/src/py3make/_utils.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.0b1/src/py3make/_version.py` & `py3make-1.0.1/src/py3make/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 except:  # pragma: no cover
     _sh = None
 
 from subprocess import STDOUT
 __all__ = ["__version__"]
 
 # major, minor, patch, -extra
-version_info = 1, 0, 0, "b1"
+version_info = 1, 0, 1
 
 # Nice string for the version
 __version__ = '.'.join(map(str, version_info))
 
 
 # auto -extra based on commit hash (if not tagged as release)
 if (_sh is not None) and (len(version_info) < 4):  # pragma: no cover
```

### Comparing `py3make-1.0.0b1/src/py3make.egg-info/PKG-INFO` & `py3make-1.0.1/src/py3make.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: py3make
-Version: 1.0.0b1
+Version: 1.0.1
 Summary: Makefile execution powered by pure Python
 Author-email: Stephen Karl Larroque <LRQ3000@gmail.com>, Casper da Costa-Luis <casper.dcl@physics.org>
 Maintainer-email: tqdm developers <python.tqdm@gmail.com>
 License: Mozilla Public License 2.0
 Project-URL: Homepage, https://github.com/lrq3000/py3make
 Project-URL: Documentation, https://github.com/lrq3000/py3make/blob/master/README.md
 Project-URL: Source, https://github.com/lrq3000/py3make
 Project-URL: Tracker, https://github.com/lrq3000/py3make/issues
 Project-URL: Download, https://github.com/lrq3000/py3make/releases
 Project-URL: Changelog, https://allmychanges.com/p/python/py3make/
 Keywords: make,makefile,gnumake,gnu,console,terminal,cli,py3make,pymake,py-make
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Environment :: Console
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: POSIX :: BSD
 Classifier: Operating System :: POSIX :: BSD :: FreeBSD
 Classifier: Operating System :: POSIX :: Linux
@@ -198,17 +198,17 @@
 - Stephen Karl Larroque (`lrq3000 <https://github.com/lrq3000>`__, core logic & maintenance Py3)
 - Casper da Costa-Luis (`casperdcl <https://github.com/casperdcl>`__, modularization & self-referential aliases & ironing out edge cases & documentation)
 
 We are grateful for all |GitHub-Contributions|!
 
 .. |Build-Status| image:: https://github.com/lrq3000/py3make/actions/workflows/ci-build.yml/badge.svg?event=push
     :target: https://github.com/lrq3000/py3make/actions/workflows/ci-build.yml
-.. |Coverage-Status| image:: https://coveralls.io/repos/lrq3000/py3make/badge.svg?branch=master
-   :target: https://coveralls.io/github/lrq3000/py3make
-.. |Branch-Coverage-Status| image:: https://codecov.io/gh/lrq3000/py3make/branch/master/graph/badge.svg
+.. |Coverage-Status| image:: https://coveralls.io/repos/github/lrq3000/py3make/badge.svg?branch=main
+   :target: https://coveralls.io/github/lrq3000/py3make?branch=main
+.. |Branch-Coverage-Status| image:: https://codecov.io/gh/lrq3000/py3make/branch/main/graph/badge.svg?token=JCKB7CEBCC 
    :target: https://codecov.io/gh/lrq3000/py3make
 .. |Codacy-Grade| image:: https://app.codacy.com/project/badge/Grade/64b870375f664419b5f2a0a956006db7
    :target: https://app.codacy.com/gh/lrq3000/py3make/dashboard
 .. |GitHub-Status| image:: https://img.shields.io/github/tag/lrq3000/py3make.svg?maxAge=86400&logo=github&logoColor=white
    :target: https://github.com/lrq3000/py3make/releases
 .. |GitHub-Forks| image:: https://img.shields.io/github/forks/lrq3000/py3make.svg?logo=github&logoColor=white
    :target: https://github.com/lrq3000/py3make/network
@@ -230,9 +230,11 @@
    :target: https://pypi.org/project/py3make
 .. |PyPI-Versions| image:: https://img.shields.io/pypi/pyversions/py3make.svg?logo=python&logoColor=white
    :target: https://pypi.org/project/py3make
 .. |Libraries-Rank| image:: https://img.shields.io/librariesio/sourcerank/pypi/py3make.svg?logo=koding&logoColor=white
    :target: https://libraries.io/pypi/py3make
 .. |Libraries-Dependents| image:: https://img.shields.io/librariesio/dependent-repos/pypi/py3make.svg?logo=koding&logoColor=white
     :target: https://github.com/lrq3000/py3make/network/dependents
-.. |LICENCE| image:: https://img.shields.io/pypi/l/py3make.svg
+.. |LICENCE| image:: https://img.shields.io/badge/License-MIT-yellow.svg
+   :target: https://opensource.org/licenses/MIT
+.. |LICENCEAUTO| image:: https://img.shields.io/pypi/l/py3make.svg
    :target: https://raw.githubusercontent.com/lrq3000/py3make/master/LICENCE
```

### Comparing `py3make-1.0.0b1/src/py3make.egg-info/SOURCES.txt` & `py3make-1.0.1/src/py3make.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3make-1.0.0b1/tests/test_main.py` & `py3make-1.0.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.0b1/tox.ini` & `py3make-1.0.1/tox.ini`

 * *Files identical despite different names*

