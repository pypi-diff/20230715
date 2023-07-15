# Comparing `tmp/yet_another_wizz_cli-1.2.2.tar.gz` & `tmp/yet_another_wizz_cli-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet_another_wizz_cli-1.2.2.tar", last modified: Mon Jul 10 19:31:40 2023, max compression
+gzip compressed data, was "yet_another_wizz_cli-1.2.3.tar", last modified: Sat Jul 15 11:38:03 2023, max compression
```

## Comparing `yet_another_wizz_cli-1.2.2.tar` & `yet_another_wizz_cli-1.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.782389 yet_another_wizz_cli-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-10 19:31:40.782389 yet_another_wizz_cli-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3957 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:31:40.782389 yet_another_wizz_cli-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.778390 yet_another_wizz_cli-1.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.778390 yet_another_wizz_cli-1.2.2/src/yaw_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.778390 yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/subcommands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.778390 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/default_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/directories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    16003 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/project.py
--rw-r--r--   0 runner    (1001) docker     (123)    19030 2023-07-10 19:31:29.000000 yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:31:40.778390 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4638 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-10 19:31:40.000000 yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.372470 yet_another_wizz_cli-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-15 11:38:03.372470 yet_another_wizz_cli-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 11:38:03.372470 yet_another_wizz_cli-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.368470 yet_another_wizz_cli-1.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.368470 yet_another_wizz_cli-1.2.3/src/yaw_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.368470 yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9512 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17459 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/subcommands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.372470 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17790 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7091 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/default_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/directories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12588 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16003 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15053 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19009 2023-07-15 11:37:50.000000 yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 11:38:03.372470 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4653 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 11:38:03.000000 yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/top_level.txt
```

### Comparing `yet_another_wizz_cli-1.2.2/LICENSE` & `yet_another_wizz_cli-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/PKG-INFO` & `yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yet_another_wizz_cli
-Version: 1.2.2
+Name: yet-another-wizz-cli
+Version: 1.2.3
 Summary: Command line client for yet_another_wizz.
 Home-page: https://github.com/jlvdb/yet_another_wizz_cli.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
@@ -13,40 +13,49 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: plot
 Provides-Extra: style
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
-yet_another_wizz_cli
-====================
+.. image:: https://github.com/jlvdb/yet_another_wizz/blob/main/docs/source/_static/logo-dark.png?raw=true
+    :width: 1000
+    :alt: yet_another_wizz
+
+|
 
 .. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
     :target: https://pypi.org/project/yet_another_wizz_cli/
 .. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz_cli/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz_cli
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
 
 
+Commandline tool
+================
+
 *yet_another_wizz_cli* implements a command line interface for the clustering
 redshift code `yet_another_wizz <https://github.com/jlvdb/yet_another_wizz>`_:
 
 - code: https://github.com/jlvdb/yet_another_wizz_cli.git
 - PyPI: https://pypi.org/project/yet_another_wizz_cli/
 
 The documentation of this commandline tool is part of the official documentation
 of *yet_another_wizz* itself, including some usage examples:
 
 - docs: https://yet-another-wizz.readthedocs.io/
 
+Refer especially to the sections **User guide / Usage examples** and
+**User guide / Command line tools**.
+
 .. Note::
     When using this code in published work, please cite
     *van den Busch et al. (2020), A&A 642, A200*
     (`arXiv:2007.01846 <https://arxiv.org/abs/2007.01846>`_)
 
 
 Installation
@@ -79,14 +88,30 @@
 file can be printed to the terminal using::
 
     $ yaw_cli run --dump
 
 For more details refer to the to *User guide / Command line tools* section in
 the documentation of *yet_another_wizz*.
 
+Example
+~~~~~~~
+
+An example of the extended logging messages generated when running
+``yaw_cli run``:
+
+.. image:: https://raw.githubusercontent.com/jlvdb/asciinema_editor/main/examples/yaw_cli_small.gif
+    :width: 800
+    :alt: yet_another_wizz_cli example run
+
+The automatically generated check plots of the clustering redshift estimates:
+
+.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz_cli/main/data/nz_estimate.png
+    :width: 800
+    :alt: yet_another_wizz_cli example output
+
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
 
 https://github.com/jlvdb/yet_another_wizz_cli/issues
@@ -101,40 +126,7 @@
 Acknowledgements
 ----------------
 
 Jan Luca van den Busch acknowledges support from the European Research Council
 under grant numbers 770935. The authors also thank Hendrik Hildebrandt,
 Benjamin Joachimi, Angus H. Wright, and Chris Blake for vital feedback and
 support throughout the development of this software.
-
-
-Change log
-==========
-
-
-Version 1.2.2
--------------
-
-Added simple unit tests that run a randommised setup.
-
-.. rubric:: Bug fixes
-
-- Fixed the install dependency, which was pointing to ``yet_another_wizz``
-  instead of the section in the client setup.
-- Fixed formatting errors in the default configuration file: The task sections
-  were missing ":" if they were followed by a mapping of default arguments, the
-  filepath entry in the randoms sections was not indented correctly.
-
-
-Version 1.2.1
--------------
-
-.. rubric:: Bug fixes
-
-- Corrected the incorrectly named dependency for ``yet_another_wizz``.
-
-
-Version 1.2
------------
-
-Initial release as separate package. Previously the package was bundled with
-``yet_another_wizz`` itself.
```

### Comparing `yet_another_wizz_cli-1.2.2/README.rst` & `yet_another_wizz_cli-1.2.3/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,33 +1,42 @@
-yet_another_wizz_cli
-====================
+.. image:: https://github.com/jlvdb/yet_another_wizz/blob/main/docs/source/_static/logo-dark.png?raw=true
+    :width: 1000
+    :alt: yet_another_wizz
+
+|
 
 .. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
     :target: https://pypi.org/project/yet_another_wizz_cli/
 .. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz_cli/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz_cli
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
 
 
+Commandline tool
+================
+
 *yet_another_wizz_cli* implements a command line interface for the clustering
 redshift code `yet_another_wizz <https://github.com/jlvdb/yet_another_wizz>`_:
 
 - code: https://github.com/jlvdb/yet_another_wizz_cli.git
 - PyPI: https://pypi.org/project/yet_another_wizz_cli/
 
 The documentation of this commandline tool is part of the official documentation
 of *yet_another_wizz* itself, including some usage examples:
 
 - docs: https://yet-another-wizz.readthedocs.io/
 
+Refer especially to the sections **User guide / Usage examples** and
+**User guide / Command line tools**.
+
 .. Note::
     When using this code in published work, please cite
     *van den Busch et al. (2020), A&A 642, A200*
     (`arXiv:2007.01846 <https://arxiv.org/abs/2007.01846>`_)
 
 
 Installation
@@ -60,14 +69,30 @@
 file can be printed to the terminal using::
 
     $ yaw_cli run --dump
 
 For more details refer to the to *User guide / Command line tools* section in
 the documentation of *yet_another_wizz*.
 
+Example
+~~~~~~~
+
+An example of the extended logging messages generated when running
+``yaw_cli run``:
+
+.. image:: https://raw.githubusercontent.com/jlvdb/asciinema_editor/main/examples/yaw_cli_small.gif
+    :width: 800
+    :alt: yet_another_wizz_cli example run
+
+The automatically generated check plots of the clustering redshift estimates:
+
+.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz_cli/main/data/nz_estimate.png
+    :width: 800
+    :alt: yet_another_wizz_cli example output
+
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
 
 https://github.com/jlvdb/yet_another_wizz_cli/issues
@@ -82,40 +107,7 @@
 Acknowledgements
 ----------------
 
 Jan Luca van den Busch acknowledges support from the European Research Council
 under grant numbers 770935. The authors also thank Hendrik Hildebrandt,
 Benjamin Joachimi, Angus H. Wright, and Chris Blake for vital feedback and
 support throughout the development of this software.
-
-
-Change log
-==========
-
-
-Version 1.2.2
--------------
-
-Added simple unit tests that run a randommised setup.
-
-.. rubric:: Bug fixes
-
-- Fixed the install dependency, which was pointing to ``yet_another_wizz``
-  instead of the section in the client setup.
-- Fixed formatting errors in the default configuration file: The task sections
-  were missing ":" if they were followed by a mapping of default arguments, the
-  filepath entry in the randoms sections was not indented correctly.
-
-
-Version 1.2.1
--------------
-
-.. rubric:: Bug fixes
-
-- Corrected the incorrectly named dependency for ``yet_another_wizz``.
-
-
-Version 1.2
------------
-
-Initial release as separate package. Previously the package was bundled with
-``yet_another_wizz`` itself.
```

### Comparing `yet_another_wizz_cli-1.2.2/pyproject.toml` & `yet_another_wizz_cli-1.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/main.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,15 +240,15 @@
             return
         # create a logger and execute the task
         levels = {0: "warn", 1: "info", 2: "debug"}
         logger = init_logger(levels[args.verbose], plain=True)
         try:
             if args.task:
                 if args.task == "run":
-                    message = f"running setup from from:{Colors.rst} {args.setup}"
+                    message = f"running setup from file:{Colors.rst} {args.setup}"
                 else:
                     message = f"running task {args.task.upper()}"
                 print(f"{Colors.grn}YAW {Colors.sep} {message}{Colors.rst}")
                 command = self._subcommands[args.task]
                 command.run(args)
                 print_yaw_message("done")
             else:
```

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/subcommands.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/subcommands.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/commandline/utils.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/commandline/utils.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/__init__.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/data.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/data.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/default_setup.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/default_setup.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/directories.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/directories.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/logger.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/logger.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import logging
 import os
 import sys
+import warnings
 
 
 def term_supports_color() -> bool:
     plat = sys.platform
     supported = plat != "Pocket PC" and (plat != "win32" or "ANSICON" in os.environ)
     isatty = hasattr(sys.stdout, "isatty") and sys.stdout.isatty()
     return supported and isatty
@@ -61,16 +62,26 @@
         return formatter.format(record)
 
 
 def print_yaw_message(msg: str, color: str = Colors.blu) -> None:
     print(f"{color}YAW {Colors.sep} {msg}{Colors.rst}")
 
 
+class LoggerWrapper(object):
+    def __init__(self, name: str) -> None:
+        self.logger = logging.getLogger(name)
+
+    def write(self, message: str, *arg, **kwargs) -> None:
+        self.logger.warning(message)
+
+
 def get_logger() -> logging.Logger:
-    return logging.getLogger("yaw")
+    logger = LoggerWrapper("yaw")
+    warnings.showwarning = logger.write
+    return logger.logger
 
 
 def init_logger(level: str = "info", plain: bool = True) -> logging.Logger:
     level = getattr(logging, level.upper())
     handler = logging.StreamHandler(sys.stdout)
     if plain:
         handler.setFormatter(CustomFormatter())
```

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/merge.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/merge.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/plot.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/plot.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/processing.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/processing.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/project.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/project.py`

 * *Files identical despite different names*

### Comparing `yet_another_wizz_cli-1.2.2/src/yaw_cli/pipeline/tasks.py` & `yet_another_wizz_cli-1.2.3/src/yaw_cli/pipeline/tasks.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
 class MergedTask(Task):
     pass
 
 
 class RepeatableTask(Task):
     @abstractmethod
     def get_identifier(self) -> Any:
-        raise NotImplementedError
+        pass
 
     def __eq__(self, other: Task) -> bool:
         if super().__eq__(other) and hasattr(other, "get_identifier"):
             # additionally compare on the argument level
             return self.get_identifier() == other.get_identifier()
         return False
```

### Comparing `yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/PKG-INFO` & `yet_another_wizz_cli-1.2.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: yet-another-wizz-cli
-Version: 1.2.2
+Name: yet_another_wizz_cli
+Version: 1.2.3
 Summary: Command line client for yet_another_wizz.
 Home-page: https://github.com/jlvdb/yet_another_wizz_cli.git
 Author-email: Jan Luca van den Busch <jlvdb@astro.ruhr-uni-bochum.de>
 License: GPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Programming Language :: Python :: 3
@@ -13,40 +13,49 @@
 Description-Content-Type: text/x-rst
 Provides-Extra: plot
 Provides-Extra: style
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE
 
-yet_another_wizz_cli
-====================
+.. image:: https://github.com/jlvdb/yet_another_wizz/blob/main/docs/source/_static/logo-dark.png?raw=true
+    :width: 1000
+    :alt: yet_another_wizz
+
+|
 
 .. image:: https://img.shields.io/pypi/v/yet_another_wizz_cli?logo=pypi&logoColor=blue
     :target: https://pypi.org/project/yet_another_wizz_cli/
 .. image:: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml/badge.svg
     :target: https://github.com/jlvdb/yet_another_wizz_cli/actions/workflows/run-tests.yml
 .. image:: https://codecov.io/gh/jlvdb/yet_another_wizz_cli/branch/main/graph/badge.svg?token=PC41ME2AR8
     :target: https://codecov.io/gh/jlvdb/yet_another_wizz_cli
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 .. image:: https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336
     :target: https://pycqa.github.io/isort/
 
 
+Commandline tool
+================
+
 *yet_another_wizz_cli* implements a command line interface for the clustering
 redshift code `yet_another_wizz <https://github.com/jlvdb/yet_another_wizz>`_:
 
 - code: https://github.com/jlvdb/yet_another_wizz_cli.git
 - PyPI: https://pypi.org/project/yet_another_wizz_cli/
 
 The documentation of this commandline tool is part of the official documentation
 of *yet_another_wizz* itself, including some usage examples:
 
 - docs: https://yet-another-wizz.readthedocs.io/
 
+Refer especially to the sections **User guide / Usage examples** and
+**User guide / Command line tools**.
+
 .. Note::
     When using this code in published work, please cite
     *van den Busch et al. (2020), A&A 642, A200*
     (`arXiv:2007.01846 <https://arxiv.org/abs/2007.01846>`_)
 
 
 Installation
@@ -79,14 +88,30 @@
 file can be printed to the terminal using::
 
     $ yaw_cli run --dump
 
 For more details refer to the to *User guide / Command line tools* section in
 the documentation of *yet_another_wizz*.
 
+Example
+~~~~~~~
+
+An example of the extended logging messages generated when running
+``yaw_cli run``:
+
+.. image:: https://raw.githubusercontent.com/jlvdb/asciinema_editor/main/examples/yaw_cli_small.gif
+    :width: 800
+    :alt: yet_another_wizz_cli example run
+
+The automatically generated check plots of the clustering redshift estimates:
+
+.. image:: https://raw.githubusercontent.com/jlvdb/yet_another_wizz_cli/main/data/nz_estimate.png
+    :width: 800
+    :alt: yet_another_wizz_cli example output
+
 
 Reporting bugs and requesting features
 --------------------------------------
 
 For bug reports or requesting new features, please use the github issue page:
 
 https://github.com/jlvdb/yet_another_wizz_cli/issues
@@ -101,40 +126,7 @@
 Acknowledgements
 ----------------
 
 Jan Luca van den Busch acknowledges support from the European Research Council
 under grant numbers 770935. The authors also thank Hendrik Hildebrandt,
 Benjamin Joachimi, Angus H. Wright, and Chris Blake for vital feedback and
 support throughout the development of this software.
-
-
-Change log
-==========
-
-
-Version 1.2.2
--------------
-
-Added simple unit tests that run a randommised setup.
-
-.. rubric:: Bug fixes
-
-- Fixed the install dependency, which was pointing to ``yet_another_wizz``
-  instead of the section in the client setup.
-- Fixed formatting errors in the default configuration file: The task sections
-  were missing ":" if they were followed by a mapping of default arguments, the
-  filepath entry in the randoms sections was not indented correctly.
-
-
-Version 1.2.1
--------------
-
-.. rubric:: Bug fixes
-
-- Corrected the incorrectly named dependency for ``yet_another_wizz``.
-
-
-Version 1.2
------------
-
-Initial release as separate package. Previously the package was bundled with
-``yet_another_wizz`` itself.
```

### Comparing `yet_another_wizz_cli-1.2.2/src/yet_another_wizz_cli.egg-info/SOURCES.txt` & `yet_another_wizz_cli-1.2.3/src/yet_another_wizz_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

