# Comparing `tmp/pytest-tap-3.3.tar.gz` & `tmp/pytest-tap-3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/matt/projects/pytest-tap/dist/tmp8ol0wpwl/pytest-tap-3.3.tar", last modified: Wed Oct 27 04:05:54 2021, max compression
+gzip compressed data, was "pytest-tap-3.4.tar", last modified: Sat Jul 15 20:16:53 2023, max compression
```

## Comparing `pytest-tap-3.3.tar` & `pytest-tap-3.4.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2021-10-27 04:05:54.477634 pytest-tap-3.3/
--rw-r--r--   0 matt       (501) staff       (20)      231 2020-03-24 23:34:41.000000 pytest-tap-3.3/AUTHORS
--rw-r--r--   0 matt       (501) staff       (20)     1342 2021-10-26 21:45:37.000000 pytest-tap-3.3/LICENSE
--rw-r--r--   0 matt       (501) staff       (20)       77 2021-10-27 03:50:08.000000 pytest-tap-3.3/MANIFEST.in
--rw-r--r--   0 matt       (501) staff       (20)     3696 2021-10-27 04:05:54.477781 pytest-tap-3.3/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)     1868 2021-10-27 03:50:54.000000 pytest-tap-3.3/README.rst
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2021-10-27 04:05:54.473971 pytest-tap-3.3/docs/
--rw-r--r--   0 matt       (501) staff       (20)     2424 2021-10-27 03:57:28.000000 pytest-tap-3.3/docs/releases.rst
--rw-r--r--   0 matt       (501) staff       (20)      309 2021-10-27 04:05:54.478681 pytest-tap-3.3/setup.cfg
--rw-r--r--   0 matt       (501) staff       (20)     1920 2021-10-27 03:59:50.000000 pytest-tap-3.3/setup.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2021-10-27 04:05:54.471706 pytest-tap-3.3/src/
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2021-10-27 04:05:54.474607 pytest-tap-3.3/src/pytest_tap/
--rw-r--r--   0 matt       (501) staff       (20)       20 2021-10-27 03:59:50.000000 pytest-tap-3.3/src/pytest_tap/__init__.py
--rw-r--r--   0 matt       (501) staff       (20)     5284 2021-10-27 03:47:19.000000 pytest-tap-3.3/src/pytest_tap/plugin.py
-drwxr-xr-x   0 matt       (501) staff       (20)        0 2021-10-27 04:05:54.477371 pytest-tap-3.3/src/pytest_tap.egg-info/
--rw-r--r--   0 matt       (501) staff       (20)     3696 2021-10-27 04:05:54.000000 pytest-tap-3.3/src/pytest_tap.egg-info/PKG-INFO
--rw-r--r--   0 matt       (501) staff       (20)      394 2021-10-27 04:05:54.000000 pytest-tap-3.3/src/pytest_tap.egg-info/SOURCES.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2021-10-27 04:05:54.000000 pytest-tap-3.3/src/pytest_tap.egg-info/dependency_links.txt
--rw-r--r--   0 matt       (501) staff       (20)       36 2021-10-27 04:05:54.000000 pytest-tap-3.3/src/pytest_tap.egg-info/entry_points.txt
--rw-r--r--   0 matt       (501) staff       (20)        1 2019-10-20 00:39:43.000000 pytest-tap-3.3/src/pytest_tap.egg-info/not-zip-safe
--rw-r--r--   0 matt       (501) staff       (20)       29 2021-10-27 04:05:54.000000 pytest-tap-3.3/src/pytest_tap.egg-info/requires.txt
--rw-r--r--   0 matt       (501) staff       (20)       11 2021-10-27 04:05:54.000000 pytest-tap-3.3/src/pytest_tap.egg-info/top_level.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-15 20:16:53.827582 pytest-tap-3.4/
+-rw-r--r--   0 matt       (501) staff       (20)      253 2023-07-15 20:10:50.000000 pytest-tap-3.4/AUTHORS
+-rw-r--r--   0 matt       (501) staff       (20)     1342 2021-10-26 21:45:37.000000 pytest-tap-3.4/LICENSE
+-rw-r--r--   0 matt       (501) staff       (20)       77 2022-12-13 01:54:38.000000 pytest-tap-3.4/MANIFEST.in
+-rw-r--r--   0 matt       (501) staff       (20)     4128 2023-07-15 20:16:53.827724 pytest-tap-3.4/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)     1846 2023-07-15 17:34:23.000000 pytest-tap-3.4/README.rst
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-15 20:16:53.815460 pytest-tap-3.4/docs/
+-rw-r--r--   0 matt       (501) staff       (20)     2776 2023-07-15 20:10:55.000000 pytest-tap-3.4/docs/releases.rst
+-rw-r--r--   0 matt       (501) staff       (20)      310 2023-07-15 20:16:53.828348 pytest-tap-3.4/setup.cfg
+-rw-r--r--   0 matt       (501) staff       (20)     1999 2023-07-15 20:11:15.000000 pytest-tap-3.4/setup.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-15 20:16:53.812826 pytest-tap-3.4/src/
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-15 20:16:53.816182 pytest-tap-3.4/src/pytest_tap/
+-rw-r--r--   0 matt       (501) staff       (20)       20 2023-07-15 20:11:15.000000 pytest-tap-3.4/src/pytest_tap/__init__.py
+-rw-r--r--   0 matt       (501) staff       (20)     6311 2023-07-15 20:10:50.000000 pytest-tap-3.4/src/pytest_tap/plugin.py
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-15 20:16:53.826110 pytest-tap-3.4/src/pytest_tap.egg-info/
+-rw-r--r--   0 matt       (501) staff       (20)     4128 2023-07-15 20:16:53.000000 pytest-tap-3.4/src/pytest_tap.egg-info/PKG-INFO
+-rw-r--r--   0 matt       (501) staff       (20)      454 2023-07-15 20:16:53.000000 pytest-tap-3.4/src/pytest_tap.egg-info/SOURCES.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2023-07-15 20:16:53.000000 pytest-tap-3.4/src/pytest_tap.egg-info/dependency_links.txt
+-rw-r--r--   0 matt       (501) staff       (20)       35 2023-07-15 20:16:53.000000 pytest-tap-3.4/src/pytest_tap.egg-info/entry_points.txt
+-rw-r--r--   0 matt       (501) staff       (20)        1 2019-10-20 00:39:43.000000 pytest-tap-3.4/src/pytest_tap.egg-info/not-zip-safe
+-rw-r--r--   0 matt       (501) staff       (20)       29 2023-07-15 20:16:53.000000 pytest-tap-3.4/src/pytest_tap.egg-info/requires.txt
+-rw-r--r--   0 matt       (501) staff       (20)       11 2023-07-15 20:16:53.000000 pytest-tap-3.4/src/pytest_tap.egg-info/top_level.txt
+drwxr-xr-x   0 matt       (501) staff       (20)        0 2023-07-15 20:16:53.827314 pytest-tap-3.4/tests/
+-rw-r--r--   0 matt       (501) staff       (20)      672 2023-07-15 17:34:23.000000 pytest-tap-3.4/tests/test_help.py
+-rw-r--r--   0 matt       (501) staff       (20)     6687 2023-07-15 17:34:23.000000 pytest-tap-3.4/tests/test_plugin.py
+-rw-r--r--   0 matt       (501) staff       (20)      824 2023-07-15 20:10:50.000000 pytest-tap-3.4/tests/test_xdist.py
```

### Comparing `pytest-tap-3.3/LICENSE` & `pytest-tap-3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-tap-3.3/PKG-INFO` & `pytest-tap-3.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 Metadata-Version: 2.1
 Name: pytest-tap
-Version: 3.3
+Version: 3.4
 Summary: Test Anything Protocol (TAP) reporting plugin for pytest
 Home-page: https://github.com/python-tap/pytest-tap
 Author: Matt Layman
 Author-email: matthewlayman@gmail.com
 License: BSD
 Keywords: TAP,unittest,pytest
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE
 
 
 pytest-tap is a reporting plugin for pytest that outputs
 `Test Anything Protocol (TAP) <http://testanything.org/>`_ data.
 TAP is a line based test protocol for recording test data in a standard way.
 
-Follow development on `GitHub <https://github.com/python-tap/pytest-tap>`_.
-Developer documentation is on
+Use ``pytest --tap`` after installing to get started.
+
+Follow `GitHub <https://github.com/python-tap/pytest-tap>`_
+for more information or to follow this plugin's development.
+Additional developer documentation about Python and TAP is on
 `Read the Docs <https://tappy.readthedocs.io/>`_.
 
 
 Releases
 ========
 
+Version 3.4, July 15, 2023
+--------------------------
+
+* Deprecate ``--tap-stream`` in favor of ``--tap`` for streaming mode.
+* When using xdist, report the plan at the beginning of execution.
+* Add support for Python 3.11.
+* Drop support for Python 3.7 (it is end-of-life).
+* Drop support for Python 3.6 (it is end-of-life).
+* Drop support for PyPy.
+
 Version 3.3, October 27, 2021
 -----------------------------
 
 * Add support for Python 3.10.
 * Fix bug with help printing when streaming mode is enabled (#59).
 * Drop support for Python 3.5 (it is end-of-life).
 * Remove unmaintained (and likely inaccurate) locale info.
@@ -109,9 +121,7 @@
 * Drop support for Python 2.6
 
 Version 1.9, Released June 11, 2016
 -----------------------------------
 
 * Initial release as stand-alone plugin.
   The version number aligns with tappy.
-
-
```

### Comparing `pytest-tap-3.3/README.rst` & `pytest-tap-3.4/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 pytest-tap
 ==========
 
-|version| |license| |travis| |travismac| |appveyor| |coverage|
+|version| |license| |coverage|
 
 .. |version| image:: https://img.shields.io/pypi/v/pytest-tap.svg
     :target: https://pypi.python.org/pypi/pytest-tap
     :alt: PyPI version
 .. |license| image:: https://img.shields.io/pypi/l/pytest-tap.svg
     :target: https://raw.githubusercontent.com/python-tap/pytest-tap/master/LICENSE
     :alt: BSD license
@@ -30,28 +30,28 @@
 Usage
 -----
 
 This is an example usage from the plugin's test suite.
 
 .. code-block:: console
 
-   $ pytest --tap-stream
+   $ pytest --tap
    1..12
-   ok 1 - TestPlugin.test_generates_reports_for_combined
-   ok 2 - TestPlugin.test_generates_reports_for_files
-   ok 3 - TestPlugin.test_generates_reports_for_stream
-   ok 4 - TestPlugin.test_includes_options
-   ok 5 - TestPlugin.test_skips_reporting_with_no_output_option
-   ok 6 - TestPlugin.test_track_when_call_report
-   ok 7 - TestPlugin.test_tracker_combined_set
-   ok 8 - TestPlugin.test_tracker_outdir_set
-   ok 9 - TestPlugin.test_tracker_stream_set
-   ok 10 - TestPlugin.test_tracks_not_ok
-   ok 11 - TestPlugin.test_tracks_ok
-   ok 12 - TestPlugin.test_tracks_skip
+   ok 1 tests/test_help.py::test_includes_options
+   ok 2 tests/test_help.py::test_handle_help_with_stream
+   ok 3 tests/test_plugin.py::test_stream
+   ok 4 tests/test_plugin.py::test_stream_simple_flag
+   ok 5 tests/test_plugin.py::test_combined
+   ok 6 tests/test_plugin.py::test_files
+   ok 7 tests/test_plugin.py::test_outdir
+   ok 8 tests/test_plugin.py::test_xfail_no_reason
+   ok 9 tests/test_plugin.py::test_xfail_nonstrict
+   ok 10 tests/test_plugin.py::test_xfail_strict
+   ok 11 tests/test_plugin.py::test_unittest_expected_failure
+   ok 12 tests/test_plugin.py::test_setup_failure
 
 Contributing
 ------------
 
 The project welcomes contributions of all kinds.
 Check out the `contributing guidelines <https://github.com/python-tap/pytest-tap/blob/master/.github/contributing.md>`_
 for tips on how to get started.
```

### Comparing `pytest-tap-3.3/docs/releases.rst` & `pytest-tap-3.4/docs/releases.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Releases
 ========
 
+Version 3.4, July 15, 2023
+--------------------------
+
+* Deprecate ``--tap-stream`` in favor of ``--tap`` for streaming mode.
+* When using xdist, report the plan at the beginning of execution.
+* Add support for Python 3.11.
+* Drop support for Python 3.7 (it is end-of-life).
+* Drop support for Python 3.6 (it is end-of-life).
+* Drop support for PyPy.
+
 Version 3.3, October 27, 2021
 -----------------------------
 
 * Add support for Python 3.10.
 * Fix bug with help printing when streaming mode is enabled (#59).
 * Drop support for Python 3.5 (it is end-of-life).
 * Remove unmaintained (and likely inaccurate) locale info.
```

### Comparing `pytest-tap-3.3/setup.py` & `pytest-tap-3.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """
 pytest-tap is a reporting plugin for pytest that outputs
 `Test Anything Protocol (TAP) <http://testanything.org/>`_ data.
 TAP is a line based test protocol for recording test data in a standard way.
 
-Follow development on `GitHub <https://github.com/python-tap/pytest-tap>`_.
-Developer documentation is on
+Use ``pytest --tap`` after installing to get started.
+
+Follow `GitHub <https://github.com/python-tap/pytest-tap>`_
+for more information or to follow this plugin's development.
+Additional developer documentation about Python and TAP is on
 `Read the Docs <https://tappy.readthedocs.io/>`_.
 """
 
 from setuptools import find_packages, setup
 
 
 if __name__ == "__main__":
     with open("docs/releases.rst", "r") as f:
         releases = f.read()
 
     long_description = __doc__ + "\n\n" + releases
 
     setup(
         name="pytest-tap",
-        version="3.3",
+        version="3.4",
         url="https://github.com/python-tap/pytest-tap",
         license="BSD",
         author="Matt Layman",
         author_email="matthewlayman@gmail.com",
         description="Test Anything Protocol (TAP) reporting plugin for pytest",
         long_description=long_description,
         packages=find_packages(where="src"),
@@ -35,15 +38,14 @@
         install_requires=["pytest>=3.0", "tap.py>=3.0,<4.0"],
         classifiers=[
             "Development Status :: 5 - Production/Stable",
             "Framework :: Pytest",
             "Intended Audience :: Developers",
             "License :: OSI Approved :: BSD License",
             "Operating System :: OS Independent",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
             "Programming Language :: Python :: Implementation :: PyPy",
             "Topic :: Software Development :: Testing",
         ],
```

### Comparing `pytest-tap-3.3/src/pytest_tap/plugin.py` & `pytest-tap-3.4/src/pytest_tap/plugin.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,132 @@
+import argparse
 import sys
 
 import pytest
 from tap.formatter import format_as_diagnostics
 from tap.tracker import Tracker
 
-# Because of how pytest hooks work, there is not much choice
-# except to use module level state. Ugh.
-tracker = Tracker()
-ENABLED = False
+
+class TAPPlugin:
+    def __init__(self, config: pytest.Config) -> None:
+        self._tracker = Tracker(
+            outdir=config.option.tap_outdir,
+            combined=config.option.tap_combined,
+            streaming=config.option.tap_stream,
+            stream=sys.stdout,
+        )
+
+        if self._tracker.streaming:
+            reporter = config.pluginmanager.getplugin("terminalreporter")
+            if reporter:
+                config.pluginmanager.unregister(reporter)
+            # A common pytest pattern is to use test functions without classes.
+            # The header looks really dumb for that pattern because it puts
+            # out a lot of line noise since every function gets its own header.
+            # Disable it automatically for streaming.
+            self._tracker.header = False
+
+    @pytest.hookimpl()
+    def pytest_runtestloop(self, session):
+        """Output the plan line first."""
+        option = session.config.option
+        if option.tap_stream or option.tap_combined:
+            self._tracker.set_plan(session.testscollected)
+
+    @pytest.hookimpl(optionalhook=True)
+    def pytest_xdist_node_collection_finished(self, node, ids):
+        """Output the plan line first when using xdist."""
+        if self._tracker.streaming or self._tracker.combined:
+            self._tracker.set_plan(len(ids))
+
+    @pytest.hookimpl()
+    def pytest_runtest_logreport(self, report: pytest.TestReport):
+        """Add a test result to the tracker."""
+        is_trackable_result = (
+            (report.when == "setup" and report.outcome == "skipped")
+            or (report.when == "setup" and report.outcome == "failed")
+            or report.when == "call"
+        )
+        if not is_trackable_result:
+            return
+
+        description = str(report.location[0]) + "::" + str(report.location[2])
+        testcase = report.location[0]
+
+        # Handle xfails first because they report in unusual ways.
+        # Non-strict xfails will include `wasxfail` while strict xfails won't.
+        if hasattr(report, "wasxfail"):
+            reason = ""
+            # pytest adds an ugly "reason: " for expectedFailure
+            # even though the standard library doesn't accept a reason
+            # for that decorator.
+            # Ignore the "reason: " from pytest.
+            if report.wasxfail and report.wasxfail != "reason: ":
+                reason = ": {}".format(report.wasxfail)
+
+            if report.skipped:
+                directive = "TODO expected failure{}".format(reason)
+                self._tracker.add_not_ok(testcase, description, directive=directive)
+            elif report.passed:
+                directive = "TODO unexpected success{}".format(reason)
+                self._tracker.add_ok(testcase, description, directive=directive)
+        elif report.passed:
+            self._tracker.add_ok(testcase, description)
+        elif report.failed:
+            diagnostics = _make_as_diagnostics(report)
+
+            # pytest treats an unexpected success from unitest.expectedFailure
+            # as a failure.
+            # To match up with TAPTestResult and the TAP spec, treat the pass
+            # as an ok with a todo directive instead.
+            if "Unexpected success" in str(report.longrepr):
+                self._tracker.add_ok(
+                    testcase, description, directive="TODO unexpected success"
+                )
+                return
+
+            # A strict xfail that passes (i.e., XPASS) should be marked as a failure.
+            # The only indicator that strict xfail occurred
+            # for XPASS is to check longrepr.
+            if (
+                isinstance(report.longrepr, str)
+                and "[XPASS(strict)]" in report.longrepr
+            ):
+                self._tracker.add_not_ok(
+                    testcase,
+                    description,
+                    directive="unexpected success: {}".format(report.longrepr),
+                )
+                return
+
+            self._tracker.add_not_ok(testcase, description, diagnostics=diagnostics)
+        elif report.skipped:
+            reason = report.longrepr[2].split(":", 1)[1].strip()  # type: ignore
+            self._tracker.add_skip(testcase, description, reason)
+
+    @pytest.hookimpl()
+    def pytest_unconfigure(self, config: pytest.Config):
+        """Dump the results."""
+        self._tracker.generate_tap_reports()
 
 
 def pytest_addoption(parser):
     """Include all the command line options."""
     group = parser.getgroup("terminal reporting", "reporting", after="general")
     group.addoption(
-        "--tap-stream",
+        "--tap",
         default=False,
+        dest="tap_stream",
         action="store_true",
         help="Stream TAP output instead of the default test runner output.",
     )
+    # Deprecated, but keeping for backwards compatibility.
+    group.addoption(
+        "--tap-stream", default=False, action="store_true", help=argparse.SUPPRESS
+    )
     group.addoption(
         "--tap-files",
         default=False,
         action="store_true",
         help="Store all TAP test results into individual files per test case.",
     )
     group.addoption(
@@ -37,114 +141,27 @@
         help=(
             "An optional output directory to write TAP files to. "
             "If the directory does not exist, it will be created."
         ),
     )
 
 
-@pytest.mark.trylast
-def pytest_configure(config):
-    """Set all the options before the test run."""
+@pytest.hookimpl(trylast=True)
+def pytest_configure(config: pytest.Config) -> None:
+    """Enable the plugin if the TAP flags are used."""
     # The help printing uses the terminalreporter,
     # which is unregistered by the streaming mode.
     if config.option.help:
         return
 
-    global ENABLED
-    ENABLED = (
+    if (
         config.option.tap_stream
         or config.option.tap_combined
         or config.option.tap_files
-    )
-
-    tracker.outdir = config.option.tap_outdir
-    tracker.combined = config.option.tap_combined
-    if config.option.tap_stream:
-        reporter = config.pluginmanager.getplugin("terminalreporter")
-        if reporter:
-            config.pluginmanager.unregister(reporter)
-        tracker.streaming = True
-        tracker.stream = sys.stdout
-        # A common pytest pattern is to use test functions without classes.
-        # The header looks really dumb for that pattern because it puts
-        # out a lot of line noise since every function gets its own header.
-        # Disable it automatically for streaming.
-        tracker.header = False
-
-
-def pytest_runtestloop(session):
-    """Output the plan line first."""
-    option = session.config.option
-    if ENABLED and (option.tap_stream or option.tap_combined):
-        tracker.set_plan(session.testscollected)
-
-
-def pytest_runtest_logreport(report):
-    """Add a test result to the tracker."""
-    if not ENABLED:
-        return
-
-    is_trackable_result = (
-        (report.when == "setup" and report.outcome == "skipped")
-        or (report.when == "setup" and report.outcome == "failed")
-        or report.when == "call"
-    )
-    if not is_trackable_result:
-        return
-
-    description = str(report.location[0]) + "::" + str(report.location[2])
-    testcase = report.location[0]
-
-    # Handle xfails first because they report in unusual ways.
-    # Non-strict xfails will include `wasxfail` while strict xfails won't.
-    if hasattr(report, "wasxfail"):
-        reason = ""
-        # pytest adds an ugly "reason: " for expectedFailure
-        # even though the standard library doesn't accept a reason for that decorator.
-        # Ignore the "reason: " from pytest.
-        if report.wasxfail and report.wasxfail != "reason: ":
-            reason = ": {}".format(report.wasxfail)
-
-        if report.skipped:
-            directive = "TODO expected failure{}".format(reason)
-            tracker.add_not_ok(testcase, description, directive=directive)
-        elif report.passed:
-            directive = "TODO unexpected success{}".format(reason)
-            tracker.add_ok(testcase, description, directive=directive)
-    elif report.passed:
-        tracker.add_ok(testcase, description)
-    elif report.failed:
-        diagnostics = _make_as_diagnostics(report)
-
-        # pytest treats an unexpected success from unitest.expectedFailure as a failure.
-        # To match up with TAPTestResult and the TAP spec, treat the pass
-        # as an ok with a todo directive instead.
-        if isinstance(report.longrepr, str) and "Unexpected success" in report.longrepr:
-            tracker.add_ok(testcase, description, directive="TODO unexpected success")
-            return
-
-        # A strict xfail that passes (i.e., XPASS) should be marked as a failure.
-        # The only indicator that strict xfail occurred for XPASS is to check longrepr.
-        if isinstance(report.longrepr, str) and "[XPASS(strict)]" in report.longrepr:
-            tracker.add_not_ok(
-                testcase,
-                description,
-                directive="unexpected success: {}".format(report.longrepr),
-            )
-            return
-
-        tracker.add_not_ok(testcase, description, diagnostics=diagnostics)
-    elif report.skipped:
-        reason = report.longrepr[2].split(":", 1)[1].strip()
-        tracker.add_skip(testcase, description, reason)
+    ):
+        config.pluginmanager.register(TAPPlugin(config), "tapplugin")
 
 
 def _make_as_diagnostics(report):
     """Format a report as TAP diagnostic output."""
     lines = report.longreprtext.splitlines(keepends=True)
     return format_as_diagnostics(lines)
-
-
-def pytest_unconfigure(config):
-    """Dump the results."""
-    if ENABLED:
-        tracker.generate_tap_reports()
```

### Comparing `pytest-tap-3.3/src/pytest_tap.egg-info/PKG-INFO` & `pytest-tap-3.4/src/pytest_tap.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 Metadata-Version: 2.1
 Name: pytest-tap
-Version: 3.3
+Version: 3.4
 Summary: Test Anything Protocol (TAP) reporting plugin for pytest
 Home-page: https://github.com/python-tap/pytest-tap
 Author: Matt Layman
 Author-email: matthewlayman@gmail.com
 License: BSD
 Keywords: TAP,unittest,pytest
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Testing
 License-File: LICENSE
 
 
 pytest-tap is a reporting plugin for pytest that outputs
 `Test Anything Protocol (TAP) <http://testanything.org/>`_ data.
 TAP is a line based test protocol for recording test data in a standard way.
 
-Follow development on `GitHub <https://github.com/python-tap/pytest-tap>`_.
-Developer documentation is on
+Use ``pytest --tap`` after installing to get started.
+
+Follow `GitHub <https://github.com/python-tap/pytest-tap>`_
+for more information or to follow this plugin's development.
+Additional developer documentation about Python and TAP is on
 `Read the Docs <https://tappy.readthedocs.io/>`_.
 
 
 Releases
 ========
 
+Version 3.4, July 15, 2023
+--------------------------
+
+* Deprecate ``--tap-stream`` in favor of ``--tap`` for streaming mode.
+* When using xdist, report the plan at the beginning of execution.
+* Add support for Python 3.11.
+* Drop support for Python 3.7 (it is end-of-life).
+* Drop support for Python 3.6 (it is end-of-life).
+* Drop support for PyPy.
+
 Version 3.3, October 27, 2021
 -----------------------------
 
 * Add support for Python 3.10.
 * Fix bug with help printing when streaming mode is enabled (#59).
 * Drop support for Python 3.5 (it is end-of-life).
 * Remove unmaintained (and likely inaccurate) locale info.
@@ -109,9 +121,7 @@
 * Drop support for Python 2.6
 
 Version 1.9, Released June 11, 2016
 -----------------------------------
 
 * Initial release as stand-alone plugin.
   The version number aligns with tappy.
-
-
```

