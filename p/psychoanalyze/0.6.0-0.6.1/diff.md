# Comparing `tmp/psychoanalyze-0.6.0.tar.gz` & `tmp/psychoanalyze-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.6.0.tar", max compression
+gzip compressed data, was "psychoanalyze-0.6.1.tar", max compression
```

## Comparing `psychoanalyze-0.6.0.tar` & `psychoanalyze-0.6.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-07-15 09:39:04.526433 psychoanalyze-0.6.0/LICENSE
--rw-r--r--   0        0        0     1105 2023-07-15 09:39:04.526433 psychoanalyze-0.6.0/README.md
--rw-r--r--   0        0        0     1357 2023-07-15 09:41:16.677281 psychoanalyze-0.6.0/psychoanalyze/__init__.py
--rw-r--r--   0        0        0      756 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/analysis/__init__.py
--rw-r--r--   0        0        0     1288 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/analysis/bayes.py
--rw-r--r--   0        0        0     1120 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/analysis/ecdf.py
--rw-r--r--   0        0        0     2302 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/analysis/strength_duration.py
--rw-r--r--   0        0        0     2373 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/analysis/weber.py
--rw-r--r--   0        0        0     1153 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/__init__.py
--rw-r--r--   0        0        0     8080 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/blocks.py
--rw-r--r--   0        0        0     7763 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/points.py
--rw-r--r--   0        0        0     2868 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/sessions.py
--rw-r--r--   0        0        0      841 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/stimulus.py
--rw-r--r--   0        0        0     1678 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/subjects.py
--rw-r--r--   0        0        0     5206 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/trials.py
--rw-r--r--   0        0        0     2938 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/data/types.py
--rw-r--r--   0        0        0     1589 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/plot.py
--rw-r--r--   0        0        0     1518 2023-07-15 09:39:04.598435 psychoanalyze-0.6.0/psychoanalyze/sigmoids.py
--rw-r--r--   0        0        0     1881 2023-07-15 09:41:16.677281 psychoanalyze-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 psychoanalyze-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-07-15 10:19:00.005840 psychoanalyze-0.6.1/LICENSE
+-rw-r--r--   0        0        0     1105 2023-07-15 10:19:00.005840 psychoanalyze-0.6.1/README.md
+-rw-r--r--   0        0        0     1357 2023-07-15 10:21:13.073870 psychoanalyze-0.6.1/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0      756 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/analysis/__init__.py
+-rw-r--r--   0        0        0     1288 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/analysis/bayes.py
+-rw-r--r--   0        0        0     1120 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/analysis/ecdf.py
+-rw-r--r--   0        0        0     2302 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/analysis/strength_duration.py
+-rw-r--r--   0        0        0     2373 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/analysis/weber.py
+-rw-r--r--   0        0        0     1153 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/__init__.py
+-rw-r--r--   0        0        0     8080 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/blocks.py
+-rw-r--r--   0        0        0     7763 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/points.py
+-rw-r--r--   0        0        0     2868 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/sessions.py
+-rw-r--r--   0        0        0      841 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/stimulus.py
+-rw-r--r--   0        0        0     1678 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/subjects.py
+-rw-r--r--   0        0        0     5206 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/trials.py
+-rw-r--r--   0        0        0     2938 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/data/types.py
+-rw-r--r--   0        0        0     1589 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     1518 2023-07-15 10:19:00.081840 psychoanalyze-0.6.1/psychoanalyze/sigmoids.py
+-rw-r--r--   0        0        0     1881 2023-07-15 10:21:13.073870 psychoanalyze-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     2695 1970-01-01 00:00:00.000000 psychoanalyze-0.6.1/PKG-INFO
```

### Comparing `psychoanalyze-0.6.0/LICENSE` & `psychoanalyze-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/README.md` & `psychoanalyze-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/__init__.py` & `psychoanalyze-0.6.1/psychoanalyze/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/analysis/__init__.py` & `psychoanalyze-0.6.1/psychoanalyze/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/analysis/bayes.py` & `psychoanalyze-0.6.1/psychoanalyze/analysis/bayes.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/analysis/ecdf.py` & `psychoanalyze-0.6.1/psychoanalyze/analysis/ecdf.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/analysis/strength_duration.py` & `psychoanalyze-0.6.1/psychoanalyze/analysis/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/analysis/weber.py` & `psychoanalyze-0.6.1/psychoanalyze/analysis/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/data/__init__.py` & `psychoanalyze-0.6.1/psychoanalyze/data/__init__.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/data/blocks.py` & `psychoanalyze-0.6.1/psychoanalyze/data/blocks.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/data/points.py` & `psychoanalyze-0.6.1/psychoanalyze/data/points.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/data/sessions.py` & `psychoanalyze-0.6.1/psychoanalyze/data/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/data/stimulus.py` & `psychoanalyze-0.6.1/psychoanalyze/data/stimulus.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/data/subjects.py` & `psychoanalyze-0.6.1/psychoanalyze/data/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/data/trials.py` & `psychoanalyze-0.6.1/psychoanalyze/data/trials.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/data/types.py` & `psychoanalyze-0.6.1/psychoanalyze/data/types.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/plot.py` & `psychoanalyze-0.6.1/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/psychoanalyze/sigmoids.py` & `psychoanalyze-0.6.1/psychoanalyze/sigmoids.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.6.0/pyproject.toml` & `psychoanalyze-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.6.0"
+version = "0.6.1"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.4"
```

### Comparing `psychoanalyze-0.6.0/PKG-INFO` & `psychoanalyze-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.6.0
+Version: 0.6.1
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.4
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

