# Comparing `tmp/turbo_docs-1.0.3.tar.gz` & `tmp/turbo_docs-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-1.0.3.tar", last modified: Sat Jul 15 12:50:22 2023, max compression
+gzip compressed data, was "turbo_docs-1.0.4.tar", last modified: Sat Jul 15 13:32:18 2023, max compression
```

## Comparing `turbo_docs-1.0.3.tar` & `turbo_docs-1.0.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-15 12:50:22.735780 turbo_docs-1.0.3/
--rw-rw-rw-   0        0        0     2833 2023-07-15 12:50:22.731274 turbo_docs-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2336 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-15 12:50:22.735780 turbo_docs-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      881 2023-07-15 12:49:43.000000 turbo_docs-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-15 12:50:22.665515 turbo_docs-1.0.3/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.3/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-15 12:50:22.704918 turbo_docs-1.0.3/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.3/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     2144 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/turbo_docs/commands/docs.py
--rw-rw-rw-   0        0        0     1038 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     2399 2023-07-15 12:47:32.000000 turbo_docs-1.0.3/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-07-15 12:50:22.726107 turbo_docs-1.0.3/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.3/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      826 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1760 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      799 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-07-15 12:50:22.691596 turbo_docs-1.0.3/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2833 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       48 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 13:32:18.512179 turbo_docs-1.0.4/
+-rw-rw-rw-   0        0        0     2833 2023-07-15 13:32:18.509608 turbo_docs-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-07-15 12:53:32.000000 turbo_docs-1.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 13:32:18.514220 turbo_docs-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      901 2023-07-15 12:59:29.000000 turbo_docs-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:32:18.448570 turbo_docs-1.0.4/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.4/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:32:18.486086 turbo_docs-1.0.4/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.4/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2144 2023-07-03 17:25:01.000000 turbo_docs-1.0.4/turbo_docs/commands/docs.py
+-rw-rw-rw-   0        0        0     1038 2023-07-03 17:25:01.000000 turbo_docs-1.0.4/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     2399 2023-07-15 12:47:32.000000 turbo_docs-1.0.4/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:32:18.504585 turbo_docs-1.0.4/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.4/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      826 2023-07-03 17:25:01.000000 turbo_docs-1.0.4/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1743 2023-07-15 13:31:59.000000 turbo_docs-1.0.4/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      799 2023-07-03 17:25:01.000000 turbo_docs-1.0.4/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-07-15 13:32:18.473373 turbo_docs-1.0.4/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2833 2023-07-15 13:32:18.000000 turbo_docs-1.0.4/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-07-15 13:32:18.000000 turbo_docs-1.0.4/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 13:32:18.000000 turbo_docs-1.0.4/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-15 13:32:18.000000 turbo_docs-1.0.4/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-07-15 13:32:18.000000 turbo_docs-1.0.4/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-15 13:32:18.000000 turbo_docs-1.0.4/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-1.0.3/PKG-INFO` & `turbo_docs-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 1.0.3
+Version: 1.0.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `turbo_docs-1.0.3/README.md` & `turbo_docs-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.3/setup.py` & `turbo_docs-1.0.4/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="1.0.3",
+	version="1.0.4",
 	packages=find_packages(),
 	install_requires=[
 		"openai",
 		"click",
 		"pyperclip",
     	"toml",
         "pathspec",
         "llm-blocks",
+        "tiktoken"
 	],
 	entry_points={
 		"console_scripts": [
 			"turbo_docs=turbo_docs.generate:driver"
 		],
 	},
 	classifiers=[
```

### Comparing `turbo_docs-1.0.3/turbo_docs/commands/docs.py` & `turbo_docs-1.0.4/turbo_docs/commands/docs.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.3/turbo_docs/commands/readme.py` & `turbo_docs-1.0.4/turbo_docs/commands/readme.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.3/turbo_docs/generate.py` & `turbo_docs-1.0.4/turbo_docs/generate.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.3/turbo_docs/utils/cli_options.py` & `turbo_docs-1.0.4/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.3/turbo_docs/utils/directory.py` & `turbo_docs-1.0.4/turbo_docs/utils/directory.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 def read_text(path: Path) -> str:
     """Assuming all non-textual files are in the turbo_docs.toml ignore list"""
     try:
         with open(path, "r") as file:
             return file.read()
         
     except UnicodeDecodeError:
-        print(f"File {path} contains non-textual content. Add to 'turbo_docs.toml' if this file should be ignored.")
         with open(path, 'r', encoding='utf-8', errors='replace') as file:
             return file.read()
         
     except Exception as e:
         raise e
 
 
@@ -33,14 +32,15 @@
 
 
 def get_repo_text_dict():
     """Return a dictionary of all text in the current repo"""
     if not Path("turbo_docs.toml").exists():
         ignored_patterns = []
         print("Warning: 'turbo_docs.toml' not found. All files will be included.")
+        print("See https://github.com/voynow/turbo-docs/blob/main/turbo_docs.toml for an example.")
     else:
         config = toml.load("turbo_docs.toml")
         ignored_patterns = config.get("ignore", [])
 
     pathspec = PathSpec.from_lines(GitWildMatchPattern, ignored_patterns)
     return collect_text_from_files(Path("."), pathspec)
```

### Comparing `turbo_docs-1.0.3/turbo_docs/utils/openai_api.py` & `turbo_docs-1.0.4/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.3/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-1.0.4/turbo_docs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-docs
-Version: 1.0.3
+Version: 1.0.4
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

