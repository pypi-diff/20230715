# Comparing `tmp/py3make-1.0.3.tar.gz` & `tmp/py3make-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py3make-1.0.3.tar", last modified: Sat Jul 15 16:32:13 2023, max compression
+gzip compressed data, was "py3make-1.0.4.tar", last modified: Sat Jul 15 21:08:40 2023, max compression
```

## Comparing `py3make-1.0.3.tar` & `py3make-1.0.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.703621 py3make-1.0.3/
--rw-rw-rw-   0        0        0     6890 2023-07-15 16:30:55.000000 py3make-1.0.3/CONTRIBUTE
--rw-rw-rw-   0        0        0     2087 2023-07-15 16:30:55.000000 py3make-1.0.3/LICENCE
--rw-rw-rw-   0        0        0      245 2023-07-15 16:30:55.000000 py3make-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0     4620 2023-07-15 16:30:55.000000 py3make-1.0.3/Makefile
--rw-rw-rw-   0        0        0     9752 2023-07-15 16:32:13.687985 py3make-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     7211 2023-07-15 16:30:55.000000 py3make-1.0.3/README.rst
-drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.687985 py3make-1.0.3/examples/
--rw-rw-rw-   0        0        0      355 2023-07-15 16:30:55.000000 py3make-1.0.3/examples/Makefile
--rw-rw-rw-   0        0        0      463 2023-07-15 16:30:55.000000 py3make-1.0.3/examples/simple_examples.py
--rw-rw-rw-   0        0        0     5577 2023-07-15 16:30:55.000000 py3make-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-07-15 16:32:13.703621 py3make-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      459 2023-07-15 16:30:55.000000 py3make-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.672391 py3make-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.687985 py3make-1.0.3/src/py3make/
--rw-rw-rw-   0        0        0      241 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/__init__.py
--rw-rw-rw-   0        0        0       33 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/__main__.py
--rw-rw-rw-   0        0        0     3380 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/_main.py
--rw-rw-rw-   0        0        0     4806 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/_pymake.py
--rw-rw-rw-   0        0        0     1819 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/_utils.py
--rw-rw-rw-   0        0        0      996 2023-07-15 16:30:55.000000 py3make-1.0.3/src/py3make/_version.py
-drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.687985 py3make-1.0.3/src/py3make.egg-info/
--rw-rw-rw-   0        0        0     9752 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      540 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      126 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-15 16:32:13.000000 py3make-1.0.3/src/py3make.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-15 16:32:13.687985 py3make-1.0.3/tests/
--rw-rw-rw-   0        0        0     2003 2023-07-15 16:30:55.000000 py3make-1.0.3/tests/test_main.py
--rw-rw-rw-   0        0        0      169 2023-07-15 16:30:55.000000 py3make-1.0.3/tests/test_pymake.py
--rw-rw-rw-   0        0        0      302 2023-07-15 16:30:55.000000 py3make-1.0.3/tests/test_version.py
--rw-rw-rw-   0        0        0      816 2023-07-15 16:30:55.000000 py3make-1.0.3/tox.ini
+drwxrwxrwx   0        0        0        0 2023-07-15 21:08:40.012574 py3make-1.0.4/
+-rw-rw-rw-   0        0        0     6890 2023-07-15 21:07:50.000000 py3make-1.0.4/CONTRIBUTE
+-rw-rw-rw-   0        0        0     2087 2023-07-15 21:07:50.000000 py3make-1.0.4/LICENCE
+-rw-rw-rw-   0        0        0      171 2023-07-15 21:07:50.000000 py3make-1.0.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     4620 2023-07-15 21:07:50.000000 py3make-1.0.4/Makefile
+-rw-rw-rw-   0        0        0     9737 2023-07-15 21:08:40.012574 py3make-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7211 2023-07-15 21:07:50.000000 py3make-1.0.4/README.rst
+drwxrwxrwx   0        0        0        0 2023-07-15 21:08:39.996951 py3make-1.0.4/examples/
+-rw-rw-rw-   0        0        0      355 2023-07-15 21:07:50.000000 py3make-1.0.4/examples/Makefile
+-rw-rw-rw-   0        0        0      463 2023-07-15 21:07:50.000000 py3make-1.0.4/examples/simple_examples.py
+-rw-rw-rw-   0        0        0     5562 2023-07-15 21:07:50.000000 py3make-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-07-15 21:08:40.012574 py3make-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      459 2023-07-15 21:07:50.000000 py3make-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 21:08:39.996951 py3make-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-15 21:08:40.012574 py3make-1.0.4/src/py3make/
+-rw-rw-rw-   0        0        0      241 2023-07-15 21:07:50.000000 py3make-1.0.4/src/py3make/__init__.py
+-rw-rw-rw-   0        0        0       33 2023-07-15 21:07:50.000000 py3make-1.0.4/src/py3make/__main__.py
+-rw-rw-rw-   0        0        0     3380 2023-07-15 21:07:50.000000 py3make-1.0.4/src/py3make/_main.py
+-rw-rw-rw-   0        0        0     4806 2023-07-15 21:07:50.000000 py3make-1.0.4/src/py3make/_pymake.py
+-rw-rw-rw-   0        0        0     1819 2023-07-15 21:07:50.000000 py3make-1.0.4/src/py3make/_utils.py
+-rw-rw-rw-   0        0        0      996 2023-07-15 21:07:50.000000 py3make-1.0.4/src/py3make/_version.py
+drwxrwxrwx   0        0        0        0 2023-07-15 21:08:40.012574 py3make-1.0.4/src/py3make.egg-info/
+-rw-rw-rw-   0        0        0     9737 2023-07-15 21:08:39.000000 py3make-1.0.4/src/py3make.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      540 2023-07-15 21:08:39.000000 py3make-1.0.4/src/py3make.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 21:08:39.000000 py3make-1.0.4/src/py3make.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-07-15 21:08:39.000000 py3make-1.0.4/src/py3make.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      126 2023-07-15 21:08:39.000000 py3make-1.0.4/src/py3make.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-07-15 21:08:39.000000 py3make-1.0.4/src/py3make.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 21:08:40.012574 py3make-1.0.4/tests/
+-rw-rw-rw-   0        0        0     2003 2023-07-15 21:07:50.000000 py3make-1.0.4/tests/test_main.py
+-rw-rw-rw-   0        0        0      169 2023-07-15 21:07:50.000000 py3make-1.0.4/tests/test_pymake.py
+-rw-rw-rw-   0        0        0      302 2023-07-15 21:07:50.000000 py3make-1.0.4/tests/test_version.py
+-rw-rw-rw-   0        0        0      816 2023-07-15 21:07:50.000000 py3make-1.0.4/tox.ini
```

### Comparing `py3make-1.0.3/CONTRIBUTE` & `py3make-1.0.4/CONTRIBUTE`

 * *Files identical despite different names*

### Comparing `py3make-1.0.3/LICENCE` & `py3make-1.0.4/LICENCE`

 * *Files identical despite different names*

### Comparing `py3make-1.0.3/Makefile` & `py3make-1.0.4/Makefile`

 * *Files identical despite different names*

### Comparing `py3make-1.0.3/PKG-INFO` & `py3make-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: py3make
-Version: 1.0.3
+Version: 1.0.4
 Summary: Makefile execution powered by pure Python
 Author-email: Stephen Karl Larroque <LRQ3000@gmail.com>, Casper da Costa-Luis <casper.dcl@physics.org>
 Maintainer-email: tqdm developers <python.tqdm@gmail.com>
-License: Mozilla Public License 2.0
+License: MIT License
 Project-URL: Homepage, https://github.com/lrq3000/py3make
 Project-URL: Documentation, https://github.com/lrq3000/py3make/blob/master/README.md
 Project-URL: Source, https://github.com/lrq3000/py3make
 Project-URL: Tracker, https://github.com/lrq3000/py3make/issues
 Project-URL: Download, https://github.com/lrq3000/py3make/releases
 Project-URL: Changelog, https://allmychanges.com/p/python/py3make/
 Keywords: make,makefile,gnumake,gnu,console,terminal,cli,py3make,pymake,py-make
```

### Comparing `py3make-1.0.3/README.rst` & `py3make-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `py3make-1.0.3/pyproject.toml` & `py3make-1.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     {name = "Stephen Karl Larroque", email = "LRQ3000@gmail.com"},
 	{name = "Casper da Costa-Luis", email = "casper.dcl@physics.org"},
     ]
 maintainers = [
     {name = "tqdm developers", email = "python.tqdm@gmail.com"},
     ]
 requires-python = ">=3.7"
-license = {text = "Mozilla Public License 2.0"} # { file = "LICENSE" }
+license = {text = "MIT License"} # { file = "LICENSE" }
 keywords = ["make", "makefile", "gnumake", "gnu", "console", "terminal", "cli", "py3make", "pymake", "py-make"]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'License :: OSI Approved :: MIT License',
     'Environment :: Console',
 	'Operating System :: MacOS :: MacOS X',
 	'Operating System :: Microsoft :: Windows',
```

### Comparing `py3make-1.0.3/src/py3make/_main.py` & `py3make-1.0.4/src/py3make/_main.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.3/src/py3make/_pymake.py` & `py3make-1.0.4/src/py3make/_pymake.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.3/src/py3make/_utils.py` & `py3make-1.0.4/src/py3make/_utils.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.3/src/py3make/_version.py` & `py3make-1.0.4/src/py3make/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 except:  # pragma: no cover
     _sh = None
 
 from subprocess import STDOUT
 __all__ = ["__version__"]
 
 # major, minor, patch, -extra
-version_info = 1, 0, 3
+version_info = 1, 0, 4
 
 # Nice string for the version
 __version__ = '.'.join(map(str, version_info))
 
 
 # auto -extra based on commit hash (if not tagged as release)
 if (_sh is not None) and (len(version_info) < 4):  # pragma: no cover
```

### Comparing `py3make-1.0.3/src/py3make.egg-info/PKG-INFO` & `py3make-1.0.4/src/py3make.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: py3make
-Version: 1.0.3
+Version: 1.0.4
 Summary: Makefile execution powered by pure Python
 Author-email: Stephen Karl Larroque <LRQ3000@gmail.com>, Casper da Costa-Luis <casper.dcl@physics.org>
 Maintainer-email: tqdm developers <python.tqdm@gmail.com>
-License: Mozilla Public License 2.0
+License: MIT License
 Project-URL: Homepage, https://github.com/lrq3000/py3make
 Project-URL: Documentation, https://github.com/lrq3000/py3make/blob/master/README.md
 Project-URL: Source, https://github.com/lrq3000/py3make
 Project-URL: Tracker, https://github.com/lrq3000/py3make/issues
 Project-URL: Download, https://github.com/lrq3000/py3make/releases
 Project-URL: Changelog, https://allmychanges.com/p/python/py3make/
 Keywords: make,makefile,gnumake,gnu,console,terminal,cli,py3make,pymake,py-make
```

### Comparing `py3make-1.0.3/src/py3make.egg-info/SOURCES.txt` & `py3make-1.0.4/src/py3make.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py3make-1.0.3/tests/test_main.py` & `py3make-1.0.4/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `py3make-1.0.3/tox.ini` & `py3make-1.0.4/tox.ini`

 * *Files identical despite different names*

