# Comparing `tmp/PySnooper-1.1.1.tar.gz` & `tmp/PySnooper-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\PySnooper-1.1.1.tar", last modified: Sat Apr  2 15:00:18 2022, max compression
+gzip compressed data, was "PySnooper-1.2.0.tar", last modified: Sat Jul 15 15:03:42 2023, max compression
```

## Comparing `PySnooper-1.1.1.tar` & `PySnooper-1.2.0.tar`

### file list

```diff
@@ -1,48 +1,50 @@
-drwxrwxrwx   0        0        0        0 2022-04-02 15:00:18.575000 PySnooper-1.1.1/
--rw-rw-rw-   0        0        0     1085 2019-05-13 09:19:52.000000 PySnooper-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      144 2019-09-02 17:02:20.000000 PySnooper-1.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6214 2022-04-02 15:00:18.574000 PySnooper-1.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2022-04-02 15:00:18.539000 PySnooper-1.1.1/PySnooper.egg-info/
--rw-rw-rw-   0        0        0     6214 2022-04-02 15:00:18.000000 PySnooper-1.1.1/PySnooper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1014 2022-04-02 15:00:18.000000 PySnooper-1.1.1/PySnooper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-04-02 15:00:18.000000 PySnooper-1.1.1/PySnooper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-04-02 15:00:18.000000 PySnooper-1.1.1/PySnooper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2022-04-02 15:00:18.000000 PySnooper-1.1.1/PySnooper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4022 2022-03-29 15:00:43.000000 PySnooper-1.1.1/README.md
-drwxrwxrwx   0        0        0        0 2022-04-02 15:00:18.545000 PySnooper-1.1.1/pysnooper/
--rw-rw-rw-   0        0        0      842 2022-04-02 15:00:09.000000 PySnooper-1.1.1/pysnooper/__init__.py
--rw-rw-rw-   0        0        0     2775 2021-05-09 11:48:25.000000 PySnooper-1.1.1/pysnooper/pycompat.py
--rw-rw-rw-   0        0        0    23274 2022-04-02 14:55:22.000000 PySnooper-1.1.1/pysnooper/tracer.py
--rw-rw-rw-   0        0        0     2383 2021-05-09 11:48:17.000000 PySnooper-1.1.1/pysnooper/utils.py
--rw-rw-rw-   0        0        0     3789 2021-05-09 11:48:17.000000 PySnooper-1.1.1/pysnooper/variables.py
--rw-rw-rw-   0        0        0       37 2019-05-13 09:19:52.000000 PySnooper-1.1.1/requirements.in
--rw-rw-rw-   0        0        0      132 2019-05-13 09:19:52.000000 PySnooper-1.1.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2022-04-02 15:00:18.576000 PySnooper-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1625 2021-05-19 08:23:39.000000 PySnooper-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2022-04-02 15:00:18.551000 PySnooper-1.1.1/tests/
--rw-rw-rw-   0        0        0       61 2019-05-13 09:19:52.000000 PySnooper-1.1.1/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-02 15:00:18.556000 PySnooper-1.1.1/tests/mini_toolbox/
--rw-rw-rw-   0        0        0     8570 2021-05-09 11:48:17.000000 PySnooper-1.1.1/tests/mini_toolbox/__init__.py
--rw-rw-rw-   0        0        0    14828 2019-06-18 18:34:46.000000 PySnooper-1.1.1/tests/mini_toolbox/contextlib.py
--rw-rw-rw-   0        0        0    56522 2021-05-09 11:48:25.000000 PySnooper-1.1.1/tests/mini_toolbox/pathlib.py
-drwxrwxrwx   0        0        0        0 2022-04-02 15:00:18.561000 PySnooper-1.1.1/tests/samples/
--rw-rw-rw-   0        0        0        0 2019-05-13 09:19:52.000000 PySnooper-1.1.1/tests/samples/__init__.py
--rw-rw-rw-   0        0        0     1346 2022-03-29 15:00:43.000000 PySnooper-1.1.1/tests/samples/exception.py
--rw-rw-rw-   0        0        0     1069 2022-03-29 15:00:43.000000 PySnooper-1.1.1/tests/samples/indentation.py
--rw-rw-rw-   0        0        0     2411 2022-03-29 15:00:43.000000 PySnooper-1.1.1/tests/samples/recursion.py
--rw-rw-rw-   0        0        0     1561 2022-03-29 15:00:43.000000 PySnooper-1.1.1/tests/test_chinese.py
--rw-rw-rw-   0        0        0      316 2021-05-09 11:48:17.000000 PySnooper-1.1.1/tests/test_mini_toolbox.py
-drwxrwxrwx   0        0        0        0 2022-04-02 15:00:18.565000 PySnooper-1.1.1/tests/test_multiple_files/
--rw-rw-rw-   0        0        0        0 2019-09-02 17:02:20.000000 PySnooper-1.1.1/tests/test_multiple_files/__init__.py
-drwxrwxrwx   0        0        0        0 2022-04-02 15:00:18.569000 PySnooper-1.1.1/tests/test_multiple_files/multiple_files/
--rw-rw-rw-   0        0        0        0 2019-09-02 17:02:20.000000 PySnooper-1.1.1/tests/test_multiple_files/multiple_files/__init__.py
--rw-rw-rw-   0        0        0      149 2019-09-02 17:02:20.000000 PySnooper-1.1.1/tests/test_multiple_files/multiple_files/bar.py
--rw-rw-rw-   0        0        0      255 2022-03-29 15:00:43.000000 PySnooper-1.1.1/tests/test_multiple_files/multiple_files/foo.py
--rw-rw-rw-   0        0        0     1626 2021-05-09 11:48:17.000000 PySnooper-1.1.1/tests/test_multiple_files/test_multiple_files.py
--rw-rw-rw-   0        0        0     1644 2022-03-29 15:00:43.000000 PySnooper-1.1.1/tests/test_not_implemented.py
--rw-rw-rw-   0        0        0    65133 2022-04-02 14:55:22.000000 PySnooper-1.1.1/tests/test_pysnooper.py
-drwxrwxrwx   0        0        0        0 2022-04-02 15:00:18.573000 PySnooper-1.1.1/tests/test_utils/
--rw-rw-rw-   0        0        0        0 2019-09-02 17:02:20.000000 PySnooper-1.1.1/tests/test_utils/__init__.py
--rw-rw-rw-   0        0        0      476 2019-09-02 17:02:20.000000 PySnooper-1.1.1/tests/test_utils/test_ensure_tuple.py
--rw-rw-rw-   0        0        0     3962 2022-04-02 14:55:22.000000 PySnooper-1.1.1/tests/test_utils/test_regex.py
--rw-rw-rw-   0        0        0    14737 2021-05-19 08:22:09.000000 PySnooper-1.1.1/tests/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:42.465229 PySnooper-1.2.0/
+-rw-rw-rw-   0        0        0      419 2023-07-15 14:26:30.000000 PySnooper-1.2.0/AUTHORS
+-rw-rw-rw-   0        0        0     1106 2019-04-24 09:27:26.000000 PySnooper-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      150 2020-05-16 19:29:33.000000 PySnooper-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5174 2023-07-15 15:03:42.465229 PySnooper-1.2.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:42.394235 PySnooper-1.2.0/PySnooper.egg-info/
+-rw-rw-rw-   0        0        0     5174 2023-07-15 15:03:42.000000 PySnooper-1.2.0/PySnooper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1047 2023-07-15 15:03:42.000000 PySnooper-1.2.0/PySnooper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 15:03:42.000000 PySnooper-1.2.0/PySnooper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-15 15:03:42.000000 PySnooper-1.2.0/PySnooper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-15 15:03:42.000000 PySnooper-1.2.0/PySnooper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4022 2022-01-14 18:27:51.000000 PySnooper-1.2.0/README.md
+-rw-rw-rw-   0        0        0       84 2023-07-15 14:26:30.000000 PySnooper-1.2.0/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:42.405229 PySnooper-1.2.0/pysnooper/
+-rw-rw-rw-   0        0        0      842 2023-07-15 14:57:54.000000 PySnooper-1.2.0/pysnooper/__init__.py
+-rw-rw-rw-   0        0        0     2775 2021-02-27 09:13:43.000000 PySnooper-1.2.0/pysnooper/pycompat.py
+-rw-rw-rw-   0        0        0    23451 2023-07-15 14:57:19.000000 PySnooper-1.2.0/pysnooper/tracer.py
+-rw-rw-rw-   0        0        0     2383 2020-05-16 19:29:33.000000 PySnooper-1.2.0/pysnooper/utils.py
+-rw-rw-rw-   0        0        0     3789 2020-05-16 19:29:33.000000 PySnooper-1.2.0/pysnooper/variables.py
+-rw-rw-rw-   0        0        0       37 2019-04-24 20:17:25.000000 PySnooper-1.2.0/requirements.in
+-rw-rw-rw-   0        0        0      138 2019-04-24 20:17:25.000000 PySnooper-1.2.0/requirements.txt
+-rw-rw-rw-   0        0        0     1184 2023-07-15 15:03:42.469226 PySnooper-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1723 2023-07-15 15:02:23.000000 PySnooper-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:42.422225 PySnooper-1.2.0/tests/
+-rw-rw-rw-   0        0        0       64 2020-05-16 19:29:33.000000 PySnooper-1.2.0/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:42.430225 PySnooper-1.2.0/tests/mini_toolbox/
+-rw-rw-rw-   0        0        0     8570 2020-06-12 09:34:24.000000 PySnooper-1.2.0/tests/mini_toolbox/__init__.py
+-rw-rw-rw-   0        0        0    15264 2020-05-16 19:29:33.000000 PySnooper-1.2.0/tests/mini_toolbox/contextlib.py
+-rw-rw-rw-   0        0        0    56522 2021-02-27 09:13:43.000000 PySnooper-1.2.0/tests/mini_toolbox/pathlib.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:42.442236 PySnooper-1.2.0/tests/samples/
+-rw-rw-rw-   0        0        0        0 2020-05-16 19:29:33.000000 PySnooper-1.2.0/tests/samples/__init__.py
+-rw-rw-rw-   0        0        0     1346 2022-01-14 18:21:02.000000 PySnooper-1.2.0/tests/samples/exception.py
+-rw-rw-rw-   0        0        0     1069 2022-01-14 18:23:30.000000 PySnooper-1.2.0/tests/samples/indentation.py
+-rw-rw-rw-   0        0        0     2411 2022-01-14 18:23:30.000000 PySnooper-1.2.0/tests/samples/recursion.py
+-rw-rw-rw-   0        0        0     1509 2022-07-01 10:05:53.000000 PySnooper-1.2.0/tests/test_chinese.py
+-rw-rw-rw-   0        0        0      316 2020-05-16 19:29:33.000000 PySnooper-1.2.0/tests/test_mini_toolbox.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:42.447227 PySnooper-1.2.0/tests/test_multiple_files/
+-rw-rw-rw-   0        0        0        0 2020-05-16 19:29:33.000000 PySnooper-1.2.0/tests/test_multiple_files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:42.454228 PySnooper-1.2.0/tests/test_multiple_files/multiple_files/
+-rw-rw-rw-   0        0        0        0 2020-05-16 19:29:33.000000 PySnooper-1.2.0/tests/test_multiple_files/multiple_files/__init__.py
+-rw-rw-rw-   0        0        0      155 2020-05-16 19:29:33.000000 PySnooper-1.2.0/tests/test_multiple_files/multiple_files/bar.py
+-rw-rw-rw-   0        0        0      255 2022-01-14 18:20:14.000000 PySnooper-1.2.0/tests/test_multiple_files/multiple_files/foo.py
+-rw-rw-rw-   0        0        0     1626 2020-05-16 19:29:33.000000 PySnooper-1.2.0/tests/test_multiple_files/test_multiple_files.py
+-rw-rw-rw-   0        0        0     1644 2022-01-14 18:23:30.000000 PySnooper-1.2.0/tests/test_not_implemented.py
+-rw-rw-rw-   0        0        0    65133 2023-07-15 14:26:30.000000 PySnooper-1.2.0/tests/test_pysnooper.py
+drwxrwxrwx   0        0        0        0 2023-07-15 15:03:42.463224 PySnooper-1.2.0/tests/test_utils/
+-rw-rw-rw-   0        0        0        0 2020-05-16 19:29:33.000000 PySnooper-1.2.0/tests/test_utils/__init__.py
+-rw-rw-rw-   0        0        0      495 2020-05-16 19:29:33.000000 PySnooper-1.2.0/tests/test_utils/test_ensure_tuple.py
+-rw-rw-rw-   0        0        0     3962 2023-07-15 14:26:30.000000 PySnooper-1.2.0/tests/test_utils/test_regex.py
+-rw-rw-rw-   0        0        0    14737 2021-07-30 14:24:28.000000 PySnooper-1.2.0/tests/utils.py
```

### Comparing `PySnooper-1.1.1/LICENSE` & `PySnooper-1.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2019 Ram Rachum and collaborators
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2019 Ram Rachum and collaborators
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `PySnooper-1.1.1/PySnooper.egg-info/SOURCES.txt` & `PySnooper-1.2.0/PySnooper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,15 @@
+AUTHORS
 LICENSE
 MANIFEST.in
 README.md
+pyproject.toml
 requirements.in
 requirements.txt
+setup.cfg
 setup.py
 PySnooper.egg-info/PKG-INFO
 PySnooper.egg-info/SOURCES.txt
 PySnooper.egg-info/dependency_links.txt
 PySnooper.egg-info/requires.txt
 PySnooper.egg-info/top_level.txt
 pysnooper/__init__.py
```

### Comparing `PySnooper-1.1.1/README.md` & `PySnooper-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/pysnooper/__init__.py` & `PySnooper-1.2.0/pysnooper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 from .tracer import Tracer as snoop
 from .variables import Attrs, Exploding, Indices, Keys
 import collections
 
 __VersionInfo = collections.namedtuple('VersionInfo',
                                        ('major', 'minor', 'micro'))
 
-__version__ = '1.1.1'
+__version__ = '1.2.0'
 __version_info__ = __VersionInfo(*(map(int, __version__.split('.'))))
 
 del collections, __VersionInfo # Avoid polluting the namespace
```

### Comparing `PySnooper-1.1.1/pysnooper/pycompat.py` & `PySnooper-1.2.0/pysnooper/pycompat.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/pysnooper/tracer.py` & `PySnooper-1.2.0/pysnooper/tracer.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 from . import utils, pycompat
 if pycompat.PY2:
     from io import open
 
 
 ipython_filename_pattern = re.compile('^<ipython-input-([0-9]+)-.*>$')
 ansible_filename_pattern = re.compile(r'^(.+\.zip)[/|\\](ansible[/|\\]modules[/|\\].+\.py)$')
+RETURN_OPCODES = {
+    'RETURN_GENERATOR', 'RETURN_VALUE', 'RETURN_CONST',
+    'INSTRUMENTED_RETURN_GENERATOR', 'INSTRUMENTED_RETURN_VALUE',
+    'INSTRUMENTED_RETURN_CONST', 'YIELD_VALUE', 'INSTRUMENTED_YIELD_VALUE'
+}
 
 
 def get_local_reprs(frame, watch=(), custom_repr=(), max_length=None, normalize=False):
     code = frame.f_code
     vars_order = (code.co_varnames + code.co_cellvars + code.co_freevars +
                   tuple(frame.f_locals.keys()))
 
@@ -463,15 +468,15 @@
         thread_info = ""
         if self.thread_info:
             if self.normalize:
                 raise NotImplementedError("normalize is not supported with "
                                           "thread_info")
             current_thread = threading.current_thread()
             thread_info = "{ident}-{name} ".format(
-                ident=current_thread.ident, name=current_thread.getName())
+                ident=current_thread.ident, name=current_thread.name)
         thread_info = self.set_thread_info_padding(thread_info)
 
         ### Reporting newish and modified variables: ##########################
         #                                                                     #
         old_local_reprs = self.frame_to_local_reprs.get(frame, {})
         self.frame_to_local_reprs[frame] = local_reprs = \
                                        get_local_reprs(frame,
@@ -523,16 +528,15 @@
         # https://stackoverflow.com/a/12800909/2482744
         code_byte = frame.f_code.co_code[frame.f_lasti]
         if not isinstance(code_byte, int):
             code_byte = ord(code_byte)
         ended_by_exception = (
                 event == 'return'
                 and arg is None
-                and (opcode.opname[code_byte]
-                     not in ('RETURN_VALUE', 'YIELD_VALUE'))
+                and opcode.opname[code_byte] not in RETURN_OPCODES
         )
 
         if ended_by_exception:
             self.write('{_FOREGROUND_RED}{indent}Call ended by exception{_STYLE_RESET_ALL}'.
                        format(**locals()))
         else:
             self.write(u'{indent}{_STYLE_DIM}{timestamp} {thread_info}{event:9} '
```

### Comparing `PySnooper-1.1.1/pysnooper/utils.py` & `PySnooper-1.2.0/pysnooper/utils.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/pysnooper/variables.py` & `PySnooper-1.2.0/pysnooper/variables.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/setup.py` & `PySnooper-1.2.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-# Copyright 2019 Ram Rachum and collaborators.
-# This program is distributed under the MIT license.
-import setuptools
-import re
-
-
-def read_file(filename):
-    with open(filename) as file:
-        return file.read()
-
-version = re.search("__version__ = '([0-9.]*)'",
-                    read_file('pysnooper/__init__.py')).group(1)
-
-setuptools.setup(
-    name='PySnooper',
-    version=version,
-    author='Ram Rachum',
-    author_email='ram@rachum.com',
-    description="A poor man's debugger for Python.",
-    long_description=read_file('README.md'),
-    long_description_content_type='text/markdown',
-    url='https://github.com/cool-RR/PySnooper',
-    packages=setuptools.find_packages(exclude=['tests*']),
-    install_requires=read_file('requirements.in'),
-    extras_require={
-        'tests': {
-            'pytest',
-        },
-    },
-    classifiers=[
-        'Environment :: Console',
-        'Intended Audience :: Developers',
-        'Programming Language :: Python :: 2.7',
-        'Programming Language :: Python :: 3.4',
-        'Programming Language :: Python :: 3.5',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: 3.9',
-        'Programming Language :: Python :: 3.10',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Programming Language :: Python :: Implementation :: PyPy',
-        'License :: OSI Approved :: MIT License',
-        'Operating System :: OS Independent',
-        'Topic :: Software Development :: Debuggers',
-    ],
-)
+# Copyright 2019 Ram Rachum and collaborators.
+# This program is distributed under the MIT license.
+import setuptools
+import re
+
+
+def read_file(filename):
+    with open(filename) as file:
+        return file.read()
+
+version = re.search("__version__ = '([0-9.]*)'",
+                    read_file('pysnooper/__init__.py')).group(1)
+
+setuptools.setup(
+    name='PySnooper',
+    version=version,
+    author='Ram Rachum',
+    author_email='ram@rachum.com',
+    description="A poor man's debugger for Python.",
+    long_description=read_file('README.md'),
+    long_description_content_type='text/markdown',
+    url='https://github.com/cool-RR/PySnooper',
+    packages=setuptools.find_packages(exclude=['tests*']),
+    install_requires=read_file('requirements.in'),
+    extras_require={
+        'tests': {
+            'pytest',
+        },
+    },
+    classifiers=[
+        'Environment :: Console',
+        'Intended Audience :: Developers',
+        'Programming Language :: Python :: 2.7',
+        'Programming Language :: Python :: 3.4',
+        'Programming Language :: Python :: 3.5',
+        'Programming Language :: Python :: 3.6',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: Implementation :: CPython',
+        'Programming Language :: Python :: Implementation :: PyPy',
+        'License :: OSI Approved :: MIT License',
+        'Operating System :: OS Independent',
+        'Topic :: Software Development :: Debuggers',
+    ],
+)
```

### Comparing `PySnooper-1.1.1/tests/mini_toolbox/__init__.py` & `PySnooper-1.2.0/tests/mini_toolbox/__init__.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/tests/mini_toolbox/contextlib.py` & `PySnooper-1.2.0/tests/mini_toolbox/contextlib.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,436 +1,436 @@
-"""contextlib2 - backports and enhancements to the contextlib module"""
-
-import sys
-import warnings
-from collections import deque
-from functools import wraps
-
-__all__ = ["contextmanager", "closing", "ContextDecorator", "ExitStack",
-           "redirect_stdout", "redirect_stderr", "suppress"]
-
-# Backwards compatibility
-__all__ += ["ContextStack"]
-
-class ContextDecorator(object):
-    "A base class or mixin that enables context managers to work as decorators."
-
-    def refresh_cm(self):
-        """Returns the context manager used to actually wrap the call to the
-        decorated function.
-
-        The default implementation just returns *self*.
-
-        Overriding this method allows otherwise one-shot context managers
-        like _GeneratorContextManager to support use as decorators via
-        implicit recreation.
-
-        DEPRECATED: refresh_cm was never added to the standard library's
-                    ContextDecorator API
-        """
-        warnings.warn("refresh_cm was never added to the standard library",
-                      DeprecationWarning)
-        return self._recreate_cm()
-
-    def _recreate_cm(self):
-        """Return a recreated instance of self.
-
-        Allows an otherwise one-shot context manager like
-        _GeneratorContextManager to support use as
-        a decorator via implicit recreation.
-
-        This is a private interface just for _GeneratorContextManager.
-        See issue #11647 for details.
-        """
-        return self
-
-    def __call__(self, func):
-        @wraps(func)
-        def inner(*args, **kwds):
-            with self._recreate_cm():
-                return func(*args, **kwds)
-        return inner
-
-
-class _GeneratorContextManager(ContextDecorator):
-    """Helper for @contextmanager decorator."""
-
-    def __init__(self, func, args, kwds):
-        self.gen = func(*args, **kwds)
-        self.func, self.args, self.kwds = func, args, kwds
-        # Issue 19330: ensure context manager instances have good docstrings
-        doc = getattr(func, "__doc__", None)
-        if doc is None:
-            doc = type(self).__doc__
-        self.__doc__ = doc
-        # Unfortunately, this still doesn't provide good help output when
-        # inspecting the created context manager instances, since pydoc
-        # currently bypasses the instance docstring and shows the docstring
-        # for the class instead.
-        # See http://bugs.python.org/issue19404 for more details.
-
-    def _recreate_cm(self):
-        # _GCM instances are one-shot context managers, so the
-        # CM must be recreated each time a decorated function is
-        # called
-        return self.__class__(self.func, self.args, self.kwds)
-
-    def __enter__(self):
-        try:
-            return next(self.gen)
-        except StopIteration:
-            raise RuntimeError("generator didn't yield")
-
-    def __exit__(self, type, value, traceback):
-        if type is None:
-            try:
-                next(self.gen)
-            except StopIteration:
-                return
-            else:
-                raise RuntimeError("generator didn't stop")
-        else:
-            if value is None:
-                # Need to force instantiation so we can reliably
-                # tell if we get the same exception back
-                value = type()
-            try:
-                self.gen.throw(type, value, traceback)
-                raise RuntimeError("generator didn't stop after throw()")
-            except StopIteration as exc:
-                # Suppress StopIteration *unless* it's the same exception that
-                # was passed to throw().  This prevents a StopIteration
-                # raised inside the "with" statement from being suppressed.
-                return exc is not value
-            except RuntimeError as exc:
-                # Don't re-raise the passed in exception
-                if exc is value:
-                    return False
-                # Likewise, avoid suppressing if a StopIteration exception
-                # was passed to throw() and later wrapped into a RuntimeError
-                # (see PEP 479).
-                if _HAVE_EXCEPTION_CHAINING and exc.__cause__ is value:
-                    return False
-                raise
-            except:
-                # only re-raise if it's *not* the exception that was
-                # passed to throw(), because __exit__() must not raise
-                # an exception unless __exit__() itself failed.  But throw()
-                # has to raise the exception to signal propagation, so this
-                # fixes the impedance mismatch between the throw() protocol
-                # and the __exit__() protocol.
-                #
-                if sys.exc_info()[1] is not value:
-                    raise
-
-
-def contextmanager(func):
-    """@contextmanager decorator.
-
-    Typical usage:
-
-        @contextmanager
-        def some_generator(<arguments>):
-            <setup>
-            try:
-                yield <value>
-            finally:
-                <cleanup>
-
-    This makes this:
-
-        with some_generator(<arguments>) as <variable>:
-            <body>
-
-    equivalent to this:
-
-        <setup>
-        try:
-            <variable> = <value>
-            <body>
-        finally:
-            <cleanup>
-
-    """
-    @wraps(func)
-    def helper(*args, **kwds):
-        return _GeneratorContextManager(func, args, kwds)
-    return helper
-
-
-class closing(object):
-    """Context to automatically close something at the end of a block.
-
-    Code like this:
-
-        with closing(<module>.open(<arguments>)) as f:
-            <block>
-
-    is equivalent to this:
-
-        f = <module>.open(<arguments>)
-        try:
-            <block>
-        finally:
-            f.close()
-
-    """
-    def __init__(self, thing):
-        self.thing = thing
-    def __enter__(self):
-        return self.thing
-    def __exit__(self, *exc_info):
-        self.thing.close()
-
-
-class _RedirectStream(object):
-
-    _stream = None
-
-    def __init__(self, new_target):
-        self._new_target = new_target
-        # We use a list of old targets to make this CM re-entrant
-        self._old_targets = []
-
-    def __enter__(self):
-        self._old_targets.append(getattr(sys, self._stream))
-        setattr(sys, self._stream, self._new_target)
-        return self._new_target
-
-    def __exit__(self, exctype, excinst, exctb):
-        setattr(sys, self._stream, self._old_targets.pop())
-
-
-class redirect_stdout(_RedirectStream):
-    """Context manager for temporarily redirecting stdout to another file.
-
-        # How to send help() to stderr
-        with redirect_stdout(sys.stderr):
-            help(dir)
-
-        # How to write help() to a file
-        with open('help.txt', 'w') as f:
-            with redirect_stdout(f):
-                help(pow)
-    """
-
-    _stream = "stdout"
-
-
-class redirect_stderr(_RedirectStream):
-    """Context manager for temporarily redirecting stderr to another file."""
-
-    _stream = "stderr"
-
-
-class suppress(object):
-    """Context manager to suppress specified exceptions
-
-    After the exception is suppressed, execution proceeds with the next
-    statement following the with statement.
-
-         with suppress(FileNotFoundError):
-             os.remove(somefile)
-         # Execution still resumes here if the file was already removed
-    """
-
-    def __init__(self, *exceptions):
-        self._exceptions = exceptions
-
-    def __enter__(self):
-        pass
-
-    def __exit__(self, exctype, excinst, exctb):
-        # Unlike isinstance and issubclass, CPython exception handling
-        # currently only looks at the concrete type hierarchy (ignoring
-        # the instance and subclass checking hooks). While Guido considers
-        # that a bug rather than a feature, it's a fairly hard one to fix
-        # due to various internal implementation details. suppress provides
-        # the simpler issubclass based semantics, rather than trying to
-        # exactly reproduce the limitations of the CPython interpreter.
-        #
-        # See http://bugs.python.org/issue12029 for more details
-        return exctype is not None and issubclass(exctype, self._exceptions)
-
-
-# Context manipulation is Python 3 only
-_HAVE_EXCEPTION_CHAINING = sys.version_info[0] >= 3
-if _HAVE_EXCEPTION_CHAINING:
-    def _make_context_fixer(frame_exc):
-        def _fix_exception_context(new_exc, old_exc):
-            # Context may not be correct, so find the end of the chain
-            while 1:
-                exc_context = new_exc.__context__
-                if exc_context is old_exc:
-                    # Context is already set correctly (see issue 20317)
-                    return
-                if exc_context is None or exc_context is frame_exc:
-                    break
-                new_exc = exc_context
-            # Change the end of the chain to point to the exception
-            # we expect it to reference
-            new_exc.__context__ = old_exc
-        return _fix_exception_context
-
-    def _reraise_with_existing_context(exc_details):
-        try:
-            # bare "raise exc_details[1]" replaces our carefully
-            # set-up context
-            fixed_ctx = exc_details[1].__context__
-            raise exc_details[1]
-        except BaseException:
-            exc_details[1].__context__ = fixed_ctx
-            raise
-else:
-    # No exception context in Python 2
-    def _make_context_fixer(frame_exc):
-        return lambda new_exc, old_exc: None
-
-    # Use 3 argument raise in Python 2,
-    # but use exec to avoid SyntaxError in Python 3
-    def _reraise_with_existing_context(exc_details):
-        exc_type, exc_value, exc_tb = exc_details
-        exec ("raise exc_type, exc_value, exc_tb")
-
-# Handle old-style classes if they exist
-try:
-    from types import InstanceType
-except ImportError:
-    # Python 3 doesn't have old-style classes
-    _get_type = type
-else:
-    # Need to handle old-style context managers on Python 2
-    def _get_type(obj):
-        obj_type = type(obj)
-        if obj_type is InstanceType:
-            return obj.__class__ # Old-style class
-        return obj_type # New-style class
-
-# Inspired by discussions on http://bugs.python.org/issue13585
-class ExitStack(object):
-    """Context manager for dynamic management of a stack of exit callbacks
-
-    For example:
-
-        with ExitStack() as stack:
-            files = [stack.enter_context(open(fname)) for fname in filenames]
-            # All opened files will automatically be closed at the end of
-            # the with statement, even if attempts to open files later
-            # in the list raise an exception
-
-    """
-    def __init__(self):
-        self._exit_callbacks = deque()
-
-    def pop_all(self):
-        """Preserve the context stack by transferring it to a new instance"""
-        new_stack = type(self)()
-        new_stack._exit_callbacks = self._exit_callbacks
-        self._exit_callbacks = deque()
-        return new_stack
-
-    def _push_cm_exit(self, cm, cm_exit):
-        """Helper to correctly register callbacks to __exit__ methods"""
-        def _exit_wrapper(*exc_details):
-            return cm_exit(cm, *exc_details)
-        _exit_wrapper.__self__ = cm
-        self.push(_exit_wrapper)
-
-    def push(self, exit):
-        """Registers a callback with the standard __exit__ method signature
-
-        Can suppress exceptions the same way __exit__ methods can.
-
-        Also accepts any object with an __exit__ method (registering a call
-        to the method instead of the object itself)
-        """
-        # We use an unbound method rather than a bound method to follow
-        # the standard lookup behaviour for special methods
-        _cb_type = _get_type(exit)
-        try:
-            exit_method = _cb_type.__exit__
-        except AttributeError:
-            # Not a context manager, so assume its a callable
-            self._exit_callbacks.append(exit)
-        else:
-            self._push_cm_exit(exit, exit_method)
-        return exit # Allow use as a decorator
-
-    def callback(self, callback, *args, **kwds):
-        """Registers an arbitrary callback and arguments.
-
-        Cannot suppress exceptions.
-        """
-        def _exit_wrapper(exc_type, exc, tb):
-            callback(*args, **kwds)
-        # We changed the signature, so using @wraps is not appropriate, but
-        # setting __wrapped__ may still help with introspection
-        _exit_wrapper.__wrapped__ = callback
-        self.push(_exit_wrapper)
-        return callback # Allow use as a decorator
-
-    def enter_context(self, cm):
-        """Enters the supplied context manager
-
-        If successful, also pushes its __exit__ method as a callback and
-        returns the result of the __enter__ method.
-        """
-        # We look up the special methods on the type to match the with statement
-        _cm_type = _get_type(cm)
-        _exit = _cm_type.__exit__
-        result = _cm_type.__enter__(cm)
-        self._push_cm_exit(cm, _exit)
-        return result
-
-    def close(self):
-        """Immediately unwind the context stack"""
-        self.__exit__(None, None, None)
-
-    def __enter__(self):
-        return self
-
-    def __exit__(self, *exc_details):
-        received_exc = exc_details[0] is not None
-
-        # We manipulate the exception state so it behaves as though
-        # we were actually nesting multiple with statements
-        frame_exc = sys.exc_info()[1]
-        _fix_exception_context = _make_context_fixer(frame_exc)
-
-        # Callbacks are invoked in LIFO order to match the behaviour of
-        # nested context managers
-        suppressed_exc = False
-        pending_raise = False
-        while self._exit_callbacks:
-            cb = self._exit_callbacks.pop()
-            try:
-                if cb(*exc_details):
-                    suppressed_exc = True
-                    pending_raise = False
-                    exc_details = (None, None, None)
-            except:
-                new_exc_details = sys.exc_info()
-                # simulate the stack of exceptions by setting the context
-                _fix_exception_context(new_exc_details[1], exc_details[1])
-                pending_raise = True
-                exc_details = new_exc_details
-        if pending_raise:
-            _reraise_with_existing_context(exc_details)
-        return received_exc and suppressed_exc
-
-# Preserve backwards compatibility
-class ContextStack(ExitStack):
-    """Backwards compatibility alias for ExitStack"""
-
-    def __init__(self):
-        warnings.warn("ContextStack has been renamed to ExitStack",
-                      DeprecationWarning)
-        super(ContextStack, self).__init__()
-
-    def register_exit(self, callback):
-        return self.push(callback)
-
-    def register(self, callback, *args, **kwds):
-        return self.callback(callback, *args, **kwds)
-
-    def preserve(self):
-        return self.pop_all()
+"""contextlib2 - backports and enhancements to the contextlib module"""
+
+import sys
+import warnings
+from collections import deque
+from functools import wraps
+
+__all__ = ["contextmanager", "closing", "ContextDecorator", "ExitStack",
+           "redirect_stdout", "redirect_stderr", "suppress"]
+
+# Backwards compatibility
+__all__ += ["ContextStack"]
+
+class ContextDecorator(object):
+    "A base class or mixin that enables context managers to work as decorators."
+
+    def refresh_cm(self):
+        """Returns the context manager used to actually wrap the call to the
+        decorated function.
+
+        The default implementation just returns *self*.
+
+        Overriding this method allows otherwise one-shot context managers
+        like _GeneratorContextManager to support use as decorators via
+        implicit recreation.
+
+        DEPRECATED: refresh_cm was never added to the standard library's
+                    ContextDecorator API
+        """
+        warnings.warn("refresh_cm was never added to the standard library",
+                      DeprecationWarning)
+        return self._recreate_cm()
+
+    def _recreate_cm(self):
+        """Return a recreated instance of self.
+
+        Allows an otherwise one-shot context manager like
+        _GeneratorContextManager to support use as
+        a decorator via implicit recreation.
+
+        This is a private interface just for _GeneratorContextManager.
+        See issue #11647 for details.
+        """
+        return self
+
+    def __call__(self, func):
+        @wraps(func)
+        def inner(*args, **kwds):
+            with self._recreate_cm():
+                return func(*args, **kwds)
+        return inner
+
+
+class _GeneratorContextManager(ContextDecorator):
+    """Helper for @contextmanager decorator."""
+
+    def __init__(self, func, args, kwds):
+        self.gen = func(*args, **kwds)
+        self.func, self.args, self.kwds = func, args, kwds
+        # Issue 19330: ensure context manager instances have good docstrings
+        doc = getattr(func, "__doc__", None)
+        if doc is None:
+            doc = type(self).__doc__
+        self.__doc__ = doc
+        # Unfortunately, this still doesn't provide good help output when
+        # inspecting the created context manager instances, since pydoc
+        # currently bypasses the instance docstring and shows the docstring
+        # for the class instead.
+        # See http://bugs.python.org/issue19404 for more details.
+
+    def _recreate_cm(self):
+        # _GCM instances are one-shot context managers, so the
+        # CM must be recreated each time a decorated function is
+        # called
+        return self.__class__(self.func, self.args, self.kwds)
+
+    def __enter__(self):
+        try:
+            return next(self.gen)
+        except StopIteration:
+            raise RuntimeError("generator didn't yield")
+
+    def __exit__(self, type, value, traceback):
+        if type is None:
+            try:
+                next(self.gen)
+            except StopIteration:
+                return
+            else:
+                raise RuntimeError("generator didn't stop")
+        else:
+            if value is None:
+                # Need to force instantiation so we can reliably
+                # tell if we get the same exception back
+                value = type()
+            try:
+                self.gen.throw(type, value, traceback)
+                raise RuntimeError("generator didn't stop after throw()")
+            except StopIteration as exc:
+                # Suppress StopIteration *unless* it's the same exception that
+                # was passed to throw().  This prevents a StopIteration
+                # raised inside the "with" statement from being suppressed.
+                return exc is not value
+            except RuntimeError as exc:
+                # Don't re-raise the passed in exception
+                if exc is value:
+                    return False
+                # Likewise, avoid suppressing if a StopIteration exception
+                # was passed to throw() and later wrapped into a RuntimeError
+                # (see PEP 479).
+                if _HAVE_EXCEPTION_CHAINING and exc.__cause__ is value:
+                    return False
+                raise
+            except:
+                # only re-raise if it's *not* the exception that was
+                # passed to throw(), because __exit__() must not raise
+                # an exception unless __exit__() itself failed.  But throw()
+                # has to raise the exception to signal propagation, so this
+                # fixes the impedance mismatch between the throw() protocol
+                # and the __exit__() protocol.
+                #
+                if sys.exc_info()[1] is not value:
+                    raise
+
+
+def contextmanager(func):
+    """@contextmanager decorator.
+
+    Typical usage:
+
+        @contextmanager
+        def some_generator(<arguments>):
+            <setup>
+            try:
+                yield <value>
+            finally:
+                <cleanup>
+
+    This makes this:
+
+        with some_generator(<arguments>) as <variable>:
+            <body>
+
+    equivalent to this:
+
+        <setup>
+        try:
+            <variable> = <value>
+            <body>
+        finally:
+            <cleanup>
+
+    """
+    @wraps(func)
+    def helper(*args, **kwds):
+        return _GeneratorContextManager(func, args, kwds)
+    return helper
+
+
+class closing(object):
+    """Context to automatically close something at the end of a block.
+
+    Code like this:
+
+        with closing(<module>.open(<arguments>)) as f:
+            <block>
+
+    is equivalent to this:
+
+        f = <module>.open(<arguments>)
+        try:
+            <block>
+        finally:
+            f.close()
+
+    """
+    def __init__(self, thing):
+        self.thing = thing
+    def __enter__(self):
+        return self.thing
+    def __exit__(self, *exc_info):
+        self.thing.close()
+
+
+class _RedirectStream(object):
+
+    _stream = None
+
+    def __init__(self, new_target):
+        self._new_target = new_target
+        # We use a list of old targets to make this CM re-entrant
+        self._old_targets = []
+
+    def __enter__(self):
+        self._old_targets.append(getattr(sys, self._stream))
+        setattr(sys, self._stream, self._new_target)
+        return self._new_target
+
+    def __exit__(self, exctype, excinst, exctb):
+        setattr(sys, self._stream, self._old_targets.pop())
+
+
+class redirect_stdout(_RedirectStream):
+    """Context manager for temporarily redirecting stdout to another file.
+
+        # How to send help() to stderr
+        with redirect_stdout(sys.stderr):
+            help(dir)
+
+        # How to write help() to a file
+        with open('help.txt', 'w') as f:
+            with redirect_stdout(f):
+                help(pow)
+    """
+
+    _stream = "stdout"
+
+
+class redirect_stderr(_RedirectStream):
+    """Context manager for temporarily redirecting stderr to another file."""
+
+    _stream = "stderr"
+
+
+class suppress(object):
+    """Context manager to suppress specified exceptions
+
+    After the exception is suppressed, execution proceeds with the next
+    statement following the with statement.
+
+         with suppress(FileNotFoundError):
+             os.remove(somefile)
+         # Execution still resumes here if the file was already removed
+    """
+
+    def __init__(self, *exceptions):
+        self._exceptions = exceptions
+
+    def __enter__(self):
+        pass
+
+    def __exit__(self, exctype, excinst, exctb):
+        # Unlike isinstance and issubclass, CPython exception handling
+        # currently only looks at the concrete type hierarchy (ignoring
+        # the instance and subclass checking hooks). While Guido considers
+        # that a bug rather than a feature, it's a fairly hard one to fix
+        # due to various internal implementation details. suppress provides
+        # the simpler issubclass based semantics, rather than trying to
+        # exactly reproduce the limitations of the CPython interpreter.
+        #
+        # See http://bugs.python.org/issue12029 for more details
+        return exctype is not None and issubclass(exctype, self._exceptions)
+
+
+# Context manipulation is Python 3 only
+_HAVE_EXCEPTION_CHAINING = sys.version_info[0] >= 3
+if _HAVE_EXCEPTION_CHAINING:
+    def _make_context_fixer(frame_exc):
+        def _fix_exception_context(new_exc, old_exc):
+            # Context may not be correct, so find the end of the chain
+            while 1:
+                exc_context = new_exc.__context__
+                if exc_context is old_exc:
+                    # Context is already set correctly (see issue 20317)
+                    return
+                if exc_context is None or exc_context is frame_exc:
+                    break
+                new_exc = exc_context
+            # Change the end of the chain to point to the exception
+            # we expect it to reference
+            new_exc.__context__ = old_exc
+        return _fix_exception_context
+
+    def _reraise_with_existing_context(exc_details):
+        try:
+            # bare "raise exc_details[1]" replaces our carefully
+            # set-up context
+            fixed_ctx = exc_details[1].__context__
+            raise exc_details[1]
+        except BaseException:
+            exc_details[1].__context__ = fixed_ctx
+            raise
+else:
+    # No exception context in Python 2
+    def _make_context_fixer(frame_exc):
+        return lambda new_exc, old_exc: None
+
+    # Use 3 argument raise in Python 2,
+    # but use exec to avoid SyntaxError in Python 3
+    def _reraise_with_existing_context(exc_details):
+        exc_type, exc_value, exc_tb = exc_details
+        exec ("raise exc_type, exc_value, exc_tb")
+
+# Handle old-style classes if they exist
+try:
+    from types import InstanceType
+except ImportError:
+    # Python 3 doesn't have old-style classes
+    _get_type = type
+else:
+    # Need to handle old-style context managers on Python 2
+    def _get_type(obj):
+        obj_type = type(obj)
+        if obj_type is InstanceType:
+            return obj.__class__ # Old-style class
+        return obj_type # New-style class
+
+# Inspired by discussions on http://bugs.python.org/issue13585
+class ExitStack(object):
+    """Context manager for dynamic management of a stack of exit callbacks
+
+    For example:
+
+        with ExitStack() as stack:
+            files = [stack.enter_context(open(fname)) for fname in filenames]
+            # All opened files will automatically be closed at the end of
+            # the with statement, even if attempts to open files later
+            # in the list raise an exception
+
+    """
+    def __init__(self):
+        self._exit_callbacks = deque()
+
+    def pop_all(self):
+        """Preserve the context stack by transferring it to a new instance"""
+        new_stack = type(self)()
+        new_stack._exit_callbacks = self._exit_callbacks
+        self._exit_callbacks = deque()
+        return new_stack
+
+    def _push_cm_exit(self, cm, cm_exit):
+        """Helper to correctly register callbacks to __exit__ methods"""
+        def _exit_wrapper(*exc_details):
+            return cm_exit(cm, *exc_details)
+        _exit_wrapper.__self__ = cm
+        self.push(_exit_wrapper)
+
+    def push(self, exit):
+        """Registers a callback with the standard __exit__ method signature
+
+        Can suppress exceptions the same way __exit__ methods can.
+
+        Also accepts any object with an __exit__ method (registering a call
+        to the method instead of the object itself)
+        """
+        # We use an unbound method rather than a bound method to follow
+        # the standard lookup behaviour for special methods
+        _cb_type = _get_type(exit)
+        try:
+            exit_method = _cb_type.__exit__
+        except AttributeError:
+            # Not a context manager, so assume its a callable
+            self._exit_callbacks.append(exit)
+        else:
+            self._push_cm_exit(exit, exit_method)
+        return exit # Allow use as a decorator
+
+    def callback(self, callback, *args, **kwds):
+        """Registers an arbitrary callback and arguments.
+
+        Cannot suppress exceptions.
+        """
+        def _exit_wrapper(exc_type, exc, tb):
+            callback(*args, **kwds)
+        # We changed the signature, so using @wraps is not appropriate, but
+        # setting __wrapped__ may still help with introspection
+        _exit_wrapper.__wrapped__ = callback
+        self.push(_exit_wrapper)
+        return callback # Allow use as a decorator
+
+    def enter_context(self, cm):
+        """Enters the supplied context manager
+
+        If successful, also pushes its __exit__ method as a callback and
+        returns the result of the __enter__ method.
+        """
+        # We look up the special methods on the type to match the with statement
+        _cm_type = _get_type(cm)
+        _exit = _cm_type.__exit__
+        result = _cm_type.__enter__(cm)
+        self._push_cm_exit(cm, _exit)
+        return result
+
+    def close(self):
+        """Immediately unwind the context stack"""
+        self.__exit__(None, None, None)
+
+    def __enter__(self):
+        return self
+
+    def __exit__(self, *exc_details):
+        received_exc = exc_details[0] is not None
+
+        # We manipulate the exception state so it behaves as though
+        # we were actually nesting multiple with statements
+        frame_exc = sys.exc_info()[1]
+        _fix_exception_context = _make_context_fixer(frame_exc)
+
+        # Callbacks are invoked in LIFO order to match the behaviour of
+        # nested context managers
+        suppressed_exc = False
+        pending_raise = False
+        while self._exit_callbacks:
+            cb = self._exit_callbacks.pop()
+            try:
+                if cb(*exc_details):
+                    suppressed_exc = True
+                    pending_raise = False
+                    exc_details = (None, None, None)
+            except:
+                new_exc_details = sys.exc_info()
+                # simulate the stack of exceptions by setting the context
+                _fix_exception_context(new_exc_details[1], exc_details[1])
+                pending_raise = True
+                exc_details = new_exc_details
+        if pending_raise:
+            _reraise_with_existing_context(exc_details)
+        return received_exc and suppressed_exc
+
+# Preserve backwards compatibility
+class ContextStack(ExitStack):
+    """Backwards compatibility alias for ExitStack"""
+
+    def __init__(self):
+        warnings.warn("ContextStack has been renamed to ExitStack",
+                      DeprecationWarning)
+        super(ContextStack, self).__init__()
+
+    def register_exit(self, callback):
+        return self.push(callback)
+
+    def register(self, callback, *args, **kwds):
+        return self.callback(callback, *args, **kwds)
+
+    def preserve(self):
+        return self.pop_all()
```

### Comparing `PySnooper-1.1.1/tests/mini_toolbox/pathlib.py` & `PySnooper-1.2.0/tests/mini_toolbox/pathlib.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/tests/samples/exception.py` & `PySnooper-1.2.0/tests/samples/exception.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/tests/samples/indentation.py` & `PySnooper-1.2.0/tests/samples/indentation.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/tests/samples/recursion.py` & `PySnooper-1.2.0/tests/samples/recursion.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/tests/test_multiple_files/test_multiple_files.py` & `PySnooper-1.2.0/tests/test_multiple_files/test_multiple_files.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/tests/test_not_implemented.py` & `PySnooper-1.2.0/tests/test_not_implemented.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/tests/test_pysnooper.py` & `PySnooper-1.2.0/tests/test_pysnooper.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/tests/test_utils/test_regex.py` & `PySnooper-1.2.0/tests/test_utils/test_regex.py`

 * *Files identical despite different names*

### Comparing `PySnooper-1.1.1/tests/utils.py` & `PySnooper-1.2.0/tests/utils.py`

 * *Files identical despite different names*

