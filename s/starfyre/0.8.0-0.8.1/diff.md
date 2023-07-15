# Comparing `tmp/starfyre-0.8.0.tar.gz` & `tmp/starfyre-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starfyre-0.8.0.tar", max compression
+gzip compressed data, was "starfyre-0.8.1.tar", max compression
```

## Comparing `starfyre-0.8.0.tar` & `starfyre-0.8.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4751 2023-07-06 20:03:56.649057 starfyre-0.8.0/README.md
--rw-r--r--   0        0        0      454 2023-07-06 20:03:56.649057 starfyre-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      949 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/__init__.py
--rw-r--r--   0        0        0     1981 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/__main__.py
--rw-r--r--   0        0        0     5392 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/compiler.py
--rw-r--r--   0        0        0      535 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/component.py
--rw-r--r--   0        0        0     3550 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/dom_methods.py
--rw-r--r--   0        0        0      126 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/global_components.py
--rw-r--r--   0        0        0        0 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/js/__init__.py
--rw-r--r--   0        0        0     1093 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/js/store.js
--rw-r--r--   0        0        0     9071 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/parser.py
--rw-r--r--   0        0        0     3544 2023-07-06 20:03:56.649057 starfyre-0.8.0/starfyre/transpiler.py
--rw-r--r--   0        0        0     5289 1970-01-01 00:00:00.000000 starfyre-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     4751 2023-07-15 12:43:05.678508 starfyre-0.8.1/README.md
+-rw-r--r--   0        0        0      454 2023-07-15 12:43:05.678508 starfyre-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      949 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/__init__.py
+-rw-r--r--   0        0        0     1981 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/__main__.py
+-rw-r--r--   0        0        0     5636 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/compiler.py
+-rw-r--r--   0        0        0      535 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/component.py
+-rw-r--r--   0        0        0     3550 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/dom_methods.py
+-rw-r--r--   0        0        0      126 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/global_components.py
+-rw-r--r--   0        0        0        0 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/js/__init__.py
+-rw-r--r--   0        0        0     1093 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/js/store.js
+-rw-r--r--   0        0        0     9071 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/parser.py
+-rw-r--r--   0        0        0     3544 2023-07-15 12:43:05.678508 starfyre-0.8.1/starfyre/transpiler.py
+-rw-r--r--   0        0        0     5289 1970-01-01 00:00:00.000000 starfyre-0.8.1/PKG-INFO
```

### Comparing `starfyre-0.8.0/README.md` & `starfyre-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.0/starfyre/__init__.py` & `starfyre-0.8.1/starfyre/__init__.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.0/starfyre/__main__.py` & `starfyre-0.8.1/starfyre/__main__.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.0/starfyre/compiler.py` & `starfyre-0.8.1/starfyre/compiler.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,23 @@
 def get_fyre_files(project_dir):
     fyre_files = []
     for file in os.listdir(project_dir):
         if file.endswith(".fyre"):
             fyre_files.append(file)
     return fyre_files
 
-def resolve_css_import(css_file_path: Path):
+
+def resolve_css_import(css_file_name, working_directory):
     """Read a css file and save it's content to a list"""
     css_content = [] 
 
-    with open(css_file_path.resolve(), "r") as import_file:
+    if css_file_name.startswith("."):
+        css_file_name = css_file_name.replace(".", str(working_directory), 1)
+
+    with open(css_file_name, "r") as import_file:
         for line in import_file.readlines():
             css_content.append(line)
 
     return css_content           
 
 
 def parse(fyre_file_name): 
@@ -55,16 +59,17 @@
             elif line.startswith("<script"):
                 current_line_type = "js"
                 continue
             elif line.startswith("--client"):
                 current_line_type = "client"  # this is a hack
                 continue
             elif css_import_match:
-                css_import = css_import_match.group(1)
-                css_content = resolve_css_import(Path(css_import))
+                css_import = css_import_match.group(1)                
+                project_dir = Path(os.path.dirname(fyre_file_name))                                
+                css_content = resolve_css_import(css_import, project_dir)
                 css_lines += css_content
                 continue
             elif (
                 "</style>" in line
                 or "</pyml>" in line
                 or "</script>" in line
                 or "--" in line
```

### Comparing `starfyre-0.8.0/starfyre/component.py` & `starfyre-0.8.1/starfyre/component.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.0/starfyre/dom_methods.py` & `starfyre-0.8.1/starfyre/dom_methods.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.0/starfyre/js/store.js` & `starfyre-0.8.1/starfyre/js/store.js`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.0/starfyre/parser.py` & `starfyre-0.8.1/starfyre/parser.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.0/starfyre/transpiler.py` & `starfyre-0.8.1/starfyre/transpiler.py`

 * *Files identical despite different names*

### Comparing `starfyre-0.8.0/PKG-INFO` & `starfyre-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: starfyre
-Version: 0.8.0
+Version: 0.8.1
 Summary: A Python Framework for writing Reactive web Front-Ends
 License: BSD 2.0
 Author: Sanskar Jethi
 Author-email: sansyrox@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

