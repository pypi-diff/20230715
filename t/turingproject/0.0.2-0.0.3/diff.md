# Comparing `tmp/turingproject-0.0.2.tar.gz` & `tmp/turingproject-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turingproject-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "turingproject-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `turingproject-0.0.2.tar` & `turingproject-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1097 2023-07-10 17:06:18.276845 turingproject-0.0.2/LICENSE
--rw-r--r--   0        0        0     1220 2023-07-10 07:50:09.061716 turingproject-0.0.2/README.md
--rw-r--r--   0        0        0      402 2023-07-13 21:01:49.770440 turingproject-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-10 17:08:53.340385 turingproject-0.0.2/src/turingproject/__init__.py
--rw-r--r--   0        0        0     1803 2023-07-13 20:48:06.343368 turingproject-0.0.2/src/turingproject/calculator.py
--rw-r--r--   0        0        0     1428 1970-01-01 00:00:00.000000 turingproject-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-07-10 17:06:18.276845 turingproject-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1220 2023-07-10 07:50:09.061716 turingproject-0.0.3/README.md
+-rw-r--r--   0        0        0      402 2023-07-15 09:06:25.246992 turingproject-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-10 17:08:53.340385 turingproject-0.0.3/src/turingproject/__init__.py
+-rw-r--r--   0        0        0     1803 2023-07-13 20:48:06.343368 turingproject-0.0.3/src/turingproject/calculator.py
+-rw-r--r--   0        0        0     1428 1970-01-01 00:00:00.000000 turingproject-0.0.3/PKG-INFO
```

### Comparing `turingproject-0.0.2/LICENSE` & `turingproject-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `turingproject-0.0.2/README.md` & `turingproject-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `turingproject-0.0.2/src/turingproject/calculator.py` & `turingproject-0.0.3/src/turingproject/calculator.py`

 * *Files identical despite different names*

### Comparing `turingproject-0.0.2/PKG-INFO` & `turingproject-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turingproject
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Author-email: Vitalijus Kiubis <vitalijus.kiubis@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 
 # Calculator Package
```

