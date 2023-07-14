# Comparing `tmp/GPT4Readability-0.0.3.tar.gz` & `tmp/GPT4Readability-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GPT4Readability-0.0.3.tar", last modified: Thu Jul 13 00:50:23 2023, max compression
+gzip compressed data, was "GPT4Readability-0.0.4.tar", last modified: Fri Jul 14 23:14:02 2023, max compression
```

## Comparing `GPT4Readability-0.0.3.tar` & `GPT4Readability-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/GPT4Readability/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/GPT4Readability/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/prompts/readme_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/prompts/refactor_prompt.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/readme_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/suggestions_gen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/GPT4Readability/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/GPT4Readability.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-13 00:50:23.000000 GPT4Readability-0.0.3/GPT4Readability.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4494 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3718 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:50:23.297659 GPT4Readability-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-13 00:50:06.000000 GPT4Readability-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:14:02.587057 GPT4Readability-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:14:02.583057 GPT4Readability-0.0.4/GPT4Readability/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:14:02.583057 GPT4Readability-0.0.4/GPT4Readability/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/prompts/readme_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2332 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/prompts/refactor_prompt.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/readme_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/suggestions_gen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7473 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/GPT4Readability/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 23:14:02.583057 GPT4Readability-0.0.4/GPT4Readability.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-14 23:14:02.000000 GPT4Readability-0.0.4/GPT4Readability.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-07-14 23:14:02.583057 GPT4Readability-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4142 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 23:14:02.587057 GPT4Readability-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-14 23:13:50.000000 GPT4Readability-0.0.4/setup.py
```

### Comparing `GPT4Readability-0.0.3/GPT4Readability/__main__.py` & `GPT4Readability-0.0.4/GPT4Readability/__main__.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.3/GPT4Readability/prompts/readme_prompt.txt` & `GPT4Readability-0.0.4/GPT4Readability/prompts/readme_prompt.txt`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.3/GPT4Readability/prompts/refactor_prompt.txt` & `GPT4Readability-0.0.4/GPT4Readability/prompts/refactor_prompt.txt`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.3/GPT4Readability/readme_gen.py` & `GPT4Readability-0.0.4/GPT4Readability/readme_gen.py`

 * *Files 19% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         inb_msg = inb_msg.replace("[repo_name]", reponame.replace(".git",""))
     else:
         inb_msg = remove_line_with_pattern_from_string(inb_msg)
 
 
     docs = get_docs(root_dir)
     texts = split_docs(docs)
-    chain = loadLLM(model)
-    LOCAL_vector_store = makeEmbeddings(texts)
-    LOCAL_resp = askQs(LOCAL_vector_store, chain, inb_msg)
+    if len(texts) > 8300: # For now this is roughly the size we can accept
+       LOCAL_resp = 'The GitHub repository is too large (I am working on getting this working with larger repositories)'
+    else:
+        chain = loadLLM(model)
+        LOCAL_vector_store = makeEmbeddings(texts)
+        LOCAL_resp = askQs(LOCAL_vector_store, chain, inb_msg)
 
     # Write the string to the README.md file
     with open(os.path.join(root_dir,output_name), 'w') as f:
         f.write(LOCAL_resp)
```

### Comparing `GPT4Readability-0.0.3/GPT4Readability/suggestions_gen.py` & `GPT4Readability-0.0.4/GPT4Readability/suggestions_gen.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.3/GPT4Readability/utils.py` & `GPT4Readability-0.0.4/GPT4Readability/utils.py`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.3/GPT4Readability.egg-info/PKG-INFO` & `GPT4Readability-0.0.4/GPT4Readability.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPT4Readability
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool to automatically generate a README.md and suggest code improvements for any python code repository
 Home-page: https://github.com/loevlie/GPT4Readability
 Author: Dennis Johan Loevlie
 Author-email: loevliedenny@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -23,27 +23,30 @@
 [![Issues Badge](https://img.shields.io/github/issues/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/issues)
 [![Pull Requests Badge](https://img.shields.io/github/issues-pr/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/pulls)
 [![Contributors Badge](https://img.shields.io/github/contributors/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/graphs/contributors)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
 GPT4Readability is a powerful tool designed to automatically generate a comprehensive README.md file and suggest code improvements for any Python code repository. With its advanced AI capabilities, GPT4Readability goes beyond surface-level interpretation, allowing it to establish connections between disparate parts of code and gain an in-depth understanding of the code's functionality, structure, and intent.  
 
-> Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.
+> Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.  Any other changes made will be listed below:
+
+* I added the version (0.0.3) to the installation section.
+* UPDATE: Integrated into [Huggingface Spaces 🤗](https://huggingface.co/spaces) using [Gradio](https://github.com/gradio-app/gradio). Try out the Web Demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/JohanDL/GPT4Readability)
 
 ## Features
 
 - Automatic generation of a detailed README.md file for your Python codebase
 - Suggestions for code improvements to enhance readability and maintainability
 
 ## Installation
 
 To use GPT4Readability, you need to have Python 3.6 or higher installed on your system. You can install GPT4Readability and its dependencies using the following command:
 
 ```shell
-pip install GPT4Readability
+pip install GPT4Readability==0.0.3
 ```
 
 ## Usage
 
 GPT4Readability provides two main functionalities: README generation and code improvement suggestions. You can choose to use either one or both of these functions.
 
 ### README Generation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `GPT4Readability-0.0.3/LICENSE` & `GPT4Readability-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `GPT4Readability-0.0.3/PKG-INFO` & `GPT4Readability-0.0.4/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: GPT4Readability
-Version: 0.0.3
+Version: 0.0.4
 Summary: A tool to automatically generate a README.md and suggest code improvements for any python code repository
 Home-page: https://github.com/loevlie/GPT4Readability
 Author: Dennis Johan Loevlie
 Author-email: loevliedenny@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
@@ -23,27 +23,30 @@
 [![Issues Badge](https://img.shields.io/github/issues/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/issues)
 [![Pull Requests Badge](https://img.shields.io/github/issues-pr/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/pulls)
 [![Contributors Badge](https://img.shields.io/github/contributors/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/graphs/contributors)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
 GPT4Readability is a powerful tool designed to automatically generate a comprehensive README.md file and suggest code improvements for any Python code repository. With its advanced AI capabilities, GPT4Readability goes beyond surface-level interpretation, allowing it to establish connections between disparate parts of code and gain an in-depth understanding of the code's functionality, structure, and intent.  
 
-> Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.
+> Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.  Any other changes made will be listed below:
+
+* I added the version (0.0.3) to the installation section.
+* UPDATE: Integrated into [Huggingface Spaces 🤗](https://huggingface.co/spaces) using [Gradio](https://github.com/gradio-app/gradio). Try out the Web Demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/JohanDL/GPT4Readability)
 
 ## Features
 
 - Automatic generation of a detailed README.md file for your Python codebase
 - Suggestions for code improvements to enhance readability and maintainability
 
 ## Installation
 
 To use GPT4Readability, you need to have Python 3.6 or higher installed on your system. You can install GPT4Readability and its dependencies using the following command:
 
 ```shell
-pip install GPT4Readability
+pip install GPT4Readability==0.0.3
 ```
 
 ## Usage
 
 GPT4Readability provides two main functionalities: README generation and code improvement suggestions. You can choose to use either one or both of these functions.
 
 ### README Generation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `GPT4Readability-0.0.3/README.md` & `GPT4Readability-0.0.4/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -4,27 +4,30 @@
 [![Issues Badge](https://img.shields.io/github/issues/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/issues)
 [![Pull Requests Badge](https://img.shields.io/github/issues-pr/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/pulls)
 [![Contributors Badge](https://img.shields.io/github/contributors/loevlie/GPT4Readability)](https://github.com/loevlie/GPT4Readability/graphs/contributors)
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat)](https://github.com/dwyl/esta/issues)
 
 GPT4Readability is a powerful tool designed to automatically generate a comprehensive README.md file and suggest code improvements for any Python code repository. With its advanced AI capabilities, GPT4Readability goes beyond surface-level interpretation, allowing it to establish connections between disparate parts of code and gain an in-depth understanding of the code's functionality, structure, and intent.  
 
-> Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.
+> Other than this sentence this readme file and this [suggestions file](https://github.com/loevlie/GPT4Readability/blob/main/suggestions.md) were both generated by GPT4Readability using gpt-3.5-turbo.  Any other changes made will be listed below:
+
+* I added the version (0.0.3) to the installation section.
+* UPDATE: Integrated into [Huggingface Spaces 🤗](https://huggingface.co/spaces) using [Gradio](https://github.com/gradio-app/gradio). Try out the Web Demo: [![Hugging Face Spaces](https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Spaces-blue)](https://huggingface.co/spaces/JohanDL/GPT4Readability)
 
 ## Features
 
 - Automatic generation of a detailed README.md file for your Python codebase
 - Suggestions for code improvements to enhance readability and maintainability
 
 ## Installation
 
 To use GPT4Readability, you need to have Python 3.6 or higher installed on your system. You can install GPT4Readability and its dependencies using the following command:
 
 ```shell
-pip install GPT4Readability
+pip install GPT4Readability==0.0.3
 ```
 
 ## Usage
 
 GPT4Readability provides two main functionalities: README generation and code improvement suggestions. You can choose to use either one or both of these functions.
 
 ### README Generation
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `GPT4Readability-0.0.3/setup.py` & `GPT4Readability-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md', 'r') as readme:
     # ignore gifs
     description = ''.join([i for i in readme.readlines()
                            if not i.startswith('![')])
 
 setup(
     name='GPT4Readability',
-    version='0.0.3',
+    version='0.0.4',
     url='https://github.com/loevlie/GPT4Readability',
     author='Dennis Johan Loevlie',
     author_email='loevliedenny@gmail.com',
     description='A tool to automatically generate a README.md and suggest code improvements for any python code repository',
     long_description=description,
     long_description_content_type='text/markdown',
     packages=find_packages(),  # automatically discover all packages and subpackages
```

