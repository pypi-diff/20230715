# Comparing `tmp/html_plot-0.1.3.tar.gz` & `tmp/html_plot-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_plot-0.1.3.tar", max compression
+gzip compressed data, was "html_plot-0.1.4.tar", max compression
```

## Comparing `html_plot-0.1.3.tar` & `html_plot-0.1.4.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2541 2023-07-15 11:20:15.215124 html_plot-0.1.3/README.md
--rw-r--r--   0        0        0     2250 2023-07-13 04:34:08.072113 html_plot-0.1.3/html_plot/__init__.py
--rw-r--r--   0        0        0      559 2023-07-15 11:16:36.741294 html_plot-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     3363 1970-01-01 00:00:00.000000 html_plot-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     2541 2023-07-15 11:20:15.215124 html_plot-0.1.4/README.md
+-rw-r--r--   0        0        0     2250 2023-07-13 04:34:08.072113 html_plot-0.1.4/html_plot/__init__.py
+-rw-r--r--   0        0        0      609 2023-07-15 11:41:56.854634 html_plot-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     3470 1970-01-01 00:00:00.000000 html_plot-0.1.4/PKG-INFO
```

### Comparing `html_plot-0.1.3/README.md` & `html_plot-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `html_plot-0.1.3/html_plot/__init__.py` & `html_plot-0.1.4/html_plot/__init__.py`

 * *Files identical despite different names*

### Comparing `html_plot-0.1.3/pyproject.toml` & `html_plot-0.1.4/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 [tool.poetry]
 name = "html-plot"
-version = "0.1.3"
-description = "Render Matplotlib plots as HTML objects in Jupyter, so that they can be placed in HTML tables, downloaded on click, and more."
+version = "0.1.4"
+description = "Render Matplotlib plots as HTML objects in Jupyter, so that they can be placed in HTML tables, downloaded on click, and more"
 license = "OSL-3.0 OR AGPL-3.0-or-later"
 authors = ["kxmh42 <kxmh42@users.noreply.github.com>"]
 readme = "README.md"
+repository = "https://github.com/kxmh42/html-plot"
 packages = [{include = "html_plot"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 matplotlib = "^3.7.1"
 numpy = "^1.24.2"
 python-box = "^7.0.1"
```

### Comparing `html_plot-0.1.3/PKG-INFO` & `html_plot-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: html-plot
-Version: 0.1.3
-Summary: Render Matplotlib plots as HTML objects in Jupyter, so that they can be placed in HTML tables, downloaded on click, and more.
+Version: 0.1.4
+Summary: Render Matplotlib plots as HTML objects in Jupyter, so that they can be placed in HTML tables, downloaded on click, and more
+Home-page: https://github.com/kxmh42/html-plot
 License: OSL-3.0 OR AGPL-3.0-or-later
 Author: kxmh42
 Author-email: kxmh42@users.noreply.github.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: ipython (>=8.12.0,<9.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: python-box (>=7.0.1,<8.0.0)
+Project-URL: Repository, https://github.com/kxmh42/html-plot
 Description-Content-Type: text/markdown
 
 This package can be used to render Matplotlib plots as HTML objects in
 Jupyter, so that they can be placed in HTML tables, downloaded on click,
 and more.
 
 # Installation
```

