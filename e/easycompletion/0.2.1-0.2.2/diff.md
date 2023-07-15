# Comparing `tmp/easycompletion-0.2.1.tar.gz` & `tmp/easycompletion-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easycompletion-0.2.1.tar", last modified: Fri Jul 14 09:05:12 2023, max compression
+gzip compressed data, was "easycompletion-0.2.2.tar", last modified: Sat Jul 15 00:36:29 2023, max compression
```

## Comparing `easycompletion-0.2.1.tar` & `easycompletion-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 09:05:12.377098 easycompletion-0.2.1/
--rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.2.1/LICENSE
--rw-r--r--   0 shawwalters   (501) staff       (20)     7213 2023-07-14 09:05:12.376940 easycompletion-0.2.1/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)     6452 2023-07-14 09:03:44.000000 easycompletion-0.2.1/README.md
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 09:05:12.375576 easycompletion-0.2.1/easycompletion/
--rw-r--r--   0 shawwalters   (501) staff       (20)      776 2023-07-14 09:05:08.000000 easycompletion-0.2.1/easycompletion/__init__.py
--rw-r--r--   0 shawwalters   (501) staff       (20)      511 2023-07-10 21:02:57.000000 easycompletion-0.2.1/easycompletion/constants.py
--rw-r--r--   0 shawwalters   (501) staff       (20)    14537 2023-07-14 09:00:43.000000 easycompletion-0.2.1/easycompletion/model.py
--rw-r--r--   0 shawwalters   (501) staff       (20)     5231 2023-07-12 20:37:03.000000 easycompletion-0.2.1/easycompletion/prompt.py
-drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-14 09:05:12.376685 easycompletion-0.2.1/easycompletion.egg-info/
--rw-r--r--   0 shawwalters   (501) staff       (20)     7213 2023-07-14 09:05:12.000000 easycompletion-0.2.1/easycompletion.egg-info/PKG-INFO
--rw-r--r--   0 shawwalters   (501) staff       (20)      319 2023-07-14 09:05:12.000000 easycompletion-0.2.1/easycompletion.egg-info/SOURCES.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-14 09:05:12.000000 easycompletion-0.2.1/easycompletion.egg-info/dependency_links.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       30 2023-07-14 09:05:12.000000 easycompletion-0.2.1/easycompletion.egg-info/requires.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-14 09:05:12.000000 easycompletion-0.2.1/easycompletion.egg-info/top_level.txt
--rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-14 09:05:12.377144 easycompletion-0.2.1/setup.cfg
--rw-r--r--   0 shawwalters   (501) staff       (20)     1430 2023-07-14 09:05:08.000000 easycompletion-0.2.1/setup.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-15 00:36:29.275543 easycompletion-0.2.2/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1126 2023-07-07 00:23:10.000000 easycompletion-0.2.2/LICENSE
+-rw-r--r--   0 shawwalters   (501) staff       (20)     7213 2023-07-15 00:36:29.275373 easycompletion-0.2.2/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)     6452 2023-07-14 09:03:44.000000 easycompletion-0.2.2/README.md
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-15 00:36:29.273554 easycompletion-0.2.2/easycompletion/
+-rw-r--r--   0 shawwalters   (501) staff       (20)      776 2023-07-15 00:36:24.000000 easycompletion-0.2.2/easycompletion/__init__.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)      511 2023-07-10 21:02:57.000000 easycompletion-0.2.2/easycompletion/constants.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)    14537 2023-07-14 09:00:43.000000 easycompletion-0.2.2/easycompletion/model.py
+-rw-r--r--   0 shawwalters   (501) staff       (20)     5511 2023-07-15 00:35:11.000000 easycompletion-0.2.2/easycompletion/prompt.py
+drwxr-xr-x   0 shawwalters   (501) staff       (20)        0 2023-07-15 00:36:29.275107 easycompletion-0.2.2/easycompletion.egg-info/
+-rw-r--r--   0 shawwalters   (501) staff       (20)     7213 2023-07-15 00:36:29.000000 easycompletion-0.2.2/easycompletion.egg-info/PKG-INFO
+-rw-r--r--   0 shawwalters   (501) staff       (20)      319 2023-07-15 00:36:29.000000 easycompletion-0.2.2/easycompletion.egg-info/SOURCES.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)        1 2023-07-15 00:36:29.000000 easycompletion-0.2.2/easycompletion.egg-info/dependency_links.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       30 2023-07-15 00:36:29.000000 easycompletion-0.2.2/easycompletion.egg-info/requires.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       15 2023-07-15 00:36:29.000000 easycompletion-0.2.2/easycompletion.egg-info/top_level.txt
+-rw-r--r--   0 shawwalters   (501) staff       (20)       38 2023-07-15 00:36:29.275616 easycompletion-0.2.2/setup.cfg
+-rw-r--r--   0 shawwalters   (501) staff       (20)     1430 2023-07-15 00:36:24.000000 easycompletion-0.2.2/setup.py
```

### Comparing `easycompletion-0.2.1/LICENSE` & `easycompletion-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.1/PKG-INFO` & `easycompletion-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.2.1
+Version: 0.2.2
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.2.1/README.md` & `easycompletion-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.1/easycompletion/__init__.py` & `easycompletion-0.2.2/easycompletion/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 easycompletion
 
 Leveraging conversational AI for bicameral decision making.
 """
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __author__ = "Moon (https://github.com/AutonomousResearchGroup)"
 __credits__ = "https://github.com/AutonomousResearchGroup/easycompletion"
 
 from .model import (
     openai_function_call,
     openai_text_call,
     compose_function,
```

### Comparing `easycompletion-0.2.1/easycompletion/model.py` & `easycompletion-0.2.2/easycompletion/model.py`

 * *Files identical despite different names*

### Comparing `easycompletion-0.2.1/easycompletion/prompt.py` & `easycompletion-0.2.2/easycompletion/prompt.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 import tiktoken
+import sys
 
 from .constants import (
     default_text_model,
     default_chunk_length,
 )
 
 
@@ -142,14 +143,22 @@
     """
     prompt = prompt_template  # Initial prompt template.
 
     # Replacing placeholders in the template with the actual values from the parameters.
     for key, value in parameters.items():
         if isinstance(value, str):
             prompt = prompt.replace("{{" + key + "}}", value)
+        elif isinstance(value, int):
+            prompt = prompt.replace("{{" + key + "}}", str(value))
         elif isinstance(value, dict):
             for k, v in value.items():
                 prompt = prompt.replace("{{" + key + "}}", k + "::" + v)
         elif isinstance(value, list):
             for item in value:
                 prompt = prompt.replace("{{" + key + "}}", item + "\n")
+        elif value is None:
+            prompt = prompt.replace("{{" + key + "}}", "None")
+        else:
+            print("ERROR PARSING")
+            sys.exit(1)
+
     return prompt
```

### Comparing `easycompletion-0.2.1/easycompletion.egg-info/PKG-INFO` & `easycompletion-0.2.2/easycompletion.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easycompletion
-Version: 0.2.1
+Version: 0.2.2
 Summary: Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.
 Home-page: https://github.com/AutonomousResearchGroup/easycompletion
 Author: Moon
 Author-email: shawmakesmagic@gmail.com
 License: MIT
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Science/Research
```

### Comparing `easycompletion-0.2.1/setup.py` & `easycompletion-0.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     long_description = [line for line in long_description if not "<img" in line]
     # now join all the lines back together
     long_description = "\n".join(long_description)
 
 
 setup(
     name="easycompletion",
-    version='0.2.1',
+    version='0.2.2',
     description="Easy text completion and function calling using the OpenAI API. Also includes useful utilities for counting tokens, composing prompts and trimming them to fit within the token limit.",
     long_description=long_description,  # added this line
     long_description_content_type="text/markdown",  # and this line
     url="https://github.com/AutonomousResearchGroup/easycompletion",
     author="Moon",
     author_email="shawmakesmagic@gmail.com",
     license="MIT",
```

