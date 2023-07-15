# Comparing `tmp/problem_bank_scripts-0.8.2.tar.gz` & `tmp/problem_bank_scripts-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "problem_bank_scripts-0.8.2.tar", max compression
+gzip compressed data, was "problem_bank_scripts-0.9.0.tar", max compression
```

## Comparing `problem_bank_scripts-0.8.2.tar` & `problem_bank_scripts-0.9.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.8.2/LICENSE
--rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.8.2/README.md
--rw-r--r--   0        0        0     1075 2023-07-15 03:02:33.108784 problem_bank_scripts-0.8.2/pyproject.toml
--rw-r--r--   0        0        0       59 2023-07-15 03:02:42.698673 problem_bank_scripts-0.8.2/src/problem_bank_scripts/__init__.py
--rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.8.2/src/problem_bank_scripts/attributions.json
--rw-r--r--   0        0        0    13614 2023-07-07 00:02:47.412321 problem_bank_scripts-0.8.2/src/problem_bank_scripts/prairielearn.py
--rw-r--r--   0        0        0    47690 2023-07-15 03:03:30.028907 problem_bank_scripts-0.8.2/src/problem_bank_scripts/problem_bank_scripts.py
--rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.8.2/src/problem_bank_scripts/qti_export.py
--rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.8.2/src/problem_bank_scripts/webwork_to_md.py
--rw-r--r--   0        0        0     2644 2023-07-15 03:03:43.096069 problem_bank_scripts-0.8.2/setup.py
--rw-r--r--   0        0        0     2576 2023-07-15 03:03:43.096274 problem_bank_scripts-0.8.2/PKG-INFO
+-rwxr-xr-x   0        0        0        1 2021-05-16 14:07:02.985176 problem_bank_scripts-0.9.0/LICENSE
+-rw-r--r--   0        0        0     1605 2023-06-15 01:42:11.784217 problem_bank_scripts-0.9.0/README.md
+-rw-r--r--   0        0        0     1075 2023-07-15 03:07:04.164417 problem_bank_scripts-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       59 2023-07-15 03:07:19.915066 problem_bank_scripts-0.9.0/src/problem_bank_scripts/__init__.py
+-rw-r--r--   0        0        0     1757 2023-06-15 17:31:34.807559 problem_bank_scripts-0.9.0/src/problem_bank_scripts/attributions.json
+-rw-r--r--   0        0        0    13614 2023-07-07 00:02:47.412321 problem_bank_scripts-0.9.0/src/problem_bank_scripts/prairielearn.py
+-rw-r--r--   0        0        0    47863 2023-07-15 03:05:06.482962 problem_bank_scripts-0.9.0/src/problem_bank_scripts/problem_bank_scripts.py
+-rw-r--r--   0        0        0      129 2022-06-24 05:48:29.289246 problem_bank_scripts-0.9.0/src/problem_bank_scripts/qti_export.py
+-rw-r--r--   0        0        0    19225 2022-06-24 07:32:56.504377 problem_bank_scripts-0.9.0/src/problem_bank_scripts/webwork_to_md.py
+-rw-r--r--   0        0        0     2644 2023-07-15 03:07:57.680062 problem_bank_scripts-0.9.0/setup.py
+-rw-r--r--   0        0        0     2576 2023-07-15 03:07:57.680268 problem_bank_scripts-0.9.0/PKG-INFO
```

### Comparing `problem_bank_scripts-0.8.2/README.md` & `problem_bank_scripts-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.8.2/pyproject.toml` & `problem_bank_scripts-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "problem_bank_scripts"
-version = "0.8.2"
+version = "0.9.0"
 description = "A package with useful functions to convert between different problem bank formats."
 authors = ["Open Problem Bank Team"]
 license = "MIT"
 readme = "README.md"
 documentation = "https://problem_bank_scripts.readthedocs.io/en/latest/"
 homepage = "https://github.com/open-resources/problem_bank_scripts"
 repository = "https://github.com/open-resources/problem_bank_scripts"
```

### Comparing `problem_bank_scripts-0.8.2/src/problem_bank_scripts/attributions.json` & `problem_bank_scripts-0.9.0/src/problem_bank_scripts/attributions.json`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.8.2/src/problem_bank_scripts/prairielearn.py` & `problem_bank_scripts-0.9.0/src/problem_bank_scripts/prairielearn.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.8.2/src/problem_bank_scripts/problem_bank_scripts.py` & `problem_bank_scripts-0.9.0/src/problem_bank_scripts/problem_bank_scripts.py`

 * *Files 0% similar despite different names*

```diff
@@ -495,16 +495,20 @@
     server_py = f""""""
 
     server_py += server_dict.get("imports", "") + "\n"
 
     try:
         for function, code in server_dict.items():
             indented_code = code.replace("\n", "\n    ")
-            if code:
-                server_py += f"def {function}(data):\n    {indented_code}\n"
+            # With the custom header, add functions to server.py as-is
+            if function == "custom":
+                server_py += f"{code}"
+            else:
+                if code:
+                    server_py += f"def {function}(data):\n    {indented_code}\n"
     except:
         raise
 
     return server_py
 
 
 def write_server_py(output_path, parsed_question):
```

### Comparing `problem_bank_scripts-0.8.2/src/problem_bank_scripts/webwork_to_md.py` & `problem_bank_scripts-0.9.0/src/problem_bank_scripts/webwork_to_md.py`

 * *Files identical despite different names*

### Comparing `problem_bank_scripts-0.8.2/setup.py` & `problem_bank_scripts-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'numpy>=1.22,<2.0',
  'pandas>=2.0,<3.0',
  'problem-bank-helpers>=0.1.14,<0.2.0',
  'sympy>=1.8,<2.0']
 
 setup_kwargs = {
     'name': 'problem-bank-scripts',
-    'version': '0.8.2',
+    'version': '0.9.0',
     'description': 'A package with useful functions to convert between different problem bank formats.',
     'long_description': '# Problem Bank Scripts \n\n[![Python](https://img.shields.io/badge/python-3.9-blue)]()\n[![codecov](https://codecov.io/gh/open-resources/problem_bank_scripts/branch/main/graph/badge.svg)](https://codecov.io/gh/open-resources/problem_bank_scripts)\n[![Documentation Status](https://readthedocs.org/projects/problem_bank_scripts/badge/?version=latest)](https://problem_bank_scripts.readthedocs.io/en/latest/?badge=latest)\n\n\n## Installation\n\n```bash\n$ pip install -i https://test.pypi.org/simple/ problem_bank_scripts\n```\n\n## Update version\n\nHere are the steps to increment the version (replace patch with major/minor/patch)\n\n```\npoetry version patch\n\npico src/problem_bank_scripts/__init__.py\n\npico tests/test_problem_bank_scripts.py\n\npoetry run pytest\n\ncd docs; poetry run make html; cd ..\n\ngit add .; git commit -m "increment version"; git push\n\npoetry build\n\npoetry publish\n```\n\n\n## Features\n\n- TODO\n\n## Dependencies\n\n- TODO\n\n## Usage\n\n- TODO\n\n## Documentation\n\nThe official documentation is hosted on Read the Docs: https://problem_bank_scripts.readthedocs.io/en/latest/\n\n## Contributors\n\nWe welcome and recognize all contributions. You can see a list of current contributors in the [contributors tab](https://github.com/open-resources/problem_bank_scripts/graphs/contributors).\n\n### Credits\n\nThis package was created with Cookiecutter and the UBC-MDS/cookiecutter-ubc-mds project template, modified from the [pyOpenSci/cookiecutter-pyopensci](https://github.com/pyOpenSci/cookiecutter-pyopensci) project template and the [audreyr/cookiecutter-pypackage](https://github.com/audreyr/cookiecutter-pypackage).\n',
     'author': 'Open Problem Bank Team',
     'author_email': None,
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/open-resources/problem_bank_scripts',
```

### Comparing `problem_bank_scripts-0.8.2/PKG-INFO` & `problem_bank_scripts-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: problem-bank-scripts
-Version: 0.8.2
+Version: 0.9.0
 Summary: A package with useful functions to convert between different problem bank formats.
 Home-page: https://github.com/open-resources/problem_bank_scripts
 License: MIT
 Author: Open Problem Bank Team
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

