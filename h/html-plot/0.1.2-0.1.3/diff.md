# Comparing `tmp/html_plot-0.1.2.tar.gz` & `tmp/html_plot-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_plot-0.1.2.tar", max compression
+gzip compressed data, was "html_plot-0.1.3.tar", max compression
```

## Comparing `html_plot-0.1.2.tar` & `html_plot-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      944 2023-04-04 21:14:46.423138 html_plot-0.1.2/README.md
--rw-r--r--   0        0        0     2250 2023-04-04 21:04:14.713853 html_plot-0.1.2/html_plot/__init__.py
--rw-r--r--   0        0        0      469 2023-04-04 21:15:17.931378 html_plot-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 html_plot-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     2541 2023-07-15 11:20:15.215124 html_plot-0.1.3/README.md
+-rw-r--r--   0        0        0     2250 2023-07-13 04:34:08.072113 html_plot-0.1.3/html_plot/__init__.py
+-rw-r--r--   0        0        0      559 2023-07-15 11:16:36.741294 html_plot-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     3363 1970-01-01 00:00:00.000000 html_plot-0.1.3/PKG-INFO
```

### Comparing `html_plot-0.1.2/html_plot/__init__.py` & `html_plot-0.1.3/html_plot/__init__.py`

 * *Files identical despite different names*

