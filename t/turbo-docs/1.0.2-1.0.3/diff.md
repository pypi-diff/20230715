# Comparing `tmp/turbo_docs-1.0.2.tar.gz` & `tmp/turbo_docs-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "turbo_docs-1.0.2.tar", last modified: Mon Jul  3 17:56:36 2023, max compression
+gzip compressed data, was "turbo_docs-1.0.3.tar", last modified: Sat Jul 15 12:50:22 2023, max compression
```

## Comparing `turbo_docs-1.0.2.tar` & `turbo_docs-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-03 17:56:36.511887 turbo_docs-1.0.2/
--rw-rw-rw-   0        0        0     2833 2023-07-03 17:56:36.511887 turbo_docs-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2336 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-03 17:56:36.512884 turbo_docs-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      927 2023-07-03 17:56:00.000000 turbo_docs-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:56:36.499167 turbo_docs-1.0.2/turbo_docs/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.2/turbo_docs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:56:36.505878 turbo_docs-1.0.2/turbo_docs/commands/
--rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.2/turbo_docs/commands/__init__.py
--rw-rw-rw-   0        0        0     2144 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/turbo_docs/commands/docs.py
--rw-rw-rw-   0        0        0     1038 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/turbo_docs/commands/readme.py
--rw-rw-rw-   0        0        0     2347 2023-07-03 17:55:45.000000 turbo_docs-1.0.2/turbo_docs/generate.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:56:36.510885 turbo_docs-1.0.2/turbo_docs/utils/
--rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.2/turbo_docs/utils/__init__.py
--rw-rw-rw-   0        0        0      826 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/turbo_docs/utils/cli_options.py
--rw-rw-rw-   0        0        0     1760 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/turbo_docs/utils/directory.py
--rw-rw-rw-   0        0        0      799 2023-07-03 17:25:01.000000 turbo_docs-1.0.2/turbo_docs/utils/openai_api.py
-drwxrwxrwx   0        0        0        0 2023-07-03 17:56:36.503166 turbo_docs-1.0.2/turbo_docs.egg-info/
--rw-rw-rw-   0        0        0     2833 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       58 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       76 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-03 17:56:36.000000 turbo_docs-1.0.2/turbo_docs.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-15 12:50:22.735780 turbo_docs-1.0.3/
+-rw-rw-rw-   0        0        0     2833 2023-07-15 12:50:22.731274 turbo_docs-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2336 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-15 12:50:22.735780 turbo_docs-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      881 2023-07-15 12:49:43.000000 turbo_docs-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-15 12:50:22.665515 turbo_docs-1.0.3/turbo_docs/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.3/turbo_docs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-15 12:50:22.704918 turbo_docs-1.0.3/turbo_docs/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-29 00:25:31.000000 turbo_docs-1.0.3/turbo_docs/commands/__init__.py
+-rw-rw-rw-   0        0        0     2144 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/turbo_docs/commands/docs.py
+-rw-rw-rw-   0        0        0     1038 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/turbo_docs/commands/readme.py
+-rw-rw-rw-   0        0        0     2399 2023-07-15 12:47:32.000000 turbo_docs-1.0.3/turbo_docs/generate.py
+drwxrwxrwx   0        0        0        0 2023-07-15 12:50:22.726107 turbo_docs-1.0.3/turbo_docs/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-10 17:16:33.000000 turbo_docs-1.0.3/turbo_docs/utils/__init__.py
+-rw-rw-rw-   0        0        0      826 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/turbo_docs/utils/cli_options.py
+-rw-rw-rw-   0        0        0     1760 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/turbo_docs/utils/directory.py
+-rw-rw-rw-   0        0        0      799 2023-07-03 17:25:01.000000 turbo_docs-1.0.3/turbo_docs/utils/openai_api.py
+drwxrwxrwx   0        0        0        0 2023-07-15 12:50:22.691596 turbo_docs-1.0.3/turbo_docs.egg-info/
+-rw-rw-rw-   0        0        0     2833 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       58 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       48 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-07-15 12:50:22.000000 turbo_docs-1.0.3/turbo_docs.egg-info/top_level.txt
```

### Comparing `turbo_docs-1.0.2/PKG-INFO` & `turbo_docs-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo_docs
-Version: 1.0.2
+Version: 1.0.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `turbo_docs-1.0.2/README.md` & `turbo_docs-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.2/setup.py` & `turbo_docs-1.0.3/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
 	name="turbo_docs",
-	version="1.0.2",
+	version="1.0.3",
 	packages=find_packages(),
 	install_requires=[
-		"requests",
 		"openai",
 		"click",
 		"pyperclip",
-		"redbaron",
-		"gitpython",
     	"toml",
         "pathspec",
         "llm-blocks",
 	],
 	entry_points={
 		"console_scripts": [
 			"turbo_docs=turbo_docs.generate:driver"
```

### Comparing `turbo_docs-1.0.2/turbo_docs/commands/docs.py` & `turbo_docs-1.0.3/turbo_docs/commands/docs.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.2/turbo_docs/commands/readme.py` & `turbo_docs-1.0.3/turbo_docs/commands/readme.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.2/turbo_docs/generate.py` & `turbo_docs-1.0.3/turbo_docs/generate.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,15 +50,16 @@
 
     'turbo_docs --docs' generates a docs for each file
         Useful for keeping documentation up to date
     """
     dir_text_dict = directory.get_repo_text_dict()
 
     if readme:
-        del dir_text_dict[Path("README.md")]
+        if Path("README.md") in dir_text_dict:
+            del dir_text_dict[Path("README.md")]
         dir_text_str = directory.convert_dict_to_string(dir_text_dict)
         model = resolve_model(gpt3)
         readme_module.readme(dir_text_str, model)
         print("Generated README.md")
 
     if docs:
         model = resolve_model(gpt3)
```

### Comparing `turbo_docs-1.0.2/turbo_docs/utils/cli_options.py` & `turbo_docs-1.0.3/turbo_docs/utils/cli_options.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.2/turbo_docs/utils/directory.py` & `turbo_docs-1.0.3/turbo_docs/utils/directory.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.2/turbo_docs/utils/openai_api.py` & `turbo_docs-1.0.3/turbo_docs/utils/openai_api.py`

 * *Files identical despite different names*

### Comparing `turbo_docs-1.0.2/turbo_docs.egg-info/PKG-INFO` & `turbo_docs-1.0.3/turbo_docs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: turbo-docs
-Version: 1.0.2
+Version: 1.0.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

